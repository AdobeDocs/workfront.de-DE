---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Systemebene und Gruppenstatus neu anordnen
description: Als Workfront-Administrator können Sie die Reihenfolge der Projekt-, Aufgaben- und Problemstatus für jeden Benutzer im System oder für eine einzelne Gruppe ändern.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6fee45a6-1a55-4351-8b08-88244c742ed5
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 7%

---

# Systemebene und Gruppenstatus neu anordnen

Als Workfront-Administrator können Sie die Reihenfolge der Projekt-, Aufgaben- und Problemstatus für jeden Benutzer im System oder für eine einzelne Gruppe ändern.

<!--The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.-->

![Status](assets/statuses.png)

>[!NOTE]
>
>* Die Neuanordnung der Status auf Systemebene wirkt sich nicht auf die Reihenfolge der Status innerhalb von Gruppen aus.
>
>  Die Status innerhalb einer neu erstellten Gruppe der obersten Ebene übernehmen jedoch die Reihenfolge der Status auf Systemebene. (Eine neue Untergruppe übernimmt die Reihenfolge der Status in der Gruppe eine Ebene höher.)
>
>* Sie können gesperrte Status neu anordnen. Informationen zu gesperrten Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
>* Gruppenadministratoren können auch die in ihren Gruppen verwendeten Status neu anordnen. Weitere Informationen finden Sie unter [Gruppenstatus neu anordnen](../../../administration-and-setup/manage-groups/manage-group-statuses/reorder-group-statuses-from-groups-area.md).
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

## Status für Aufgaben und Projekte systemweit oder für eine Gruppe neu anordnen

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Projektvoreinstellungen > Status**.
1. (Bedingt) Wenn Sie den Status für eine Gruppe neu anordnen, geben Sie den Namen der Gruppe in das Feld oben rechts ein. Klicken Sie dann auf den Namen, wenn er angezeigt wird.

   ![Systemstatus](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Klicken Sie über der angezeigten Statusliste auf die Registerkarte **Projekte** oder **Aufgaben**.

1. Ziehen Sie die Status per Drag-and-Drop in die gewünschte Reihenfolge.

   Der neue Bestellstatus wird automatisch gespeichert.

1. Um die neue Statusreihenfolge zu testen, navigieren Sie zu einer Aufgabe oder einem Projekt, klicken Sie auf den Status in der oberen rechten Ecke und stellen Sie sicher, dass die angezeigten Status in der von Ihnen konfigurierten Reihenfolge angezeigt werden.

## Status für Probleme neu anordnen

1. Klicken Sie auf das **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront und dann auf **Setup** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Klicken Sie **Projektvoreinstellungen > Status.**
1. (Bedingt) Wenn Sie den Status für eine Gruppe neu anordnen, geben Sie den Namen der Gruppe in das Feld oben rechts ein. Klicken Sie dann auf den Namen, wenn er angezeigt wird.

   ![Problemstatus für Gruppe](assets/issue-statuses-group-name.png)

1. Klicken Sie auf die **Probleme**.
1. (Optional) Wählen Sie einen Problemtyp aus **Fehlerbericht**, **Änderungsanforderung**, **Problem** oder **Anfrage**).

   >[!NOTE]
   >
   >* Die Reihenfolge der Status für die primäre Liste kann nicht angepasst werden.
   >* Es wird empfohlen, die Statusreihenfolge für jeden Anfragetyp auf die gleiche Weise zu ändern. Weitere Informationen zu Problemtypen finden Sie unter [Konfigurieren von Anfragetypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Ziehen Sie die Status per Drag-and-Drop in die gewünschte Reihenfolge.

   Der neue Bestellstatus wird automatisch gespeichert.

1. Um die neue Statusreihenfolge zu testen, wechseln Sie zu einem Problem, klicken Sie auf den Status in der oberen rechten Ecke und stellen Sie sicher, dass die angezeigten Status in der von Ihnen konfigurierten Reihenfolge angezeigt werden.
