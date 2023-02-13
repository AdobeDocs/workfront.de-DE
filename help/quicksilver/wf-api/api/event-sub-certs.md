---
content-type: api
navigation-topic: api-navigation-topic
title: Ereignisabonnementzertifikate
description: Ereignisabonnementzertifikate
author: Becky
feature: Workfront API
source-git-commit: 53ef8f4fda22c912c274841d07ad865aa04141c8
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

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

Weitere Informationen finden Sie unter [NGiNX-Dokumentation für ngx_http_ssl_module](http://nginx.org/en/docs/http/ngx_http_ssl_module.html).

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
* [Apache Module mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Zuordnung von Zertifikat zu Umgebung

| WF-Umgebung | Certificate Common Name | Certificate Subject (DN) | | — | — | — | | Produktion | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com| | Vorschau | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com | | Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com | | Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Zertifikate herunterladen

Klicken Sie auf die folgenden Links, um die Clientzertifikate herunterzuladen.

* [Client-Zertifikat - Produktionsumgebung](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [Client-Zertifikat - Vorschau der Umgebung](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [Client-Zertifikat - Sandbox-Umgebung](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>Sie können dasselbe Client-Zertifikat für beide Sandbox-Umgebungen verwenden.

