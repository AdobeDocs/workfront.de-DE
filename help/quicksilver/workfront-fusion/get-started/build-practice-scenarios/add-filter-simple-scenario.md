---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Hinzufügen eines Filters zu einem Basisszenario
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: b43355ed-9329-4080-8e61-7177eb580994
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# Hinzufügen eines Filters zu einem einfachen Szenario in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Hinzufügen eines Filters zu einem Basisszenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/build-practice-scenarios/add-filter-basic-scenario.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit Filtern können Sie sicherstellen, dass Ihr Szenario nur fortschreitet, wenn bestimmte Bedingungen erfüllt sind.

In diesem Beispiel fügen Sie Ihrem Szenario einen Filter hinzu, mit dem ein neues Projekt nur dann aus einer Anfrage erstellt werden kann, wenn die Anfrage an eine bestimmte Anfrage-Warteschlange gesendet wurde.

Dieses Beispiel ändert das in erstellte Szenario [Erstellen eines einfachen Szenarios](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront-Trigger-Module enthalten Filter, die den Start eines Szenarios nur ermöglichen, wenn bestimmte Bedingungen erfüllt sind. Da jedoch für jeden Anwendungsfall, bei dem es sich nicht um einen Trigger Workfronts handelt, Filter zwischen Modulen verwendet werden, ist es wichtig zu erfahren, wie Sie Filter zwischen Modulen verwenden können. In diesem Beispiel wird ein Filter zwischen Modulen für Funktionen verwendet, die mit einem Filter innerhalb des Moduls erfüllt werden könnten.

## Voraussetzungen

Sie müssen das unter &quot;[ eines einfachen Szenarios“ beschriebene Szenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) bevor Sie dieses Verfahren ausführen.

## Filter hinzufügen

### Vorbereiten des Hinzufügens des Filters

1. Öffnen Sie das erste Szenario.
1. Wählen Sie **Bereich** Ausgaben“ `Project` aus.
Sie sollten jetzt `ID`, `Name` und `Project` ausgewählt haben.
1. Klicken Sie auf OK , um die Moduleinstellungen zu speichern.
1. Öffnen Sie Workfront.
1. Suchen Sie in Workfront das Projekt, das die Anfrage-Warteschlange darstellt, mit der das Fusionsszenario arbeiten soll.

   Dieses Projekt muss sich in demselben Workfront-Konto befinden, für das die Fusion-Verbindung eingerichtet ist.

1. Notieren Sie sich die Projekt-ID in der URL.

   Beispiel: https://\&lt;MyDomain\>.my.workfront.com/project/\&lt;ProjectID\>/tasks

### Hinzufügen und Konfigurieren des Filters

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Klicken Sie auf das Schraubenschlüsselsymbol ![Schraubenschlüsselsymbol](assets/wrench-icon.png) zwischen dem ersten und zweiten Modul und wählen Sie **Filter einrichten** aus.
1. Geben Sie im Feld Titel einen Titel für diesen Filter ein, z. B. „Filter für Anfrage-Warteschlange“.
1. Ordnen Sie **Bereich** Bedingung“ im oberen Feld die `projectID` des ersten Moduls zu.

   ![Projekt-ID zuordnen](assets/map-proj-id.png)
1. Belassen Sie **Operator** Bedingung) auf Gleich.
1. Fügen Sie im unteren Feld des Bereichs **Bedingung** die Projekt-ID ein, die Sie über die Projekt-URL in notiert haben [Vorbereiten des Filters](#prepare-to-add-the-filter).
1. Klicken Sie **OK**, um die Filtereinstellungen zu speichern.

### Testen und Aktivieren

1. Wechseln Sie zur Workfront-Umgebung, mit der sich Fusion verbindet, und fügen Sie dem Projekt, das Sie im Filter angegeben haben, ein Problem hinzu. Ein weiteres Problem zu einem anderen Projekt hinzufügen.
1. Klicken Sie **[!UICONTROL Einmal ausführen]** in der linken unteren Ecke des Szenario-Editors.
1. Überprüfen Sie die Ausgabe, um sicherzustellen, dass das Szenario erwartungsgemäß ausgeführt wurde.

   Beide Probleme sollten in der Ausgabe des ersten Szenarios angezeigt werden, aber nur das Problem im angegebenen Projekt sollte als Eingabe in das zweite Szenario erscheinen.
1. Wenn Sie sich vergewissert haben, dass das Szenario erwartungsgemäß funktioniert, klicken Sie auf **Umschalter** Planung“ unten links im Bildschirm auf **Ein**.

   Dadurch wird das Szenario aktiviert.
1. Klicken Sie [!DNL Workfront Fusion] auf **[!UICONTROL Speichern]** in der linken unteren Ecke, um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie häufig, während Sie ein Szenario verfeinern und testen.

## Ressourcen

* Weitere Informationen zu Filtern finden Sie unter [Hinzufügen eines Filters zu einem Szenario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
