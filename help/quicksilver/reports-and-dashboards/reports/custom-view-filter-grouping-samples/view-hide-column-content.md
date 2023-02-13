---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Inhalt einer Spalte ausblenden"
description: Möglicherweise möchten Sie Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Ansicht: Inhalt einer Spalte ausblenden

Möglicherweise möchten Sie Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.

>[!TIP]
>
>* Sie können ausgeblendete Spalten verwenden, um nach einem bestimmten Objekt zu sortieren, das nicht in der Ansicht angezeigt werden soll.\
   >  Sie können beispielsweise in einer Aufgabenansicht nach Aufgabennummer sortieren und die Informationen zur Aufgabennummer in der Ansicht ausblenden. In diesem Fall hilft das Objekt, auf das in der Spalte verwiesen wird, die Ansicht zu sortieren, die Informationen dieses Objekts werden jedoch nicht in der Ansicht angezeigt.
>* Wenn Sie eine Spalte ausblenden, beachten Sie, dass die Informationen in der Spalte ausgeblendet sind, die Spalte jedoch noch in der Ansicht vorhanden ist.
>


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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Beispiel: Sortieren und Ausblenden der Spalte &quot;Task Number&quot;in einer Aufgabenansicht:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht**.

1. Klicken **Spalte hinzufügen** und beginnen Sie mit der Eingabe von &quot;Task Number&quot;im **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:

   <pre><strong>display name=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueFormat=int<br><strong>width=0</strong></pre>Die wichtigsten Änderungen in diesem Code, durch die die Spalte ausgeblendet wird, sind:

   ```
   displayname
   ```

   Diese Zeile muss leer sein.

   ```
   valuefield
   ```

   Dies wurde durch *value*, und muss leer sein.

   ```
   width
   ```

   : Je nach Feld muss der Wert *0* oder *1*.

1. Klicken **Speichern**, dann **Ansicht speichern**.
