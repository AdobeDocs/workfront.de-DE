---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Löscht Elemente in einer Liste durch Vergleich zweier Felder'
description: Sie können Elemente aus einer Liste filtern, indem Sie zwei ihrer Felder miteinander vergleichen. Beispielsweise können Sie nur Aufgaben anzeigen, bei denen das tatsächliche Abschlussdatum der Aufgabe größer als das geplante Abschlussdatum ist.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 4532e08bddf993426e9d4eed6f7f8bd638663188
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Filter: Löscht Elemente in einer Liste durch Vergleich zweier Felder

<!--Audited: 10/2024-->

Sie können Elemente aus einer Liste filtern, indem Sie zwei ihrer Felder miteinander vergleichen. Beispielsweise können Sie nur Aufgaben anzeigen, bei denen das tatsächliche Abschlussdatum der Aufgabe größer als das geplante Abschlussdatum ist.

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtern von Elementen durch Vergleich zweier Felder

1. Gehen Sie zu einer Liste von Aufgaben.
1. Wählen Sie aus dem Dropdownmenü **Filter** die Option **Neuer Filter** aus.

1. Fügen Sie einen Filter für **Aufgabe:Tatsächliches Abschlussdatum** > **Größer als** > **Datum auswählen** hinzu.

   >[!TIP]
   >
   >Wählen Sie den Filter-Modifikator aus, den Sie für das ausgewählte Feld verwenden möchten (falls verfügbar).

1. Klicken Sie auf **Textmodus**.
1. Fügen Sie in dem angezeigten Bereich den folgenden Code hinzu:

   `actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt`

1. Klicken Sie auf **Anwenden** > **Als neu speichern**.
