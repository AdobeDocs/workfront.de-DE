---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Elemente nach Status gleichen Namens anzeigen, wenn die Status verschiedenen Gruppen zugeordnet sind'
description: Sie können der Gruppe A einen Aufgabenstatus mit dem Namen Neuer Status mit der aus drei Buchstaben bestehenden Taste NST zuweisen. Gruppe B kann ein anderer Aufgabenstatus zugewiesen werden, der auch "Neuer Status" mit dem dreistelligen Schlüssel NES genannt wird. Obwohl die Namen für die zwei Status identisch sein können, ist der aus drei Buchstaben bestehende Code immer eindeutig. Weitere Informationen zu Gruppenstatus finden Sie unter Erstellen oder Bearbeiten eines Gruppenstatus.
author: Courtney
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 11%

---

# Filter: Elemente nach gleichnamigen Status anzeigen, wenn die Status mit verschiedenen Gruppen verknüpft sind

<!--Audited: 10/2024-->

Der Gruppe A kann ein Aufgabenstatus mit dem Namen *Neuer Status* mit dem aus drei Buchstaben bestehenden Schlüssel *NST* zugewiesen werden. Möglicherweise ist der Gruppe B ein anderer Aufgabenstatus zugewiesen, der auch *Neuer Status* mit dem aus drei Buchstaben bestehenden Schlüssel *NES heißt.* Obwohl die Namen für die 2 Status identisch sein können, ist der 3-Buchstaben-Code immer eindeutig.

Weitere Informationen zu Gruppenstatus finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Mit dem Filter-Generator können Sie nicht zwischen den zwei Status mit demselben Namen unterscheiden. Sie müssen den Textmodus in einem benutzerdefinierten Filter verwenden, um zwischen den beiden Status zu unterscheiden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Anbieter oder Anforderung zum Ändern eines Filters </p>
   <p>Standard oder Abo zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen zum Ändern eines Filters</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Elemente mit Status gleichen Namens anzeigen, wenn die Status verschiedenen Gruppen zugeordnet sind

1. Wechseln Sie zum Dropdown-Menü **Filter** für den Filter, den Sie für eine Liste von Aufgaben anpassen möchten.\
   Dies funktioniert auch bei Projekten und Problemen gleich.
1. Klicken Sie auf **Neuer Filter**.
1. Wählen Sie aus dem ersten Dropdownmenü in der oberen linken Ecke Aufgabe > Status aus.
1. Wählen Sie **Equals** für den Modifizierer aus, und wählen Sie dann einen der Status aus, für den Sie einen Bericht erstellen möchten.

   Fügen Sie z. B. in einem Aufgabenbericht **Status ist gleich Neuer Status** hinzu, wenn Sie nur Aufgaben anzeigen möchten, die den Status **Neuer Status** aufweisen.

   >[!TIP]
   >
   >Beachten Sie, dass für den Status &quot;Neuer Status&quot; nur eine Option zur Verfügung steht.

1. Klicken Sie auf **Textmodus**.\
   Der folgende Code sollte im angegebenen Bereich angezeigt werden:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Hier wird nur ein Status angezeigt. In der Statuszeile wird eine der Tasten mit drei Buchstaben für einen der Status angezeigt.

1. Fügen Sie die folgenden zwei Codezeilen hinzu, um den Status hinzuzufügen, der im Filter fehlt:

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Klicken Sie auf **Anwenden** und anschließend auf **Als neu speichern**.

   In der Liste werden beide Aufgaben mit dem Status &quot;Neuer Status&quot; aus Gruppe A und mit dem Status &quot;Neuer Status&quot; aus Gruppe B angezeigt.
