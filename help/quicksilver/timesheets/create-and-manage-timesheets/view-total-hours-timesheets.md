---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Anzeigen der Gesamtstunden in einer Arbeitszeittabelle
description: Sie können die Gesamtzahl der Stunden auf Ihrer Arbeitszeittabelle anzeigen. Die Gesamtzahl der Arbeitszeittabellen-Stunden umfasst die für Projekte, Aufgaben, Probleme protokollierten Stunden sowie alle allgemeinen Stunden.
author: Lisa
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
TQID: https://experienceleague.adobe.com/oh6bBQz6sfxCpodHahZXtlMMuYYT-4U7-5MP6TQeuIs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 10%
---
# Anzeigen der Gesamtstunden in einer Arbeitszeittabelle

<!--Audited: 8/2024-->

Sie können die Gesamtzahl der Stunden auf Ihrer Arbeitszeittabelle anzeigen. Die Gesamtzahl der Arbeitszeittabellen-Stunden umfasst die für Projekte, Aufgaben, Probleme protokollierten Stunden sowie alle allgemeinen Stunden.

Die Gesamtstunden spiegeln die Stunden wider, die über die Arbeitszeittabelle, den Bereich „Aktualisierungen“ oder für Projekte, Aufgaben oder Probleme im Bereich „Stunden“ eingereicht wurden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td> <p>Licht oder höher </p>
   <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme anzeigen oder erhöhen</p> </td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für Aufgaben und Probleme</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Die Gesamtstunden einer Arbeitszeittabelle in der Kopfzeile der Arbeitszeittabelle anzeigen

Die Gesamtstunden einer Arbeitszeittabelle können Sie in der Kopfzeile der Arbeitszeittabelle einsehen.

![Feld „Gesamtstunden“](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## Zeigen Sie die Gesamtstunden auf Ihrer Arbeitszeittabelle in einer Liste von Arbeitszeittabellen an

{{step1-to-timesheets}}

Alle Arbeitszeittabellen, auf die Sie Zugriff haben, werden standardmäßig angezeigt.

![Arbeitszeittabellen-Liste](assets/list-of-all-timesheets.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Arbeitszeittabellen zu aktualisieren:

   * Wählen Sie **Meine Arbeitszeittabellen-Genehmigungen** in der rechten oberen Ecke der Seite aus, um nur die von Ihnen genehmigten Arbeitszeittabellen anzuzeigen.

     ODER

     Wählen Sie **Meine Arbeitszeittabellen** aus, um nur Ihre Arbeitszeittabellen anzuzeigen.

     Dadurch werden die Filter **Meine Arbeitszeittabellen-Genehmigungen** oder **Meine Arbeitszeittabelle** auf die Liste der Arbeitszeittabellen angewendet.

   * Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-nwepng.png), um einen Filter anzuwenden oder einen neuen Filter zu erstellen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Die Optionen Meine Arbeitszeittabellen-Genehmigungen und Meine Arbeitszeittabellen werden nicht oben in der Arbeitszeittabellenliste oder in der Filterliste angezeigt, wenn Workfront-Admins oder Gruppenadmins diese Filter entweder aus den Listensteuerelementen im Bereich Setup oder aus Ihrer Layoutvorlage entfernt haben. Weitere Informationen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Optional) Klicken Sie auf **Ansicht** ![Ansichtssymbol](assets/view-icon.png) oder **Gruppierung** ![Gruppierungssymbol](assets/grouping.png), um eine Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Die Gesamtstundenzahl für jede Arbeitszeittabelle wird in der Spalte **Gesamtstunden** angezeigt.

   ![Spalte „Gesamtstunden“](assets/total-hours-column.png)

   >[!TIP]
   >
   >Bei Verwendung der Standardansicht für eine Liste von Arbeitszeittabellen wird die Spalte Gesamtstunden rot angezeigt, wenn die für die Elemente in der Arbeitszeittabelle protokollierte Zeit die Anzahl der Stunden im Zeitrahmen der Arbeitszeittabelle überschreitet. Weitere Informationen finden Sie im Feld „Gesamtstunden“ im [Glossar der Adobe Workfront-](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).
