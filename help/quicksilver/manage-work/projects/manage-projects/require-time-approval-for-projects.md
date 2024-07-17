---
product-area: projects
navigation-topic: manage-projects
title: Genehmigung für ein Projekt erforderlich
description: Genehmigung für ein Projekt erforderlich
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Genehmigung für ein Projekt erforderlich

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

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
   <td> <p>Planen Sie die Genehmigung des Projekts mit einer gewissen Zeit.</p>
   <p>Überprüfen oder höher zur Genehmigung von Stunden, die in einem Projekt angemeldet sind</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten oder höher</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt oder höher anzeigen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
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
     <li>Sie haben eine Planungslizenz mit Administratorzugriff auf Timesheets &amp; Hours. In diesem Fall:
      <ul>
       <li>Sie können alle Stunden für Projekte genehmigen oder ablehnen, für die Sie mindestens über die Berechtigung zum Anzeigen verfügen. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

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
1. Klicken Sie im linken Bereich auf den Bereich **Stunden** . Dies kann sich unter dem Bereich **Mehr anzeigen** befinden.

1. Die Stunden, die für Probleme, Aufgaben und die Projektanzeige protokolliert werden, sollten den Status &quot;**Gesendet**&quot;haben.\
   Klicken Sie links neben den Stundeneinträgen auf das Kästchen, um die Stunden auszuwählen, die genehmigt werden sollen.

1. Klicken Sie auf **Genehmigen**.\
   Der Status der Stunden ändert sich in **Genehmigt**.\
   Wenn Sie die genehmigten Stunden später ablehnen, ändert sich der Status der Stunden in **Nicht genehmigt**.\
   Wenn Sie die genehmigten Stunden in einen Rechnungsdatensatz aufnehmen, ändert sich der Status der Stunden in **Abgerechnet und Genehmigt**. Stunden, die zu einem Rechnungsdatensatz hinzugefügt wurden, können nicht gelöscht werden. Weitere Informationen zum Erstellen von Rechnungsdatensätzen finden Sie im Artikel [Erstellen von Rechnungsdatensätzen](../../../manage-work/projects/project-finances/create-billing-records.md) .

1. (Optional) Klicken Sie auf **Ablehnen** , um die Zeiteinträge im Projekt abzulehnen.\
   Der Status der Stunden ändert sich in **Abgelehnt**.
