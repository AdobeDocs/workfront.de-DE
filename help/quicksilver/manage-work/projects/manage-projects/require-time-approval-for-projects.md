---
product-area: projects
navigation-topic: manage-projects
title: Genehmigung für ein Projekt erforderlich
description: Genehmigung für ein Projekt erforderlich
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# Genehmigung für ein Projekt erforderlich

<!--audited: 08/2024-->

Sie können das Projekt so konfigurieren, dass die für das Projekt protokollierten Stunden vom Projekteigentümer genehmigt werden. Wenn Stunden auf diese Weise konfiguriert werden, müssen sie zunächst vom Projekteigentümer genehmigt werden, bevor sie für einen Abrechnungsdatensatz verwendet werden können.\
Weitere Informationen zu Rechnungsdatensätzen finden Sie im Artikel [Erstellen von Rechnungsdatensätzen](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Durch die Aktivierung dieser Option wird die Möglichkeit eines Timesheet-Genehmigers, die Uhrzeit auf dem Timesheet zu validieren, nicht entfernt. Wenn der Projekteigentümer die Zeit nicht validiert oder ablehnt, kann ein Timesheet-Genehmiger die Zeit weiterhin auf einem Timesheet genehmigen.

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
   <td> <p>So benötigen Sie Zeit, um das Projekt zu genehmigen:</p>
   <ul><li>Neu: Standard</li>
   <li>Aktuell: Plan</li></ul>

<p>So genehmigen Sie die in einem Projekt angemeldeten Stunden:</p>
   <ul><li>Neu: Licht oder höher</li>
   <li>Überprüfen oder höher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten oder höher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt oder höher anzeigen</p>
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzlicher Zugriff</td> 
   <td> <p>Sie müssen mindestens eine der folgenden Bedingungen erfüllen, um die Zeit für ein Projekt zu genehmigen:</p> 
    <ul> 
     <li>Sie sind der Projekteigentümer mit dem oben angegebenen Zugriff und Berechtigungen. In diesem Fall können Sie Folgendes tun, wenn eine der folgenden Bedingungen erfüllt ist: 
      <ul>
       <li>Wenn Sie über Verwaltungsberechtigungen für das Projekt verfügen, können Sie Stunden genehmigen oder ablehnen, die von einem anderen Benutzer im Projekt protokolliert wurden.</li>
       <li> Wenn Sie über Contribute- oder Projektzugriff verfügen, können Sie nur die von Ihnen oder einem anderen Benutzer, der Sie meldet, protokollierten Stunden genehmigen oder ablehnen.<br></li>
      </ul></li> 
     <li>Sie haben eine Planungslizenz mit Administratorzugriff auf Timesheets &amp; Hours. In diesem Fall:
      <ul>
       <li>Sie können alle Stunden für Projekte genehmigen oder ablehnen, für die Sie mindestens über die Berechtigung zum Anzeigen verfügen. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Genehmigung für ein Projekt erforderlich

So fordern Sie die Genehmigung des Projektmanagers für Stunden am Projekt an:

1. Rufen Sie das Projekt auf, für das Sie eine stundenlange Genehmigung benötigen möchten.
1. Klicken Sie auf das Symbol **Mehr** ![](assets/more-icon.png) rechts neben dem Projektnamen und dann auf **Bearbeiten**.\
   Das Dialogfeld Projekt bearbeiten wird angezeigt.

1. Wählen Sie im Abschnitt **Projekteinstellungen** die Option **Genehmigung der Zeit für dieses Projekt erforderlich**.
1. Klicken Sie auf **Speichern**.\
   Wenn jetzt Zeit protokolliert und genehmigt wird, werden diese Stunden gesperrt und können nicht von dem Benutzer geändert werden, der sie in das Projekt oder das Timesheet eingegeben hat. Nur ein Workfront-Administrator kann die aufgezeichnete Zeit anpassen.

## Zeit für ein Projekt genehmigen und ablehnen

Als Projektmanager können Sie Stunden genehmigen oder ablehnen, die für Aufgaben, Probleme oder das Projekt protokolliert werden.

Die Genehmigung der Stunden auf Projektebene hat keine Auswirkungen auf das Zeitblatt der Benutzer, die die Stunden protokolliert haben. Beispielsweise können die Stunden im Projekt vom Projektmanager genehmigt werden, aber das Timesheet muss noch vom Manager des Benutzers oder vom Timesheet-Genehmiger genehmigt werden.

Wenn Sie ein Projekt so einrichten, dass eine Genehmigung zu den protokollierten Stunden erforderlich ist, muss der Projektmanager die Stunden validieren, damit sie in einem Abrechnungsdatensatz für das Projekt enthalten sein können. Weitere Informationen zum Erstellen von Rechnungsdatensätzen finden Sie im Artikel [Erstellen von Rechnungsdatensätzen](../../../manage-work/projects/project-finances/create-billing-records.md).

So genehmigen oder ablehnen Sie Stunden für ein Projekt:

1. Wechseln Sie zum Projekt.
1. Klicken Sie im linken Bereich auf den Bereich **Stunden** . Dies kann sich unter dem Bereich **Mehr anzeigen** befinden.

1. Die Stunden, die für Probleme, Aufgaben und die Projektanzeige protokolliert werden, sollten den Status &quot;**Gesendet**&quot;haben.\
   Klicken Sie links neben den Stundeneinträgen auf das Kästchen, um die Stunden auszuwählen, die genehmigt werden sollen.

1. Klicken Sie oben in der Stundenliste auf das Symbol **Genehmigen** ![](assets/approve-hours-icon.png) .\
   Der Status der Stunden ändert sich in **Genehmigt**.\
   Wenn Sie die genehmigten Stunden später ablehnen, ändert sich der Status der Stunden in **Nicht genehmigt**.\
   Wenn Sie die genehmigten Stunden in einen Rechnungsdatensatz aufnehmen, ändert sich der Status der Stunden in **Abgerechnet und Genehmigt**. Stunden, die zu einem Rechnungsdatensatz hinzugefügt wurden, können nicht gelöscht werden. Weitere Informationen zum Erstellen von Rechnungsdatensätzen finden Sie im Artikel [Erstellen von Rechnungsdatensätzen](../../../manage-work/projects/project-finances/create-billing-records.md) .

1. (Optional) Klicken Sie auf das Symbol **Ablehnen** ![](assets/reject-hours-icon.png), um die Zeiteinträge im Projekt abzulehnen.\
   Der Status der Stunden ändert sich in **Abgelehnt**.

   >[!NOTE]
   >
   >   Wenn die Stunden, die Sie auswählen, in einem Rechnungsdatensatz enthalten sind, der als Abgerechnet oder Abgerechnet und Genehmigt markiert wurde, werden die Symbole Genehmigen und Ablehnen nicht angezeigt. Sie können nur Stunden genehmigen, die noch nicht in einem Rechnungsdatensatz abgerechnet wurden.

