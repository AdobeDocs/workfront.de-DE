---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Neuanordnen der Status auf Systemebene und Gruppe
description: Als Workfront-Administrator können Sie die Reihenfolge der Projekte, Aufgaben und Ausgabestatus für alle Benutzer im System oder für eine Gruppe ändern.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 6%

---

# Neuanordnen der Status auf Systemebene und Gruppe

Als Workfront-Administrator können Sie die Reihenfolge der Projekte, Aufgaben und Ausgabestatus für alle Benutzer im System oder für eine Gruppe ändern.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![](assets/statuses.png)

>[!NOTE]
>
>* Die Neuanordnung der Status auf Systemebene wirkt sich nicht auf die Reihenfolge der Status in Gruppen aus.
>
>  Die Status in einer neu erstellten Gruppe der obersten Ebene übernehmen jedoch die Reihenfolge der Systemstatus. (Eine neue Untergruppe übernimmt die Reihenfolge der Status in der Gruppe um eine Ebene.)
>
>* Sie können gesperrte Status neu anordnen. Weitere Informationen zu gesperrten Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Gruppenadministratoren können auch die in ihren Gruppen verwendeten Status neu anordnen. Weitere Informationen finden Sie unter [Neuanordnen von Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan* </td> 
   <td>Alle</td> 
  </tr> 
  <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Workfront-Administrator sein. Weitere Informationen zu Workfront-Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben.

## Standardreihenfolge der Status

Standardmäßig werden die Status in der folgenden Reihenfolge angezeigt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th width="33.33%">Projekt</th> 
   <th width="33.33%">Aufgabe</th> 
   <th width="33.33%">Problem</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li>Aktuell</li> 
     <li>Eingestellt</li> 
     <li> Zurückgestellt </li> 
     <li> In Planung </li> 
     <li> Abgeschlossen </li> 
     <li> Angefordert </li> 
     <li> Genehmigt </li> 
     <li> Abgelehnt </li> 
     <li> Idee </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Neu</li> 
     <li>In Arbeit</li> 
     <li>Abgeschlossen</li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li>Neu</li> 
     <li>In Arbeit</li> 
     <li>Neu geöffnet</li> 
     <li>Warten auf Feedback</li> 
     <li>Zurückgestellt</li> 
     <li>Kann nicht duplizieren</li> 
     <li>Geschlossen</li> 
     <li>Gelöst</li> 
     <li>Abschluss bestätigt</li> 
     <li>Lässt sich nicht lösen</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Neuanordnen des Status für Aufgaben und Projekte systemweit oder für eine Gruppe

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Bereich auf **Projekteinstellungen > Status**.
1. (Bedingt) Wenn Sie den Status einer Gruppe neu anordnen, geben Sie den Namen der Gruppe in das Feld oben rechts ein und klicken Sie dann auf den Namen, sobald er angezeigt wird.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Klicken Sie über der angezeigten Liste Status auf die Registerkarte **Projekte** oder **Aufgaben** .

1. Ziehen Sie die Status in die gewünschte Reihenfolge.

   Die neue Statusreihenfolge wird automatisch gespeichert.

1. Um die neue Statusreihenfolge zu testen, navigieren Sie zu einer Aufgabe oder einem Projekt, klicken Sie auf den Status in der oberen rechten Ecke und stellen Sie sicher, dass die angezeigten Status in der von Ihnen konfigurierten Reihenfolge sind.

## Status für Probleme neu anordnen

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **Projekteinstellungen > Status.**
1. (Bedingt) Wenn Sie den Status einer Gruppe neu anordnen, geben Sie den Namen der Gruppe in das Feld oben rechts ein und klicken Sie dann auf den Namen, sobald er angezeigt wird.

   ![](assets/issue-statuses-group-name.png)

1. Klicken Sie auf die Registerkarte **Probleme**.
1. (Optional) Wählen Sie einen Problemtyp aus (**Fehlerbericht**, **Reihenfolge ändern**, **Problem** oder **Anfrage**).

   >[!NOTE]
   >
   >* Sie können die Reihenfolge der Status für die Master-Liste nicht anpassen.
   >* Es wird empfohlen, die Reihenfolge der Status für jeden Ausgabetyp auf die gleiche Weise festzulegen. Weitere Informationen zu Problemtypen finden Sie unter [Anfragetypen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Ziehen Sie die Status in die gewünschte Reihenfolge.

   Die neue Statusreihenfolge wird automatisch gespeichert.

1. Um die neue Statusreihenfolge zu testen, gehen Sie zu einem Problem, klicken Sie auf den Status in der oberen rechten Ecke und stellen Sie sicher, dass die angezeigten Status in der von Ihnen konfigurierten Reihenfolge sind.
