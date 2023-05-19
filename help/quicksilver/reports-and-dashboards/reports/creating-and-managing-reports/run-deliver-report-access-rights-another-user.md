---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Einen Bericht mit Zugriffsrechten für einen anderen Benutzer ausführen und bereitstellen
description: Standardmäßig können Benutzer nur die Objekte in einem Bericht sehen, für die sie zur Ansicht berechtigt sind.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: e68e470da3b03e418584898c4098f0be302c68ec
workflow-type: tm+mt
source-wordcount: '1206'
ht-degree: 0%

---

# Einen Bericht mit Zugriffsrechten für einen anderen Benutzer ausführen und bereitstellen

Standardmäßig können Benutzer nur die Objekte in einem Bericht sehen, für die sie zur Ansicht berechtigt sind.

Sie können allen Benutzern gestatten, in einem Bericht dieselben Ergebnisse anzuzeigen wie anderen Benutzern, unabhängig von ihrer Zugriffsebene oder Berechtigungsstufe für die Objekte im Bericht.

Wenn Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen, der einen höheren Zugriff hat (z. B. die Zugriffsrechte eines Adobe Workfront-Administrators), können alle Benutzer, die zur Ansicht des Berichts berechtigt sind, die Informationen im Bericht als den in ReportBuilder angegebenen Benutzer anzeigen. Sie können dies für beide Berichte einrichten, die Benutzer in der Benutzeroberfläche von Workfront finden, oder für Berichte, die an Benutzer als Anhang zu einer E-Mail gesendet werden.

>[!TIP]
>
>Sie sollten die **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** nur dann mit einem aktiven Benutzer verknüpft werden, wenn der Bericht mit den Zugriffsrechten dieses Benutzers angezeigt werden soll. Beispielsweise kann ein Benutzer mit einer Arbeits-Lizenz nicht berechtigt sein, alle Elemente in einem Bericht anzuzeigen, der von einem Planungs-Lizenzbenutzer oder einem Systemadministrator erstellt wurde, es sei denn, der Bericht wird mit den Zugriffsrechten eines Planers oder Systemadministrators angezeigt.\
Wenn der Bericht für Benutzer mit ähnlichem Zugriff wie der in der Variablen **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** ein, können Sie dieses Feld leer lassen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht anzeigen (zum Anzeigen des gelieferten Berichts)</p> <p>Berechtigungen für einen Bericht verwalten (zum Ausführen des Berichts)</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Bericht mit Zugriffsrechten für einen anderen Benutzer anzeigen

Füllen der **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** -Feld stellt sicher, dass ein Bericht die gleichen Daten enthält, unabhängig davon, welcher Benutzer auf den Bericht zugreift. Der Bericht wird so angezeigt wie für den angegebenen Benutzer.

Die Benutzer, die auf den Bericht zugreifen, müssen mindestens über Anzeigeberechtigungen für den Bericht verfügen, damit sie ihn sehen können. Wenn der Benutzer in der **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** deaktiviert ist, wird der Bericht nicht mehr für andere Benutzer angezeigt, für die der Bericht freigegeben ist.

So führen Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers aus:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Berichte**.

1. Wählen Sie den Bericht aus, der mit den Zugriffsrechten eines anderen Benutzers angezeigt werden soll.
1. Klicken **Berichtaktionen** Klicken Sie auf **Bearbeiten**.

1. Klicken **Berichtseinstellungen**.

1. Im **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** ein, geben Sie den Namen des Benutzers ein, als den der Bericht angezeigt werden soll, und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.\
   ![](assets/qs-access-rights-of-350x251.png)

   >[!NOTE]
   Benutzer mit einer niedrigeren Zugriffsebene, die Berichte erstellen dürfen, können keinen anderen Benutzer als sich für die **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** -Feld.

1. Klicken **Fertig**.
1. Klicken **Speichern und schließen**.\
   Der Bericht wird nun für alle Benutzer angezeigt, für die der Bericht freigegeben ist, als ob er von dem in der Variablen **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** -Feld.

