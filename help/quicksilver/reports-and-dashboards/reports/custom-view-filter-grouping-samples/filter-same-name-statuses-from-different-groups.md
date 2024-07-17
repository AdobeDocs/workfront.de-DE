---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: Elemente nach gleichnamigen Status anzeigen, wenn die Status verschiedenen Gruppen zugeordnet sind"
description: Mit dem 3-Buchstaben-Schlüssel NST können Sie Gruppe A einen Aufgabenstatus mit dem Namen Neuer Status zuweisen. Möglicherweise ist der Gruppe B ein anderer Aufgabenstatus mit dem Namen Neuer Status mit dem 3-Buchstaben-Schlüssel NES zugewiesen. Obwohl die Namen für die beiden Status identisch sein können, ist der 3-Buchstaben-Code immer eindeutig. Weitere Informationen zum Gruppenstatus finden Sie unter Erstellen oder Bearbeiten eines Gruppenstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 0%

---

# Filter: Zeigt Elemente nach Status mit demselben Namen an, wenn die Status mit verschiedenen Gruppen verknüpft sind

Sie können Gruppe A einen Aufgabenstatus mit dem Namen *Neuer Status* mit dem 3-Buchstaben-Schlüssel *NST* zuweisen. Möglicherweise wird Gruppe B ein anderer Aufgabenstatus mit dem Namen *Neuer Status* mit dem 3-Buchstaben-Schlüssel *NES zugewiesen.* Obwohl die Namen für die beiden Status identisch sein können, ist der 3-Buchstaben-Code immer eindeutig.\
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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Filteranforderung </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigen von Elementen nach Status des gleichen Namens, wenn die Status mit verschiedenen Gruppen verknüpft sind

1. Gehen Sie zum Filter, den Sie für eine Liste von Aufgaben anpassen möchten, z. B. .\
   Dies gilt auch für Projekte und Probleme.
1. Klicken Sie auf **Filterregel hinzufügen** für das Feld **Status** des Objekts Ihrer Liste.\
   Fügen Sie beispielsweise in einem Aufgabenbericht **Status gleich Neuer Status** hinzu, wenn Sie nur Aufgaben anzeigen möchten, die den Status **Neuer Status** aufweisen.

   >[!TIP]
   >
   >Beachten Sie, dass Sie nur eine Option für einen Status mit dem Namen &quot;Neuer Status&quot;haben.

1. Klicken Sie auf **Wechseln zum Textmodus**.\
   Der folgende Code sollte angezeigt werden:
   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Hier wird nur ein Status angezeigt. Die Statuszeile zeigt einen der 3-Buchstaben-Schlüssel für einen der Status an.

1. Fügen Sie die folgenden 2 Codezeilen hinzu, um den Status hinzuzufügen, der im Filter fehlt:
   <pre>OR:1:status=NES<br>OR:1:status_Mod=in</pre>

1. Klicken Sie auf **Fertig** und dann auf **Filter speichern**.

   Die Liste zeigt beide Aufgaben mit dem Status &quot;Neuer Status&quot;aus Gruppe A und dem Status &quot;Neuer Status&quot;aus Gruppe B an.
