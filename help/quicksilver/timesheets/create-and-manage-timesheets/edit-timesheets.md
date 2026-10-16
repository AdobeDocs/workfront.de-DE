---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Bearbeiten von Informationen in Arbeitszeittabellen
description: Benutzende mit administrativem Zugriff auf Arbeitszeittabellen können Informationen zu bestehenden Arbeitszeittabellen in Adobe Workfront bearbeiten. Sie können beispielsweise den Eigentümer, die genehmigenden Personen oder den Zeitrahmen der Arbeitszeittabelle bearbeiten.
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
TQID: https://experienceleague.adobe.com/--QshuygnTfcEJtt6-Tx-2QtNT-5p9TrTWaQTMBZNAg
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
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 9%
---
# Bearbeiten von Informationen in Arbeitszeittabellen

Benutzende mit administrativem Zugriff auf Arbeitszeittabellen können Informationen zu bestehenden Arbeitszeittabellen in Adobe Workfront bearbeiten. Sie können beispielsweise den Eigentümer, die genehmigenden Personen oder den Zeitrahmen der Arbeitszeittabelle bearbeiten.

Sie können Informationen auf einer einzigen Arbeitszeittabelle bearbeiten oder mehrere Arbeitszeittabellen gleichzeitig bearbeiten.

>[!IMPORTANT]
>
>Wenn Benutzende mit Arbeitszeittabellen-Profilen verknüpft sind und die Arbeitszeittabellen automatisch generiert werden, werden die Änderungen, die Sie an vorhandenen Arbeitszeittabellen vornehmen, nicht in Arbeitszeittabellen übernommen, die für zukünftige Datumsangaben generiert werden. Für alle automatisch generierten Arbeitszeittabellen werden die Einstellungen in den Arbeitszeittabellen-Profilen festgelegt. Weitere Informationen finden Sie unter [Arbeitszeittabellen-Profile erstellen](../create-and-manage-timesheets/create-timesheet-profiles.md)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><p>Administrativer Zugriff auf Arbeitszeittabellen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Arbeitszeittabellen bearbeiten

{{step1-to-timesheets}}

Alle Arbeitszeittabellen, auf die Sie Zugriff haben, werden standardmäßig angezeigt.

![Arbeitszeittabellen-Liste](assets/list-of-all-timesheets.png)

1. (Optional) Klicken Sie auf das **Suche**-Symbol ![Suchsymbol](assets/search-icon.png) und geben Sie einen Suchbegriff ein, um nach einer bestimmten Arbeitszeittabelle zu suchen. Sie können beispielsweise nach einem Arbeitszeittabellen-Zeitrahmen oder einem Eigentümernamen suchen.

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

1. Wählen Sie eine oder mehrere Arbeitszeittabellen aus und klicken Sie dann oben in **Arbeitszeittabellenliste auf** Bearbeiten![Symbol ](assets/edit-icon.png)Bearbeiten“.
1. Zeigen Sie die folgenden Informationen an oder geben Sie sie ein:

   | Feldname | Beschreibung |
   | --------- | ---------- |
   | Besitzer bzw. Besitzerin | <p>Dies ist der Name des Benutzers, für den die Arbeitszeittabelle erstellt wurde. Dieses Feld kann nicht bearbeitet werden.</p><p>Dieses Feld wird nicht angezeigt, wenn Sie mehrere Arbeitszeittabellen auswählen.</p> |
   | Startdatum | Dies ist das Startdatum der Arbeitszeittabelle. |
   | Enddatum | Dies ist das Enddatum der Arbeitszeittabelle. |
   | Status | <p>Dies ist der Status der Arbeitszeittabelle. Im Folgenden finden Sie mögliche Statusoptionen für Arbeitszeittabellen:</p><ul><li>**Öffnen**: Die Arbeitszeittabelle ist geöffnet und Stundeneinträge können bearbeitet werden.</li><li>**Übermittelt**: Die Arbeitszeittabelle wird zur Genehmigung an die benannten genehmigenden Personen weitergeleitet.</li><li>**Abgelehnt**: Die Arbeitszeittabelle wurde von den genehmigenden Personen nicht genehmigt und steht nun wieder zur Bearbeitung der Zeiteinträge zur Verfügung.</li><li>**Geschlossen**: Die Arbeitszeittabelle wird entweder vom Benutzer geschlossen oder von der genehmigenden Person genehmigt und ist daher jetzt geschlossen. Sie können keine Zeit zu einer geschlossenen Arbeitszeittabelle hinzufügen.</li></ul> |
   | Genehmigende Personen | <p>Genehmigende Personen sind Benutzer, die die Arbeitszeittabelle für die mit der Arbeitszeittabelle verbundenen Benutzer genehmigen. Nur Benutzer mit Verwaltungsrechten für Arbeitszeittabellen können als genehmigende Personen festgelegt werden. Weitere Informationen zu Arbeitszeittabellen-Administratorrechten finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).</p> <p>Geben Sie die Namen der genehmigenden Personen für Arbeitszeittabellen ein und wählen Sie sie aus, wenn sie in der Liste angezeigt werden.</p> <p>Eine Arbeitszeittabelle kann mehrere genehmigende Personen enthalten. Wenn eine der genehmigenden Personen die Arbeitszeittabelle genehmigt hat, wird diese als &quot;**&quot;** und verschwindet aus der Liste der Arbeitszeittabellen-Genehmigungen aller verbleibenden genehmigenden Personen.</p> |
   | Kann Zeit bearbeiten | <p>Wählen Sie diese Option aus, wenn Sie genehmigenden Personen erlauben möchten, Stunden auf der Arbeitszeittabelle zu bearbeiten.</p><p>Diese Option ist nicht verfügbar, wenn Sie mehrere Arbeitszeittabellen auswählen.</p> |
   | Überstunden | <p>Sie können das Feld „Überstunden“ auf der Arbeitszeittabelle ausblenden.</p><p>Standardmäßig ist diese Option deaktiviert.</p> |

1. Klicken Sie auf **Speichern**.
