---
product-area: reporting
navigation-topic: reporting-elements
title: Filter, Ansichten oder Gruppierungen freigeben
description: Sie können Filter, Ansichten und Gruppierungen, auf die Sie Zugriff haben, für andere Benutzer freigeben.
author: Nolan
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1178'
ht-degree: 1%

---

# Filter, Ansichten oder Gruppierungen freigeben

<!-- Audited: 11/2024 -->

<!--(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)
(NOTE: This is linked from the TOC article in WF Basics > permissions section)-->

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf die Ansicht oder Bearbeitung von Objekten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Objekte finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Bearbeiten bestimmter von Ihnen erstellter Objekte oder zum Freigeben von Inhalten gewähren. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Wie Zugriffsebenen und -berechtigungen zusammenarbeiten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Sie können Filter, Ansichten und Gruppierungen, auf die Sie Zugriff haben, für andere Benutzer freigeben.

Wenn ein Filter, eine Ansicht oder eine Gruppierung für Sie freigegeben ist, können Sie diesen Filter, diese Ansicht oder diese Gruppierung auf Ihre Listen anwenden. Je nach dem Ihnen gewährten Zugriff können Sie ihn ändern und für andere Benutzer freigeben.

Informationen zum Erstellen eines Filters, einer Ansicht oder einer Gruppierung finden Sie in den folgenden Artikeln:

