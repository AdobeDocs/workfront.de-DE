---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Filter zu einem einfachen Szenario hinzufügen
description: Mit Filtern können Sie sicherstellen, dass Ihr Szenario nur weitergeht, wenn bestimmte Bedingungen erfüllt sind.
author: Becky
feature: Workfront Fusion
exl-id: b43355ed-9329-4080-8e61-7177eb580994
source-git-commit: 1a405d38968922388589ddb3f2979b4e59cd50b8
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 1%

---

# Filter zu einem einfachen Szenario in [!DNL Adobe Workfront Fusion] hinzufügen

Mit Filtern können Sie sicherstellen, dass Ihr Szenario nur weitergeht, wenn bestimmte Bedingungen erfüllt sind.

In diesem Beispiel fügen Sie Ihrem Szenario einen Filter hinzu, mit dem ein neues Projekt nur dann aus einer Anforderung erstellt werden kann, wenn die Anforderung an eine bestimmte Anforderungswarteschlange gesendet wurde.

Dieses Beispiel ändert das Szenario, das in [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) erstellt wurde.

>[!NOTE]
>
>Workfront-Trigger-Module enthalten Filter, mit denen ein Szenario nur gestartet werden kann, wenn bestimmte Bedingungen erfüllt sind. Da jedoch zwischen Modulfiltern für jeden Anwendungsfall ohne Trigger und Nicht-Workfront verwendet werden, ist es wichtig, zu lernen, wie Sie Filter zwischen Modulen verwenden. In diesem Beispiel wird ein Filter zwischen Modulen für Funktionen verwendet, die mit einem In-Modul-Filter erfüllt werden können.

## Voraussetzungen

Sie müssen das unter [Basisszenario erstellen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/create-simple-scenario.md) beschriebene Szenario erstellen, bevor Sie dieses Verfahren befolgen.

## Filter hinzufügen

### Vorbereiten des Hinzufügens des Filters

1. Öffnen Sie das erste Szenario.
1. Wählen Sie im Bereich **Ausgaben** die Option `Project` aus.
Jetzt sollten `ID`, `Name` und `Project` ausgewählt sein.
1. Klicken Sie auf OK , um die Moduleinstellungen zu speichern.
1. Öffnen Sie Workfront.
1. Suchen Sie in Workfront das Projekt, das die Anforderungswarteschlange darstellt, mit der das Fusion-Szenario arbeiten soll.

   Dieses Projekt muss sich in demselben Workfront-Konto befinden, für das die Fusion-Verbindung eingerichtet ist.

1. Notieren Sie sich die Projekt-ID in der URL.

   Beispiel: https://\&lt;MyDomain\>.my.workfront.com/project/\&lt;ProjectID\>/tasks

### Filter hinzufügen und konfigurieren

1. Öffnen Sie das Szenario im Szenario-Editor.
1. Klicken Sie zwischen dem ersten und dem zweiten Modul auf das Schraubenschlüsselsymbol ![Schraubenschlüsselsymbol](assets/wrench-icon.png) und wählen Sie **Filter einrichten**.
1. Geben Sie im Feld Titel einen Titel für diesen Filter ein, z. B. &quot;Nach Anforderungswarteschlange filtern&quot;.
1. Ordnen Sie im Bereich **Bedingung** im oberen Feld die `projectID` aus dem ersten Modul zu.

   ![Projekt-ID zuordnen](assets/map-proj-id.png)
1. Lassen Sie den Operator **Bedingung** gleich.
1. Fügen Sie im unteren Feld des Bereichs **Bedingung** die Projekt-ID ein, die Sie aus der Projekt-URL in [Vorbereiten des Hinzufügens des Filters](#prepare-to-add-the-filter) notiert haben.
1. Klicken Sie auf **OK** , um die Filtereinstellungen zu speichern.

### Testen und Aktivieren

1. Wechseln Sie zur Workfront-Umgebung, mit der Fusion eine Verbindung herstellen soll, und fügen Sie dem Projekt, das Sie im Filter angegeben haben, ein Problem hinzu. Fügen Sie einem anderen Projekt ein anderes Problem hinzu.
1. Klicken Sie in der linken unteren Ecke des Szenario-Editors auf **[!UICONTROL Einmal ausführen]** .
1. Überprüfen Sie die Ausgabe, um sicherzustellen, dass das Szenario erwartungsgemäß ausgeführt wurde.

   Beide Probleme sollten in der Ausgabe des ersten Szenarios angezeigt werden, aber nur das Problem im angegebenen Projekt sollte als Eingabe im zweiten Szenario angezeigt werden —
1. Wenn Sie sich davon überzeugt haben, dass das Szenario erwartungsgemäß funktioniert, klicken Sie auf den Umschalter **Planung** unten links im Bildschirm auf **Ein** .

   Dadurch wird das Szenario aktiviert.
1. Klicken Sie in [!DNL Workfront Fusion] unten links auf **[!UICONTROL Speichern]** , um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

## Ressourcen

* Weitere Informationen zu Filtern finden Sie unter [Filter zu einem Szenario hinzufügen](/help/quicksilver/workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).
