---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Webhook zu einem grundlegenden Szenario hinzufügen
description: Webhooks, auch als Instant Trigger bezeichnet, sind ein spezifisches Trigger-Modul, das bei jeder Änderung und nicht nach einem bestimmten Zeitplan ein Szenario starten kann.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 0%

---

# Einen Webhook zu einem grundlegenden Szenario hinzufügen in [!DNL Adobe Workfront Fusion]

Webhooks, auch als Instant Trigger bezeichnet, sind ein spezifisches Trigger-Modul, das bei jeder Änderung und nicht nach einem bestimmten Zeitplan ein Szenario starten kann.

In diesem Beispiel fügen Sie einen Webhook hinzu, um ein Szenario zu starten, sobald Anforderungen an eine bestimmte Warteschlange gesendet wurden. Das Szenario konvertiert diese Anforderungen dann in ein Projekt.

Dieses Beispiel ändert das Szenario, das in [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Voraussetzungen

Sie müssen das Szenario erstellen, das unter [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) vor der Anwendung dieses Verfahrens.

## Webhook hinzufügen und konfigurieren

1. Öffnen Sie das Objektmodul Konvertieren .
1. Löschen Sie im Feld Ausgabe-ID den schwarzen ID-Block. Der Block ist schwarz, da das Modul, von dem er zugeordnet wurde, nicht mehr verfügbar ist.
1. Wählen Sie den ID-Block unter dem ersten Modul (Überwachungsereignisse) aus, um ihn dem zweiten Modul zuzuordnen.
1. Klicks **OK**.

### Webhook-Modul hinzufügen

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Klicken Sie mit der rechten Maustaste auf das erste Modul und wählen Sie **Modul löschen**.

   Das -Modul wird gelöscht, wobei ein leerer Platzhalter verbleibt.

1. Klicken Sie auf das leere Modul und wählen Sie **Adobe Workfront** aus der Liste der Apps.
1. Auswählen **Ereignisse beobachten**.
1. Klicks **Hinzufügen** neben dem Webhook-Feld.
1. Wählen Sie im Feld &quot;Record Type&quot;die Option **Problem**, sodass das -Modul auf Änderungen in Problemen Trigger.
1. Wählen Sie im Feld Status die Option **Neuer Status**. Dies ist ein erforderliches Feld, das für den Filter verwendet wird, das in diesem Beispiel nicht behandelt wird.
1. Wählen Sie im Feld &quot;Record Origin&quot;die Option **Nur neuer Datensatz**. Dadurch kann das Szenario beim Hinzufügen eines Problems Trigger werden, nicht beim Aktualisieren oder Löschen.
1. Klicks **Speichern** , um die Modulkonfiguration zu speichern.


