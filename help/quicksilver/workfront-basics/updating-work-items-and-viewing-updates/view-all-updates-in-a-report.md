---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Anzeigen aller Aktualisierungen in einem Notizbericht
description: Anzeigen aller Aktualisierungen in einem Notizbericht
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# Anzeigen aller Aktualisierungen in einem Notizbericht

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Im Bereich Aktualisierungen eines Objekts wird standardmäßig eine maximale Anzahl von 200 Aktualisierungen angezeigt. Um alle Aktualisierungen anzuzeigen, die von einem Benutzer für ein Objekt eingegeben wurden, können Sie einen Notizbericht erstellen, der alle Aktualisierungen ausgibt.

>[!NOTE]
>
>Sie können einen Bericht erstellen, um Aktualisierungen zu Objekten in der Vorschau mit dem Journaleintragsbericht anzuzeigen. Weitere Informationen finden Sie unter [Bericht über Aktualisierungen](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Neu: Standard </p>
   <p>Aktuell: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene</strong></td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Berichte, Dashboards und Kalender erstellen</p> </li> 
     <li> <p>Filter, Ansichten und Gruppierungen erstellen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Anzeigen</p> <p><b>NOTIZ</b></p>
   <p>Wenn Sie für ein Objekt keine Berechtigung zum Anzeigen oder eine höhere Berechtigung haben, werden Informationen zu diesem Objekt nicht im Bericht angezeigt.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Notizbericht erstellen

Das Erstellen eines Berichts für Anmerkungen für ein beliebiges Objekt ist unabhängig vom Objekt identisch.

So erstellen Sie beispielsweise einen Notizbericht für alle Notizen zu einem Projekt:

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken Sie auf **Berichte**.
1. Klicken Sie **Neuer Bericht** und wählen Sie dann **Hinweis**.

1. (Optional) Klicken Sie auf **Ansichten** und dann auf **Spalte hinzufügen**, um den **Namen** des **Projekts** in der Berichtsansicht hinzuzufügen. 

1. (Optional) Klicken Sie auf **Gruppierungen** und dann auf **Gruppierung hinzufügen**, um nach dem **Projektnamen** zu gruppieren, wenn Sie mehrere Projekte gleichzeitig auswerten.\
   Dadurch wird sichergestellt, dass die Notizen nach ihren jeweiligen Projekten gruppiert werden, wodurch der Bericht leichter zu lesen ist. 

1. (Optional) Klicken Sie auf **Filter** und dann **Filterregel hinzufügen**.
1. Fügen Sie einen Filter für **Hinweis** > **Notizentext** > **Ist nicht leer** hinzu.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Wenn ein Projektfeld aktualisiert wurde, zum Zeitpunkt der Aktualisierung jedoch keine Anmerkung hinzugefügt wurde, wird **Anmerkungstext** der Aktualisierung als **(Kein Text zur Aktualisierung hinzugefügt)**.


1. (Optional) Fügen Sie einen weiteren Filter für **Projekt** > **Name** > **Gleich** hinzu und fügen Sie einen oder mehrere Projektnamen hinzu, für die Sie Anmerkungen anzeigen möchten.
1. Klicken Sie auf **Speichern + schließen**.\
   Im Bericht werden alle Aktualisierungen angezeigt, die von allen Benutzern eingegeben wurden, die berechtigt sind, mindestens das Projekt anzuzeigen.
