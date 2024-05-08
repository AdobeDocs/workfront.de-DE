---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Filter zu einem einfachen Szenario hinzufügen
description: Mit Filtern können Sie sicherstellen, dass Ihr Szenario nur weitergeht, wenn bestimmte Bedingungen erfüllt sind.
author: Becky
feature: Workfront Fusion
source-git-commit: 5ba5b2e37e2ce58d96d11f24786feef57f8eb638
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Filter zu einem einfachen Szenario hinzufügen in [!DNL Adobe Workfront Fusion]

Mit Filtern können Sie sicherstellen, dass Ihr Szenario nur weitergeht, wenn bestimmte Bedingungen erfüllt sind.

In diesem Beispiel fügen Sie Ihrem Szenario einen Filter hinzu, mit dem ein neues Projekt nur dann aus einer Anforderung erstellt werden kann, wenn die Anforderung an eine bestimmte Anforderungswarteschlange gesendet wurde.

Dieses Beispiel ändert das Szenario, das in [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md).

>[!NOTE]
>
>Workfront-Trigger-Module enthalten Filter, mit denen ein Szenario nur gestartet werden kann, wenn bestimmte Bedingungen erfüllt sind. Da jedoch zwischen Modulfiltern für jeden Anwendungsfall ohne Trigger und Nicht-Workfront verwendet werden, ist es wichtig, zu lernen, wie Sie Filter zwischen Modulen verwenden. In diesem Beispiel wird ein Filter zwischen Modulen für Funktionen verwendet, die mit einem In-Modul-Filter erfüllt werden können.

## Voraussetzungen

Sie müssen das Szenario erstellen, das unter [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) vor der Anwendung dieses Verfahrens.

## Filter hinzufügen

### Vorbereiten des Hinzufügens des Filters

1. Öffnen Sie das erste Szenario.
1. Im **Ausgaben** Bereich, auswählen `Project`.
Sie sollten jetzt `ID`, `Name`, und `Project` ausgewählt ist.
1. Klicken Sie auf OK , um die Moduleinstellungen zu speichern.
1. Öffnen Sie Workfront.
1. Suchen Sie in Workfront das Projekt, das die Anforderungswarteschlange darstellt, mit der das Fusion-Szenario arbeiten soll.

   Dieses Projekt muss sich in demselben Workfront-Konto befinden, für das die Fusion-Verbindung eingerichtet ist.

1. Notieren Sie sich die Projekt-ID in der URL.

   Beispiel: https://\&lt;mydomain>.my.workfront.com/project/\&lt;projectid>/tasks

### Filter hinzufügen und konfigurieren

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Klicken Sie auf das Schraubenschlüsselsymbol ![Schraubensymbol](assets/wrench-icon.png) zwischen dem ersten und dem zweiten Modul und wählen Sie **Filter einrichten**.
1. Geben Sie im Feld Titel einen Titel für diesen Filter ein, z. B. &quot;Nach Anforderungswarteschlange filtern&quot;.
1. Im **Bedingung** -Bereich im oberen Feld die `projectID` aus dem ersten Modul.

   ![Projekt-ID zuordnen](assets/map-proj-id.png)
1. Lassen Sie die **Bedingung** Operator als Gleich.
1. Im unteren Feld der **Bedingung** -Bereich, fügen Sie die Projekt-ID ein, die Sie aus der Projekt-URL in [Vorbereiten des Hinzufügens des Filters](#prepare-to-add-the-filter).
1. Klicks **OK** , um die Filtereinstellungen zu speichern.

### Testen und Aktivieren

1. Wechseln Sie zur Workfront-Umgebung, mit der Fusion eine Verbindung herstellen soll, und fügen Sie dem Projekt, das Sie im Filter angegeben haben, ein Problem hinzu. Fügen Sie einem anderen Projekt ein anderes Problem hinzu.
1. Klicks **[!UICONTROL Einmal ausführen]** in der linken unteren Ecke des Szenario-Editors.
1. Überprüfen Sie die Ausgabe, um sicherzustellen, dass das Szenario erwartungsgemäß ausgeführt wurde.

   Beide Probleme sollten in der Ausgabe des ersten Szenarios angezeigt werden, aber nur das Problem im angegebenen Projekt sollte als Eingabe im zweiten Szenario angezeigt werden —
1. Wenn Sie sich davon überzeugt haben, dass das Szenario erwartungsgemäß funktioniert, klicken Sie auf das **Planung** in der linken unteren Ecke des Bildschirms auf **on**.

   Dadurch wird das Szenario aktiviert.
1. In [!DNL Workfront Fusion]klicken **[!UICONTROL Speichern]** in der Nähe der linken unteren Ecke, um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

## Ressourcen

* Weitere Informationen zu Filtern finden Sie unter [Hinzufügen eines Filters zu einem Szenario](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

