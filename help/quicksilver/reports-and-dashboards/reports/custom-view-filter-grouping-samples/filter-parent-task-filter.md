---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Übergeordnete Aufgaben anzeigen'
description: Sie können die folgenden Aufgabenfilter anwenden, um Arbeitsaufgaben anzuzeigen. Arbeitsaufgaben sind Aufgaben, die unabhängig bearbeitet werden können und keine übergeordneten Aufgaben für andere Aufgaben sind. In einem Beispiel identifiziert ein Filter untergeordnete Aufgaben, die selbst übergeordnete Elemente sein könnten. In diesem Fall arbeiten sie nicht mit Aufgaben.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# Filter: Übergeordnete Aufgaben anzeigen

<!--Audited: 10/2024-->

Sie können die folgenden Aufgabenfilter anwenden, um Arbeitsaufgaben anzuzeigen. Arbeitsaufgaben sind Aufgaben, die unabhängig bearbeitet werden können und keine übergeordneten Aufgaben für andere Aufgaben sind. In einem Beispiel identifiziert ein Filter untergeordnete Aufgaben, die selbst übergeordnete Elemente sein könnten. In diesem Fall arbeiten sie nicht mit Aufgaben.

>[!TIP]
>
>* Wenn Sie in Erwägung ziehen, einem Bericht mehr als einen Filter hinzuzufügen, empfehlen wir, alle Filter über die ReportBuilder-Oberfläche hinzuzufügen und nach dem Hinzufügen aller anderen Filterregeln auf In Textmodus wechseln zu klicken. Anschließend können Sie den Code für den Filter für die übergeordnete Aufgabe wie oben beschrieben hinzufügen. 
>* Es wird außerdem empfohlen, eine Gruppierung für den Projektnamen hinzuzufügen, um den Bericht leichter lesbar zu machen. Weitere Informationen zum Hinzufügen von Gruppierungen zu Berichten finden Sie im Artikel [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aufgaben ohne untergeordnete Elemente anzeigen (sie können übergeordnete Elemente haben)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um Aufgaben ohne untergeordnete Elemente anzuzeigen. Sie könnten eigene Eltern haben und Kinder anderer Aufgaben sein.

1. Klicken Sie oben rechts im Menü **Hauptmenü** ![](assets/main-menu-icon.png) oder, falls verfügbar, im Menü **Hauptmenü** ![](assets/lines-main-menu.png) oben links auf **Berichte**.

1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht** aus.
1. Klicken Sie auf **Filter**.
1. Klicken Sie auf **Filterregel hinzufügen**.
1. Geben Sie in die Zeile **Feldname eingeben...** den Wert **Anzahl der untergeordneten Elemente** ein und klicken Sie dann auf **Aufgabe >> Anzahl der untergeordneten Elemente** , wenn er in der Liste angezeigt wird.

1. Wählen Sie **Equal (Case Sensitive)** für Ihren Modifikator und geben Sie dann **0** für die Anzahl der untergeordneten Elemente ein.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Oder

   Klicken Sie auf **In den Textmodus wechseln** und kopieren Sie im Textbearbeitungsfenster den folgenden Text und fügen Sie ihn ein.

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben abgerufen, die in Ihrem System Aufgaben ausführen. Einige dieser Aufgaben können übergeordnet sein, sind jedoch keine übergeordneten Aufgaben.

## Aufgaben mit übergeordneten Elementen anzeigen (sie können untergeordnete Elemente haben)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um Aufgaben mit übergeordneten Elementen anzuzeigen, d. h. sie sind untergeordnete Aufgaben. Diese Aufgaben können jedoch auch eigene untergeordnete Elemente haben, da der Filter ihre untergeordneten Elemente nicht ausschließt. Untergeordnete Aufgaben, die auch übergeordnete Elemente für andere Aufgaben sind, werden nicht als Arbeitsaufgaben betrachtet.

1. Klicken Sie oben rechts im Menü **Hauptmenü** ![](assets/main-menu-icon.png) oder, falls verfügbar, im Menü **Hauptmenü** ![](assets/lines-main-menu.png) oben links auf **Berichte**.

1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht** aus.
1. Klicken Sie auf **Filter**.
1. Klicken Sie auf **Filterregel hinzufügen**.
1. Geben Sie in die Zeile **Feldname eingeben...** den Wert **Übergeordnete ID** ein und wählen Sie dann **Aufgabe >> Übergeordnete ID** aus, wenn sie in der Liste angezeigt wird.
1. Wählen Sie **Ist nicht leer** für Ihren Modifikator aus.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Oder

   Klicken Sie auf **In den Textmodus wechseln** und kopieren Sie im Textbearbeitungsfenster den folgenden Text und fügen Sie ihn ein: 

   `parentID_Mod=notblank`

1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben in Ihrem System abgerufen, die Eltern und untergeordnete Aufgaben dieser Eltern sind. Einige dieser Aufgaben können selbst übergeordnet sein.

## Aufgaben ohne untergeordnete Elemente und keine übergeordneten Elemente anzeigen (eigenständige Aufgaben)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um eigenständige Arbeitsaufgaben anzuzeigen. Diese Aufgaben haben kein Elternteil und keine eigenen Kinder.

1. Klicken Sie oben rechts im Menü **Hauptmenü** ![](assets/main-menu-icon.png) oder, falls verfügbar, im Menü **Hauptmenü** ![](assets/lines-main-menu.png) oben links auf **Berichte**.

1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht** aus.
1. Klicken Sie auf **Filter**.
1. Klicken Sie auf **Filterregel hinzufügen**.
1. Geben Sie in der Zeile **Feldname eingeben...** die Zeile **Anzahl der untergeordneten Elemente** ein und wählen Sie dann **Aufgabe >> Anzahl der untergeordneten Elemente** aus der Liste aus.
1. Wählen Sie **Equal (Case Sensitive)** für Ihren Modifikator und geben Sie dann **0** für die Anzahl der untergeordneten Elemente ein.
1. Klicken Sie auf **Hinzufügen einer weiteren Filterregel**.
1. Geben Sie in der Zeile **Feldname eingeben...** die Zeile **Übergeordnete ID** ein und wählen Sie dann **Aufgabe >> Übergeordnete ID** aus der Liste aus.
1. Wählen Sie **Ist leer** für den Modifikator aus.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Oder

   Klicken Sie anstelle der Schritte 6-10 <!--ensure steps above stay accurate--> auf **In den Textmodus wechseln** und kopieren Sie im Textbearbeitungsfenster den folgenden Text:

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben in Ihrem System abgerufen, die keine Eltern oder Kinder haben. Dies sind eigenständige Arbeitsaufgaben.
