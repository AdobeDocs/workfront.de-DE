---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Inhalt einer Spalte ausblenden"
description: Möglicherweise möchten Sie Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '423'
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
   <td> <p>Alle</p> </td> 
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
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Beispiel: Sortieren und Ausblenden der Spalte &quot;Task Number&quot;in einer Aufgabenansicht:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Klicken Sie im Dropdownmenü **Ansicht** auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen** und beginnen Sie mit der Eingabe &quot;Aufgabennummer&quot;im Feld **In dieser Spalte anzeigen** und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:

   <pre><strong>displayName=</strong>linkedname=direct<br>querysort=taskNumber<br>sortOrder=1<br>sortType=asc<br>textmode=true<br><strong>value=</strong>valueFormat=int<br><strong>width=0</strong></pre>Die wichtigsten Änderungen in diesem Code, die die Spalte ausblenden, sind:

   ```
   displayname
   ```

   Diese Zeile muss leer sein.

   ```
   valuefield
   ```

   Dieser Wert wurde durch den Wert *1} ersetzt und muss leer sein.*

   ```
   width
   ```

   : Abhängig vom Feld muss dieser den Wert *0* oder *1* haben.

1. Klicken Sie auf **Speichern** und dann auf **Ansicht speichern**.
