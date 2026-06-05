---
content-type: api
navigation-topic: api-navigation-topic
title: Ereignisabonnement-Zertifikate
description: Ereignisabonnement-Zertifikate
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/rFy1Sc7UKGbenuOywbCTw4ezfmmRRDKMihHJD--LPto
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 337
ht-degree: 4%

---

# Konfigurieren von Client-TLS für Ereignisabonnement

<!--
Configuring Client TLS for Event Subscription
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


>[!NOTE]
>
>Ereignisabonnements verwenden TLS Version 1.3, wenn der Server, an den das Ereignisabonnement Ereignisse sendet, Version 1.3 unterstützt. Wenn der Verbindungs-Server Version 1.3 nicht unterstützt, verwendet das Ereignisabonnement TLS Version 1.2.



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

* [Client-Zertifikat - Produktionsumgebung](assets/prod-ES-client-cert-oct25.crt)
* [Client-Zertifikat - Vorschau-Umgebung](assets/preview-ES-client-cert-oct25.crt)
* [Client-Zertifikat - Sandbox-Umgebung](assets/sandbox-ES-client-cert-oct25.crt)

>[!NOTE]
>
>Sie können dasselbe Client-Zertifikat für beide Sandbox-Umgebungen verwenden.
