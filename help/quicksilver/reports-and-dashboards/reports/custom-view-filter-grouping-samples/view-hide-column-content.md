---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Inhalt einer Spalte ausblenden"
description: Möglicherweise möchten Sie Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Ansicht: Inhalt einer Spalte ausblenden

<!--Audited: 11/2024-->

Möglicherweise möchten Sie Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.

>[!NOTE]
>
>* Sie können ausgeblendete Spalten verwenden, um nach einem bestimmten Objekt zu sortieren, das nicht in der Ansicht angezeigt werden soll.\
>  Sie können beispielsweise in einer Aufgabenansicht nach Aufgabennummer sortieren und die Informationen zur Aufgabennummer in der Ansicht ausblenden. In diesem Fall hilft das Objekt, auf das in der Spalte verwiesen wird, die Ansicht zu sortieren, die Informationen dieses Objekts werden jedoch nicht in der Ansicht angezeigt.
>* Wenn Sie eine Spalte ausblenden, beachten Sie, dass die Informationen in der Spalte ausgeblendet sind, die Spalte jedoch noch in der Ansicht vorhanden ist.
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beispiel: Sortieren und Ausblenden der Spalte &quot;Task Number&quot;in einer Aufgabenansicht:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Klicken Sie im Dropdownmenü **Ansicht** auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen** und beginnen Sie mit der Eingabe &quot;Aufgabennummer&quot;im Feld **In dieser Spalte anzeigen** und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

1. Klicken Sie auf **Wechseln zum Textmodus** und dann auf **Text bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus bearbeiten** finden, und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   Die wichtigsten Änderungen in diesem Code, die die Spalte ausblenden, sind:

   * `displayname=`: Diese Zeile muss leer sein.
   * `valuefield=`: Dieser Wert wurde durch `value` ersetzt und muss leer sein.
   * `width=`: Abhängig vom Feld muss dieser den Wert **0** oder **1** haben.

1. Klicken Sie auf **Fertig** und dann auf **Ansicht speichern**.
