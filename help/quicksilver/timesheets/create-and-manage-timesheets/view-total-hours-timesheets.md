---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Gesamtstunden auf dem Timesheet anzeigen
description: Sie können die Gesamtanzahl der Stunden auf Ihrem Zeitblatt anzeigen. Die Gesamtanzahl der Timesheet-Stunden umfasst die protokollierten Stunden für Projekte, Aufgaben, Probleme und alle allgemeinen Stunden.
author: Alina
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

# Gesamtstunden auf dem Timesheet anzeigen

Sie können die Gesamtanzahl der Stunden auf Ihrem Zeitblatt anzeigen. Die Gesamtanzahl der Timesheet-Stunden umfasst die protokollierten Stunden für Projekte, Aufgaben, Probleme und alle allgemeinen Stunden.

Die Gesamtstunden beziehen sich auf Stunden, die über das Timesheet, den Bereich Updates oder im Bereich Stunden für Projekte, Aufgaben oder Probleme gesendet wurden.

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
   <td> <p>Überarbeitung </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff oder höher auf Aufgaben und Probleme anzeigen</p> <p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Höhere Berechtigungen für Aufgaben und Probleme</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben.

## Gesamtstunden eines Zeitblatts in der Kopfzeile des Zeitblatts anzeigen

Sie können die Gesamtstunden eines Zeitblatts in der Kopfzeile des Zeitblatts anzeigen.

![](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Anzeigen der Gesamtstunden auf Ihrem Timesheet in einer Liste von Timesheets

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Timesheets**. Die **Alle** -Filter ist standardmäßig ausgewählt und zeigt alle Timesheets an, auf die Sie Zugriff haben.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Timesheets zu aktualisieren:

   * Auswählen **Meine Datenblatt-Genehmigungen** oben rechts auf der Seite, um nur die von Ihnen genehmigten Timesheets anzuzeigen

      Oder

      Auswählen **Meine Timesheets** , um nur Ihre Timesheets anzuzeigen.

      Dadurch wird die Liste der Timesheets mit den Filtern My Timesheet Approvals oder My Timesheet aktualisiert.

      ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf das Filtersymbol ![](assets/filter-nwepng.png) um einen anderen Filter anzuwenden oder einen neuen zu erstellen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Filter in Adobe Workfront erstellen oder bearbeiten](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).
   >[!NOTE]
   >
   >Die Optionen Meine Timesheet-Genehmigungen und Meine Timesheets werden nicht oben in der Timesheet-Liste oder in der Filterliste angezeigt, wenn Ihr Workfront-Administrator oder ein Gruppenadministrator die Filter Meine Timesheet-Genehmigungen und Meine Timesheets entweder aus den Listen-Steuerelementen im Bereich Einrichtung oder aus Ihrer Layout-Vorlage entfernt hat. Weitere Informationen finden Sie in den folgenden Artikeln:
   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)


1. (Optional) Klicken Sie auf die **Ansicht** ![](assets/view-icon.png) oder **Gruppierung** ![](assets/grouping.png) Symbole, um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Filter in Adobe Workfront erstellen oder bearbeiten](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Die Gesamtzahl der Stunden für jedes Zeitblatt wird im **Stunden insgesamt** Spalte.

   ![](assets/total-hours-column-highlighted-all-timesheets-list-nwe-350x120.png)

   >[!TIP]
   Bei Verwendung der Standardansicht für eine Liste von Timesheets wird die Spalte Gesamtstunden in Rot angezeigt, wenn die für die Elemente auf dem Timesheet protokollierte Zeit die Anzahl der Stunden im Zeitrahmen des Zeitblatts überschreitet. Weitere Informationen finden Sie im Feld &quot;Gesamtstunden&quot;unter [Glossar der Adobe Workfront-Terminologie](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
