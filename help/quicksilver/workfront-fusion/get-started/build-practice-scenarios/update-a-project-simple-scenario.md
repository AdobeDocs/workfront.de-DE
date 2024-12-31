---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Hinzufügen eines Trigger-Moduls zu einem Basisszenario
description: Erfahren Sie, wie Sie ein Szenariomodul hinzufügen, damit das Trigger regelmäßig nach neuen Anfragen suchen und diese in Projekte konvertieren kann.
author: Becky
feature: Workfront Fusion
exl-id: f4588063-024f-4520-986e-45342a6b6777
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Verwenden einer Funktion zum Aktualisieren eines Projekts in einem einfachen Szenario in [!DNL Adobe Workfront Fusion]

Das Aktualisieren eines Workfront-Arbeitselements ist ein gängiges Anwendungsbeispiel für Workfront Fusion. In diesem Beispiel verwenden Sie eine Funktion, um den Namen eines Projekts so zu ändern, dass er in Großbuchstaben geschrieben wird.

Fusion enthält viele Arten von Funktionen, mit denen Sie bedingte Logik für Ihre Daten transformieren und ausführen können. Weitere Informationen zur Verwendung von Funktionen finden Sie unter [Zuordnen von Informationen von einem Modul zum anderen in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).

Dieses Beispiel ändert das in erstellte Szenario [Erstellen eines einfachen Szenarios](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

## Voraussetzungen

Sie müssen das unter &quot;[ eines einfachen Szenarios“ beschriebene Szenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) bevor Sie dieses Verfahren ausführen.

## Verwenden einer Funktion zum Aktualisieren eines Projekts

### Hinzufügen des Moduls Eintrag aktualisieren zu Ihrem Szenario

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Bewegen Sie den Mauszeiger über den Teilkreis rechts neben dem Modul und klicken Sie dann auf **[!UICONTROL Weitere Module hinzufügen]**.
1. Wählen Sie [!DNL Adobe Workfront] aus der Liste der Programme und dann das Modul **[!UICONTROL Eintrag aktualisieren]**.
1. Wählen Sie im Feld ID den ID-Block aus, der sich unter dem Modul Objekt konvertieren befindet. Dies ist die ID des Projekts, das von diesem Modul ausgegeben wurde.

   ![ID aus dem Konvertierungsobjekt](assets/id-convert-object.png)

1. Wählen Sie im Feld Datensatztyp die Option Projekt aus, da das zu aktualisierende Objekt ein Projekt ist.
1. Klicken Sie im Bereich Zuzuordnende Felder auswählen auf Name.

   Ein Namensfeld wird geöffnet.

### Zuordnen der Funktion für die Namensaktualisierung

Wenn dieses Szenario eine Anfrage in ein Projekt konvertiert, ist der Projektname mit der Anfrage identisch. Die Funktion übernimmt hier diesen Namen und schreibt alle Buchstaben groß.

1. Klicken Sie auf das **Name**.

   Das Zuordnungsbedienfeld wird geöffnet.
1. Klicken Sie im Zuordnungsbereich auf das Symbol **Text und binäre Funktionen** . ![Symbol für Textfunktionen](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-text&binary-functions.png)
1. Wählen Sie die Funktion **upper**.

   Die Funktion wird im Feld Name angezeigt, einschließlich der Formatierung für die erwartete Eingabe.

   Die Eingabe für dieses Beispiel ist der Name des Problems, aus dem das Projekt konvertiert wurde.

1. Bewegen Sie den Cursor zwischen den Klammern, denn hier wird die Eingabe eingefügt.
1. Klicken Sie im Zuordnungsbereich auf das Symbol **Modulausgabe** . ![Modul-Ausgabesymbol](/help/quicksilver/workfront-fusion/functions/assets/toolbar-icon-functions-you-map-from-other-modules.png)
1. Wählen Sie den Namensblock aus, der von Ihrem ersten Modul ausgegeben wurde.

   Der Block Name wird in der Funktion angezeigt.

   ![Namensblock in der Funktion](assets/map-name.png)

1. Klicken Sie auf OK , um die Moduleinstellungen zu speichern.

### Testen und Aktivieren

1. Testen Sie das Szenario, indem **Einmal ausführen** in der linken unteren Ecke des Bildschirms klicken.
1. Überprüfen Sie die Ausgabe, um sicherzustellen, dass das Szenario erwartungsgemäß ausgeführt wurde.
1. Wenn Sie sich vergewissert haben, dass das Szenario erwartungsgemäß funktioniert, klicken Sie auf **Umschalter** Planung“ unten links im Bildschirm auf **Ein**.

   Dadurch wird das Szenario aktiviert. Aktive Szenarien werden nach dem im Trigger-Modul festgelegten Zeitplan ausgeführt.
1. Klicken Sie [!DNL Workfront Fusion] auf **[!UICONTROL Speichern]** in der linken unteren Ecke, um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie häufig, während Sie ein Szenario verfeinern und testen.

## Ressourcen:

* [Zuordnen von Elementen mithilfe von Funktionen in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md)
