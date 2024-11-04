---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Trigger-Modul zu einem Basisszenario hinzufügen
description: Erfahren Sie, wie Sie ein Trigger-Modul hinzufügen, damit das Szenario regelmäßig nach neuen Anforderungen sucht und sie in Projekte konvertiert.
author: Becky
feature: Workfront Fusion
exl-id: 067ee6a1-f4c1-4602-ac39-0283255cced8
source-git-commit: 7ad3fbcfa5be5074016f399560cca509d81f4714
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Trigger-Modul zu einem Basisszenario hinzufügen

Trigger-Module werden am Anfang eines Szenarios platziert. Diese Module beginnen die Ausführung eines Szenarios, wenn bestimmte Kriterien eine Änderung in einem bestimmten Dienst bewirken. Die Änderung kann in der Erstellung neuer Datensätze, dem Löschen von Datensätzen, dem Aktualisieren von Datensätzen usw. bestehen.

Abrufmodule überprüfen den Dienst in einem bestimmten Zeitintervall und geben Informationen zu Änderungen zurück, die während dieses Zeitintervalls aufgetreten sind. Wenn keine Änderungen vorgenommen wurden, führt der Trigger das Szenario nicht aus.

In diesem Beispiel fügen Sie ein Trigger-Modul hinzu, das alle 15 Minuten ausgeführt wird und ein Szenario startet, wenn Anforderungen an eine bestimmte Warteschlange gesendet wurden. Das Szenario konvertiert diese Anforderungen dann in ein Projekt.

Dieses Beispiel ändert das Szenario, das in [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) erstellt wurde.

## Voraussetzungen

Sie müssen das unter [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) beschriebene Szenario erstellen, bevor Sie dieses Verfahren befolgen.

## Hinzufügen und Konfigurieren des Trigger-Moduls

### Trigger-Modul hinzufügen

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Klicken Sie mit der rechten Maustaste auf das erste Modul (Suche) und wählen Sie **Modul löschen** aus.

   Das -Modul wird gelöscht, wobei ein leerer Platzhalter verbleibt.

1. Klicken Sie auf das leere Modul und wählen Sie **Adobe Workfront** aus der Liste der Apps aus.
1. Wählen Sie **Datensatz überwachen** aus.
1. Stellen Sie sicher, dass das Modul dieselbe Verbindung wie die anderen Module im Szenario verwendet.
1. Wählen Sie im Filterfeld **Nur neue Datensätze** aus.
1. Wählen Sie im Feld &quot;Record Type&quot;die Option **Issue** aus.
1. Wählen Sie im Feld &quot;Outputs&quot;die Optionen `ID`, `Name` und `Project ID` aus.
1. Klicken Sie auf **OK** , um die Moduleinstellungen zu speichern.

   Das Fenster Startort wird angezeigt.

1. Wählen Sie **Von jetzt an auf** aus.

### Trigger-Modul planen

1. Klicken Sie auf die Uhr im Modul &quot;Watch Records&quot;.

   Das Fenster Planung wird geöffnet.

1. Wählen Sie im Feld Ausführungsszenario die Option **In regelmäßigen Abständen** aus.

1. Klicken Sie auf **OK**.

### Zweites Modul aktualisieren

Da das erste Modul ersetzt wurde, muss das zweite Modul dem neuen ersten Modul zugeordnet werden.

1. Öffnen Sie das Objektmodul Konvertieren .
1. Löschen Sie im Feld Ausgabe-ID den schwarzen ID-Block. Der Block ist schwarz, da das Modul, von dem er zugeordnet wurde, nicht mehr verfügbar ist.
1. Wählen Sie den ID-Block unter dem ersten Modul (Listen überwachen) aus, um ihn dem zweiten Modul zuzuordnen.
1. Klicken Sie auf **OK**.

### Testen und Aktivieren

1. Wechseln Sie zur Workfront-Umgebung, mit der Fusion eine Verbindung herstellt, und fügen Sie ein Problem hinzu.
1. Klicken Sie in der linken unteren Ecke des Szenario-Editors auf **[!UICONTROL Einmal ausführen]** .
1. Überprüfen Sie die Ausgabe, um sicherzustellen, dass das Szenario erwartungsgemäß ausgeführt wurde.
1. Wenn Sie sich davon überzeugt haben, dass das Szenario erwartungsgemäß funktioniert, klicken Sie auf den Umschalter **Planung** unten links im Bildschirm auf **Ein** .

   Dadurch wird das Szenario aktiviert.
1. Klicken Sie in [!DNL Workfront Fusion] unten links auf **[!UICONTROL Speichern]** , um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

## Ressourcen

* Weitere Informationen zu Webhooks finden Sie unter [Instant Trigger (Webhooks) in  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
