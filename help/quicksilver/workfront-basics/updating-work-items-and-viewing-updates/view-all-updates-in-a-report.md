---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Anzeigen aller Aktualisierungen in einem Notizbericht
description: Um alle Aktualisierungen anzuzeigen, die von einem Benutzer für ein Objekt eingegeben wurden, können Sie einen Notizbericht erstellen, der alle Aktualisierungen ausgibt.
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# Anzeigen aller Aktualisierungen in einem Notizbericht

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Im Bereich Aktualisierungen eines Objekts wird standardmäßig eine maximale Anzahl von 200 Aktualisierungen angezeigt. Um alle Aktualisierungen anzuzeigen, die von einem Benutzer für ein Objekt eingegeben wurden, können Sie einen Notizbericht erstellen, der alle Aktualisierungen ausgibt.

>[!NOTE]
>
>Sie können einen Bericht erstellen, um Aktualisierungen zu Objekten in der Vorschau mit dem Journaleintragsbericht anzuzeigen. Weitere Informationen finden Sie unter [Bericht im Bereich Aktualisierungen mit einem Journaleintragsbericht](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard </p>
   <p>Aktuell: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Berichte, Dashboards und Kalender erstellen</p> </li> 
     <li> <p>Filter, Ansichten und Gruppierungen erstellen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen</p>
    <p>Hinweis: Wenn Sie für ein Objekt keine Anzeigeberechtigung oder höher haben, werden Informationen zu diesem Objekt nicht im Bericht angezeigt.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Notizbericht erstellen

Das Erstellen eines Berichts für Anmerkungen für ein beliebiges Objekt ist unabhängig vom Objekt identisch.

So erstellen Sie beispielsweise einen Notizbericht für alle Notizen zu einem Projekt:

{{step1-to-reports}}

1. Klicken Sie oben links auf der Seite auf **Neuer Bericht** und wählen Sie dann **Hinweis**.

1. (Optional) Klicken Sie auf **(Spalten) Ansicht** und dann auf **Spalte hinzufügen**, um den **Namen** des **Projekts** in der Berichtsansicht hinzuzufügen. 

1. (Optional) Wenn Sie Berichte zu mehreren Projekten gleichzeitig erstellen, klicken Sie auf **Gruppierungen** und dann auf **Gruppierung hinzufügen**, um nach dem **Namen** des **Projekts**. Dadurch wird sichergestellt, dass die Notizen nach ihren jeweiligen Projekten gruppiert werden, wodurch der Bericht leichter zu lesen ist. 

1. (Optional) Klicken Sie auf **Filter** und dann **Filterregel hinzufügen**.
1. Fügen Sie einen Filter für **Hinweis** > **Notizentext** > **Ist nicht leer** hinzu.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Wenn ein Projektfeld aktualisiert wurde, zum Zeitpunkt der Aktualisierung jedoch keine Anmerkung hinzugefügt wurde, wird **Anmerkungstext** der Aktualisierung als **(Kein Text zur Aktualisierung hinzugefügt)**.


1. (Optional) Fügen Sie einen weiteren Filter für **Projekt** > **Name** > **Gleich** hinzu und fügen Sie einen oder mehrere Projektnamen hinzu, für die Sie Anmerkungen anzeigen möchten.
1. Klicken Sie **Speichern + Schließen**. Im Bericht werden alle Aktualisierungen angezeigt, die von allen Benutzern eingegeben wurden, die über die Berechtigung zum Anzeigen des Projekts verfügen.
