---
product-area: reporting
navigation-topic: reporting-elements
title: Filter, Ansichten oder Gruppierungen freigeben
description: Sie können Filter, Ansichten und Gruppierungen, auf die Sie Zugriff haben, für andere Benutzer freigeben.
author: Lisa
feature: Reports and Dashboards
exl-id: 63a6db90-d52c-4147-a442-7904ef9e9d49
source-git-commit: 8ac8981a40f051f11eef231397cd231ae1d8ddff
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 1%

---

# Filter, Ansichten oder Gruppierungen freigeben

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: CONSIDER SPLITTING THIS in three articles for each reporting element?)</p>
<p>(NOTE: This is linked from the TOC article in WF Basics > permissions section)&nbsp;</p>
</div>
-->

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf die Ansicht oder Bearbeitung von Objekten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Objekte finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Bearbeiten bestimmter von Ihnen erstellter Objekte oder zum Freigeben von Inhalten gewähren. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Wie Zugriffsebenen und Berechtigungen zusammenarbeiten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Sie können Filter, Ansichten und Gruppierungen, auf die Sie Zugriff haben, für andere Benutzer freigeben.

Wenn ein Filter, eine Ansicht oder eine Gruppierung für Sie freigegeben ist, können Sie diesen Filter, diese Ansicht oder diese Gruppierung auf Ihre Listen anwenden. Je nach dem Ihnen gewährten Zugriff können Sie ihn ändern und für andere Benutzer freigeben.

Informationen zum Erstellen eines Filters, einer Ansicht oder einer Gruppierung finden Sie in den folgenden Artikeln:

