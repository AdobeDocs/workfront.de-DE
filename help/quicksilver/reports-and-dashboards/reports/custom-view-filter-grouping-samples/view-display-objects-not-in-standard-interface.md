---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Anzeigen von Objekten, die nicht in der Standardoberfläche enthalten sind'
description: 'Sie können Objekte anzeigen, die nicht in der Benutzeroberfläche des Standardmodus enthalten sind. Dies ist nur möglich, wenn Sie sie über den Textmodus referenzieren. Sie können auf eine der folgenden Arten bestimmen, welche Felder in eine Ansicht aufgenommen werden können: BEARBEITEN SIE MICH.'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Ansicht: Anzeigen von Objekten, die nicht in der Standardoberfläche enthalten sind

Sie können Objekte anzeigen, die nicht in der Benutzeroberfläche des Standardmodus enthalten sind. Dies ist nur möglich, wenn Sie sie über den Textmodus referenzieren.\
Sie können auf eine der folgenden Arten bestimmen, welche Felder in eine Ansicht aufgenommen werden können:

* Verwenden Sie die [API-Explorer](../../../wf-api/general/api-explorer.md) , um andere Objekte zu finden, auf die über den Textmodus verwiesen werden kann.\
   Nicht alle im API Explorer dokumentierten Felder sind gültige Felder für den Textmodus. Einige Felder sind nur über die API meldebar.

* Suchen Sie das ID-Feld des Objekts in einer Spalte. Die meisten Objekte mit einer Feld-ID haben auch einen entsprechenden Spalten- oder Feldnamen, auf den über die Benutzeroberfläche des Standardmodus möglicherweise nicht zugegriffen werden kann.

   Sie können den Textmodus verwenden, um die Spalte oder den Feldnamen anstelle der ID in eine Ansicht aufzunehmen, indem Sie die `fieldnameID` mit dem `fieldname:name`.

   In der Benutzeroberfläche für den Standardmodus kann beispielsweise die Variable **Portfolio Owner ID** -Feld für eine Projektansicht verfügbar ist, aber die **Name des Portfolios-Eigentümers** nicht. Sie können den Textmodus verwenden, um die **Name des Portfolios-Eigentümers** in der Spalte einer Ansicht.

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

## Beispiel: Hinzufügen der Spalte &quot;Portfolio Owner Name&quot;zu einer Projektansicht

1. Gehen Sie zu einer Projektliste.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht**.

1. Klicken **Spalte hinzufügen** Geben Sie dann &quot;Portfolio Owner ID&quot;in die **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Ersetzen Sie die `valuefield` Linie (`valuefield=portfolio:ownerID`) mit der folgenden Zeile:

   ```
   valuefield=portfolio:owner:name
   ```

   Oder

   Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   In diesem Beispiel sortiert der Bericht den Bericht nach der Portfolio-Eigentümer-ID, wie durch die Variable `querysort` Linie.

   >[!TIP]
   >
   >So ersetzen Sie beliebige Felder `ID` durch das Feld `name` im Textmodus immer ersetzen `ID` mit `:name` im `valuefield` Linie.

1. Klicken **Speichern**, dann **Ansicht speichern**.
