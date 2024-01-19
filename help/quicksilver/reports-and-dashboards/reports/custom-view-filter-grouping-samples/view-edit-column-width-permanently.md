---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Breite einer Spalte dauerhaft bearbeiten"
description: Sie können die Breite von Spalten vorübergehend ändern, indem Sie die Ränder an die gewünschte Breite ziehen und dort ablegen. Weitere Informationen finden Sie unter Spaltenbreite und -reihenfolge ändern .
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 261c1b73d785094de4ee8549c856a091920ba04a
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Ansicht: Breite einer Spalte dauerhaft bearbeiten

<!-- Audited: 1/2024 -->

Sie können die Breite von Spalten vorübergehend ändern, indem Sie die Ränder an die gewünschte Breite ziehen und dort ablegen. Weitere Informationen finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Um die Breite einer beliebigen Spalte einer Ansicht dauerhaft zu ändern, müssen Sie den Textmodus in der Spalte verwenden, während Sie die Ansicht bearbeiten.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu:<ul><li>Mitwirkender beim Ändern einer Ansicht</li><li>Standard zum Ändern eines Berichts</li></ul></p><p>Oder</p>Aktuell:<ul><li>Anforderung zum Ändern einer Ansicht</li><li>Berichtänderung planen</li></ul></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Dauerhaftes Bearbeiten der Spaltenbreite

>[!IMPORTANT]
>
>Wenn Sie die Breite einer Spalte manuell ändern, wie im Abschnitt beschrieben [Länge und Reihenfolge der Spalten vorübergehend ändern](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md#modify-width-and-order-of-columns-temporarily) im Artikel [Spaltenbreite und -reihenfolge ändern](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) Wenn Sie die Breite der Spalte dauerhaft geändert haben, wird die Breite der Spalte entsprechend der manuellen Größenanpassung beibehalten. In diesem Fall wird die Breite der Spalte, die gemäß den folgenden Schritten aktualisiert wurde, überschrieben. Sie können die Spalte entsprechend der in den folgenden Schritten definierten Breite anzeigen, nachdem Sie Ihren Cache gelöscht oder sich über einen anderen Browser angemeldet haben.
>
>Weitere Informationen zum Anpassen der Spaltenbreite bei Verwendung der Benutzeroberfläche für den Textmodus finden Sie in den Definitionen &quot;Breite&quot;und &quot;Stretch&quot;im [Glossar der Adobe Workfront-Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. Navigieren Sie zu einer Liste von Objekten.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht**.

1. Klicks **Spalte hinzufügen** um eine neue Spalte hinzuzufügen.

   Oder

   Klicken Sie auf die Spaltenüberschrift einer vorhandenen Spalte.

1. Klicks **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Fügen Sie den folgenden Code zum Textmodus der Spalte hinzu:

   ```
   width=200
   usewidths=true
   ```

   Für **width** eine beliebige Zahl (in Pixel) angeben, die angibt, wie breit die Spalte in der Ansicht angezeigt werden soll.

1. Klicks **Speichern**, dann **Ansicht speichern**.


