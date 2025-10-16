---
product-area: reporting
navigation-topic: reporting-elements
title: Filter, Ansichten oder Gruppierungen freigeben
description: Sie können Filter, Ansichten und Gruppierungen freigeben, auf die Sie Zugriff haben, um sie für andere Benutzer anzuzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1170'
ht-degree: 2%

---

# Filter, Ansichten oder Gruppierungen freigeben

<!-- Audited: 11/2024 -->

<!--(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)
(NOTE: This is linked from the TOC article in WF Basics > permissions section)-->

Ihr Adobe Workfront-Administrator gewährt Benutzenden Zugriff zum Anzeigen oder Bearbeiten von Objekten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Objekte finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Bearbeiten bestimmter Objekte erteilen, die Sie erstellt haben oder auf die Sie Zugriff haben. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Funktionsweise von Zugriffsebenen und Berechtigungen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Sie können Filter, Ansichten und Gruppierungen freigeben, auf die Sie Zugriff haben, um sie für andere Benutzer anzuzeigen.

Wenn ein Filter, eine Ansicht oder eine Gruppierung für Sie freigegeben ist, können Sie diesen Filter, diese Ansicht oder die Gruppierung auf Ihre Listen anwenden. Je nach dem Ihnen gewährten Zugriff können Sie diesen möglicherweise ändern und für andere Benutzer freigeben.

Informationen zum Erstellen eines Filters, einer Ansicht oder einer Gruppierung finden Sie in den folgenden Artikeln:

* [Übersicht über Filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Übersicht über Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</strong></td> 
   <td> 
    <p>Mitwirkender oder höher</p>
    <p>Anfrage oder höher</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Filter, Ansichten, Gruppierungen</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
    <td> <p>Anzeigen von oder höheren Berechtigungen mit Zugriff zum Freigeben für eine Ansicht, einen Filter oder eine Gruppierung</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter, Ansichten oder Gruppierungen freigeben

<!--(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)-->

Die Freigabe von Filtern in Auswahllisten unterscheidet sich je nachdem, über welche Benutzeroberfläche der Filter freigegeben wird: Standard oder Legacy. Informationen zu den Typen von Filtererstellungsschnittstellen finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Sie können Ansichten und Gruppierungen nur in der veralteten -Benutzeroberfläche freigeben.

### Freigeben von Filtern über die Standard-Builder-Oberfläche

Sie können einen Filter in der Standardschnittstelle aus Listen von Projekten, Aufgaben, Problemen, Portfolios, Programmen, Benutzern, Vorlagen oder Gruppen freigeben. Die Standard-Builder-Oberfläche für Filter ist für keine anderen Objekte oder für Ansichten oder Gruppierungen verfügbar.

Freigeben von Filtern über die Standard-Builder-Oberfläche:

1. Navigieren Sie zu einer Liste mit Projekten, Aufgaben oder Problemen.
1. Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-nwepng.png).

   ![Standardfilter-Generator](assets/new-filters-all-filter-types.png)

1. Überprüfen Sie die folgenden Filterlisten:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Favorit</strong></td>
   <td>Filter, die Sie als Favoriten markiert haben. Wenn Sie einen Filter als Favoriten festlegen, wird seine ursprüngliche Position unter dem Filternamen angezeigt und in der Originalliste ausgeblendet, es sei denn, Sie entfernen ihn als Favoriten.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Gespeichert</strong></td>
   <td>Von Ihnen selbst erstellte und gespeicherte Filter. Standardmäßig werden in dieser Liste gespeicherte Filter in der Reihenfolge der zuletzt gespeicherten angezeigt. Sie können die Filternamen jedoch ziehen, um die Liste manuell neu anzuordnen.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Standardeinstellungen für das System</strong></td>
   <td>Workfront-Systemstandardfilter sowie Filter, die der Workfront-Administrator Ihrer Filterliste hinzugefügt hat, entweder auf Systemebene oder in Ihrer Layout-Vorlage.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Für mich freigegeben</strong></td>
   <td>Filter, die von anderen erstellt und für Sie freigegeben wurden oder die systemweit freigegeben sind.</td>
   </tr>
   </tbody>
   </table>

