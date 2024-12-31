---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen : Ausblenden des Inhalts einer Spalte'
description: Sie können Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.
author: Nolan
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

# Anzeigen : Blendet den Inhalt einer Spalte aus

<!--Audited: 11/2024-->

Sie können Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.

>[!NOTE]
>
>* Sie können ausgeblendete Spalten verwenden, um nach einem bestimmten Objekt zu sortieren, das Sie nicht in der Ansicht anzeigen möchten.\
>  Sie können beispielsweise in einer Vorgangsansicht nach Vorgangsnummer sortieren und die Informationen zur Vorgangsnummer aus der Ansicht ausblenden. In diesem Fall hilft das Objekt, auf das in der Spalte verwiesen wird, beim Sortieren der Ansicht, aber die Informationen zu diesem Objekt werden nicht in der Ansicht angezeigt.
>* Beachten Sie beim Ausblenden einer Spalte, dass die Informationen in der Spalte ausgeblendet sind, die Spalte jedoch weiterhin in der Ansicht vorhanden ist.
>

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

## Beispiel: Sortieren und Ausblenden der Spalte „Aufgabennummer“ in einer Aufgabenansicht:

1. Zu einer Aufgabenliste gehen.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen** und geben Sie „Aufgabennummer“ in das Feld **In dieser Spalte anzeigen** und wählen Sie diese aus, wenn sie in der Liste angezeigt wird.

1. Klicken Sie **Wechseln Sie in den Textmodus** und dann **Text bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

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
   * `valuefield=`: Dies wurde durch `value` ersetzt und muss leer sein.
   * `width=`: Abhängig vom Feld muss dieser den Wert **0** oder **1** haben.

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
