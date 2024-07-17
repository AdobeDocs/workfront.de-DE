---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Alle Aktualisierungen in einem Hinweis-Bericht anzeigen
description: Alle Aktualisierungen in einem Hinweis-Bericht anzeigen
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 1%

---

# Alle Aktualisierungen in einem Hinweis-Bericht anzeigen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Im Bereich Updates eines Objekts wird standardmäßig maximal 200 Updates angezeigt. Um alle Aktualisierungen anzuzeigen, die ein Benutzer für ein Objekt eingegeben hat, können Sie einen Hinweis-Bericht erstellen, der alle Aktualisierungen anzeigt.

>[!NOTE]
>
>Sie können einen Bericht erstellen, um mithilfe des Journaleintragsberichts Aktualisierungen zu Objekten in der Vorschau anzuzeigen. Weitere Informationen finden Sie unter [Bericht über den Aktualisierungsbereich](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Abo</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Neu: Standard </p>
   <p>Aktuell: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Erstellen von Berichten, Dashboards und Kalendern</p> </li> 
     <li> <p>Erstellen von Filtern, Ansichten und Gruppen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Anzeigen</p> <p><b>NOTIZ</b></p>
   <p>Wenn Sie keine Ansichtsberechtigung oder eine höhere Berechtigung für ein Objekt haben, werden die Informationen für dieses Objekt nicht im Bericht angezeigt.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in Adobe Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Erstellen eines Berichts mit Anmerkungen

Das Erstellen eines Berichts für Anmerkungen für Objekte ist unabhängig vom Objekt identisch.

So erstellen Sie beispielsweise einen Notiz -Bericht für alle Notizen in einem Projekt:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Berichte**.
1. Klicken Sie auf **Neuer Bericht** und wählen Sie dann **Hinweis** aus.

1. (Optional) Klicken Sie auf **Ansichten** und dann auf **Spalte hinzufügen** , um den **Namen** des **Projekts** in der Ansicht des Berichts hinzuzufügen. 

1. (Optional) Klicken Sie auf **Gruppierungen** und dann auf **Gruppierung hinzufügen** , um sie nach dem **Projektnamen** zu gruppieren, wenn Sie gleichzeitig über mehrere Projekte berichten.\
   Dadurch wird sichergestellt, dass die Notizen nach ihren jeweiligen Projekten gruppiert werden, was das Lesen des Berichts erleichtert. 

1. (Optional) Klicken Sie auf **Filter,** und dann auf **Filterregel hinzufügen**.
1. Fügen Sie einen Filter für **Hinweis** > **Hinweis-Text** > **ist nicht leer** hinzu.

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   Wenn ein Projektfeld aktualisiert wurde, zum Zeitpunkt der Aktualisierung jedoch keine Notiz hinzugefügt wurde, wird der **Hinweis-Text** der Aktualisierung als **(Kein zu aktualisierender Text)** angezeigt.


1. (Optional) Fügen Sie einen weiteren Filter für **Projekt** > **Name** > **Entspricht** hinzu und fügen Sie einen oder mehrere Projektnamen hinzu, für die Sie Notizen anzeigen möchten.
1. Klicken Sie auf **Speichern + schließen**.\
   Alle Aktualisierungen, die im Projekt von allen Benutzern mit der Berechtigung zum Anzeigen des Projekts eingegeben wurden, werden im Bericht angezeigt.
