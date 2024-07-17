---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Bericht ausführen
description: Sie können jeden Bericht ausführen, auf den Sie Zugriff haben.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 61fcb4c3646f60fa5f667d874af3320360d5d286
workflow-type: tm+mt
source-wordcount: '528'
ht-degree: 0%

---


# Bericht ausführen

Sie können jeden Bericht ausführen, auf den Sie Zugriff haben.

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender anzeigen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht anzeigen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Bericht ausführen

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Berichte**.![](assets/main-menu-icon.png)

1. Wählen Sie aus den folgenden Optionen aus:

   * **Meine Berichte:** Von Ihnen erstellte Berichte.
   * **Für mich freigegeben:** Berichte, die von anderen Benutzern für Sie freigegeben wurden.
   * **Alle Berichte:** Alle Berichte im System, auf die Sie Zugriff haben.

1. Klicken Sie auf den Namen des Berichts, den Sie ausführen möchten.\
   Oder\
   Wenn der Bericht mit Eingabeaufforderungen erstellt wurde, wählen Sie die entsprechenden Informationen aus den Dropdown-Menüs aus und klicken Sie dann auf **Bericht ausführen**.\
   Weitere Informationen zu Eingabeaufforderungen finden Sie unter [Eine Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   Der Inhalt des Berichts wird mit einem Zeitstempel in der oberen rechten Ecke des Berichts angezeigt, der das Datum, die Uhrzeit und die Zeitzone enthält, zu der der Bericht aus dem Kontext des Benutzers ausgeführt wurde, der den Bericht ausgeführt hat.

1. (Optional) Klicken Sie auf das Symbol **Neu laden** ![](assets/qs-report-refresh-icon.png) , um die Ergebnisse in einem Bericht zu aktualisieren, wenn der Bericht bereits seit einiger Zeit in Ihrem Browser angezeigt wird.

1. (Bedingt) Wenn der Bericht Filter oder Eingabeaufforderungen verwendet, klicken Sie auf **Filter und Eingabeaufforderungen anzeigen** , um eine Liste mit Filtern und Eingabeaufforderungen anzuzeigen, die für den angezeigten Bericht verwendet werden. Wenn der Bericht nur Filter oder nur Eingabeaufforderungen enthält, wird stattdessen **Filter anzeigen** oder **Eingabeaufforderungen anzeigen** angezeigt.

   ![Filter und Eingabeaufforderungen anzeigen](assets/qs-reports-showfiltersandprompts-2022-350x136.png)

   Informationen werden unter dem Berichtnamen auf der linken Seite der Seite angezeigt. Bei Eingabeaufforderungen handelt es sich um Informationen zu den Eingabeaufforderungen, die zum Zeitpunkt der Berichterstellung getroffen wurden, wie in Schritt 4 beschrieben.

1. Wenn Sie benutzerdefinierte Eingabeaufforderungen verwenden, werden diese nicht angezeigt. Nur die Systemaufforderungen werden angezeigt. Benutzerdefinierte Filter werden immer angezeigt.

## Zwischengespeicherten Bericht anzeigen

Ihr Bericht kann zwischengespeichert werden, wenn er bereits seit einiger Zeit in Ihrem Browser angezeigt wird. Sie können das Neuladen eines zwischengespeicherten Berichts erzwingen, wenn Sie eine der folgenden Aktionen durchführen:

* Bearbeiten Sie die Berichtseinstellungen und speichern Sie den Bericht.
* Ändern Sie die Ansicht, Gruppe oder den Filter.
* Klicken Sie auf das Symbol **Neu laden**
Diese Option ist rechts oben auf der Seite im Meldungsfeld verfügbar, das die Speicherzeit des Berichts angibt, oder in der oberen rechten Ecke des Dashboards, in dem der Bericht platziert wird. Weitere Informationen zum Neuladen von Dashboards finden Sie im Abschnitt &quot;Dashboards anzeigen&quot;im Artikel [Erste Schritte mit Dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md) .

* Greifen Sie über die erste Seite hinaus auf eine beliebige Seite des Berichts zu, indem Sie zu den Registerkarten &quot;Zusammenfassung&quot;, &quot;Matrix&quot;oder &quot;Diagramm&quot;navigieren.
