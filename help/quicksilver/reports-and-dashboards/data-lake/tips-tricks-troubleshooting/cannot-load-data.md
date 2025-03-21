---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop kann keine Verbindung herstellen
description: Beim Versuch, eine Verbindung zwischen Tableau Desktop und Data Connect herzustellen, wird ein Fehler angezeigt.
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

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