* [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Mitwirkende oder höher</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Anforderung oder höher</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen anzeigen oder höher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td><p>Anzeigen oder höherer Berechtigungen mit Zugriff auf die Freigabe für Ansichten, Filter oder Gruppierungen</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter, Ansichten oder Gruppierungen freigeben

<!--(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)-->

Die Freigabe von Filtern in ausgewählten Listen hängt davon ab, von welcher Benutzeroberfläche aus Sie den Filter freigeben: Standard oder veraltet. Informationen zu den Typen von Filtererstellungs-Schnittstellen finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Sie können Ansichten und Gruppierungen nur in der alten Benutzeroberfläche freigeben.

### Freigeben von Filtern über die Standard-Builder-Benutzeroberfläche

Sie können einen Filter in der Standardbenutzeroberfläche aus Listen mit Projekten, Aufgaben, Problemen, Portfolios, Programmen, Benutzern, Vorlagen oder Gruppen freigeben. Die standardmäßige Builder-Oberfläche für Filter ist für keine anderen Objekte oder für Ansichten oder Gruppierungen verfügbar.

Geben Sie einen Filter über die Standard-Builder-Oberfläche frei:

1. Gehen Sie zu einer Liste von Projekten, Aufgaben oder Problemen.
1. Klicken Sie auf das Symbol **Filter** ![Filtersymbol](assets/filter-nwepng.png).

   ![Standardfilter-Builder](assets/new-filters-all-filter-types.png)

1. Überprüfen Sie die folgenden Filterlisten:

   <table style="table-layout:auto">
   <col>
   <col>
   <tbody>
   <tr>
   <td role="rowheader"><strong>Favorit</strong></td>
   <td>Filter, die Sie als Favoriten gekennzeichnet haben. Wenn Sie einen Filter bevorzugen, wird seine ursprüngliche Position unter dem Filternamen angezeigt und er wird aus der ursprünglichen Liste ausgeblendet, es sei denn, Sie entfernen ihn als Favoriten.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Gespeichert</strong></td>
   <td>Filter, die Sie selbst erstellt und gespeichert haben. Standardmäßig werden in dieser Liste gespeicherte Filter in der Reihenfolge angezeigt, in der sie zuletzt gespeichert wurden. Die Filternamen können jedoch per Drag-and-Drop manuell neu angeordnet werden.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Standardeinstellungen für das System</strong></td>
   <td>Workfront-Systemstandardfilter sowie Filter, die der Workfront-Administrator Ihrer Filterliste entweder auf Systemebene oder in Ihrer Layoutvorlage hinzugefügt hat.</td>
   </tr>
   <tr>
   <td role="rowheader"><strong>Für mich freigegeben</strong></td>
   <td>Filter, die von anderen erstellt und für Sie freigegeben wurden oder die systemweit freigegeben sind.</td>
   </tr>
   </tbody>
   </table>

1. Bewegen Sie den Mauszeiger über einen Filter, auf den Sie mindestens Zugriff haben, um ihn anzuzeigen und freizugeben. Klicken Sie dann auf das Menü **Mehr** und ![Mehr Menü](assets/more-icon-spectrum.png) und klicken Sie dann auf **Freigeben**.

   ![Weitere Menüoptionen](assets/new-filters-more-menu-options-with-delete.png)

   Das Freigabefeld Filter wird angezeigt.

1. Beginnen Sie mit der Eingabe der Namen von Benutzern, Teams, Rollen, Gruppen oder Unternehmen, für die Sie freigeben möchten, in das Feld **Zugriff auf** gewähren .

   ![Feld für die Filterfreigabe](assets/new-filters-share-filter.png)

1. (Optional) Klicken Sie auf den Rechtspfeil neben dem Namen einer Entität, um deren Berechtigungen für den Filter zu bearbeiten, und aktivieren Sie dann die Option **Ansicht** oder **Verwalten** . **Ansicht** ist die Standardeinstellung.

   ![Berechtigungen freigeben](assets/new-filters-sharing-permissions.png)

1. (Optional) Aktivieren oder deaktivieren Sie die zusätzlichen Berechtigungen für eine Entität, indem Sie eine der folgenden Aktionen ausführen:

   1. Klicken Sie auf **Anzeigen** und deaktivieren Sie die Option **Freigeben** . Sie ist standardmäßig aktiviert.
   1. Klicken Sie auf **Verwalten** und deaktivieren Sie entweder die Option **Freigeben** oder die Option **Löschen** . Sie sind standardmäßig aktiviert.

      >[!NOTE]
      >
      >Wenn Sie die Option Zugriff mit Löschoption verwalten aktivieren, können diese Benutzer den Filter von allen Benutzern löschen, auch wenn sie nicht Eigentümer des Filters sind.

   >[!TIP]
   >
   >Benutzer können keine höhere Berechtigung als ihre Zugriffsstufe erhalten. Wenn sie keinen Zugriff auf Filter bearbeiten in ihrer Zugriffsebene haben, können sie keine Berechtigungen zum Verwalten eines Filters erhalten. Workfront deaktiviert die Option Verwalten für diese Benutzer und die Option ist abgeblendet.

1. Klicken Sie auf **Teilen**. Der Filter wird für die angegebenen Entitäten freigegeben.

   >[!TIP]
   >
   >Durch die Freigabe für Gruppen erhält der Filter Berechtigungen für die Mitglieder der Gruppe und für alle Untergruppen.

   Die von Ihnen freigegebenen Filter werden im Abschnitt **Für mich freigegeben** des Filterbereichs für diese Entitäten angezeigt.

   ![Für mich freigegebene Filter](assets/new-filters-shared-with-me.png)

### Freigeben von Filtern, Ansichten und Gruppierungen über die alte Benutzeroberfläche

Die Freigabe von Filtern, Ansichten und Gruppierungen in der alten Benutzeroberfläche ist identisch.

1. Gehen Sie zu einer Liste von Objekten oder einem Bericht.
1. (Bedingt) Klicken Sie in einer Liste auf das Symbol &quot;**Filter**&quot;, &quot;**Ansicht**&quot;oder &quot;**Gruppierung**&quot;, bewegen Sie den Mauszeiger über den Filter, die Ansicht oder die Gruppierung, die Sie freigeben möchten, und klicken Sie auf das Symbol &quot;**Mehr**&quot;![Mehr&quot;](assets/more-icon.png) und dann auf &quot;**Freigabe**&quot;.

   Klicken Sie in einem Bericht auf das Dropdown-Menü **Filter**, **Ansicht** oder **Gruppierung** und wählen Sie dann den Filter, die Ansicht oder die Gruppierung aus, die Sie freigeben möchten.

1. (Bedingt) Klicken Sie beim Freigeben aus einem Bericht erneut auf das Dropdown-Menü **Filter**, **Ansicht** oder **Gruppierung** und dann auf **Filter freigeben**, **Freigabeansicht** oder **Gruppierung freigeben**.\
   Das Dialogfeld **Filterzugriff**, **Zugriff anzeigen** oder **Gruppierungszugriff** wird angezeigt.

   ![Filter freigeben](assets/share-filter-people-box-nwe-350x458.png)

1. Führen Sie je nachdem, für wen Sie freigeben möchten, einen der folgenden Schritte aus:

   **Um sie für einzelne Benutzer, Teams, Rollen, Gruppen oder Unternehmen freizugeben:** Geben Sie im angegebenen Feld den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den/die Sie freigeben möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdownliste angezeigt wird.\
   Wiederholen Sie diesen Vorgang, um den Zugriff für mehrere Benutzer, Teams, Rollen, Gruppen oder Unternehmen freizugeben.

   >[!TIP]
   >
   >Durch die Freigabe für Gruppen erhalten die Mitglieder der Gruppe und aller Untergruppen Berechtigungen für den Filter, die Ansicht oder die Gruppierung.

   **Um sie für alle Benutzer im System freizugeben:** Klicken Sie auf das Symbol **Einstellungen** und klicken Sie dann auf **Dieses System für alle Benutzer sichtbar machen**.\
   Ihr Administrator muss die Option System-weit freigeben auswählen, damit diese Option verfügbar ist. Weitere Informationen finden Sie in den Artikeln [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) und [Berichte, Dashboards und Kalender freigeben](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md) .

1. (Bedingt) Wenn Sie die Freigabe für einzelne Benutzer, Teams, Rollen, Gruppen oder Unternehmen durchführen, klicken Sie auf das Dropdown-Menü, um die Zugriffsstufe festzulegen, die Sie gewähren möchten.

   Sie können aus den folgenden Optionen auswählen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Anzeigen</strong></td> 
      <td> <p>Wählen Sie diese Option aus, damit die freigegebenen Empfänger nur den freigegebenen Filter, die freigegebene Ansicht oder die Gruppierung verwenden können. Wenn diese Option aktiviert ist, können Empfänger keine Änderungen am freigegebenen Element vornehmen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Verwalten</strong></td> 
      <td> <p>Wählen Sie diese Option aus, damit die freigegebenen Empfänger den freigegebenen Filter, die freigegebene Ansicht oder die Gruppierung verwenden und ändern können.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Freigeben</strong></td> 
      <td> <p>Klicken Sie auf <strong>Erweiterte Einstellungen</strong> und wählen Sie dann die Option <strong>Freigabe</strong> aus oder löschen Sie sie, je nachdem, ob die Empfänger für andere freigegeben werden sollen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Benutzer, für die Sie den Filter, die Ansicht oder die Gruppierung freigegeben haben, können darauf zugreifen, indem Sie auf das Dropdown-Menü bzw. das Symbol **Filter**, **Ansicht** oder **Gruppierung** klicken und zum Abschnitt **Für mich freigegeben** scrollen.


