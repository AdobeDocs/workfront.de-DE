---
product-area: reporting
navigation-topic: reporting-elements
title: Entfernen von Filtern, Ansichten und Gruppierungen
description: Sie können Filter, Ansichten oder Gruppierungen aus Listen und Berichten entfernen, wenn Sie diese erstellt haben oder wenn sie für Sie freigegeben wurden. Standardfilter, Ansichten oder Gruppierungen können nicht entfernt werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '801'
ht-degree: 1%

---

# Entfernen von Filtern, Ansichten und Gruppierungen

<!-- Audited: 11/2024 -->

Sie können Filter, Ansichten oder Gruppierungen aus Listen und Berichten entfernen, wenn Sie diese erstellt haben oder wenn sie für Sie freigegeben wurden. Standardfilter, Ansichten oder Gruppierungen können nicht entfernt werden.

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
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
    <td> <p>Anzeigen von Berechtigungen mit Zugriff auf die Freigabe für den Filter, die Ansicht oder die Gruppierung, die Sie entfernen möchten</p></td> 
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entfernen oder Löschen eines Filters mit dem Standard Builder

Sie können einen Filter, der für Sie freigegeben wurde, über die Standard-Builder-Oberfläche aus Listen von Projekten, Aufgaben oder Problemen entfernen. Die Standardbenutzeroberfläche von Builder ist für keine anderen Objekte oder für Ansichten oder Gruppierungen verfügbar.

Sie können auch Filter, deren Inhaber Sie sind, über die Standard Builder-Benutzeroberfläche aus Listen von Projekten, Aufgaben oder Problemen löschen.

Systemstandardfilter können nicht entfernt oder gelöscht werden.

### Überlegungen zum Entfernen oder Löschen von Filtern mit dem Standard-Builder

Die folgenden Szenarien bestehen, wenn Sie einen Filter mit dem Standard Builder entfernen oder löschen:

* Wenn der Filter für Sie freigegeben wurde und Sie ihn entfernen, wird der Filter nur für Sie entfernt. Der Benutzer, der sie ursprünglich erstellt hat, und alle anderen Benutzer, für die sie freigegeben wurde, haben weiterhin Zugriff auf den Filter.
* Wenn Sie der Eigentümer des Filters sind und ihn löschen, wird der Filter aus dem Workfront-System entfernt. Der Filter steht Benutzern, für die Sie ihn zuvor freigegeben haben, nicht mehr zur Verfügung.
* Wenn Sie Workfront-Administrator sind, können Sie den Filter löschen. Er wird dann dauerhaft für alle Benutzenden, einschließlich des Eigentümers, gelöscht.

### Entfernen eines Filters mithilfe des Standard Builders

1. Navigieren Sie zu einer Liste mit Projekten, Aufgaben, Problemen, Portfolios, Programmen, Benutzern, Vorlagen oder Gruppen.
1. Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-nwepng.png).
1. Bewegen Sie den Mauszeiger über einen Filter unter **Für mich freigegeben** und klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/more-icon-spectrum.png) und dann auf **Entfernen**.
1. Wählen **in** Bestätigungsmeldung „Entfernen“ aus, um den Filter dauerhaft zu entfernen.

### Löschen eines Filters mithilfe des Standard Builders

1. Navigieren Sie zu einer Liste mit Projekten, Aufgaben, Problemen, Portfolios, Programmen, Benutzern, Vorlagen oder Gruppen.
1. Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-nwepng.png).
1. Bewegen Sie den Mauszeiger über einen Filter, für den Sie Löschberechtigungen haben, klicken Sie auf das Menü **Mehr** ![Mehr-Symbol](assets/more-icon-spectrum.png) und dann auf **Löschen**.

   ![Filter löschen](assets/new-filters-more-menu-options-with-delete.png)

1. (Optional) Klicken Sie **der Bestätigungsmeldung** Abbrechen), um das Löschen zu vermeiden, und kehren Sie zur Liste der Filter zurück.
1. Klicken Sie **der** auf „Löschen“, um den Löschvorgang zu bestätigen.

   Der Filter wird für Sie und alle Benutzenden gelöscht, die über die entsprechenden Berechtigungen verfügen.

## Entfernen von Filtern, Ansichten oder Gruppierungen mit dem Legacy-Builder

Sie können einen Filter, eine Ansicht oder eine Gruppierung für alle Listen von Objekten mithilfe der Legacy-Builder-Oberfläche entfernen.

### Überlegungen zum Entfernen von Filtern, Ansichten und Gruppierungen mit dem Legacy-Builder

Wie Sie ein Berichterstellungselement entfernen, hängt davon ab, ob Sie es ursprünglich erstellt haben oder ob es für Sie freigegeben wurde.

Die folgenden Szenarien bestehen, wenn Sie einen Filter, eine Ansicht oder eine Gruppierung entfernen:

* **Wenn Sie das Element erstellt und entfernt haben** wird das Element aus dem Workfront-System entfernt. Sie steht nicht mehr allen Benutzern zur Verfügung, für die Sie sie zuvor freigegeben haben.
* **Wenn das Element für Sie freigegeben wurde und Sie es entfernen** wird das Element nur für Sie entfernt. Der Benutzer, der sie ursprünglich erstellt hat, und alle anderen Benutzer, für die sie freigegeben wurde, haben weiterhin Zugriff darauf.

### Entfernen von Filtern, Ansichten oder Gruppierungen mit dem Legacy-Builder

1. Navigieren Sie zu einer Liste von Objekten oder einem Bericht.
1. (Bedingt) Klicken Sie in einer Liste auf das Symbol **Filter**, **Ansicht** oder **Gruppierung** und bewegen Sie dann den Mauszeiger über den Filter, die Ansicht oder die Gruppierung, die Sie entfernen möchten, klicken Sie auf das Symbol **Mehr** ![Mehr-Symbol](assets/more-icon.png) und dann auf **Entfernen**. Der Filter, die Ansicht oder die Gruppierung wird entfernt.
1. (Bedingt) Klicken Sie in einem Bericht auf das **Gruppierung**, **Filter** oder **Ansicht** und wählen Sie **Gruppierung entfernen**, **Filter entfernen** oder **Ansicht entfernen**.

   Das Dialogfeld **Meine**, **Meine Filter,** oder **Meine Ansichten** wird angezeigt.

   Alle Berichtselemente, zu deren Entfernung Sie berechtigt sind, können entfernt werden. Andere Berichtselemente werden abgeblendet angezeigt.

1. Klicken Sie auf das **x**-Symbol neben einem beliebigen Berichtselement, das Sie entfernen möchten.
1. (Bedingt) Klicken Sie auf **Ja, Löschen**, wenn Sie einen Filter, eine Ansicht oder eine Gruppierung löschen möchten, die Sie erstellt und später für andere freigegeben haben. Dadurch werden der Filter, die Ansicht oder die Gruppierung aus dem Workfront-System gelöscht.

   >[!TIP]
   >
   >Wenn Sie einen Filter, eine Ansicht oder eine Gruppierung entfernen, ohne ihn für andere freizugeben, wird er/sie aus dem System entfernt, ohne dass Sie um eine Bestätigung gebeten werden.

1. Klicken Sie auf **Fertig**.

