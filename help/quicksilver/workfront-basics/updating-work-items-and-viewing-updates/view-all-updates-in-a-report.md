---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Anzeigen aller Aktualisierungen in einem Notizbericht
description: Um alle Aktualisierungen anzuzeigen, die von einem Benutzer für ein Objekt eingegeben wurden, können Sie einen Notizbericht erstellen, der alle Aktualisierungen ausgibt.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 5%

---

# Anzeigen aller Aktualisierungen in einem Notizbericht

<!-- Audited: 10/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Im Bereich Aktualisierungen eines Objekts wird standardmäßig eine maximale Anzahl von 200 Aktualisierungen angezeigt. Um alle Aktualisierungen anzuzeigen, die von einem Benutzer für ein Objekt eingegeben wurden, können Sie einen Notizbericht erstellen, der alle Aktualisierungen ausgibt.

>[!NOTE]
>
>Sie können einen Bericht erstellen, um Aktualisierungen zu Objekten in der Vorschau mit dem Journaleintragsbericht anzuzeigen. Weitere Informationen finden Sie unter [Bericht im Bereich Aktualisierungen mit einem Journaleintragsbericht](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Bearbeiten Sie den Zugriff und erstellen Sie Folgendes:</p> 
    <ul> 
     <li> <p>Berichte, Dashboards und Kalender</p> </li> 
     <li> <p>Filter, Ansichten und Gruppierungen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Objekte im Bericht anzeigen</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to:</p> 
    <ul> 
     <li> <p>Create Reports, Dashboards, and Calendars</p> </li> 
     <li> <p>Create Filters, Views, and Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View</p>
    <p>Note: If you do not have View permission or higher to an object, information for that object doesn't display in the report.</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Notizbericht erstellen

Das Erstellen eines Berichts für Anmerkungen für ein beliebiges Objekt ist unabhängig vom Objekt identisch.

So erstellen Sie beispielsweise einen Notizbericht für alle Notizen zu einem Projekt:

{{step1-to-reports}}

1. Klicken Sie oben links auf der Seite auf **Neuer Bericht** und wählen Sie dann **Hinweis**.

1. (Optional) Klicken Sie auf **(Spalten) Ansicht** und dann auf **Spalte hinzufügen**, um den **Namen** des **Projekts** in der Berichtsansicht hinzuzufügen.

1. (Optional) Wenn Sie Berichte zu mehreren Projekten gleichzeitig erstellen, klicken Sie auf **Gruppierungen** und dann auf **Gruppierung hinzufügen**, um nach dem **Namen** des **Projekts**. Dadurch wird sichergestellt, dass die Notizen nach ihren jeweiligen Projekten gruppiert werden, wodurch der Bericht leichter zu lesen ist.

1. (Optional) Klicken Sie auf **Filter** und dann **Filterregel hinzufügen**.
1. Fügen Sie einen Filter für **Hinweis** > **Notizentext** > **Ist nicht leer** hinzu.

   ![Notizentext-Feld ist kein leerer Filter](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Wenn ein Projektfeld aktualisiert wurde, zum Zeitpunkt der Aktualisierung jedoch keine Anmerkung hinzugefügt wurde, wird **Anmerkungstext** der Aktualisierung als **(Kein Text zur Aktualisierung hinzugefügt)**.


1. (Optional) Fügen Sie einen weiteren Filter für **Projekt** > **Name** > **Gleich** hinzu und fügen Sie einen oder mehrere Projektnamen hinzu, für die Sie Anmerkungen anzeigen möchten.
1. Klicken Sie **Speichern + Schließen**. Im Bericht werden alle Aktualisierungen angezeigt, die von allen Benutzern eingegeben wurden, die über die Berechtigung zum Anzeigen des Projekts verfügen.
