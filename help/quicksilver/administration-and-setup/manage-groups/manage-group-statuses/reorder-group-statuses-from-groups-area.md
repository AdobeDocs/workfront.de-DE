---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Gruppenstatus neu anordnen
description: Als Gruppenadministrator bzw. -administratorin können Sie die Reihenfolge der Projekt-, Aufgaben- und Problemstatus für eine von Ihnen verwaltete Gruppe ändern.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 7%

---

# Gruppenstatus neu anordnen

Als Gruppenadministrator bzw. -administratorin können Sie die Reihenfolge der Projekt-, Aufgaben- und Problemstatus für eine von Ihnen verwaltete Gruppe ändern.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![Status](assets/statuses.png)

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>* Ein Workfront-Administrator kann die Status auf Systemebene neu anordnen. Dies wirkt sich nicht auf die Reihenfolge der Status innerhalb von Gruppen aus.
>
>  Die Status innerhalb einer neu erstellten Gruppe der obersten Ebene übernehmen jedoch die Reihenfolge der Status auf Systemebene. (Eine neue Untergruppe übernimmt die Reihenfolge der Status in der Gruppe eine Ebene höher.)
>
>* Sie können gesperrte Status neu anordnen. Informationen zu gesperrten Status finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

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
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
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
     <p>Aktuell</p> 
     <p>Eingestellt</p> 
     <p> Zurückgestellt </p> 
     <p> In Planung </p> 
     <p> Abgeschlossen </p> 
     <p> Angefordert </p> 
     <p> Genehmigt </p> 
     <p> Abgelehnt </p> 
     <p> Idee </p> 
   </td> 
   <td> 
     <p>Neu</p> 
     <p>In Arbeit</p> 
     <p>Abgeschlossen</p> 
   </td> 
   <td> 
     <p>Neu</p> 
     <p>In Arbeit</p> 
     <p>Neu geöffnet</p> 
     <p>Warten auf Feedback</p> 
     <p>Zurückgestellt</p> 
     <p>Kann nicht duplizieren</p> 
     <p>Geschlossen</p> 
     <p>Gelöst</p> 
     <p>Abschluss bestätigt</p> 
     <p>Lässt sich nicht lösen</p> 
   </td> 
  </tr> 
 </tbody> 
</table>

## Status für Aufgaben und Projekte in einer von Ihnen verwalteten Gruppe neu anordnen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** und klicken Sie dann auf den Namen der Gruppe.
1. Klicken Sie im linken Bedienfeld auf **Status**.
1. Klicken Sie über der angezeigten Statusliste auf die Registerkarte **Projekte** oder **Aufgaben**.

1. Ziehen Sie die Status per Drag-and-Drop in die gewünschte Reihenfolge.

   Der neue Bestellstatus wird automatisch gespeichert.

1. Um die neue Statusreihenfolge zu testen, navigieren Sie zu einer Aufgabe oder einem Projekt, das mit der Gruppe verknüpft ist, klicken Sie auf den Status in der oberen rechten Ecke und stellen Sie sicher, dass die angezeigten Status in der von Ihnen konfigurierten Reihenfolge angezeigt werden.

## Status für Probleme neu anordnen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** und klicken Sie dann auf den Namen der Gruppe.
1. Klicken Sie im linken Bedienfeld auf **Status**.
1. Klicken Sie auf die **Probleme**.
1. (Optional) Wählen Sie einen Problemtyp aus **Fehlerbericht**, **Änderungsanforderung**, **Problem** oder **Anfrage**).

   >[!NOTE]
   >
   >* Die Reihenfolge der Status für die primäre Liste kann nicht angepasst werden.
   >* Es wird empfohlen, die Statusreihenfolge für jeden Anfragetyp auf die gleiche Weise zu ändern. Weitere Informationen zu Problemtypen finden Sie unter [Konfigurieren von Anfragetypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Ziehen Sie die Status per Drag-and-Drop in die gewünschte Reihenfolge.

   Der neue Bestellstatus wird automatisch gespeichert.

1. Um die neue Statusreihenfolge zu testen, wechseln Sie zu einem Problem, das mit der Gruppe verbunden ist, klicken Sie auf den Status in der oberen rechten Ecke und stellen Sie sicher, dass die angezeigten Status in der von Ihnen konfigurierten Reihenfolge angezeigt werden.
