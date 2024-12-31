---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Die Breite einer Spalte dauerhaft bearbeiten'
description: Sie können die Spaltenbreite vorübergehend ändern, indem Sie die Ränder der Spalten an die gewünschte Breite ziehen und ablegen. Weitere Informationen finden Sie unter Ändern der Spaltenbreite und -reihenfolge.
author: Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 71c0bf664af66bec7122651c1b62dd1c28022565
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Ansicht: Die Breite einer Spalte dauerhaft bearbeiten

<!-- Audited: 11/2024 -->

Sie können die Spaltenbreite vorübergehend ändern, indem Sie die Ränder der Spalten an die gewünschte Breite ziehen und ablegen. Weitere Informationen finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Um die Breite einer Spalte einer Ansicht dauerhaft zu ändern, müssen Sie beim Bearbeiten der Ansicht den Textmodus in der Spalte verwenden.

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
   <td> <p>Neu:<ul><li>Mitwirkende zum Ändern einer Ansicht</li><li>Standard zum Ändern eines Berichts</li></ul></p><p>Oder</p>Aktuell:<ul><li>Änderung einer Ansicht anfordern</li><li>Planen der Änderung eines Berichts</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Die Breite einer Spalte dauerhaft bearbeiten

>[!IMPORTANT]
>
>Wenn Sie die Breite einer Spalte manuell ändern, wie im Abschnitt [Ändern der Breite und Reihenfolge von Spalten](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) im Artikel [Ändern der Spaltenbreite und -reihenfolge](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) beschrieben, nachdem Sie die Breite der Spalte dauerhaft geändert haben, wird die Breite der Spalte gemäß Ihrer manuellen Größenanpassung beibehalten. In diesem Fall wird die Breite der Spalte, die gemäß den folgenden Schritten aktualisiert wird, überschrieben. Sie können die Spalte entsprechend der in den folgenden Schritten definierten Breite anzeigen, nachdem Sie Ihren Cache gelöscht oder sich von einem anderen Browser aus angemeldet haben.
>
>Weitere Informationen zum Anpassen der Spaltenbreite bei Verwendung der Textmodusschnittstelle finden Sie unter den Definitionen „Breite“ und „Dehnung“ im [Glossar der Adobe Workfront-Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Navigieren Sie zu einer Liste von Objekten.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**.

1. Klicken Sie **Spalte hinzufügen**, um eine neue Spalte hinzuzufügen.

   Oder

   Klicken Sie auf die Spaltenüberschrift einer vorhandenen Spalte.

1. Klicken Sie **In Textmodus wechseln**.
1. Klicken Sie **Textmodus bearbeiten**.t
1. Fügen Sie den folgenden Code zum Textmodus der Spalte hinzu:

   ```
   width=200
   usewidths=true
   ```

   Geben Sie für **Zeile** width) eine beliebige Zahl (in Pixeln) an, die angibt, wie breit die Spalte in der Ansicht angezeigt werden soll.

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.


