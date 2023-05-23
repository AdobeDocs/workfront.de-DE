---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: die Breite einer Spalte dauerhaft bearbeiten"
description: Sie können die Breite von Spalten vorübergehend ändern, indem Sie die Ränder an die gewünschte Breite ziehen und dort ablegen. Weitere Informationen finden Sie unter Spaltenbreite und -reihenfolge ändern .
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 42633036-8e42-4cec-876c-f20a5ece2478
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Ansicht: Spaltenbreite dauerhaft bearbeiten

Sie können die Breite von Spalten vorübergehend ändern, indem Sie die Ränder an die gewünschte Breite ziehen und dort ablegen. Weitere Informationen finden Sie unter [Spaltenbreite und -reihenfolge ändern](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

Sie können die Breite einer beliebigen Spalte einer Ansicht dauerhaft ändern, indem Sie während der Bearbeitung der Ansicht den Textmodus in der Spalte verwenden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Dauerhaftes Bearbeiten der Spaltenbreite

>[!IMPORTANT]
>
>Wenn Sie die Breite einer Spalte manuell ändern, wie im Abschnitt &quot;Breite und Reihenfolge der Spalten vorübergehend ändern&quot;im Artikel beschrieben [Spaltenbreite und -reihenfolge ändern](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md) Wenn Sie die Breite der Spalte dauerhaft geändert haben, wird die Breite der Spalte entsprechend Ihrer manuellen Größenanpassung beibehalten und die Breite der Spalte, die gemäß den folgenden Schritten aktualisiert wird, wird überschrieben. Sie können die Spalte entsprechend der in den folgenden Schritten definierten Breite anzeigen, nachdem Sie Ihren Cache gelöscht oder sich über einen anderen Browser angemeldet haben.

1. Navigieren Sie zu einer Liste von Objekten.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht**.

1. Klicken **Spalte hinzufügen** um eine neue Spalte hinzuzufügen.

   Oder

   Klicken Sie auf die Spaltenüberschrift einer vorhandenen Spalte.

1. Klicken **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Fügen Sie den folgenden Code zum Textmodus der Spalte hinzu:

   ```
   width=200
   usewidths=true
   ```

   Für **width** eine beliebige Zahl (in Pixel) angeben, die angibt, wie breit die Spalte in der Ansicht angezeigt werden soll.

1. Klicken **Speichern**, dann **Ansicht speichern**.
