---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Trigger-Modul zu einem Basisszenario hinzufügen
description: Erfahren Sie, wie Sie ein Trigger-Modul hinzufügen, damit das Szenario regelmäßig nach neuen Anforderungen sucht und sie in Projekte konvertiert.
author: Becky
feature: Workfront Fusion
source-git-commit: ea3f932e02ad8a9416747d4b9aefe89d087dd414
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Trigger-Modul zu einem Basisszenario hinzufügen

Trigger-Module werden am Anfang eines Szenarios platziert. Diese Module beginnen die Ausführung eines Szenarios, wenn bestimmte Kriterien eine Änderung in einem bestimmten Dienst bewirken. Die Änderung kann in der Erstellung neuer Datensätze, dem Löschen von Datensätzen, dem Aktualisieren von Datensätzen usw. bestehen.

Abrufmodule überprüfen den Dienst in einem bestimmten Zeitintervall und geben Informationen zu Änderungen zurück, die während dieses Zeitintervalls aufgetreten sind. Wenn keine Änderungen vorgenommen wurden, führt der Trigger das Szenario nicht aus.

In diesem Beispiel fügen Sie ein Trigger-Modul hinzu, das alle 15 Minuten ausgeführt wird und ein Szenario startet, wenn Anforderungen an eine bestimmte Warteschlange gesendet wurden. Das Szenario konvertiert diese Anforderungen dann in ein Projekt.

Dieses Beispiel ändert das Szenario, das in [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Voraussetzungen

Sie müssen das Szenario erstellen, das unter [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) vor der Anwendung dieses Verfahrens.

## Hinzufügen und Konfigurieren des Trigger-Moduls

### Trigger-Modul hinzufügen

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Klicken Sie mit der rechten Maustaste auf das erste Modul (Suche) und wählen Sie **Modul löschen**.

   Das -Modul wird gelöscht, wobei ein leerer Platzhalter verbleibt.

1. Klicken Sie auf das leere Modul und wählen Sie **Adobe Workfront** aus der Liste der Apps.
1. Auswählen **Aufzeichnen von Daten**.
1. Stellen Sie sicher, dass das Modul dieselbe Verbindung wie die anderen Module im Szenario verwendet.
1. Wählen Sie im Feld Filter die Option **Nur neue Datensätze**.
1. Wählen Sie im Feld &quot;Outputs&quot;die Option `ID`, `Name`, und `Project ID`.
1. Klicks **OK** , um die Moduleinstellungen zu speichern.

   Das Fenster Startort wird angezeigt.

1. Auswählen **Von jetzt an**.

### Trigger-Modul planen

1. Klicken Sie auf die Uhr im Modul &quot;Watch Records&quot;.

   Das Fenster Planung wird geöffnet.

1. Wählen Sie im Feld Ausführungsszenario die Option **In regelmäßigen Abständen**.

1. Klicks **OK**.

### Zweites Modul aktualisieren

Da das erste Modul ersetzt wurde, muss das zweite Modul dem neuen ersten Modul zugeordnet werden.

1. Öffnen Sie das Objektmodul Konvertieren .
1. Löschen Sie im Feld Ausgabe-ID den schwarzen ID-Block. Der Block ist schwarz, da das Modul, von dem er zugeordnet wurde, nicht mehr verfügbar ist.
1. Wählen Sie den ID-Block unter dem ersten Modul (Listen überwachen) aus, um ihn dem zweiten Modul zuzuordnen.
1. Klicks **OK**.

### Testen und Aktivieren

1. Wechseln Sie zur Workfront-Umgebung, mit der Fusion eine Verbindung herstellt, und fügen Sie ein Problem hinzu.
1. Klicks **[!UICONTROL Einmal ausführen]** in der linken unteren Ecke des Szenario-Editors.
1. Überprüfen Sie die Ausgabe, um sicherzustellen, dass das Szenario erwartungsgemäß ausgeführt wurde.
1. Wenn Sie sich davon überzeugt haben, dass das Szenario erwartungsgemäß funktioniert, klicken Sie auf das **Planung** in der linken unteren Ecke des Bildschirms auf **on**.

   Dadurch wird das Szenario aktiviert.
1. In [!DNL Workfront Fusion]klicken **[!UICONTROL Speichern]** in der Nähe der linken unteren Ecke, um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

## Ressourcen

* Weitere Informationen zu Webhooks finden Sie unter [Sofortige Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/webhooks/instant-triggers-webhooks.md).
