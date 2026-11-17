---
title: Aktivieren einer Workfront Planning Workspace in GenStudio for Performance Marketing
description: Sie können einen Adobe Workfront Planning-Arbeitsbereich in GenStudio for Performance Marketing verfügbar machen, wenn Sie Zugriff auf beide Programme haben.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 9dc53e749a61247529d67ce077856ea6bea8e494
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 6%
---
# Aktivieren eines Workfront Planning Workspace für GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--Iskuhi said "ACPC projects" will be renamed when this will be released but not sure if it has been. Follow up with Syuzanna, Gurgen Mosesyan and possibly Himanshi Kumar - see slack threads -->

Wenn Ihr Unternehmen auch Adobe GenStudio for Performance Marketing kauft und Sie Adobe Workfront Planning-Kunde sind, ist der GenStudio-Arbeitsbereich auch in Workfront Planning verfügbar.

Wenn Sie bereits über einen Planungsarbeitsbereich in Workfront Planning verfügen, können Sie ihn für GenStudio for Performance Marketing aktivieren, anstatt dieselben Daten daraus in GenStudio neu zu erstellen.

Durch Aktivierung eines Arbeitsbereichs wird dieser mit einem Adobe Could Storage-Projekt verknüpft und seine Datensatztypen und -felder werden GenStudio Workspace zugeordnet. Nachdem Sie die Konfiguration abgeschlossen haben, können Sie die Datensätze des Arbeitsbereichs in GenStudio öffnen.

Sie müssen über Folgendes verfügen:

