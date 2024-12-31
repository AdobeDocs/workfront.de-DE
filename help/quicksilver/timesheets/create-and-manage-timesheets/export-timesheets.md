---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Exportieren einer Liste von Arbeitszeittabellen
description: Als Personen-Manager oder Arbeitszeittabellen-Genehmiger müssen Sie möglicherweise eine Liste von Arbeitszeittabellen herunterladen, um schnell Informationen zu den Arbeitszeittabellen der Personen anzuzeigen, für die Sie verantwortlich sind. Exportieren Sie dazu eine Liste von Arbeitszeittabellen.
author: Alina
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 2%

---

# Exportieren einer Liste von Arbeitszeittabellen

<!--Audited: 8/2024-->

Als Personen-Manager oder Arbeitszeittabellen-Genehmiger müssen Sie möglicherweise eine Liste von Arbeitszeittabellen herunterladen, um schnell Informationen zu den Arbeitszeittabellen der Personen anzuzeigen, für die Sie verantwortlich sind. Exportieren Sie dazu eine Liste von Arbeitszeittabellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Licht oder höher </p>
   <p>Aktuell: Überprüfung oder höher </p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme anzeigen oder erhöhen </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Hochladen von Berechtigungen für die Arbeitszeittabelle</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old permissions:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to Tasks and Issues</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the timesheets</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan or license type you have, contact your Workfront administrator.-->

## Exportieren einer Liste von Arbeitszeittabellen

{{step1-to-timesheets}}

Der Bereich **Arbeitszeittabellen** wird geöffnet.


![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Klicken Sie auf das **Suchen**-Symbol ![](assets/search-icon.png) geben Sie einen Suchbegriff ein und suchen Sie nach einer bestimmten Arbeitszeittabelle. Sie können beispielsweise nach einem Arbeitszeittabellen-Zeitrahmen oder Besitzernamen suchen.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Filter in der Liste der Arbeitszeittabellen zu aktualisieren:

   * Wählen Sie **Meine Arbeitszeittabellen-Genehmigungen** in der rechten oberen Ecke der Seite aus, um nur die von Ihnen genehmigten Arbeitszeittabellen anzuzeigen

     Oder

     Wählen Sie **Meine Arbeitszeittabellen** aus, um nur Ihre Arbeitszeittabellen anzuzeigen.

     Dadurch werden die Filter Meine Arbeitszeittabellen-Genehmigungen oder Meine Arbeitszeittabellen auf die Liste der Arbeitszeittabellen angewendet.

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * Klicken Sie auf das Filtersymbol ![](assets/filter-nwepng.png) , um einen anderen Filter anzuwenden, oder erstellen Sie einen neuen. Informationen zum Erstellen oder Aktualisieren von Filtern finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

   >[!NOTE]
   >
   >Die Optionen Meine Arbeitszeittabellen-Genehmigungen und Meine Arbeitszeittabellen werden nicht oben in der Arbeitszeittabellen-Liste oder in der Filterliste angezeigt, wenn Workfront-Admins oder Gruppenadmins die Filter Meine Arbeitszeittabellen und Meine Arbeitszeittabellen entweder aus den Listensteuerelementen im Setup-Bereich oder aus Ihrer Layoutvorlage entfernt haben. Weitere Informationen finden Sie in den folgenden Artikeln:
   >
   >   
   >   
   >   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. (Optional) Klicken Sie auf **Ansicht** ![](assets/view-icon.png) oder **Gruppierung** ![](assets/grouping.png), um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Wählen Sie die zu exportierenden Arbeitszeittabellen aus und klicken Sie dann auf das Symbol **Exportieren** ![](assets/export-38x15.png).

   ![](assets/all-timesheets-list-with-export-button-nwe-350x262.png)

1. Wählen Sie aus den folgenden Optionen den Dateityp aus, in den Sie die Liste der Arbeitszeittabellen exportieren möchten:

   * PDF Landscape
   * PDF Hochformat
   * PDF andere Größen
   * Excel
   * Excel (xlsx)
   * Durch Tabulatoren getrennt

   Eine Liste der Arbeitszeittabellen wird im ausgewählten Format auf den Computer heruntergeladen und enthält die folgenden Arbeitszeittabellen-Informationen:

   * Datumsbereich
   * Name der Eigentümerin bzw. des Eigentümers
   * Gesamtstunden
   * Zeitaufwand
   * Namen der genehmigenden Personen
   * Status
