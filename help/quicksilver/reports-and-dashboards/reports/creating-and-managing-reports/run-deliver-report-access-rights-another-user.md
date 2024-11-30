---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Einen Bericht mit Zugriffsrechten für einen anderen Benutzer ausführen und bereitstellen
description: Standardmäßig können Benutzer nur die Objekte in einem Bericht sehen, für die sie zur Ansicht berechtigt sind.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Einen Bericht mit Zugriffsrechten für einen anderen Benutzer ausführen und bereitstellen

<!-- Audited: 11/2024 -->

Standardmäßig können Benutzer nur die Objekte in einem Bericht sehen, für die sie zur Ansicht berechtigt sind.

Sie können allen Benutzern gestatten, in einem Bericht dieselben Ergebnisse anzuzeigen wie anderen Benutzern, unabhängig von ihrer Zugriffsebene oder Berechtigungsstufe für die Objekte im Bericht.

Wenn Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen, der einen höheren Zugriff hat (z. B. die Zugriffsrechte eines Adobe Workfront-Administrators), können alle Benutzer, die zur Ansicht des Berichts berechtigt sind, die Informationen im Bericht als den in ReportBuilder angegebenen Benutzer anzeigen. Sie können dies für beide Berichte einrichten, die Benutzer in der Benutzeroberfläche von Workfront finden, oder für Berichte, die an Benutzer als Anhang zu einer E-Mail gesendet werden.

>[!TIP]
>
>Sie sollten das Feld **Diesen Bericht ausführen durch das Feld Zugriffsrechte von:** durch einen aktiven Benutzer ersetzen, wenn der Bericht mit den Zugriffsrechten dieses Benutzers angezeigt werden soll. Beispielsweise kann ein Benutzer mit einer Arbeits-Lizenz nicht berechtigt sein, alle Elemente in einem Bericht anzuzeigen, der von einem Planungs-Lizenzbenutzer oder einem Systemadministrator erstellt wurde, es sei denn, der Bericht wird mit den Zugriffsrechten eines Planers oder Systemadministrators angezeigt.\
>Wenn der Bericht für Benutzer mit ähnlichem Zugriff wie der im Feld **Diesen Bericht mit Zugriffsrechten ausführen von:** angegebene Benutzer freigegeben ist, können Sie dieses Feld leer lassen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
      <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht anzeigen (zum Anzeigen des gelieferten Berichts)</p><p>Berechtigungen für einen Bericht verwalten (zum Ausführen des Berichts)</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bericht mit Zugriffsrechten für einen anderen Benutzer anzeigen

Wenn Sie das Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** ausfüllen, wird sichergestellt, dass ein Bericht die gleichen Daten enthält, unabhängig davon, welcher Benutzer auf den Bericht zugreift. Der Bericht wird so angezeigt wie für den angegebenen Benutzer.

Die Benutzer, die auf den Bericht zugreifen, müssen mindestens über Anzeigeberechtigungen für den Bericht verfügen, damit sie ihn sehen können. Wenn der im Feld **Diesen Bericht ausführen mit Zugriffsrechten von:** angegebene Benutzer deaktiviert ist, wird der Bericht nicht mehr für andere Benutzer angezeigt, für die der Bericht freigegeben ist.

So führen Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers aus:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Berichte]**.

1. Wählen Sie den Bericht aus, der mit den Zugriffsrechten eines anderen Benutzers angezeigt werden soll.
1. Klicken Sie auf **Berichtaktionen** und dann auf **Bearbeiten**.

1. Klicken Sie auf **Berichtseinstellungen**.

1. Geben Sie im Feld **Diesen Bericht mit Zugriffsrechten ausführen von:** den Namen des Benutzers ein, als den der Bericht angezeigt werden soll, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.\
   ![](assets/unshimmed-access-rights-of.png)

   >[!NOTE]
   >
   >Benutzer mit einer niedrigeren Zugriffsebene, die Berichte erstellen dürfen, können keinen anderen Benutzer als sich selbst für das Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** auswählen.

1. Klicken Sie auf **Fertig**.
1. Klicken Sie auf **Speichern + schließen**.\
   Der Bericht wird nun für alle Benutzer angezeigt, für die der Bericht freigegeben ist, als ob er von dem im Feld **Diesen Bericht mit Zugriffsrechten ausführen von:** angegebenen Benutzer angezeigt wurde.

