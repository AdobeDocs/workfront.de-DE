---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Arbeitszeittabellen-Informationen bearbeiten
description: Benutzende mit administrativem Zugriff auf Arbeitszeittabellen können Informationen zu bestehenden Arbeitszeittabellen in Adobe Workfront bearbeiten. Sie können beispielsweise den Eigentümer, die genehmigenden Personen oder den Zeitrahmen der Arbeitszeittabelle bearbeiten.
author: Alina
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Arbeitszeittabellen-Informationen bearbeiten

Benutzende mit administrativem Zugriff auf Arbeitszeittabellen können Informationen zu bestehenden Arbeitszeittabellen in Adobe Workfront bearbeiten. Sie können beispielsweise den Eigentümer, die genehmigenden Personen oder den Zeitrahmen der Arbeitszeittabelle bearbeiten.

Sie können Informationen auf einer einzigen Arbeitszeittabelle bearbeiten oder mehrere Arbeitszeittabellen gleichzeitig bearbeiten.

>[!IMPORTANT]
>
>Wenn Benutzende mit Arbeitszeittabellen-Profilen verknüpft sind und die Arbeitszeittabellen automatisch generiert werden, werden die Änderungen, die Sie an vorhandenen Arbeitszeittabellen vornehmen, nicht in Arbeitszeittabellen übernommen, die für zukünftige Datumsangaben generiert werden. Für alle automatisch generierten Arbeitszeittabellen werden die Einstellungen in den Arbeitszeittabellen-Profilen festgelegt. Weitere Informationen finden Sie unter [Arbeitszeittabellen-Profile erstellen](../create-and-manage-timesheets/create-timesheet-profiles.md)


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Sie müssen administrativen Zugriff auf Arbeitszeittabellen haben. </p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Arbeitszeittabellen bearbeiten

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) oben rechts in Adobe Workfront und dann auf **Arbeitszeittabellen**.

   Der **Alle**-Filter ist standardmäßig ausgewählt. Er zeigt alle Arbeitszeittabellen an, auf die Sie Zugriff haben.

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. (Optional) Klicken Sie auf das **Suchen**-Symbol ![](assets/search-icon.png) geben Sie einen Suchbegriff ein und suchen Sie nach einer bestimmten Arbeitszeittabelle. Sie können beispielsweise nach einem Arbeitszeittabellen-Zeitrahmen oder einem Eigentümernamen suchen.

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

1. (Optional) Klicken Sie auf **Ansicht** ![](assets/view-icon.png) oder **Gruppierung** ![](assets/grouping.png) Symbole, um eine andere Ansicht oder Gruppierung anzuwenden oder eine neue zu erstellen.

   Informationen zum Erstellen von Filtern, Ansichten oder Gruppierungen finden Sie in den folgenden Artikeln:

   * [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Erstellen von Gruppierungen in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. Wählen Sie eine oder mehrere Arbeitszeittabellen aus und klicken Sie dann oben in **Arbeitszeittabellenliste auf** Bearbeiten![](assets/edit-icon.png).
1. Zeigen Sie die folgenden Informationen an oder geben Sie sie an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Besitzer bzw. Besitzerin</strong> </td> 
      <td> <p>Dies ist der Name des Benutzers, für den die Arbeitszeittabelle erstellt wurde. Dieses Feld kann nicht bearbeitet werden. </p> <p>Das Feld wird nicht angezeigt, wenn Sie mehrere Arbeitszeittabellen auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Startdatum</strong> </td> 
      <td>Dies ist das Startdatum der Arbeitszeittabelle.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Enddatum</strong> </td> 
      <td> Dies ist das Enddatum der Arbeitszeittabelle.</td> 
     </tr>
<tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td> Dies ist der Status der Arbeitszeittabelle.
      Im Folgenden finden Sie mögliche Statusoptionen für Arbeitszeittabellen: 
      <ul><li><b>Öffnen</b>: Die Arbeitszeittabelle ist geöffnet und Stundeneinträge können bearbeitet werden.</li>
      <li><b>Übermittelt</b>: Die Arbeitszeittabelle wird zur Genehmigung an die benannten genehmigenden Personen weitergeleitet.</li>
      <li><b>Abgelehnt</b>: Die Arbeitszeittabelle wurde von den genehmigenden Personen nicht genehmigt und steht nun wieder zur Bearbeitung der Zeiteinträge zur Verfügung.</li>
      <li><b>Geschlossen</b>: Die Arbeitszeittabelle wird entweder vom Benutzer geschlossen oder von der genehmigenden Person genehmigt und ist daher jetzt geschlossen. Sie können keine Zeit zu einer geschlossenen Arbeitszeittabelle hinzufügen.</li>
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Genehmigende Personen</strong> </td> 
      <td> <p>Genehmigende Personen sind Benutzer, die die Arbeitszeittabelle für die mit der Arbeitszeittabelle verbundenen Benutzer genehmigen. Nur Benutzer mit administrativem Zugriff auf Arbeitszeittabellen können als genehmigende Personen festgelegt werden. </p> <p>Weitere Informationen zu Arbeitszeittabellen-Administratorrechten finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.</p> <p>Geben Sie die Namen der genehmigenden Personen für Arbeitszeittabellen ein und wählen Sie sie aus, wenn sie in der Liste angezeigt werden.</p> <p>Eine Arbeitszeittabelle kann mehrere genehmigende Personen enthalten. Wenn eine der genehmigenden Personen die Arbeitszeittabelle genehmigt hat, wird diese als "<strong>" </strong> und verschwindet aus der Liste der Arbeitszeittabellen-Genehmigungen aller verbleibenden genehmigenden Personen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Kann die Zeit bearbeiten</strong> </td> 
      <td> <p>Wählen Sie diese Option aus, wenn Sie genehmigenden Personen erlauben möchten, Stunden auf der Arbeitszeittabelle zu bearbeiten.</p> <p>Diese Option ist nicht verfügbar, wenn Sie mehrere Arbeitszeittabellen auswählen. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span style="font-weight: bold;">Überstunden</span> </td> 
      <td> <p>Sie können das Feld „Überstunden“ auf der Arbeitszeittabelle ausblenden.</p> <p>Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.
