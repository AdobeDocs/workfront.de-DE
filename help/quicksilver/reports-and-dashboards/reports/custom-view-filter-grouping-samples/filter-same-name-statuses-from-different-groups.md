---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtern : Zeigt Elemente mit demselben Namen als Status an, wenn die Status mit verschiedenen Gruppen verknüpft sind'
description: Sie können der Gruppe A einen Aufgabenstatus mit dem Namen Neuer Status mit dem aus drei Buchstaben bestehenden Schlüssel NST zuweisen. Der Gruppe B kann ein weiterer Aufgabenstatus zugewiesen werden, der ebenfalls mit dem 3-Buchstaben-Schlüssel NES als Neuer Status bezeichnet wird. Obwohl die Namen für die beiden Status identisch sein können, ist der aus drei Buchstaben bestehende Code immer eindeutig. Weitere Informationen zum Gruppenstatus finden Sie unter Erstellen oder Bearbeiten eines Gruppenstatus.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Filtern : Zeigt Elemente mit demselben Namen-Status an, wenn die Status mit verschiedenen Gruppen verknüpft sind

<!--Audited: 10/2024-->

Sie können der Gruppe A einen Aufgabenstatus mit dem Namen *Neuer Status* mit dem aus drei Buchstaben bestehenden Schlüssel *NST* zuweisen. Der Gruppe B kann ein weiterer Aufgabenstatus zugewiesen werden, der auch *Neuer Status* mit dem 3-Buchstaben-Schlüssel *NES heißt.* Obwohl die Namen für die beiden Status identisch sein können, ist der aus drei Buchstaben bestehende Code immer eindeutig.

Weitere Informationen zum Gruppenstatus finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Mit dem Filter-Builder können Sie nicht zwischen den zwei Status mit demselben Namen identifizieren. Sie müssen den Textmodus in einem benutzerdefinierten Filter verwenden, um zwischen den beiden Status zu unterscheiden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Elemente mit demselben Namensstatus anzeigen, wenn die Status mit verschiedenen Gruppen verknüpft sind

1. Gehen Sie zur **Filter** Dropdown-Liste für den Filter, den Sie anpassen möchten, um beispielsweise eine Liste von Aufgaben anzuzeigen.\
   Dies funktioniert auch für Projekte und Probleme.
1. Klicken Sie **Neuer Filter**.
1. Wählen Sie aus der ersten Dropdown-Liste oben links Aufgabe > Status aus.
1. Wählen **für** Modifikator „Gleich“ und wählen Sie dann einen der Status aus, zu denen Sie einen Bericht erstellen möchten.

   Fügen Sie beispielsweise in einem Aufgabenbericht &quot;**ist gleich neuem Status** hinzu, wenn Sie nur Aufgaben anzeigen möchten, die den Status &quot;**Status“**.

   >[!TIP]
   >
   >Beachten Sie, dass Sie für einen Status mit dem Namen Neuer Status nur eine Option haben.

1. Klicken Sie **Textmodus**.\
   Der folgende Code sollte in dem dafür vorgesehenen Feld angezeigt werden:

   <pre>OR:1:status=NST<br>OR:1:status_mod=in </pre>

   >[!NOTE]
   >
   >Hier wird nur ein Status angezeigt. In der Statuszeile wird einer der drei Buchstaben für einen Status angezeigt.

1. Fügen Sie die folgenden zwei Codezeilen hinzu, um den Status hinzuzufügen, der im Filter fehlt:

   <pre>OR:2:status=NES<br>OR:2:status_mod=in</pre>

1. Klicken Sie **Übernehmen** und dann **Als neu speichern**.

   Die Liste zeigt beide Aufgaben mit dem Status „Neuer Status“ aus Gruppe A und mit dem Status „Neuer Status“ aus Gruppe B an.
