---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtern: Eliminieren von Elementen in einer Liste durch Vergleich von zwei Feldern'
description: Sie können Elemente aus einer Liste filtern, indem Sie zwei ihrer Felder vergleichen. Beispielsweise können Sie nur Aufgaben anzeigen, deren tatsächliches Abschlussdatum nach dem geplanten Abschlussdatum liegt.
author: Lisa and Jenny
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Filtern: Eliminieren von Elementen in einer Liste durch Vergleich von zwei Feldern

<!--Audited: 10/2024-->

Sie können Elemente aus einer Liste filtern, indem Sie zwei ihrer Felder vergleichen. Beispielsweise können Sie nur Aufgaben anzeigen, deren tatsächliches Abschlussdatum nach dem geplanten Abschlussdatum liegt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Elemente durch Vergleichen zweier Felder filtern

1. Zu einer Aufgabenliste gehen.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.

1. Fügen Sie einen Filter für **Aufgabe:Actual Abschlussdatum** > **Größer als** > **Wählen Sie ein Datum** hinzu.

   >[!TIP]
   >
   >Wählen Sie den Filtermodifikator, den Sie für das ausgewählte Feld verwenden möchten, falls verfügbar.

1. Klicken Sie **Textmodus**.
1. Fügen Sie im angezeigten Bereich den folgenden Code hinzu:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate
   actualCompletionDate_Mod=gt
   ```

1. Klicken Sie **Übernehmen** > **Als neu speichern**.
