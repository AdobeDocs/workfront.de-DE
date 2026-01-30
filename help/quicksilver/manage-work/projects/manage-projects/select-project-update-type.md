---
product-area: projects
navigation-topic: manage-projects
title: Typ der Projektaktualisierung auswählen
description: Durch Auswahl eines Aktualisierungstyps für ein Projekt können Sie steuern, wie oft die Änderungen, die Sie an der Zeitleiste des Projekts vornehmen, in den übergeordneten Aufgaben oder im Projekt gespeichert werden.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 3%

---

# Wählen Sie den Projektaktualisierungstyp

Durch Auswahl eines Aktualisierungstyps für ein Projekt können Sie steuern, wie oft die Änderungen, die Sie an der Zeitleiste des Projekts vornehmen, in den übergeordneten Aufgaben oder im Projekt gespeichert werden.

Wenn die Zeitleiste des Projekts aktualisiert wird, wird sie auf der Grundlage der am Projekt vorgenommenen Änderungen, der zugehörigen Aufgaben oder der Änderungen an einem anderen Projekt, von dem die Zeitleiste abhängig ist, neu berechnet.

Beispielsweise wird durch die folgenden Änderungen an den Aufgaben im Projekt-Trigger die Zeitleiste des Projekts aktualisiert:

* Aktualisieren der Daten von Aufgaben
* Vorgängerbeziehungen von Aufgaben ändern
* Ändern Sie die hierarchischen Beziehungen, indem Sie zusätzlich zur Änderung der Aufgabenbeschränkung oder des Dauertyps Zuweisungen hinzufügen oder entfernen.

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für ein Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktualisieren des Aktualisierungstyps eines Projekts

Wenn die Aufgaben aktualisiert werden, werden ihre übergeordneten Objekte (übergeordnete Aufgaben oder das Projekt) zu dem Zeitpunkt aktualisiert, der durch den Aktualisierungstyp angegeben wird.  So geben Sie einen Aktualisierungstyp für Ihr Projekt an:

1. Wechseln Sie zu dem Projekt, dessen Aktualisierungstyp Sie angeben möchten.
1. Klicken Sie auf das Menü ![Mehr](assets/more-icon.png) neben dem Namen des Projekts und dann auf **Bearbeiten** .

1. Klicken Sie auf **Projekt** **Einstellungen**.

   ![Feld „Aktualisierungstyp“ im Projekt-Bearbeitungsfeld](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. Wählen Sie im Feld **Aktualisierungstyp** aus, ob Workfront die Zeitleiste des Projekts automatisch täglich berechnen soll, bei einer Änderung oder ob der Projektmanager sie manuell berechnen soll.

   Wählen Sie aus den Optionen in der folgenden Liste aus.

   >[!IMPORTANT]
   >
   >Wenn der Zeitplan eines Projekts länger als 15 Jahre ist, berechnet Workfront den Zeitplan nicht automatisch oder bei einer Änderung. Der Aktualisierungstyp eines Projekts, das länger als 15 Jahre dauert, ist immer „Manuell“.

   * **Automatisch und Bei Änderung** Dies ist die Standardeinstellung. Die Zeitleiste des Projekts wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt auftritt, von dem die Zeitleiste abhängig ist. Die Zeitleiste des Projekts wird ebenfalls jede Nacht aktualisiert.\
     Dies ist die empfohlene Einstellung, da sie sicherstellt, dass die Zeitleiste des Projekts immer auf dem neuesten Stand ist.

     Trigger Wenn Sie eine Aufgabe oder das Projekt aktualisieren und eine Neuberechnung der Zeitleiste durchführen, werden alle verfügbaren Daten sofort angezeigt, sodass Sie weiterarbeiten können. Bei Projekten mit mehr als 100 Aufgaben werden Datumsangaben, für die längere Berechnungen erforderlich sind, abgeblendet.

     ![Datumsangaben bei Inline-Bearbeitung abgeblendet](assets/dates-dimmed-when-insline-editing-350x146.png)

     Dies bedeutet, dass die Neuberechnung noch nicht abgeschlossen ist und sich die Daten ändern können.

   * **Nur Änderung** Die Zeitleiste des Projekts wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem die Zeitleiste abhängig ist. Geplante Aktualisierungen werden nicht durchgeführt.\
     Sie sollten diese Option auswählen, wenn Sie sich Sorgen über die Systemleistung machen und wenn Änderungen selten im Projekt oder in anderen Projekten auftreten, von denen die Zeitleiste abhängig ist.

   * **Nur automatisch** Die Zeitleiste des Projekts wird jede Nacht aktualisiert. Sie wird nicht sofort nach den Änderungen aktualisiert.\
     Sie sollten diese Option auswählen, wenn Sie sich Sorgen über die Systemleistung machen und wenn im Projekt oder in anderen Projekten, von denen die Timeline abhängig ist, täglich viele Änderungen auftreten.

     >[!NOTE]
     >
     >Ein Projekt wird nicht jede Nacht automatisch neu berechnet, wenn es sich im Status „Planung“ befindet. Er wird nur bei Änderung neu berechnet.

   * **Nur manuell:** Die Projekt-Zeitleiste wird nur aktualisiert, wenn Sie die Option **Zeitleisten neu berechnen** auswählen, wie im Abschnitt „Manuelle Neuberechnung“ im Artikel [Neuberechnen von Projekt-Zeitleisten](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) beschrieben.\
     Sie können diese Option auswählen, wenn Sie mehrere Änderungen am Projekt gleichzeitig vornehmen und die Neuberechnung der Zeitleiste nach allen Änderungen (und nicht nach jeder einzelnen Änderung) durchgeführt werden soll.

1. Klicken Sie auf **Speichern**.
