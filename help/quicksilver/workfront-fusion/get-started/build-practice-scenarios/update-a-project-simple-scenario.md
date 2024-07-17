---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Trigger-Modul zu einem Basisszenario hinzufügen
description: Erfahren Sie, wie Sie ein Trigger-Modul hinzufügen, damit das Szenario regelmäßig nach neuen Anforderungen sucht und sie in Projekte konvertiert.
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Verwenden Sie eine Funktion zum Aktualisieren eines Projekts in einem einfachen Szenario in [!DNL Adobe Workfront Fusion]

Das Aktualisieren eines Workfront-Arbeitselements ist ein gängiges Anwendungsbeispiel für Workfront Fusion. In diesem Beispiel verwenden Sie eine Funktion, um den Namen eines Projekts in Großbuchstaben zu ändern.

Fusion umfasst viele Funktionsarten, mit denen Sie Daten umwandeln und bedingte Logik ausführen können. Weitere Informationen zur Verwendung von Funktionen finden Sie unter [Zuordnen von Informationen zwischen Modulen in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Dieses Beispiel ändert das Szenario, das in [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) erstellt wurde.

## Voraussetzungen

Sie müssen das unter [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) beschriebene Szenario erstellen, bevor Sie dieses Verfahren befolgen.

## Verwenden einer Funktion zum Aktualisieren eines Projekts

### Fügen Sie Ihrem Szenario das Modul Datensatz aktualisieren hinzu.

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Bewegen Sie den Mauszeiger über den Teilkreis rechts neben dem des Moduls und klicken Sie dann auf **[!UICONTROL Neues Modul hinzufügen]**.
1. Wählen Sie [!DNL Adobe Workfront] aus der Liste der Anwendungen und dann das Modul **[!UICONTROL Datensatz aktualisieren]**.
1. Wählen Sie im Feld ID den ID-Block aus, der sich unter dem Objektmodul Convert befindet. Dies ist die ID des Projekts, das von diesem Modul ausgegeben wurde.

   ![ID aus dem Convert-Objekt](assets/id-convert-object.png)

1. Wählen Sie im Feld &quot;Record Type&quot;die Option Project aus, da das zu aktualisierende Objekt ein Projekt ist.
1. Wählen Sie im Bereich Zu zuordnende Felder auswählen die Option Name aus.

   Daraufhin wird das Feld Name geöffnet.

### Funktion für Namensaktualisierung zuordnen

Wenn in diesem Szenario eine Anforderung in ein Projekt konvertiert wird, ist der Projektname mit der Anforderung identisch. Die Funktion nimmt diesen Namen und schreibt alle Buchstaben in ihr.

1. Klicken Sie auf das Feld **Name** .

   Das Zuordnungsfenster wird geöffnet.
1. Klicken Sie im Zuordnungsfenster auf das Symbol **Text und Binärfunktionen** . ![Symbol für Textfunktionen](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Wählen Sie die Funktion **upper** aus.

   Die Funktion wird im Feld Name angezeigt, einschließlich der Formatierung für die erwartete Eingabe.

   Die Eingabe für dieses Beispiel ist der Name des Problems, aus dem das Projekt konvertiert wurde.

1. Bewegen Sie den Cursor zwischen die Klammern, da dort die Eingabe erfolgt.
1. Klicken Sie im Zuordnungsfenster auf das Symbol **Modulausgabe** . ![Ausgabesymbol des Moduls](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Wählen Sie den Namensblock aus, der von Ihrem ersten Modul ausgegeben wurde.

   Der Namensblock wird in der Funktion angezeigt.

   ![Name block in function](assets/map-name.png)

1. Klicken Sie auf OK , um die Moduleinstellungen zu speichern.

### Testen und Aktivieren

1. Testen Sie das Szenario, indem Sie in der linken unteren Ecke des Bildschirms auf **Einmal ausführen** klicken.
1. Überprüfen Sie die Ausgabe, um sicherzustellen, dass das Szenario erwartungsgemäß ausgeführt wurde.
1. Wenn Sie sich davon überzeugt haben, dass das Szenario erwartungsgemäß funktioniert, klicken Sie auf den Umschalter **Planung** unten links im Bildschirm auf **Ein** .

   Dadurch wird das Szenario aktiviert. Aktive Szenarien werden gemäß dem im Trigger-Modul festgelegten Zeitplan ausgeführt.
1. Klicken Sie in [!DNL Workfront Fusion] unten links auf **[!UICONTROL Speichern]** , um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

## Ressourcen:

* [Elemente mithilfe von Funktionen in [!DNL Adobe Workfront Fusion] zuordnen](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
