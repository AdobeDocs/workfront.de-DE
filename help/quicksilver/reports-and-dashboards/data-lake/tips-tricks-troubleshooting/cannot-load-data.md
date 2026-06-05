---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop kann keine Verbindung herstellen
description: Beim Versuch, eine Verbindung zwischen Tableau Desktop und Data Connect herzustellen, wird ein Fehler angezeigt.
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 253
ht-degree: 5%

---

# Tableau Desktop kann keine Verbindung herstellen

## Problem

Beim Versuch, eine Verbindung zwischen Tableau Desktop und Data Connect herzustellen, wird der folgende Fehler angezeigt:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Ursache

Dieser Fehler wird durch eine Proxy-Einstellung auf Ihrem lokalen Computer verursacht, die verhindert, dass Daten von Data Connect geladen werden.

Data Connect wird über Snowflake-Cloud-Services von Drittanbietern bereitgestellt. Tableau erfordert ein offenes Netzwerk für die Kommunikation mit Snowflake.

## Lösung

Zur Lösung dieses Problems können Sie Folgendes versuchen:

* **Fehlerbehebung durch Deaktivieren des Sicherheits-Tools**: Deaktivieren Sie Ihr Sicherheits-Tool, z. B. Zscaler oder Cisco, um zu sehen, ob es das Konnektivitätsproblem behebt. Wenn das Verbindungsproblem dadurch behoben wird, stellen Sie sicher, dass Ihr Sicherheits-Tool auf die neueste Version aktualisiert wurde, und fügen Sie die IP-Adresse von Data Connect (Snowflake) mit Ihrem internen Netzwerkteam zur VPN-Zulassungsliste hinzu.

* **IP-Adressen zur Zulassungsliste hinzufügen**: Stellen Sie sicher, dass Ihre Firewall-Einstellungen die von Data Connect verwendeten IP-Adressen zulassen. Verwenden Sie den `SYSTEM$ALLOWLIST()`, um die IP-Adresse zu erhalten, die Sie dann im VPN auf die Zulassungsliste gesetzt haben.

* **Firewall- und Proxy-Einstellungen überprüfen**: Überprüfen Sie, ob eine Firewall oder Proxy-Konfigurationen in Ihrem Netzwerk den Zugriff auf die Endpunkte von Snowflake blockieren. Möglicherweise müssen Sie sich an Ihren Netzwerkadministrator wenden, um die erforderlichen Snowflake-IP-Adressen und -Ports zur -Zulassungsliste Ihres Unternehmens hinzuzufügen.

* **Problemumgehungsoption**: Erstellen Sie einen Auszug aus einem Arbeitsblattbildschirm anstelle des Source-Bereichs für Daten in Tableau. Die Verbindung geht nicht verloren und der Extraktionsvorgang wird abgeschlossen.
