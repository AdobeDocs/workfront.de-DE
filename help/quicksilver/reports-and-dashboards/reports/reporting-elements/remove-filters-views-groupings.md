---
product-area: reporting
navigation-topic: reporting-elements
title: Entfernen von Filtern, Ansichten und Gruppierungen
description: Sie können Filter, Ansichten oder Gruppierungen aus Listen und Berichten entfernen, wenn Sie sie erstellt haben oder für Sie freigegeben haben. Standardfilter, Ansichten oder Gruppierungen können nicht entfernt werden.
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '844'
ht-degree: 1%

---

# Entfernen von Filtern, Ansichten und Gruppierungen

Sie können Filter, Ansichten oder Gruppierungen aus Listen und Berichten entfernen, wenn Sie sie erstellt haben oder für Sie freigegeben haben. Standardfilter, Ansichten oder Gruppierungen können nicht entfernt werden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle </p> </td> 
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
   <td> <p>Berechtigungen mit Zugriff auf die Freigabe für Filter, Ansichten oder Gruppen anzeigen, die Sie entfernen möchten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Entfernen oder Löschen von Filtern mit dem Standard-Builder

Sie können einen für Sie freigegebenen Filter aus Listen mit Projekten, Aufgaben oder Problemen mithilfe der Standard-Builder-Oberfläche entfernen. Die Standard-Builder-Oberfläche ist für keine anderen Objekte oder für Ansichten oder Gruppierungen verfügbar.

Sie können Filter, die Ihnen gehören, auch aus Listen mit Projekten, Aufgaben oder Problemen löschen, indem Sie die standardmäßige Builder-Oberfläche verwenden.

Systemstandardfilter können nicht entfernt oder gelöscht werden.

### Überlegungen zum Entfernen oder Löschen von Filtern mit dem Standard-Builder

Die folgenden Szenarien stehen zur Verfügung, wenn Sie einen Filter mit dem Standard-Builder entfernen oder löschen:

* Wenn der Filter für Sie freigegeben wurde und Sie ihn entfernen, wird der Filter nur für Sie entfernt. Der Benutzer, der ihn ursprünglich erstellt hat, und alle anderen Benutzer, für die er freigegeben wurde, haben weiterhin Zugriff auf den Filter.
* Wenn der Filter Ihnen gehört und Sie ihn löschen, wird er aus dem Workfront-System entfernt. Der Filter steht Benutzern nicht mehr zur Verfügung, die ihn zuvor freigegeben haben.
* Wenn Sie Workfront-Administrator sind, können Sie den Filter löschen und er wird für alle Benutzer, einschließlich des Eigentümers, dauerhaft gelöscht.

### Filter mit dem Standard-Builder entfernen

1. Gehen Sie zu einer Liste von Projekten, Aufgaben, Problemen, Portfolios, Programmen, Benutzern, Vorlagen oder Gruppen.
1. Klicken Sie auf das Symbol **Filter** ![Filtersymbol](assets/filter-nwepng.png).
1. Bewegen Sie den Mauszeiger über einen Filter unter **Für mich freigegeben**, klicken Sie auf das Symbol **Mehr** Menü ![Mehr und klicken Sie dann auf ](assets/more-icon-spectrum.png) und dann auf **Entfernen**.

   ![Filter entfernen](assets/new-filters-more-menu-remove-filter.png)

1. Wählen Sie in der Bestätigungsmeldung **Entfernen** aus, um den Filter dauerhaft zu entfernen.

### Filter mit dem Standard-Builder löschen

1. Gehen Sie zu einer Liste von Projekten, Aufgaben, Problemen, Portfolios, Programmen, Benutzern, Vorlagen oder Gruppen.
1. Klicken Sie auf das Symbol **Filter** ![Filtersymbol](assets/filter-nwepng.png).
1. Bewegen Sie den Mauszeiger über einen Filter, den Sie löschen können, klicken Sie auf das Symbol **Mehr** Menü ![Mehr ](assets/more-icon-spectrum.png) und klicken Sie dann auf **Löschen**.

   ![Filter löschen](assets/new-filters-more-menu-options-with-delete.png)

