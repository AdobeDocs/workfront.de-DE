---
content-type: api
navigation-topic: api-navigation-topic
title: Ereignisabonnementzertifikate
description: Ereignisabonnementzertifikate
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 8f8a5aea1eeecff76150b87a6e7fe38b21f7d033
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%

---

# Konfigurieren von Client-TLS für die Ereignisanmeldung

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

Mit Client TLS können Sie überprüfen, ob die von Ihnen erhaltene Ereignisabonnementnachricht tatsächlich von Adobe Workfront stammt. Um diese Funktion zu aktivieren, muss Ihr Server so konfiguriert sein, dass das x509-Zertifikat von Workfront angefordert und validiert wird.


## Workfront-Clientzertifikat überprüfen

Dieses Verfahren setzt voraus, dass Ihr Server für die Aufnahme von TLS-Verbindungen konfiguriert ist. Workfront unterstützt keine selbstsignierten Zertifikate.

Im Allgemeinen sind dies die Schritte, die zum Aktivieren der Client-Authentifizierung für Ihren Server erforderlich sind:

1. Laden Sie die PEM-Version des DigiCert Global Root CA-Zertifikats herunter.
1. Aktivieren Sie die Client-Zertifikatüberprüfung.

   Geben Sie das Zertifizierungsstellenzertifikat aus Schritt 1 als vertrauenswürdig an.

1. Setzen Sie die Überprüfungstiefe auf 2, da unser Zertifikat tatsächlich von der DigiCert SHA2 Secure Server CA signiert wird, einer zwischengeschalteten Zertifizierungsstelle unter DigiCert Global Root CA.
1. Überprüfen Sie, ob das Clientzertifikat tatsächlich von Workfront stammt, indem Sie den Domänennamen des Betreffs überprüfen.

## Beispiele für Serverkonfiguration

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

Weitere Informationen finden Sie in der [NGiNX-Dokumentation für ngx_http_ssl_module](https://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

Weitere Informationen finden Sie unter

* [Client-Authentifizierung und Zugriffssteuerung](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache-Modul mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Zuordnung von Zertifikat zu Umgebung

| WF-Umgebung | Certificate Common Name | Zertifikatsinhaber (DN) |
| -- | -- | -- |
| Produktion | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Vorschau | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Zertifikate herunterladen

Klicken Sie auf die folgenden Links, um die Clientzertifikate herunterzuladen.

* [Client-Zertifikat - Produktionsumgebung](assets/prod-environment-nov-2024.crt)
* [Client-Zertifikat - Vorschau der Umgebung](assets/preview-environment-nov-2024.crt)
* [Client-Zertifikat - Sandbox-Umgebung](assets/sandbox-environment-nov-2024.crt)

>[!NOTE]
>
>Sie können dasselbe Client-Zertifikat für beide Sandbox-Umgebungen verwenden.