* [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
* [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Anzeigen oder höherer Berechtigungen mit Zugriff auf die Freigabe für Ansichten, Filter oder Gruppierungen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Filter, Ansichten oder Gruppierungen freigeben

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: when the beta filters/ groupings come out either consider splitting this in different kinds of FVGs or splitting this article in FVGs for showing sharing on each one of them??)</p>
-->

Sie können Filter über die folgenden Schnittstellen in Auswahllisten freigeben:

* Standardschnittstelle
* Beta-Builder-Benutzeroberfläche

Die Freigabe von Filtern in Auswahllisten hängt davon ab, von welcher Benutzeroberfläche aus Sie den Filter freigeben. Informationen zu den Typen von Filtererstellungs-Schnittstellen finden Sie unter [Filter in Adobe Workfront erstellen oder bearbeiten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

Sie können Ansichten und Gruppierungen nur in der Standardoberfläche freigeben.

* [Freigeben von Filtern, Ansichten und Gruppierungen mithilfe der Standardschnittstelle](#share-with-standard-interface)
* [Freigeben von Filtern über die Beta-Builder-Benutzeroberfläche](#share-with-beta-builder-interface)

### Freigeben von Filtern, Ansichten und Gruppierungen mithilfe der Standardschnittstelle {#share-with-standard-interface}

Die Freigabe von Filtern, Ansichten und Gruppierungen in der Standardschnittstelle ist identisch.

1. Gehen Sie zu einer Liste von Objekten oder einem Bericht.
1. (Bedingt) Klicken Sie in einer Liste auf die **Filter**, **Ansicht** oder **Gruppierung** und den Mauszeiger über den Filter, die Ansicht oder die Gruppierung halten, den/die Sie freigeben möchten, klicken Sie auf die Schaltfläche **Mehr** icon ![Weitere Symbole](assets/more-icon.png), dann **Freigeben**.

   Klicken Sie in einem Bericht auf die **Filter**, **Ansicht** oder **Gruppierung** Dropdown-Menü aus und wählen Sie dann den Filter, die Ansicht oder die Gruppierung aus, die Sie freigeben möchten.

1. (Bedingt) Klicken Sie bei der Freigabe über einen Bericht auf die **Filter**, **Ansicht** oder **Gruppierung** erneut auf das Dropdown-Menü klicken und **Filter freigeben**, **Freigabeansicht** oder **Gruppierung freigeben**.\
   Die **Filterzugriff**, **Zugriff anzeigen** oder **Gruppierungszugriff** angezeigt.

   ![Filter freigeben](assets/share-filter-people-box-nwe-350x458.png)

1. Führen Sie je nachdem, für wen Sie freigeben möchten, einen der folgenden Schritte aus:

   **So geben Sie Inhalte für einzelne Benutzer, Teams, Rollen, Gruppen oder Unternehmen frei:** Geben Sie im angegebenen Feld den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens ein, für den/das Sie eine Freigabe vornehmen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.\
   Wiederholen Sie diesen Vorgang, um den Zugriff für mehrere Benutzer, Teams, Rollen, Gruppen oder Unternehmen freizugeben.

   >[!TIP]
   >
   >Durch die Freigabe für Gruppen erhalten die Mitglieder der Gruppe und aller Untergruppen Berechtigungen für den Filter, die Ansicht oder die Gruppierung.


   **So geben Sie eine Freigabe für alle Benutzer im System durch:** Klicken Sie auf **Einstellungen** und klicken Sie auf **Diese Funktion systemweit sichtbar machen**.\
   Ihr Administrator muss die Option System-weit freigeben auswählen, damit diese Option verfügbar ist. Weitere Informationen finden Sie in den Artikeln [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) und [Berichte, Dashboards und Kalender freigeben](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

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
      <td> <p>Klicken <strong>Erweiterte Einstellungen</strong>, wählen Sie die <strong>Freigeben</strong> -Option, je nachdem, ob die Empfänger für andere freigeben können sollen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Benutzer, für die Sie den Filter, die Ansicht oder die Gruppe freigegeben haben, können darauf zugreifen, indem Sie auf die **Filter**, **Ansicht** oder **Gruppierung** Dropdown-Menü oder -Symbol aus und scrollen Sie nach unten zum **Freigegeben für mich** Abschnitt.

### Freigeben von Filtern über die Beta-Builder-Benutzeroberfläche {#share-with-beta-builder-interface}

Beim Freigeben von Filtern aus Listen mit Projekten, Aufgaben oder Problemen können Sie diese über die Beta-Builder-Oberfläche anstelle der Standardoberfläche freigeben.

Die Beta-Builder-Oberfläche ist für keine anderen Objekte in Workfront verfügbar.

Beim Erstellen von Berichten können Sie keine Filter in der Beta-Builder-Oberfläche erstellen.

Geben Sie einen Filter über die Beta-Builder-Oberfläche frei:

1. Gehen Sie zu einer Liste von Projekten, Aufgaben oder Problemen.
1. Klicken Sie auf **Filter** icon ![Filtersymbol](assets/filter-nwepng.png), und aktivieren Sie dann die **Beta-Einstellung** ![Beta-Einstellung](assets/beta-toggle-white-on-existing-filters.png) , um auf den Beta-Builder zuzugreifen. Sie ist standardmäßig deaktiviert.

   Bestätigen Sie dann bei Bedarf die Beta-Vereinbarung.

   Dadurch wird die Beta-Filter-Builder-Oberfläche geöffnet.

   >[!TIP]
   >
   >Die Kopfzeile der Builder-Oberfläche wird blau, wenn Sie den Beta-Builder aktivieren. Nachdem Sie die Beta-Builder-Oberfläche aktiviert haben, bleibt sie in Workfront für alle Bereiche aktiviert, in denen sie verfügbar ist.

   ![Beta-Filter-Builder](assets/new-filters-all-filter-types.png)

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
   <td>Filter, die Sie selbst erstellt und gespeichert haben.</td>
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

1. Bewegen Sie den Mauszeiger über einen Filter, auf den Sie mindestens Zugriff haben, und klicken Sie auf **Mehr** Menü ![Mehr Menü](assets/more-icon-spectrum.png)Klicken Sie auf **Freigeben**.

   ![Weitere Menüoptionen](assets/new-filters-more-menu-options-with-delete.png)

   Das Freigabefeld Filter wird angezeigt.

1. Aktivieren Sie die Einstellung Systemweite anzeigen . Dadurch kann jeder in Workfront den Filter anzeigen.

   >[!IMPORTANT]
   >
   >Verwenden Sie diese Einstellung mit Vorsicht. Das Hinzufügen vieler Filter für alle Benutzer erschwert das Filtern und erschwert die Suche nach Filtern.

   Oder geben Sie die Namen der Benutzer, Teams, Rollen, Gruppen oder Unternehmen ein, für die Sie die Freigabe durchführen möchten. **Zugriff auf gewähren** -Feld.

   ![Freigabefeld filtern](assets/new-filters-share-filter.png)

1. (Optional) Klicken Sie auf den Rechtspfeil neben dem Namen einer Entität, um ihre Berechtigungen für den Filter zu bearbeiten, und aktivieren Sie dann entweder das **Ansicht** oder **Verwalten** -Option. **Ansicht** ist der Standardwert.

   ![Berechtigungen freigeben](assets/new-filters-sharing-permissions.png)

1. (Optional) Aktivieren oder deaktivieren Sie die zusätzlichen Berechtigungen für eine Entität, indem Sie eine der folgenden Aktionen ausführen:

   1. Klicken **Ansicht** und deaktivieren Sie die **Freigeben** -Option. Sie ist standardmäßig aktiviert.
   1. Klicken **Verwalten** und deaktivieren Sie entweder die **Freigeben** oder **Löschen** -Option. Sie sind standardmäßig aktiviert.

      >[!NOTE]
      >
      >Wenn Sie die Option Zugriff mit Löschoption verwalten aktivieren, können diese Benutzer den Filter von allen Benutzern löschen, auch wenn sie nicht Eigentümer des Filters sind.
   >[!TIP]
   >
   >Benutzer können keine höhere Berechtigung als ihre Zugriffsstufe erhalten. Wenn sie keinen Zugriff auf Filter bearbeiten in ihrer Zugriffsebene haben, können sie keine Berechtigungen zum Verwalten eines Filters erhalten. Workfront deaktiviert die Option Verwalten für diese Benutzer und die Option ist abgeblendet.

1. Klicken **Freigeben**. Der Filter wird für die angegebenen Entitäten freigegeben.

   >[!TIP]
   >
   >Durch die Freigabe für Gruppen erhält der Filter Berechtigungen für die Mitglieder der Gruppe und für alle Untergruppen.

   Die von Ihnen freigegebenen Filter werden im **Freigegeben für mich** des Filterbereichs für diese Entitäten.

   ![Für mich freigegebene Filter](assets/new-filters-shared-with-me.png)