1. Bewegen Sie den Mauszeiger über einen Filter, auf den Sie Zugriff haben, zumindest zum Anzeigen und Freigeben, und klicken Sie dann auf das Menü **Mehr** ![Mehr &#x200B;](assets/more-icon-spectrum.png) und anschließend auf **Freigeben**.

   ![Weitere Menüoptionen](assets/new-filters-more-menu-options-with-delete.png)

   Das Feld Filterfreigabe wird angezeigt.

1. Beginnen Sie mit der Eingabe der Namen von Benutzern, Teams, Rollen, Gruppen oder Unternehmen, die Sie für freigeben möchten, in das Feld **Zugriff erteilen für**.

   ![Filterfreigabefeld](assets/new-filters-share-filter.png)

1. (Optional) Klicken Sie auf den nach rechts zeigenden Pfeil neben dem Namen einer Entität, um deren Berechtigungen für den Filter zu bearbeiten, und aktivieren Sie dann entweder die Option **Anzeigen** oder **Verwalten**. **Ansicht** ist der Standard.

   ![Freigabeberechtigungen](assets/new-filters-sharing-permissions.png)

1. (Optional) Aktivieren oder deaktivieren Sie die zusätzlichen Berechtigungen für eine Entität, indem Sie einen der folgenden Schritte ausführen:

   1. Klicken Sie **Anzeigen** und deaktivieren Sie die Option **Freigeben**. Diese ist standardmäßig aktiviert.
   1. Klicken Sie **Verwalten** und deaktivieren Sie entweder die Option **Freigeben** oder **Löschen**. Sie sind standardmäßig aktiviert.

      >[!NOTE]
      >
      >Wenn Sie Zugriff verwalten mit der Option Löschen aktivieren, können diese Benutzer den Filter aus allen Benutzern löschen, auch wenn sie nicht der Eigentümer des Filters sind.

   >[!TIP]
   >
   >Benutzende erhalten keine höhere Berechtigung als ihre Zugriffsebene. Wenn sie in ihrer Zugriffsebene keinen Zugriff auf „Filter bearbeiten“ haben, können sie keine Berechtigungen zum Verwalten eines Filters erhalten. Workfront deaktiviert die Option Verwalten für diese Benutzenden, und die Option ist abgeblendet.

1. Klicken Sie auf **Teilen**. Der Filter wird für die angegebenen Entitäten freigegeben.

   >[!TIP]
   >
   >Bei der Freigabe für Gruppen erhalten die Mitglieder der Gruppe und aller Untergruppen Berechtigungen für den Filter.

   Die von Ihnen freigegebenen Filter werden im Abschnitt **Für mich freigegeben** des Bedienfelds „Filter“ für diese Entitäten angezeigt.

   ![Für mich freigegebene Filter](assets/new-filters-shared-with-me.png)

### Freigeben von Filtern, Ansichten und Gruppierungen über die alte Benutzeroberfläche

Die Freigabe von Filtern, Ansichten und Gruppierungen in der veralteten Benutzeroberfläche ist identisch.

1. Navigieren Sie zu einer Liste von Objekten oder einem Bericht.
1. (Bedingt) Klicken Sie in einer Liste auf das Symbol **Filter**, **Ansicht** oder **Gruppierung** und bewegen Sie dann den Mauszeiger über den Filter, die Ansicht oder die Gruppierung, die Sie freigeben möchten, und klicken Sie auf das Symbol **Mehr** ![Mehr-Symbol](assets/more-icon.png) dann auf **Freigeben**.

   Klicken Sie in einem Bericht auf das **Filter**, **Ansicht** oder **Gruppierung** Dropdown-Menü und wählen Sie dann den Filter, die Ansicht oder die Gruppierung aus, die Sie freigeben möchten.

1. (Bedingt) Klicken Sie bei der Freigabe in einem Bericht erneut auf das Dropdown-Menü **Filter**, **Ansicht** oder **Gruppierung** und klicken Sie dann auf **Filter freigeben**, **Ansicht freigeben** oder **Gruppierung freigeben**.\
   Das **Filterzugriff**, **Ansichtszugriff** oder **Gruppierungszugriff** wird angezeigt.

   ![Filter freigeben](assets/share-filter-people-box-nwe-350x458.png)

1. Führen Sie einen der folgenden Schritte aus, je nachdem, für wen Sie freigeben möchten:

   **Für einzelne Benutzer, Teams, Rollen, Gruppen oder Unternehmen freigeben:** Geben Sie in das entsprechende Feld den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den bzw. das Sie eine Freigabe durchführen möchten. Klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.\
   Wiederholen Sie diesen Vorgang, um den Zugriff für mehrere Benutzer, Teams, Rollen, Gruppen oder Unternehmen freizugeben.

   >[!TIP]
   >
   >Bei der Freigabe für Gruppen erhalten die Mitglieder der Gruppe und aller Untergruppen Berechtigungen für den Filter, die Ansicht oder die Gruppierung.

   **Für alle Benutzer im System freigeben:** Klicken Sie auf das Symbol **Einstellungen** und klicken Sie dann auf **Systemweit sichtbar machen**.\
   Ihr Administrator muss die Option Systemweit freigeben auswählen, damit diese Option verfügbar ist. Weitere Informationen finden Sie in den Artikeln [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) und &quot;[&#x200B; von Berichten, Dashboards und Kalendern](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Bedingt) Wenn Sie Berechtigungen für einzelne Benutzer, Teams, Rollen, Gruppen oder Unternehmen freigeben, klicken Sie auf das Dropdown-Menü, um die Zugriffsebene zu definieren, die Sie gewähren möchten.

   Sie können aus den folgenden Optionen auswählen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Anzeigen</strong></td> 
      <td> <p>Wählen Sie diese Option aus, damit die Freigabeempfänger nur den freigegebenen Filter, die freigegebene Ansicht oder die freigegebene Gruppierung verwenden können. Wenn diese Option ausgewählt ist, können Empfänger keine Änderungen am freigegebenen Element vornehmen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Verwalten</strong></td> 
      <td> <p>Wählen Sie diese Option aus, damit die Freigabeempfänger den freigegebenen Filter, die freigegebene Ansicht oder die freigegebene Gruppierung verwenden und ändern können.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Freigeben</strong></td> 
      <td> <p>Klicken Sie <strong>Erweiterte Einstellungen</strong> und wählen oder deaktivieren Sie dann die Option <strong>Freigeben</strong>, je nachdem, ob Sie möchten, dass die Empfänger in der Lage sind, Inhalte für andere freizugeben.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Benutzer, für die Sie den Filter, die Ansicht oder die Gruppierung freigegeben haben, können darauf zugreifen, indem sie auf das Dropdown-Menü oder das Symbol **Filter**, **Ansicht** oder **Gruppierung** klicken und nach unten zum Abschnitt **Für mich freigegeben** scrollen.


