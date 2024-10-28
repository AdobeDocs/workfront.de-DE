---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: Elemente nach Status mit identischen Namen anzeigen, wenn die Status mit verschiedenen Gruppen verknüpft sind"
description: Mit dem 3-Buchstaben-Schlüssel NST können Sie Gruppe A einen Aufgabenstatus mit dem Namen Neuer Status zuweisen. Möglicherweise ist der Gruppe B ein anderer Aufgabenstatus mit dem Namen Neuer Status mit dem 3-Buchstaben-Schlüssel NES zugewiesen. Obwohl die Namen für die beiden Status identisch sein können, ist der 3-Buchstaben-Code immer eindeutig. Weitere Informationen zum Gruppenstatus finden Sie unter Erstellen oder Bearbeiten eines Gruppenstatus.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Filter: Zeigt Elemente nach Status mit demselben Namen an, wenn die Status mit verschiedenen Gruppen verknüpft sind

<!--Audited: 10/2024-->

Sie können Gruppe A einen Aufgabenstatus mit dem Namen *Neuer Status* mit dem 3-Buchstaben-Schlüssel *NST* zuweisen. Möglicherweise wird Gruppe B ein anderer Aufgabenstatus mit dem Namen *Neuer Status* mit dem 3-Buchstaben-Schlüssel *NES zugewiesen.* Obwohl die Namen für die beiden Status identisch sein können, ist der 3-Buchstaben-Code immer eindeutig.

Weitere Informationen zum Gruppenstatus finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Mit dem Filter-Builder können Sie nicht zwischen den beiden Status identifizieren, die denselben Namen haben. Sie müssen den Textmodus in einem benutzerdefinierten Filter verwenden, um zwischen den beiden Status zu unterscheiden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen von Elementen nach Status des gleichen Namens, wenn die Status mit verschiedenen Gruppen verknüpft sind

1. Navigieren Sie zur Dropdown-Liste **Filter** für den Filter, den Sie für eine Liste von Aufgaben anpassen möchten, z. B. .\
   Dies gilt auch für Projekte und Probleme.
1. Klicken Sie auf **Neuer Filter**.
1. Wählen Sie aus der ersten Dropdown-Liste oben links &quot;Aufgabe&quot;> &quot;Status&quot;.
1. Wählen Sie **Gleich** für den Modifikator und dann einen der Status aus, über die Sie einen Bericht erstellen möchten.

   Fügen Sie beispielsweise in einem Aufgabenbericht **Status gleich Neuer Status** hinzu, wenn Sie nur Aufgaben anzeigen möchten, die den Status **Neuer Status** aufweisen.

   >[!TIP]
   >
   >Beachten Sie, dass Sie nur eine Option für einen Status mit dem Namen &quot;Neuer Status&quot;haben.

1. Klicken Sie auf **Textmodus**.\
   Der folgende Code sollte im bereitgestellten Bereich angezeigt werden:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Hier wird nur ein Status angezeigt. Die Statuszeile zeigt einen der 3-Buchstaben-Schlüssel für einen der Status an.

1. Fügen Sie die folgenden 2 Codezeilen hinzu, um den Status hinzuzufügen, der im Filter fehlt:

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Klicken Sie auf **Anwenden** und dann auf **Als neu speichern**.

   Die Liste zeigt beide Aufgaben mit dem Status &quot;Neuer Status&quot;aus Gruppe A und dem Status &quot;Neuer Status&quot;aus Gruppe B an.
