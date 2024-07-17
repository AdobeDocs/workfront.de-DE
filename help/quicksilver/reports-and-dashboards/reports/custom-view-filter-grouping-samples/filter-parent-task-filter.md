---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Übergeordnete Aufgaben anzeigen'
description: Sie können die folgenden Aufgabenfilter anwenden, um Arbeitsaufgaben anzuzeigen. Arbeitsaufgaben sind Aufgaben, die unabhängig bearbeitet werden können und keine übergeordneten Aufgaben für andere Aufgaben sind. In einem Beispiel identifiziert ein Filter untergeordnete Aufgaben, die selbst übergeordnete Elemente sein könnten. In diesem Fall arbeiten sie nicht mit Aufgaben.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4c3956e1-59e0-4bf2-8739-8064271d6281
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '760'
ht-degree: 1%

---

# Filter: Übergeordnete Aufgaben anzeigen

Sie können die folgenden Aufgabenfilter anwenden, um Arbeitsaufgaben anzuzeigen. Arbeitsaufgaben sind Aufgaben, die unabhängig bearbeitet werden können und keine übergeordneten Aufgaben für andere Aufgaben sind. In einem Beispiel identifiziert ein Filter untergeordnete Aufgaben, die selbst übergeordnete Elemente sein könnten. In diesem Fall arbeiten sie nicht mit Aufgaben.

>[!TIP]
>
>* Wenn Sie in Erwägung ziehen, einem Bericht mehr als einen Filter hinzuzufügen, empfehlen wir, alle Filter über die ReportBuilder-Oberfläche hinzuzufügen und nach dem Hinzufügen aller anderen Filterregeln auf In Textmodus wechseln zu klicken. Anschließend können Sie den Code für den Filter für die übergeordnete Aufgabe wie oben beschrieben hinzufügen. 
>* Es wird außerdem empfohlen, eine Gruppierung für den Projektnamen hinzuzufügen, um den Bericht leichter lesbar zu machen. Weitere Informationen zum Hinzufügen von Gruppierungen zu Berichten finden Sie im Artikel [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).
>

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Filteranforderung </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aufgaben ohne untergeordnete Elemente anzeigen (sie können übergeordnete Elemente haben)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um Aufgaben ohne untergeordnete Elemente anzuzeigen. Sie könnten eigene Eltern haben und Kinder anderer Aufgaben sein.

1. Klicken Sie im **Hauptmenü** ![](assets/main-menu-icon.png) auf **Berichte**.

1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht** aus.
1. Klicken Sie auf **Filter**.
1. Klicken Sie auf **Filterregel hinzufügen**.
1. Geben Sie in die Zeile **Feldname eingeben...** den Wert **Anzahl der untergeordneten Elemente** ein.

1. Wählen Sie **Equal (Case Sensitive)** für Ihren Modifikator und geben Sie dann **0** für die Anzahl der untergeordneten Elemente ein.\
   ![](assets/parent-task-filter-from-the-ui-350x76.png)

   Oder

   Klicken Sie auf **In den Textmodus wechseln** und kopieren Sie im Textbearbeitungsfenster den folgenden Text und fügen Sie ihn ein: 

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   ```


1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben abgerufen, die in Ihrem System Aufgaben ausführen. Einige dieser Aufgaben können übergeordnet sein, sind jedoch keine übergeordneten Aufgaben.

## Aufgaben mit übergeordneten Elementen anzeigen (sie können untergeordnete Elemente haben)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um Aufgaben mit übergeordneten Elementen anzuzeigen, d. h. sie sind untergeordnete Aufgaben. Diese Aufgaben können jedoch auch eigene untergeordnete Elemente haben, da der Filter ihre untergeordneten Elemente nicht ausschließt. Untergeordnete Aufgaben, die auch übergeordnete Elemente für andere Aufgaben sind, werden nicht als Arbeitsaufgaben betrachtet.

1. Klicken Sie im **Hauptmenü** ![](assets/main-menu-icon.png) auf &quot;Berichte&quot;.
1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht** aus.
1. Klicken Sie auf **Filter**.
1. Klicken Sie auf **Filterregel hinzufügen**.
1. Geben Sie in die Zeile **Feldname eingeben...** den Wert **Übergeordnete ID** ein.
1. Wählen Sie **Ist nicht leer** für Ihren Modifikator aus.

   ![](assets/filter-parent-id-not-blank-350x100.png)

   Oder

   Klicken Sie auf **In den Textmodus wechseln** und kopieren Sie im Textbearbeitungsfenster den folgenden Text und fügen Sie ihn ein: 

   `parentID_Mod=notblank`

1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben in Ihrem System abgerufen, die Eltern und untergeordnete Aufgaben dieser Eltern sind. Einige dieser Aufgaben können selbst übergeordnet sein.

## Aufgaben ohne untergeordnete Elemente und keine übergeordneten Elemente anzeigen (eigenständige Aufgaben)

Sie können den folgenden Filter auf einen Aufgabenbericht anwenden, um eigenständige Arbeitsaufgaben anzuzeigen. Diese Aufgaben haben kein Elternteil und keine eigenen Kinder.

1. Klicken Sie im **Hauptmenü** ![](assets/main-menu-icon.png) auf **Berichte**.
1. Klicken Sie auf **Neuer Bericht**.
1. Wählen Sie einen **Aufgabenbericht** aus.
1. Klicken Sie auf **Filter**.
1. Klicken Sie auf **Filterregel hinzufügen** und geben Sie in der Zeile **Feldname eingeben ...** den Zeileneintrag **Anzahl der untergeordneten Elemente** den Wert **Gleich (Groß-/Kleinschreibung beachten)** für Ihren Modifikator ein. Geben Sie dann für die Anzahl der untergeordneten Elemente den Wert **0** ein.
1. Klicken Sie auf **Andere Filterregel hinzufügen** und geben Sie in der Zeile **Feldname eingeben ...** den Zeileneintrag **Übergeordnete ID** ein und wählen Sie dann **Ist leer** aus.

   ![](assets/filter-parent-id-blank-and-zero-children-350x121.png)

   Oder

   Klicken Sie anstelle der Schritte 6 bis 7 auf **In den Textmodus wechseln** und kopieren Sie im Textbearbeitungsfenster den folgenden Text und fügen Sie ihn ein: 

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure steps above stay accurate)</p>
   -->

   ```
   numberOfChildren=0
   numberOfChildren_Mod=eq
   parentID_Mod=isblank
   ```

1. Klicken Sie auf **Speichern + schließen**.

   Dadurch wird ein Bericht für alle Aufgaben in Ihrem System abgerufen, die keine Eltern oder Kinder haben. Dies sind eigenständige Arbeitsaufgaben.