1. (Optional) Klicken Sie in der Bestätigungsmeldung auf **Abbrechen** , um das Löschen zu vermeiden und zur Filterliste zurückzukehren.
1. Klicken Sie in der Bestätigungsmeldung auf **Löschen** , um den Löschvorgang zu bestätigen.

   Der Filter wird für Sie und alle Benutzer gelöscht, die über entsprechende Berechtigungen verfügen.

## Entfernen von Filtern, Ansichten oder Gruppierungen mithilfe des Legacy-Builders

Sie können einen Filter, eine Ansicht oder eine Gruppierung für alle Objektlisten mithilfe der alten Builder-Oberfläche entfernen.

### Überlegungen zum Entfernen von Filtern, Ansichten und Gruppierungen mithilfe des Legacy-Builders

Wie Sie ein Berichterstellungselement entfernen, hängt davon ab, ob Sie es ursprünglich erstellt oder für Sie freigegeben haben.

Die folgenden Szenarien stehen zur Verfügung, wenn Sie einen Filter, eine Ansicht oder eine Gruppierung entfernen:

* **Wenn Sie das Element erstellt und entfernt haben**, wird das Element aus dem Workfront-System entfernt. Sie steht nicht mehr Benutzern zur Verfügung, für die Sie sie zuvor freigegeben haben.
* **Wenn das Element für Sie freigegeben wurde und Sie es entfernen**, wird das Element nur für Sie entfernt. Der Benutzer, der das Asset ursprünglich erstellt hat, und alle anderen Benutzer, für die es freigegeben wurde, haben weiterhin Zugriff darauf.

### Entfernen von Filtern, Ansichten oder Gruppierungen mithilfe des Legacy-Builders

1. Gehen Sie zu einer Liste von Objekten oder einem Bericht.
1. (Bedingt) Klicken Sie in einer Liste auf das Symbol &quot;**Filter**&quot;, &quot;**Ansicht**&quot;oder &quot;**Gruppierung**&quot;. Bewegen Sie dann den Mauszeiger über den zu entfernenden Filter, die gewünschte Ansicht oder Gruppierung, klicken Sie auf das Symbol &quot;**Mehr**&quot;![](assets/more-icon.png) und dann auf &quot;**Entfernen**&quot;. Der Filter, die Ansicht oder die Gruppierung werden entfernt.
1. (Bedingt) Klicken Sie in einem Bericht auf das Dropdown-Menü **Gruppierung**, **Filter** oder **Ansicht** und wählen Sie **Gruppierung entfernen**, **Filter entfernen** oder **Ansicht entfernen**.

   Das Dialogfeld **Meine Gruppierungen**, **Meine Filter,** oder **Meine Ansichten** wird angezeigt.

   Alle Berichterstellungselemente, die Sie entfernen können, sind verfügbar. Andere Berichterstellungselemente werden als abgeblendet angezeigt.

1. Klicken Sie auf das Symbol **x** neben allen Berichterstellungselementen, die Sie entfernen möchten.
1. (Bedingt) Klicken Sie auf **Ja, löschen** , wenn Sie ausgewählt haben, um einen Filter, eine Ansicht oder eine Gruppierung zu löschen, den/die Sie erstellt und später für andere freigegeben haben. Dadurch wird der Filter, die Ansicht oder die Gruppierung aus dem Workfront-System gelöscht.

   >[!TIP]
   >
   >Wenn Sie einen Filter, eine Ansicht oder eine Gruppierung entfernen, die Sie erstellt haben, ohne ihn für andere freizugeben, wird dieser aus dem System entfernt, ohne eine Bestätigung anzufordern.

1. Klicken Sie auf **Fertig**.

