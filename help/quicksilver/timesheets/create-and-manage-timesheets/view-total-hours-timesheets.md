---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Gesamtstunden auf dem Timesheet anzeigen
description: Sie können die Gesamtanzahl der Stunden auf Ihrem Timesheet anzeigen. Die Gesamtanzahl der Timesheet-Stunden umfasst die protokollierten Stunden für Projekte, Aufgaben, Probleme und alle allgemeinen Stunden.
author: Alina
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Gesamtstunden auf dem Timesheet anzeigen

<!--Audited: 8/2024-->

Sie können die Gesamtanzahl der Stunden auf Ihrem Timesheet anzeigen. Die Gesamtanzahl der Timesheet-Stunden umfasst die protokollierten Stunden für Projekte, Aufgaben, Probleme und alle allgemeinen Stunden.

Die Gesamtstunden beziehen sich auf Stunden, die über das Timesheet, den Bereich Updates oder im Bereich Stunden für Projekte, Aufgaben oder Probleme gesendet wurden.

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
   <td> <p>Neu: Licht oder höher </p>
   <p>Aktuell: Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme anzeigen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Höhere Berechtigungen für Aufgaben und Probleme</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gesamtstunden eines Zeitblatts in der Kopfzeile des Zeitblatts anzeigen

Sie können die Gesamtstunden eines Zeitblatts in der Kopfzeile des Zeitblatts anzeigen.

![](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Anzeigen der Gesamtstunden auf Ihrem Timesheet in einer Liste von Timesheets

{{step1-to-timesheets}}

Der Bereich **Timesheets** wird geöffnet.

![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Timesheets zu aktualisieren:

   * Wählen Sie oben rechts auf der Seite die Option **My Timesheet Approvals** aus, um nur die von Ihnen genehmigten Zeitpläne anzuzeigen

     Oder

     Wählen Sie **Meine Timesheets** aus, um nur Ihre Timesheets anzuzeigen.

     Dadurch wird die Liste der Timesheets mit den Filtern My Timesheet Approvals oder My Timesheet aktualisiert.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf das Filtersymbol ![](assets/filter-nwepng.png) , um einen anderen Filter anzuwenden, oder erstellen Sie einen neuen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Die Optionen Meine Timesheet-Genehmigungen und Meine Timesheets werden nicht oben in der Timesheet-Liste oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator die Filter Meine Timesheet-Genehmigungen und Meine Timesheets entweder aus den Listen-Steuerelementen im Bereich Einrichtung oder aus Ihrer Layout-Vorlage entfernt hat. Weitere Informationen finden Sie in den folgenden Artikeln:
   >
   >   
   >   
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Optional) Klicken Sie auf die Symbole **Ansicht** ![](assets/view-icon.png) oder **Gruppierung** ![](assets/grouping.png) , um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Die Gesamtstundenzahl für jedes Zeitblatt wird in der Spalte **Gesamtstunden** angezeigt.

   ![](assets/total-hours-column-highlighted-all-timesheets-list-nwe-350x120.png)

   >[!TIP]
   >
   >Bei Verwendung der Standardansicht für eine Liste von Timesheets wird die Spalte Gesamtstunden in Rot angezeigt, wenn die für die Elemente auf dem Timesheet protokollierte Zeit die Anzahl der Stunden im Zeitrahmen des Zeitblatts überschreitet. Weitere Informationen finden Sie im Feld &quot;Gesamtstunden&quot;im [Glossar der Adobe Workfront-Terminologie](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
