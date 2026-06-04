---
product-area: projects
navigation-topic: manage-projects
title: Genehmigung von Zeit für ein Projekt verlangen
description: Sie können das Projekt so konfigurieren, dass die für das Projekt protokollierten Stunden vom Projektbesitzer genehmigt werden müssen. Wenn Stunden auf diese Weise konfiguriert sind, müssen sie zunächst vom Projektbesitzer genehmigt werden, bevor sie für einen Rechnungsnachweis verwendet werden können.
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Ux3CyN-AC7EKD74-GKadkODI3rCBcIIcQIH26LKCA-Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 774
ht-degree: 6%

---

# Anfordern der Genehmigung des Zeitaufwands für ein Projekt

<!--audited: 08/2024-->

Sie können das Projekt so konfigurieren, dass die für das Projekt protokollierten Stunden vom Projektbesitzer genehmigt werden müssen. Wenn Stunden auf diese Weise konfiguriert sind, müssen sie zunächst vom Projektbesitzer genehmigt werden, bevor sie für einen Rechnungsnachweis verwendet werden können.\
Weitere Informationen zu Rechnungsnachweisen finden Sie im Artikel [Rechnungsnachweise erstellen](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Durch Aktivierung dieser Option wird die Fähigkeit einer genehmigenden Person für Arbeitszeittabellen, die Zeit in der Arbeitszeittabelle zu genehmigen, nicht entfernt. Wenn der Projektinhaber die Zeit nicht genehmigt oder ablehnt, kann ein Arbeitszeittabellen-Genehmiger die Zeit in einer Arbeitszeittabelle trotzdem genehmigen.

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
   <td> <p>So benötigen Sie Zeit für die Genehmigung des Projekts:</p>
   <ul><li><p>Standard</p></li>
   <li><p>Plan</p></li></ul>

<p>So genehmigen Sie für ein Projekt protokollierte Stunden:</p>
   <ul><li><p>Licht oder höher</p></li>
   <li><p>Überprüfen oder höher</p></li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für das Projekt oder höher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzlicher Zugriff</td> 
   <td> <p>Sie müssen mindestens eine der folgenden Bedingungen erfüllen, um die Zeit für ein Projekt zu genehmigen:</p> 
    <ul> 
     <li>Sie sind der Projektbesitzer mit den oben angegebenen Zugriffsrechten und Berechtigungen. In diesem Fall können Sie Folgendes tun, wenn eine der folgenden Bedingungen vorliegt: 
      <ul>
       <li>Wenn Sie über Verwaltungsberechtigungen für das Projekt verfügen, können Sie Stunden genehmigen oder ablehnen, die von einem anderen Benutzer für das Projekt protokolliert wurden.</li>
       <li> Wenn Sie Zugriff auf „Beitragen“ oder „Anzeigen“ für das Projekt haben, können Sie nur die von Ihnen oder einem anderen Benutzer, der Sie meldet, protokollierten Stunden genehmigen oder ablehnen.<br></li>
      </ul></li> 
     <li>Sie verfügen über eine Standard- oder Planlizenz mit administrativem Zugriff auf Arbeitszeittabellen und Stunden. In diesem Fall:
      <ul>
       <li>Sie können für die Projekte, für die Sie mindestens über die Berechtigung zum Anzeigen verfügen, beliebige Stunden genehmigen oder ablehnen. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>To require time to be approved on the project:</p>
   <ul><li>New: Standard</li>
   <li>Current: Plan</li></ul>
   
   <p>To approve hours logged on a project:</p>
   <ul><li>New: Light or higher</li>
   <li>Review or higher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects or higher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Additional access</td> 
   <td> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours. In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Anfordern der Genehmigung des Zeitaufwands für ein Projekt

So fordern Sie die Genehmigung des Projektleiters für Stunden im Projekt an:

1. Wechseln Sie zu dem Projekt, für das Sie eine Genehmigung für Stunden benötigen.
1. Klicken Sie auf das **Mehr**-Symbol ![Mehr](assets/more-icon.png) rechts neben dem Projektnamen und klicken Sie dann auf **Bearbeiten**.\
   Das Dialogfeld Projekt bearbeiten wird angezeigt.

1. Wählen Sie **Abschnitt** Projekteinstellungen“ **Zeit für die Genehmigung für dieses Projekt erforderlich** aus.
1. Klicken Sie auf **Speichern**.\
   Wenn die Zeit nun protokolliert und genehmigt wird, werden diese Stunden gesperrt und können von der Person, die sie in das Projekt oder die Arbeitszeittabelle eingegeben hat, nicht mehr geändert werden. Nur ein Workfront-Administrator kann die aufgezeichnete Zeit anpassen.

## Projektzeit validieren und ablehnen

Als Projekt-Manager können Sie Stunden genehmigen oder ablehnen, die für Aufgaben, Probleme oder das Projekt protokolliert werden.

Die Genehmigung der Stunden auf Projektebene hat keine Auswirkungen auf die Arbeitszeittabelle der Benutzer, die die Stunden protokolliert haben. Beispielsweise können die Stunden im Projekt vom Projekt-Manager genehmigt werden, die Arbeitszeittabelle muss jedoch noch vom Manager des Benutzers oder der genehmigenden Person genehmigt werden.

Wenn Sie ein Projekt so einrichten, dass die protokollierten Stunden genehmigt werden müssen, muss der Projekt-Manager die Stunden genehmigen, damit sie in einen Rechnungsnachweis für das Projekt aufgenommen werden können. Weitere Informationen zum Erstellen von Rechnungsnachweisen finden Sie im Artikel [Erstellen von Rechnungsnachweisen](../../../manage-work/projects/project-finances/create-billing-records.md).

So genehmigen Sie Stunden für ein Projekt oder lehnen sie ab:

1. Gehen Sie zum Projekt.
1. Klicken Sie auf **Bereich** Stunden“ im linken Bedienfeld.

1. Die für Probleme, Aufgaben und das Projekt protokollierten Stunden werden angezeigt und sollten den Status &quot;**&quot;**.\
   Klicken Sie links neben den Stundeneinträgen auf das Kästchen, um die Stunden auszuwählen, die genehmigt werden sollen.

1. Klicken Sie auf **Genehmigen**-Symbol ![Genehmigen](assets/approve-hours-icon.png) oben in der Stundenliste.\
   Der Status der Stunden ändert sich in **Genehmigt**.\
   Wenn Sie die genehmigten Stunden später ablehnen, ändert sich der Status der Stunden in **Nicht genehmigt**.\
   Wenn Sie die genehmigten Stunden in einen Abrechnungs-Datensatz einbeziehen, ändert sich der Status der Stunden in &quot;**und genehmigt**. Einem Rechnungsnachweis hinzugefügte Stunden können nicht gelöscht werden. Weitere Informationen zum Erstellen von Rechnungsnachweisen finden Sie im Artikel [Erstellen von Rechnungsnachweisen](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Optional) Klicken Sie auf **Ablehnen** Symbol ![Stunden ablehnen](assets/reject-hours-icon.png) um die Zeiteinträge im Projekt abzulehnen.\
   Der Status der Stunden ändert sich in **Abgelehnt**.

   >[!NOTE]
   >
   >   Wenn die von Ihnen ausgewählten Stunden in einem Rechnungsnachweis enthalten sind, der als „In Rechnung gestellt“ oder „In Rechnung gestellt und genehmigt“ gekennzeichnet wurde, werden die Symbole „Genehmigen“ und „Ablehnen“ nicht angezeigt. Sie können nur Stunden genehmigen, die noch nicht in einem Rechnungsnachweis in Rechnung gestellt wurden.

