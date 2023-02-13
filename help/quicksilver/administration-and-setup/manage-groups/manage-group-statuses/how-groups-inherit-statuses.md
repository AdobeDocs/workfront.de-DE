---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Vererben von Status durch Gruppen
description: Wenn Sie die für eine Gruppe verfügbaren Status auflisten, sehen Sie Folgendes
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Vererben von Status durch Gruppen

Wenn Sie die für eine Gruppe verfügbaren Status auflisten, sehen Sie Folgendes

* Benutzerdefinierte Status, die für die Gruppe erstellt wurden, wie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Status werden vom System und von höher in der Gruppenhierarchie übernommen, wie in diesem Artikel beschrieben.

## Erben von Status

Ihre Gruppe erbt den Status, wenn eines der folgenden Ereignisse eintritt:

* Sie erstellen die Gruppe.
* Ein Administrator sperrt einen Status in einer Gruppe mit höherer Ebene.
* Ein Administrator löscht eine andere Gruppe und wählt die Gruppe aus, die die gewünschte Position einnimmt.

In der folgenden Tabelle werden diese Umstände erläutert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wenn Sie eine Gruppe erstellen</td> 
   <td> <p>Wenn Sie eine neue Gruppe erstellen, erbt sie automatisch Folgendes:</p> 
    <ul> 
     <li>Entsperrt Status in der Gruppe eine Ebene nach oben, wenn die neue Gruppe eine Untergruppe ist.</li> 
    </ul> 
    <ul> 
     <li>Gesperrte Status auf Systemebene .</li> 
    </ul> 
     <b>BEISPIEL:</b></span></span> 
     <p>Angenommen, eine Gruppe namens Marketing hat zwei Untergruppen namens Marketing Communications und Branding.</p> 
     <p>Ein Gruppenadministrator der Marketing-Gruppe erstellt einen neuen benutzerdefinierten Status namens Discovery.</p> 
     <p>Später erstellen Sie eine neue Untergruppe unter der Marketing-Gruppe und nennen sie sie "Werbung".</p> 
     <p>Ihre Untergruppe erbt den Erkennungsstatus, da Sie die Gruppe erstellt haben, nachdem der andere Administrator den Entdeckungsstatus erstellt hat.</p> 
     <p>Da die Untergruppen Marketing Communications und Branding bereits unter der Marketing-Gruppe existierten, als dies passierte, erben sie nicht den entsperrten Erkennungsstatus.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wenn ein Administrator einen Status auf höherer Ebene sperrt</td> 
   <td> <p>Wenn ein Workfront-Administrator einen Status auf Systemebene sperrt, übernimmt Ihre Gruppe ihn zusammen mit allen anderen Gruppen im System.</p> <p>Wenn ein Administrator einen Status für eine Gruppe oberhalb Ihrer Gruppe sperrt, übernimmt Ihre Gruppe diesen ebenso wie alle anderen Untergruppen unterhalb der höheren Gruppe.</p> <p><b>NOTE</b>: Wenn später ein Administrator einen dieser Status auf Systemebene oder in einer Gruppe über Ihrer Gruppe freischaltet, behält Ihre Gruppe den Status bei, den sie zuvor geerbt hat. Jetzt handelt es sich um eine separate Version des Status und Sie können ihn nur für Ihre Gruppe anpassen.</p> 
    <p><b>BEISPIEL:</b></p>
    <p>Der Marketing-Gruppenadministrator sperrt den oben genannten Erkennungsstatus, um sicherzustellen, dass alle 3 Untergruppen über diesen Status verfügen.</p> 
    <p>Zusammen mit Ihrer Advertising-Gruppe haben die Gruppen Marketing Communications und Branding jetzt den Erkennungsstatus. Sie erbten sie, als sie in der obigen Marketinggruppe gesperrt war.</p> 
    <p>Der Marketing-Gruppenadministrator entsperrt dann den Erkennungsstatus, sodass alle 3 Untergruppen über eine eigene Version des Erkennungsstatus verfügen. Jetzt können Sie und die Administratoren der beiden anderen Gruppen den Erkennungsstatus an die Bedürfnisse Ihrer Gruppen anpassen.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wenn ein Administrator eine Gruppe löscht</td> 
   <td> <p>Wenn ein Administrator eine Gruppe löscht und Ihre Rolle im System übernimmt, übernimmt Ihre Gruppe die benutzerdefinierten Status der gelöschten Gruppe, sofern diese noch nicht in Ihrer Gruppe vorhanden sind.</p> 
   <p><b>BEISPIEL: </b></p>
     <p>Eine Gruppe namens Messaging muss mit Ihrer Advertising-Gruppe zusammengeführt werden, sodass ein Workfront-Administrator die Messaging-Gruppe löscht und Ihre Gruppe wählt, um die Position zu übernehmen.</p> 
     <p>Die Gruppe Messaging hatte einen eindeutigen Status namens In Process. Dieser Status ist jetzt für Ihre Advertising-Gruppe verfügbar.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Statuskonfigurationen übernehmen

Wenn Sie eine Gruppe der obersten Ebene erstellen, übernimmt sie die folgenden Konfigurationen auf Systemebene. Wenn Sie eine Untergruppe erstellen, übernimmt diese die folgenden Konfigurationen von der nächsthöheren Gruppe.

* Standardstatuskonfigurationen

   Weitere Informationen dazu finden Sie unter [Verwenden benutzerdefinierter Status als Standardstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Konfigurationen der Anzeigereihenfolge von Status

   Weitere Informationen dazu finden Sie unter [Neuanordnen der Status auf Systemebene und Gruppe](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Wenn jemand diese Konfigurationen ändert, nachdem Ihre Gruppe erstellt wurde, hat dies keine Auswirkungen auf ihren Status.