* Zugriff auf Workfront Planning und GenStudio for Performance Marketing.
* Ein Adobe Cloud Storage-Projekt, das mit dem Arbeitsbereich verknüpft werden soll. Ein Organisations-Admin kann in der Adobe Admin Console eine erstellen.

  Weitere Informationen finden Sie unter [Verwalten von Adobe-](https://helpx.adobe.com/de/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html)<!--ensure this site still works-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebige Workfront oder Workflows und beliebiges Planungspaket</p> 
ODER
<p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p>

</td> 
   <tr> 
<td> 
   <p> Zusätzliche Produkte</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>

<tr> 
<td> 
   <p> Adobe Admin Console-Einstellungen</p> </td> 
   <td> 
   <p> Sie müssen Adobe Storage Cloud-Projekte in der Adobe Admin Console erstellen </p>

<p>Weitere Informationen finden Sie unter <a href="https://helpx.adobe.com/de/business/enterprise/manage-storage-assets/manage-storage/projects-in-business-storage.html#project-policies">Verwalten von Projekten</a>

</td> 
  </tr>
  <tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Workflow-Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Planning-Lizenz</p></td> 
   <td><p>Planungsstandard</p>
   </td> 
  </tr>
<tr> 
   <td role="rowheader"><p>Konfiguration der Adobe Workfront-Zugriffsebene</p></td> 
   <td> <p>Wenn Sie sowohl über einen Workflow als auch über ein Planungspaket verfügen, müssen Sie der Workfront-Zugriffsebene sowohl einen Workflow- als auch einen Planning-Lizenztyp hinzufügen</p>   
</td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing-Benutzerrollen</p></td> 
   <td><p><ul><li>Jede GenStudio-Benutzerrolle, wenn Sie auf Kampagnen, Produkte und Personas zugreifen müssen</li>
   <li>GenStudio System Manager, wenn Sie auf Aktivierungen zugreifen müssen <!--and Events--></li></ul>
   Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Benutzerrollen und -berechtigungen</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Verwalten von Berechtigungen für den Arbeitsbereich <!--to add new fields or record types to the GenStudio workspace--></p></li>
   <!--
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio workspace</p> </li>  
   -->
   </ul>
   <!--
   <p>No users can remove GenStudio for Performance Marketing record types or fields from the GenStudio workspace in Workfront Planning</p>
   -->
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <!--
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   -->
   <li><p> Erstellen von Berechtigungen in Adobe GenStudio for Performance Marketing zum Erstellen von Elementen</p></li></ul>
   </td>  
</tbody> 
</table>

Informationen zum Adobe Workfront Planning-Zugriff finden Sie unter [Übersicht über den Adobe Workfront Planning-Zugriff](/help/quicksilver/planning/access/access-overview.md).

Weitere Informationen zu Adobe GenStudio for Performance Marketing finden Sie im [Adobe GenStudio for Performance Marketing-Benutzerhandbuch](https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/home).

+++ 

## Aktivieren eines Workfront Planning Workspace für GenStudio

1. Öffnen Sie in Workfront Planning den Arbeitsbereich, den Sie aktivieren möchten.
1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Workspace-Namen und klicken Sie dann auf **GenStudio aktivieren**.

   Das Feld **Make Workspace GenStudio** aktiviert“ wird mit den folgenden Schritten geöffnet:

   1. **ACPC-Projekt**: Wählen Sie das **ACPC-Projekt** (Adobe Cloud Storage-Projekt) aus, das Sie mit diesem Arbeitsbereich synchronisieren möchten, und klicken Sie dann auf **Weiter**. Benutzende greifen über dieses Projekt auf den Arbeitsbereich in GenStudio zu.

      ![GenStudio Workspace aktivieren - ACPC-Projektschritt](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Datensatztypen**: Ordnen Sie die Datensatztypen des Arbeitsbereichs den sechs Datensatztypen zu, die für GenStudio erforderlich sind:

      * Kampagnen
      * Produkte
      * Personas
      * Kanäle
      * Regionen
      * Aktivierungen

      Öffnen Sie für jeden Datensatz die Liste und wählen Sie den entsprechenden Planungs-Datensatztyp aus, oder wählen Sie **Neu hinzufügen** aus, um ihn zu erstellen, und klicken Sie dann auf **Weiter**.

      ![GenStudio Workspace aktivieren - Schritt Datensatztypen](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Felder**: Ordnen Sie die Felder für jeden Datensatztyp zu. Verwenden Sie die Registerkarten oben im Dialogfeld, um zwischen Datensatztypen zu wechseln. Wählen Sie für jedes Feld das entsprechende Feld Planung aus oder wählen Sie **Neu hinzufügen**, um ein Feld zu erstellen.

      Wiederholen Sie die Feldeinrichtung für alle Datensatztypen.

      ![Arbeitsbereich für GenStudio aktivieren - Schritt „Felder“](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Überprüfen und beseitigen Sie etwaige Warnungen.

      Ein neues Feld kann beispielsweise das primäre Feld für den Datensatztyp werden oder ein bereits verwendeter Feldalias wird umbenannt (wenn Sie bereits ein Feld mit dem Namen „Regionen“ haben, könnte das importierte in „Regionen 2“ umbenannt werden).

      Durch Zuordnen **Felds** Status“ werden die erforderlichen Optionen hinzugefügt.

   1. Klicken Sie auf **Veröffentlichen**.

      Wenn der Arbeitsbereich aktiviert ist, wird eine Bestätigungsmeldung angezeigt. Zugeordnete Datensatztypen sind im Arbeitsbereich markiert.

      Die Datensatztypen, denen zugeordnet ist, damit sie über GenStudio zugänglich sind, haben ein neues **Adobe**-Symbol auf ihren Karten.

      ![Kampagnen-Datensatztyp mit Adobe-Symbol](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Öffnen Sie GenStudio, wählen Sie **Kampagnen** und klicken Sie dann auf das **ACPC-Projekt** das Sie ursprünglich für dieses Setup konfiguriert haben, in der unteren linken Ecke des Bildschirms. Überprüfen Sie die importierten Datensatztypen und -felder.

   >[!TIP]
   >
   >Es werden nur die Datensätze angezeigt, die durch die Zugehörigkeit zu einem Adobe Cloud Storage-Projekt zulässig sind.
