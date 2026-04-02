---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen : Ausblenden des Inhalts einer Spalte'
description: Sie können Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.
author: Courtney
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 13%

---

# Ansicht: Inhalt einer Spalte ausblenden

<!--Audited: 11/2024-->

Sie können Informationen in der Spalte einer Ansicht ausblenden. Sie können dies tun, indem Sie den Textmodus der Spalte ändern.

>[!NOTE]
>
>* Sie können ausgeblendete Spalten verwenden, um nach einem bestimmten Objekt zu sortieren, das Sie nicht in der Ansicht anzeigen möchten.\
>  Sie können beispielsweise in einer Vorgangsansicht nach Vorgangsnummer sortieren und die Informationen zur Vorgangsnummer aus der Ansicht ausblenden. In diesem Fall hilft das Objekt, auf das in der Spalte verwiesen wird, beim Sortieren der Ansicht, aber die Informationen zu diesem Objekt werden nicht in der Ansicht angezeigt.
>* Beachten Sie beim Ausblenden einer Spalte, dass die Informationen in der Spalte ausgeblendet sind, die Spalte jedoch weiterhin in der Ansicht vorhanden ist.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkender oder Anfrage zum Ändern einer Ansicht </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Beispiel: Sortieren und Ausblenden der Spalte „Aufgabennummer“ in einer Aufgabenansicht:

1. Zu einer Aufgabenliste gehen.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen** und geben Sie „Aufgabennummer“ in das Feld **In dieser Spalte anzeigen** und wählen Sie diese aus, wenn sie in der Liste angezeigt wird.

1. Klicken Sie **Wechseln Sie in den Textmodus** und dann **Textmodus bearbeiten**.
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
   * `valuefield=`: Diese Zeile muss durch `value=` ersetzt werden, die leer sein muss.
   * `width=`: Abhängig vom Feld muss dieser den Wert **0** oder **1** haben.

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
