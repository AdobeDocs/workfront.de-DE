---
product-area: projects
navigation-topic: manage-projects
title: Genehmigung von Zeit für ein Projekt verlangen
description: Genehmigung von Zeit für ein Projekt verlangen
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: bffa5992a530761afe57ec62b4cbba2bf03ad1e6
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 0%

---

# Genehmigung von Zeit für ein Projekt verlangen

<!--audited: 08/2024-->

Sie können das Projekt so konfigurieren, dass die für das Projekt protokollierten Stunden vom Projektbesitzer genehmigt werden müssen. Wenn Stunden auf diese Weise konfiguriert sind, müssen sie zunächst vom Projektbesitzer genehmigt werden, bevor sie für einen Rechnungsnachweis verwendet werden können.\
Weitere Informationen zu Rechnungsnachweisen finden Sie im Artikel [Rechnungsnachweise erstellen](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Durch Aktivierung dieser Option wird die Fähigkeit einer genehmigenden Person für Arbeitszeittabellen, die Zeit in der Arbeitszeittabelle zu genehmigen, nicht entfernt. Wenn der Projektinhaber die Zeit nicht genehmigt oder ablehnt, kann ein Arbeitszeittabellen-Genehmiger die Zeit in einer Arbeitszeittabelle trotzdem genehmigen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>So benötigen Sie Zeit für die Genehmigung des Projekts:</p>
   <ul><li>Neu: Standard</li>
   <li>Aktuell: Plan</li></ul>

<p>So genehmigen Sie für ein Projekt protokollierte Stunden:</p>
   <ul><li>Neu: Licht oder höher</li>
   <li>Überprüfen oder höher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte oder höher bearbeiten</p>  </td> 
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
       <li> Wenn Sie Contribute- oder Ansichtszugriff auf das Projekt haben, können Sie nur die von Ihnen oder einer anderen Person, die Sie meldet, protokollierten Stunden genehmigen oder ablehnen.<br></li>
      </ul></li> 
     <li>Sie verfügen über eine Planlizenz mit administrativem Zugriff auf Arbeitszeittabellen und Stunden. In diesem Fall:
      <ul>
       <li>Sie können für die Projekte, für die Sie mindestens über die Berechtigung zum Anzeigen verfügen, beliebige Stunden genehmigen oder ablehnen. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Genehmigung von Zeit für ein Projekt verlangen

So fordern Sie die Genehmigung des Projektleiters für Stunden im Projekt an:

1. Wechseln Sie zu dem Projekt, für das Sie eine Genehmigung für Stunden benötigen.
1. Klicken Sie auf **Mehr**-Symbol ![](assets/more-icon.png) rechts neben dem Projektnamen und dann auf **Bearbeiten**.\
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
1. Klicken Sie auf **Bereich** Stunden“ im linken Bedienfeld. Dieser befindet sich möglicherweise unter dem Bereich **Mehr anzeigen**.

1. Die für Probleme, Aufgaben und das Projekt protokollierten Stunden werden angezeigt und sollten den Status &quot;**&quot;**.\
   Klicken Sie links neben den Stundeneinträgen auf das Kästchen, um die Stunden auszuwählen, die genehmigt werden sollen.

1. Klicken Sie oben **der** auf das Symbol „Genehmigen![](assets/approve-hours-icon.png).\
   Der Status der Stunden ändert sich in **Genehmigt**.\
   Wenn Sie die genehmigten Stunden später ablehnen, ändert sich der Status der Stunden in **Nicht genehmigt**.\
   Wenn Sie die genehmigten Stunden in einen Abrechnungs-Datensatz einbeziehen, ändert sich der Status der Stunden in &quot;**und genehmigt**. Einem Rechnungsnachweis hinzugefügte Stunden können nicht gelöscht werden. Weitere Informationen zum Erstellen von Rechnungsnachweisen finden Sie im Artikel [Erstellen von Rechnungsnachweisen](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Optional) Klicken Sie auf **Ablehnen** Symbol ![](assets/reject-hours-icon.png), um die Zeiteinträge im Projekt abzulehnen.\
   Der Status der Stunden ändert sich in **Abgelehnt**.

   >[!NOTE]
   >
   >   Wenn die von Ihnen ausgewählten Stunden in einem Rechnungsnachweis enthalten sind, der als „In Rechnung gestellt“ oder „In Rechnung gestellt und genehmigt“ gekennzeichnet wurde, werden die Symbole „Genehmigen“ und „Ablehnen“ nicht angezeigt. Sie können nur Stunden genehmigen, die noch nicht in einem Rechnungsnachweis in Rechnung gestellt wurden.