>[!IMPORTANT]
>
>Wenn Sie einen anderen Benutzer als den angemeldeten Benutzer für das Feld **Diesen Bericht ausführen mit Zugriffsrechten von:** eingeben, wirkt sich dies auf die im Bericht angezeigten Informationen aus, wenn der Bericht einen Filter enthält, der einen Platzhalter verwendet, der auf den angemeldeten Benutzer verweist. Der Bericht wird entsprechend dem Wert angezeigt, der im Feld **Diesen Bericht mit dem Feld Zugriffsberechtigungen ausführen von:** angegeben wurde, anstatt dem, was im Platzhalterfilter definiert ist.
>
>Weitere Informationen zu Platzhaltern für Benutzerfelder finden Sie im Abschnitt &quot;Benutzerbasierte Variablen&quot;in der [Übersicht über Wildcard-Filtervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Bericht mit Zugriffsrechten eines anderen Benutzers bereitstellen

Sie können Berichte einrichten, die als Anhang an eine E-Mail gesendet werden. Sie können diese bereitgestellten Berichte so einrichten, dass sie für Benutzer mit einer höheren Zugriffsebene angezeigt werden, sodass alle Benutzer dieselben Informationen in den gelieferten Berichten sehen können. Die Benutzer, die den in der E-Mail gesendeten Bericht sehen werden, müssen zur Liste der Empfänger im Berichtversand hinzugefügt werden. Weitere Informationen zum Einrichten eines Berichts für die Bereitstellung finden Sie im Artikel [Übersicht über die Berichtbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

So senden Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers:

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Workfront und klicken Sie dann auf **Berichte**.![](assets/main-menu-icon.png)

1. Wählen Sie den Bericht aus, den Sie mit den Zugriffsrechten eines anderen Benutzers bereitstellen möchten.
1. Klicken Sie auf den Namen des Berichts, um ihn auszuwählen.
1. Klicken Sie auf **Berichtaktionen**.
1. Klicken Sie auf **Bericht senden**.

1. Geben Sie im Feld **Diesen Bericht mit den Zugriffsrechten von:** an, wie der Bericht in einer E-Mail-Versand dargestellt werden soll, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. Die Standardeinstellung ist der Name des Benutzers, der den Bericht erstellt.\
   ![](assets/unshimmed-send-report-access-rights-of.png)

   >[!NOTE]
   >
   >Benutzer mit einer niedrigeren Zugriffsebene, die Berichte erstellen dürfen, können keinen anderen Benutzer als sich selbst für das Feld **Diesen Bericht mit den Zugriffsrechten von:** bereitstellen auswählen.

1. Wählen Sie das **Format** aus, das der Bericht in der E-Mail anzeigen soll:

   * HTML
   * PDF
   * Excel
   * Excel (.xlsx)
   * TSV

1. Klicken Sie auf **Jetzt senden** , um es sofort zu senden.\
   Oder\
   Klicken Sie auf **Wiederholen Versand durchführen** , um einen wiederkehrenden Versand für den Bericht zu planen.\
   Weitere Informationen zu Berichtbereitstellungen finden Sie im Artikel [Übersicht über die Berichtbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Einschränkungen für Berichte mit einer Source-Spalte

Die folgenden Berichte zeigen eine Source-Spalte an, in der Sie Informationen zum übergeordneten Objekt anzeigen können:

* Problemberichte
* Stündliche Berichte
* Dokumentberichte

Wenn Benutzer keine Berechtigungen für das übergeordnete Objekt eines Problems, einer Stunde oder eines Dokuments haben, wird die Source-Spalte des Berichts leer angezeigt, selbst wenn der Bericht für die Anzeige oder Bereitstellung mit den Zugriffsrechten eines anderen Benutzers konfiguriert ist.

Um Informationen über das übergeordnete Objekt im Bericht anzuzeigen, wird empfohlen, eine Spalte für das übergeordnete Objekt hinzuzufügen, in der der Name des übergeordneten Objekts angezeigt werden kann.

Sie können beispielsweise Folgendes zu einem Bericht mit einer Source-Spalte hinzufügen:

* Die Spalten &quot;Projektname&quot;, &quot;Aufgabenname&quot;oder &quot;Problemname&quot;in einem Dokument- oder Stundenbericht.
* Die Spalten &quot;Projektname&quot;oder &quot;Aufgabenname&quot;für einen Problembericht.
* Eine Spalte mit Textmodusausdrücken, die auf alle drei Objekte verweisen. Im Folgenden finden Sie ein Beispiel für einen Stundenbericht:

  ```
  displayname=Custom Source
  
  linkedname=opTask
  
  namekey=view.relatedcolumn
  
  namekeyargkey.0=opTask
  
  namekeyargkey.1=name
  
  textmode=true
  
  valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))
  
  valueformat=HTML
  ```

  Weitere Informationen zu Textmodusansichten finden Sie unter [Bearbeiten einer Ansicht im Textmodus](../text-mode/edit-text-mode-in-view.md).