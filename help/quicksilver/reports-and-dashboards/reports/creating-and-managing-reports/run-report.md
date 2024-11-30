---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Bericht ausführen
description: Sie können jeden Bericht ausführen, auf den Sie Zugriff haben.
author: Nolan
feature: Reports and Dashboards
exl-id: bd2202a7-040c-4291-ad02-ba8929a37e2b
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---


# Bericht ausführen

Sie können jeden Bericht ausführen, auf den Sie Zugriff haben.

<!-- Audited: 11/2024 -->

<!--
NOTE: ***Linked to Getting Started with Reporting.***This information is obsolete, because asynchronous timeline is not enabled for all customers (used to be included in the "Viewing a Cached Report" section): Some reports in Workfront can take a significant time to load. If your report takes longer than 30 seconds to load, your report is cached after it is finished loading, and a message is displayed in the upper-right corner of the page indicating that the report being viewed is a saved report from a specific time.

After a report is cached, it is available for the next 12 hours. Any user who runs the report (as described in "Running a Report") sees the cached report.)
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender anzeigen</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht anzeigen</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bericht ausführen

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Berichte]**.

1. Wählen Sie aus den folgenden Optionen aus:

   * **Meine Berichte:** Von Ihnen erstellte Berichte.
   * **Für mich freigegeben:** Berichte, die von anderen Benutzern für Sie freigegeben wurden.
   * **Alle Berichte:** Alle Berichte im System, auf die Sie Zugriff haben.

1. Klicken Sie auf den Namen des Berichts, den Sie ausführen möchten.\
   Oder\
   Wenn der Bericht mit Eingabeaufforderungen erstellt wurde, wählen Sie die entsprechenden Informationen aus den Dropdown-Menüs aus und klicken Sie dann auf **Bericht ausführen**.\
   Weitere Informationen zu Eingabeaufforderungen finden Sie unter [Eine Eingabeaufforderung zu einem Bericht hinzufügen](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).\
   Der Inhalt des Berichts wird mit einem Zeitstempel in der oberen rechten Ecke des Berichts angezeigt, der das Datum, die Uhrzeit und die Zeitzone enthält, zu der der Bericht aus dem Kontext des Benutzers ausgeführt wurde, der den Bericht ausgeführt hat.

1. (Optional) Klicken Sie auf das Symbol **Neu laden** ![Neu laden](assets/unshimmed-report-refresh-icon.png) , um die Ergebnisse in einem Bericht zu aktualisieren, wenn der Bericht bereits seit einiger Zeit in Ihrem Browser angezeigt wird.

1. (Bedingt) Wenn der Bericht Filter oder Eingabeaufforderungen verwendet, klicken Sie auf **Filter und Eingabeaufforderungen anzeigen** , um eine Liste mit Filtern und Eingabeaufforderungen anzuzeigen, die für den angezeigten Bericht verwendet werden. Wenn der Bericht nur Filter oder nur Eingabeaufforderungen enthält, wird stattdessen **Filter anzeigen** oder **Eingabeaufforderungen anzeigen** angezeigt.

   ![Filter und Eingabeaufforderungen anzeigen](assets/unshimmed-show-filters-and-prompts.png)

   Informationen werden unter dem Berichtnamen auf der linken Seite der Seite angezeigt. Bei Eingabeaufforderungen handelt es sich um Informationen zu den Eingabeaufforderungen, die zum Zeitpunkt der Berichterstellung getroffen wurden, wie in Schritt 3 beschrieben.

1. Wenn Sie benutzerdefinierte Eingabeaufforderungen verwenden, werden diese nicht angezeigt. Nur die Systemaufforderungen werden angezeigt. Benutzerdefinierte Filter werden immer angezeigt.

## Zwischengespeicherten Bericht anzeigen

Ihr Bericht kann zwischengespeichert werden, wenn er bereits seit einiger Zeit in Ihrem Browser angezeigt wird. Sie können das Neuladen eines zwischengespeicherten Berichts erzwingen, wenn Sie eine der folgenden Aktionen durchführen:

* Bearbeiten Sie die Berichtseinstellungen und speichern Sie den Bericht.
* Ändern Sie die Ansicht, Gruppe oder den Filter.
* Klicken Sie auf das Symbol **Neu laden** ![Neuladungssymbol](assets/unshimmed-report-refresh-icon.png)
Diese Option ist rechts oben auf der Seite im Meldungsfeld verfügbar, das die Speicherzeit des Berichts angibt, oder in der oberen rechten Ecke des Dashboards, in dem der Bericht platziert wird. Weitere Informationen zum Neuladen von Dashboards finden Sie im Abschnitt &quot;Dashboards anzeigen&quot;im Artikel [Erste Schritte mit Dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md) .

* Greifen Sie über die erste Seite hinaus auf eine beliebige Seite des Berichts zu, indem Sie zu den Registerkarten &quot;Zusammenfassung&quot;, &quot;Matrix&quot;oder &quot;Diagramm&quot;navigieren.
