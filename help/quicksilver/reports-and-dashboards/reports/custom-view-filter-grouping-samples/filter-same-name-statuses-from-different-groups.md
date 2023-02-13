---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''Filter: Anzeigen von Elementen nach Status mit demselben Namen, wenn die Status mit den unterschiedlichen Gruppen verknüpft sind'
description: Mit dem 3-Buchstaben-Schlüssel NST können Sie Gruppe A einen Aufgabenstatus mit dem Namen Neuer Status zuweisen. Möglicherweise ist der Gruppe B ein anderer Aufgabenstatus mit dem Namen Neuer Status mit dem 3-Buchstaben-Schlüssel NES zugewiesen. Obwohl die Namen für die beiden Status identisch sein können, ist der 3-Buchstaben-Code immer eindeutig. Weitere Informationen zum Gruppenstatus finden Sie unter Erstellen oder Bearbeiten eines Gruppenstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Filter: Elemente nach Status mit demselben Namen anzeigen, wenn die Status mit verschiedenen Gruppen verknüpft sind

Sie können den Aufgabenstatus der Gruppe A mit dem Namen *Neuer Status* mit der 3-Buchstaben-Taste *NST*. Möglicherweise ist der Gruppe B ein anderer Aufgabenstatus zugewiesen, der auch *Neuer Status* mit der 3-Buchstaben-Taste *NES.* Obwohl die Namen für die beiden Status identisch sein können, ist der 3-Buchstaben-Code immer eindeutig.\
Weitere Informationen zum Gruppenstatus finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Mit dem Filter-Builder können Sie nicht zwischen den beiden Status identifizieren, die denselben Namen haben. Sie müssen den Textmodus verwenden, um zwischen den beiden Status zu unterscheiden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigen von Elementen nach Status des gleichen Namens, wenn die Status mit verschiedenen Gruppen verknüpft sind

1. Gehen Sie zum Filter, den Sie für eine Liste von Aufgaben anpassen möchten, z. B. .\
   Dies gilt auch für Projekte und Probleme.
1. Klicken **Filterregel hinzufügen** für **Status** -Feld des Listenobjekts.\
   Fügen Sie beispielsweise in einem Aufgabenbericht **Status Gleich neuer Status**, wenn Sie nur Aufgaben anzeigen möchten, die sich im Status **Neuer Status**.

   >[!TIP]
   >
   >Beachten Sie, dass Sie nur eine Option für einen Status mit dem Namen &quot;Neuer Status&quot;haben.

1. Klicken **In den Textmodus wechseln**.\
   Der folgende Code sollte angezeigt werden:

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Hier wird nur ein Status angezeigt. Die Statuszeile zeigt einen der 3-Buchstaben-Schlüssel für einen der Status an.

1. Fügen Sie die folgenden 2 Codezeilen hinzu, um den Status hinzuzufügen, der im Filter fehlt:

   <pre>ODER:1:status=NES<br>ODER:1:status_Mod=in</pre>

1. Klicken **Fertig**, dann **Filter speichern**.

   Die Liste zeigt beide Aufgaben mit dem Status &quot;Neuer Status&quot;aus Gruppe A und dem Status &quot;Neuer Status&quot;aus Gruppe B an.
