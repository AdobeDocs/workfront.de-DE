---
product-area: projects
navigation-topic: manage-projects
title: Wählen Sie den Projektaktualisierungstyp
description: Durch Auswahl eines Aktualisierungstyps für ein Projekt können Sie steuern, wie oft die Änderungen, die Sie an der Zeitleiste des Projekts vornehmen, in den übergeordneten Aufgaben oder im Projekt gespeichert werden.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Wählen Sie den Projektaktualisierungstyp

Durch Auswahl eines Aktualisierungstyps für ein Projekt können Sie steuern, wie oft die Änderungen, die Sie an der Zeitleiste des Projekts vornehmen, in den übergeordneten Aufgaben oder im Projekt gespeichert werden.

Wenn die Zeitleiste des Projekts aktualisiert wird, wird sie auf der Grundlage der am Projekt vorgenommenen Änderungen, der zugehörigen Aufgaben oder der Änderungen an einem anderen Projekt, von dem die Zeitleiste abhängig ist, neu berechnet.

Beispielsweise wird durch die folgenden Änderungen an den Aufgaben im Projekt-Trigger die Timeline aktualisiert  des Projekts:

* Aktualisieren der Daten von Aufgaben
* Vorgängerbeziehungen von Aufgaben ändern
* Ändern Sie die hierarchischen Beziehungen, indem Sie zusätzlich zur Änderung der Aufgabenbeschränkung oder des Dauertyps Zuweisungen hinzufügen oder entfernen.

## Zugriffsanforderungen

<!-- drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für ein Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Aktualisieren des Aktualisierungstyps eines Projekts

Wenn die Aufgaben aktualisiert werden, werden ihre übergeordneten Objekte (übergeordnete Aufgaben oder das Projekt) zu dem Zeitpunkt aktualisiert, der durch den Aktualisierungstyp angegeben wird.  So geben Sie einen Aktualisierungstyp für Ihr Projekt an:

1. Wechseln Sie zu dem Projekt, dessen Aktualisierungstyp Sie angeben möchten.
1. Klicken Sie auf das Menü ![Mehr](assets/more-icon.png) neben dem Namen des Projekts und dann auf **Bearbeiten** .

1. Klicken Sie auf **Projekt** **Einstellungen**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. Wählen Sie im Feld **Aktualisierungstyp** aus, ob Workfront die Zeitleiste des Projekts automatisch täglich berechnen soll, bei einer Änderung oder ob der Projektmanager sie manuell berechnen soll.

   Wählen Sie aus den Optionen in der folgenden Liste aus. 

   >[!IMPORTANT]
   >
   >Wenn der Zeitplan eines Projekts länger als 15 Jahre ist, berechnet Workfront den Zeitplan nicht automatisch oder bei einer Änderung. Der Aktualisierungstyp eines Projekts, das länger als 15 Jahre dauert, ist immer „Manuell“.

   * **Automatisch und Bei Änderung** Dies ist die Standardeinstellung. Die Zeitleiste des Projekts wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt auftritt, von dem die Zeitleiste abhängig ist. Die Zeitleiste des Projekts wird ebenfalls jede Nacht aktualisiert. \
     Dies ist die empfohlene Einstellung, da sie sicherstellt, dass die Zeitleiste des Projekts immer auf dem neuesten Stand ist.

     Trigger Wenn Sie eine Aufgabe oder das Projekt aktualisieren und eine Neuberechnung der Zeitleiste durchführen, werden alle verfügbaren Daten sofort angezeigt, sodass Sie weiterarbeiten können. Bei Projekten mit mehr als 100 Aufgaben werden Datumsangaben, für die längere Berechnungen erforderlich sind, abgeblendet.

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

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
