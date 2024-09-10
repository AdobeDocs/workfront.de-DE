---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Neuanordnen von Gruppenstatus
description: Als Gruppenadministrator können Sie die Reihenfolge der Projekte, Aufgaben und Problemstatus für eine von Ihnen verwaltete Gruppe ändern.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 0cdb4d10-7792-4140-8dec-ef805f668f90
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 7%

---

# Neuanordnen von Gruppenstatus

Als Gruppenadministrator können Sie die Reihenfolge der Projekte, Aufgaben und Problemstatus für eine von Ihnen verwaltete Gruppe ändern.

<!--
The system version of this snippet mentions a single group because a sysadmin call also reorder statuses there. Group admin version of this article is still needed.
-->

![](assets/statuses.png)

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!NOTE]
>
>* Ein Workfront-Administrator kann die Status auf Systemebene neu anordnen. Dies hat keine Auswirkungen auf die Reihenfolge der Status in Gruppen.
>
>  Die Status in einer neu erstellten Gruppe der obersten Ebene übernehmen jedoch die Reihenfolge der Systemstatus. (Eine neue Untergruppe übernimmt die Reihenfolge der Status in der Gruppe um eine Ebene.)
>
>* Sie können gesperrte Status neu anordnen. Informationen zu gesperrten Status finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

## Neuanordnen des Status für Aufgaben und Projekte in einer von Ihnen verwalteten Gruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** und klicken Sie dann auf den Namen der Gruppe.
1. Klicken Sie im linken Bereich auf **Status**.
1. Klicken Sie über der angezeigten Liste Status auf die Registerkarte **Projekte** oder **Aufgaben** .

1. Ziehen Sie die Status in die gewünschte Reihenfolge.

   Die neue Statusreihenfolge wird automatisch gespeichert.

1. Um die neue Statusreihenfolge zu testen, navigieren Sie zu einer Aufgabe oder einem Projekt, die bzw. das der Gruppe zugeordnet ist, klicken Sie auf den Status in der oberen rechten Ecke und stellen Sie sicher, dass die angezeigten Status in der von Ihnen konfigurierten Reihenfolge sind.

## Status für Probleme neu anordnen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** und klicken Sie dann auf den Namen der Gruppe.
1. Klicken Sie im linken Bereich auf **Status**.
1. Klicken Sie auf die Registerkarte **Probleme**.
1. (Optional) Wählen Sie einen Problemtyp aus (**Fehlerbericht**, **Reihenfolge ändern**, **Problem** oder **Anfrage**).

   >[!NOTE]
   >
   >* Sie können die Reihenfolge der Status für die Master-Liste nicht anpassen.
   >* Es wird empfohlen, die Reihenfolge der Status für jeden Ausgabetyp auf die gleiche Weise festzulegen. Weitere Informationen zu Problemtypen finden Sie unter [Anfragetypen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-request-types.md).

1. Ziehen Sie die Status in die gewünschte Reihenfolge.

   Die neue Statusreihenfolge wird automatisch gespeichert.

1. Um die neue Statusreihenfolge zu testen, gehen Sie zu einem mit der Gruppe verknüpften Problem, klicken Sie auf den Status in der oberen rechten Ecke und stellen Sie sicher, dass die angezeigten Status in der von Ihnen konfigurierten Reihenfolge sind.