>[!IMPORTANT]
Eingeben eines anderen Benutzers als des angemeldeten Benutzers für die **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** wirkt sich auf die im Bericht angezeigten Informationen aus, wenn der Bericht einen Filter enthält, der einen Platzhalter verwendet, der auf den angemeldeten Benutzer verweist. Der Bericht wird entsprechend dem Wert angezeigt, der in der Variablen **Führen Sie diesen Bericht mit den Zugriffsrechten von aus:** -Feld anstelle des im Platzhalterfilter definierten Felds.
Weitere Informationen zu Platzhaltern für Benutzerfelder finden Sie im Abschnitt &quot;Benutzerbasierte Variablen&quot;unter [Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Bericht mit Zugriffsrechten eines anderen Benutzers bereitstellen

Sie können Berichte einrichten, die als Anhang an eine E-Mail gesendet werden. Sie können diese bereitgestellten Berichte so einrichten, dass sie für Benutzer mit einer höheren Zugriffsebene angezeigt werden, sodass alle Benutzer dieselben Informationen in den gelieferten Berichten sehen können. Die Benutzer, die den in der E-Mail gesendeten Bericht sehen werden, müssen zur Liste der Empfänger im Berichtversand hinzugefügt werden. Weitere Informationen zum Einrichten eines Berichts für die Bereitstellung finden Sie im Artikel [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

So senden Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Berichte**.

1. Wählen Sie den Bericht aus, den Sie mit den Zugriffsrechten eines anderen Benutzers bereitstellen möchten.
1. Klicken Sie auf den Namen des Berichts, um ihn auszuwählen.
1. Klicken **Berichtaktionen**.
1. Klicken **Bericht senden**.

1. Im **Stellen Sie diesen Bericht mit den Zugriffsrechten von bereit:** eingeben, den Namen des Benutzers eingeben, den der Bericht anzeigen soll, als er in einer E-Mail versendet wird, und ihn dann auswählen, wenn er in der Liste angezeigt wird. Die Standardeinstellung ist der Name des Benutzers, der den Bericht erstellt.\
   ![](assets/qs-send-report-access-rights-of-350x446.png)

   >[!NOTE]
   Benutzer mit einer niedrigeren Zugriffsebene, die Berichte erstellen dürfen, können keinen anderen Benutzer als sich für die **Stellen Sie diesen Bericht mit den Zugriffsrechten von bereit:** -Feld.

1. Wählen Sie die **Format** Sie möchten, dass der Bericht in der E-Mail angezeigt wird:

   * HTML
   * PDF
   * MS Excel
   * MS Excel (.xlsx)
   * TSV

1. Klicken **Jetzt senden** , um es sofort zu versenden.\
   Oder\
   Klicken **Wiederholen der Bereitstellung** um einen wiederkehrenden Versand für den Bericht zu planen.\
   Weitere Informationen zu Berichtbereitstellungen finden Sie im Artikel [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Einschränkungen für Berichte mit einer Quellspalte

Die folgenden Berichte zeigen eine Quellspalte an, in der Sie Informationen zum übergeordneten Objekt anzeigen können:

* Problemberichte
* Stündliche Berichte
* Dokumentberichte

Wenn Benutzer keine Berechtigungen für das übergeordnete Objekt eines Problems, einer Stunde oder eines Dokuments haben, wird die Spalte Quelle des Berichts leer angezeigt, selbst wenn der Bericht für die Anzeige konfiguriert ist oder mit den Zugriffsrechten eines anderen Benutzers bereitgestellt werden soll.

Um Informationen über das übergeordnete Objekt im Bericht anzuzeigen, wird empfohlen, eine Spalte für das übergeordnete Objekt hinzuzufügen, in der der Name des übergeordneten Objekts angezeigt werden kann.

Sie können beispielsweise Folgendes zu einem Bericht mit einer Quellspalte hinzufügen:

* Die Spalten &quot;Projektname&quot;, &quot;Aufgabenname&quot;oder &quot;Problemname&quot;in einem Dokument- oder Stundenbericht.
* Die Spalten Projektname oder Aufgabenname für einen Problembericht.
* Eine Spalte mit Textmodusausdrücken, die auf alle drei Objekte verweisen. Im Folgenden finden Sie ein Beispiel für einen Stundenbericht:

   `displayname=Custom Source`

   `linkedname=opTask`

   `namekey=view.relatedcolumn`

   `namekeyargkey.0=opTask`

   `namekeyargkey.1=name`

   `textmode=true`

   `valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))`

   `valueformat=HTML`

   Weitere Informationen zu Textmodusansichten finden Sie unter [Bearbeiten einer Ansicht im Textmodus](../text-mode/edit-text-mode-in-view.md).