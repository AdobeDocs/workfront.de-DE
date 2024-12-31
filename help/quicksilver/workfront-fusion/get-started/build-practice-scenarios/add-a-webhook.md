---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Hinzufügen eines Webhooks zu einem Basisszenario
description: Webhooks, auch als Instant Trigger bezeichnet, sind eine spezielle Art von Szenariomodul, das ein Trigger starten kann, wenn eine Änderung vorgenommen wird, anstatt nach einem bestimmten Zeitplan.
author: Becky
feature: Workfront Fusion
exl-id: 6694b883-6f94-449c-bcfe-5a4053e8655a
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Hinzufügen eines Webhooks zu einem einfachen Szenario in [!DNL Adobe Workfront Fusion]

Webhooks, auch als Instant Trigger bezeichnet, sind eine spezielle Art von Szenariomodul, das ein Trigger starten kann, wenn eine Änderung vorgenommen wird, anstatt nach einem bestimmten Zeitplan.

In diesem Beispiel fügen Sie einen Webhook hinzu, um ein Szenario zu starten, sobald Anforderungen an eine bestimmte Warteschlange gesendet wurden. Das Szenario konvertiert diese Anfragen dann in ein Projekt.

Dieses Beispiel ändert das in erstellte Szenario [Erstellen eines einfachen Szenarios](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Voraussetzungen

Sie müssen das unter &quot;[ eines einfachen Szenarios“ beschriebene Szenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) bevor Sie dieses Verfahren ausführen.

## Webhook hinzufügen und konfigurieren

1. Öffnen Sie das Modul Objekt konvertieren .
1. Löschen Sie im Feld „Anfrage-ID“ den Block „Schwarze ID“. Der Block ist schwarz, da das Modul, von dem aus er zugeordnet wurde, nicht mehr verfügbar ist.
1. Wählen Sie den ID-Block unter dem ersten Modul (Ereignisse beobachten) aus, um ihn dem zweiten Modul zuzuordnen.
1. Klicken Sie **OK**.

### Webhook-Modul hinzufügen

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Klicken Sie mit der rechten Maustaste auf das erste Modul und wählen Sie **Modul löschen**.

   Das Modul wird gelöscht, wobei ein leerer Platzhalter verbleibt.

1. Klicken Sie auf das leere Modul und wählen Sie **Adobe Workfront** aus der Liste der Apps aus.
1. Wählen Sie **Ereignisse ansehen** aus.
1. Klicken Sie **Hinzufügen** neben dem Feld Webhook .
1. Wählen Sie im Feld Datensatztyp die Option **Problem** aus, damit das Modul einen Trigger für Änderungen bei Problemen durchführt.
1. Wählen Sie im Feld Status die Option **Neuer Status**. Dies ist ein Pflichtfeld, das für den Filter verwendet wird, der in diesem Beispiel nicht abgedeckt wird.
1. Wählen Sie im Feld Datensatzherkunft die Option **Nur neuer Datensatz**. Dadurch kann das Szenario einen Trigger auslösen, wenn ein Problem hinzugefügt wird, und nicht, wenn ein Problem aktualisiert oder gelöscht wird.
1. Klicken Sie **Speichern**, um die Modulkonfiguration zu speichern.
