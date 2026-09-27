---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: So erben Gruppen Status
description: Wenn Sie die für eine Gruppe verfügbaren Status auflisten, sehen Sie Folgendes
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
TQID: 'https://experienceleague.adobe.com/4P19FJmlpQfFZfWrfnjmgSJsQ9InspngsEAeMlTktvA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: 254442ca-6997-5cfa-963e-f420870aea53
    internal-label: People Teams and Groups
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 0%
---
# Wie Gruppen Status übernehmen

Wenn Sie die für eine Gruppe verfügbaren Status auflisten, sehen Sie Folgendes

* Benutzerdefinierte Statuswerte, die für die Gruppe erstellt wurden, wie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md) beschrieben.
* Status, die vom System und von höheren Elementen in der Gruppenhierarchie übernommen wurden, wie in diesem Artikel erläutert.

## Übernehmen von Status

Ihre Gruppe übernimmt Status, wenn eine der folgenden Situationen eintritt:

* Sie erstellen die Gruppe.
* Ein Administrator sperrt einen Status in einer höheren Gruppe.
* Ein Administrator löscht eine andere Gruppe und wählt Ihre Gruppe als deren Platz aus.

In der folgenden Tabelle werden die einzelnen Umstände erläutert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wenn Sie eine Gruppe erstellen</td> 
   <td> <p>Wenn Sie eine neue Gruppe erstellen, erbt sie automatisch:</p> 
    <ul> 
     <li>Entsperrte Status in der Gruppe eine Ebene höher, wenn die neue Gruppe eine Untergruppe ist.</li> 
    </ul> 
    <ul> 
     <li>Gesperrte Status auf Systemebene .</li> 
    </ul> 
     <b>BEISPIEL:</b></span></span> 
     <p>Angenommen, eine Gruppe mit dem Namen Marketing verfügt über zwei Untergruppen namens Marketing-Kommunikation und -Branding.</p> 
     <p>Ein Gruppenadministrator der Marketing-Gruppe erstellt einen neuen benutzerdefinierten Status namens „Discovery“.</p> 
     <p>Später erstellen Sie eine neue Untergruppe unter der Marketing-Gruppe und nennen sie Advertising.</p> 
     <p>Ihre Untergruppe übernimmt den Erkennungsstatus, da Sie die Gruppe erstellt haben, nachdem der andere Administrator den entsperrten Erkennungsstatus erstellt hat.</p> 
     <p>Da die Untergruppen Marketing-Kommunikation und -Branding zu diesem Zeitpunkt bereits unterhalb der Marketing-Gruppe existierten, übernehmen sie den Status der entsperrten Erkennung nicht.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wenn ein Administrator einen Status auf einer höheren Ebene sperrt</td> 
   <td> <p>Wenn ein Workfront-Administrator einen Status auf Systemebene sperrt, erbt Ihre Gruppe ihn zusammen mit allen anderen Gruppen im System.</p> <p>Wenn ein Administrator einen Status für eine Gruppe sperrt, die sich über Ihrer Gruppe befindet, erbt Ihre Gruppe diesen Status ebenso wie alle anderen Untergruppen, die sich unterhalb der höheren Gruppe befinden.</p> <p><b>HINWEIS</b>: Wenn ein Administrator später einen dieser Status auf Systemebene oder in einer Gruppe über Ihrer Gruppe freischaltet, behält Ihre Gruppe den Status bei, den sie zuvor geerbt hat. Jetzt ist es eine separate Version des Status und Sie können ihn nur für Ihre Gruppe anpassen.</p> 
    <p><b>BEISPIEL:</b></p>
    <p>Der Administrator der Marketing-Gruppe sperrt den oben genannten Erkennungsstatus, um sicherzustellen, dass alle 3 Untergruppen ihn haben.</p> 
    <p>Zusammen mit Ihrer Advertising-Gruppe haben die Gruppen Marketing-Kommunikation und Branding jetzt den Status Erkennung . Sie haben sie geerbt, wenn sie in der Marketing-Gruppe über ihnen gesperrt war.</p> 
    <p>Der Administrator der Marketing-Gruppe entsperrt dann den Erkennungsstatus, sodass alle drei Untergruppen ihre eigene Version des Erkennungsstatus haben. Jetzt können Sie und die Administratoren der beiden anderen Gruppen den Erkennungsstatus an die Anforderungen Ihrer Gruppen anpassen.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wenn ein Administrator eine Gruppe löscht</td> 
   <td> <p>Wenn ein(e) Administrator(in) eine Gruppe löscht und Ihre auswählt, dass sie ihre Position im System einnimmt, übernimmt Ihre Gruppe die benutzerdefinierten Status der gelöschten Gruppe, wenn diese noch nicht in Ihrer Gruppe vorhanden sind.</p> 
   <p><b>BEISPIEL: </b></p>
     <p>Eine Gruppe namens „Messaging“ muss mit Ihrer Advertising-Gruppe zusammengeführt werden. Daher löscht ein Workfront-Administrator die Messaging-Gruppe und wählt Ihre Gruppe als Ersatz aus.</p> 
     <p>Die Messaging-Gruppe hatte einen eindeutigen Status namens In Bearbeitung. Ihre Advertising-Gruppe kann diesen Status jetzt verwenden.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Übernehmen von Statuskonfigurationen

Wenn Sie eine Gruppe der obersten Ebene erstellen, übernimmt sie die folgenden Konfigurationen von der Systemebene. Wenn Sie eine Untergruppe erstellen, übernimmt sie die folgenden Konfigurationen von der nächsthöheren Gruppe.

* Standardstatuskonfigurationen

  Weitere Informationen hierzu finden Sie unter [Verwenden benutzerdefinierter Status als Standardstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Konfigurationen der Statusanzeigereihenfolge

  Weitere Informationen hierzu finden Sie [Neuanordnen von Status auf Systemebene und Gruppenstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Wenn jemand diese Konfigurationen ändert, nachdem Ihre Gruppe erstellt wurde, sind ihre Status nicht betroffen.
