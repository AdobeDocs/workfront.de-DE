---
content-type: api
navigation-topic: api-navigation-topic
title: Ereignisabonnement-Zertifikate
description: Ereignisabonnement-Zertifikate
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 0c9cbf094ec1b3d5f48a0e4b700b9554925199e1
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%

---

# Client-TLS für Ereignisabonnement konfigurieren

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

Mit Client-TLS können Sie überprüfen, ob die Ereignisabonnementnachricht, die Sie erhalten, tatsächlich von Adobe Workfront stammt. Um diese Funktion zu aktivieren, muss Ihr Server so konfiguriert sein, dass er das x509-Zertifikat von Workfront anfordert und validiert.

<!--
>[!NOTE]
>
>* Workfront currently supports TLS version 1.2 by default.
>* Organizations can request that TLS version 1.3 be enabled for their Workfront instance.
-->


## Überprüfen des Client-Zertifikats von Workfront

Bei diesem Verfahren wird davon ausgegangen, dass Ihr Server so konfiguriert ist, dass er TLS-Verbindungen akzeptiert. Workfront unterstützt keine selbstsignierten Zertifikate.

Im Allgemeinen sind dies die Schritte, die zum Aktivieren der Client-Authentifizierung für Ihren Server erforderlich sind:

1. Herunterladen der PEM-Version des DigiCert Global Root CA-Zertifikats.
1. Aktivieren Sie die Client-Zertifikatüberprüfung.

   Geben Sie das CA-Zertifikat aus Schritt 1 als vertrauenswürdig an.

1. Stellen Sie die Überprüfungstiefe auf 2 ein, da unser Zertifikat tatsächlich vom DigiCert SHA2 Secure Server CA signiert wird, der eine Zwischenzertifikatstelle unter DigiCert Global Root CA ist.
1. Überprüfen Sie, ob das Client-Zertifikat tatsächlich von Workfront stammt, indem Sie den Domain-Namen des Antragstellers überprüfen.

## Beispiele für die Server-Konfiguration

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
 

## Zuordnung von Zertifikaten zu Umgebungen

| WF-Umgebung | Allgemeiner Zertifikatname | Zertifikatbetreff (DN) |
| -- | -- | -- |
| Produktion | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=LEHI/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Vorschau | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=LEHI/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=LEHI/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=LEHI/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Herunterladen von Zertifikaten

Klicken Sie auf die folgenden Links, um die Client-Zertifikate herunterzuladen.

* [Client-Zertifikat - Produktionsumgebung](assets/prod-environment-nov-2024.crt)
* [Client-Zertifikat - Vorschau-Umgebung](assets/preview-environment-nov-2024.crt)
* [Client-Zertifikat - Sandbox-Umgebung](assets/sandbox-environment-nov-2024.crt)

>[!NOTE]
>
>Sie können dasselbe Client-Zertifikat für beide Sandbox-Umgebungen verwenden.
