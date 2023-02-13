---
product-area: projects
navigation-topic: manage-projects
title: Wählen Sie den Projektaktualisierungstyp aus
description: Durch die Auswahl eines Aktualisierungstyps für ein Projekt können Sie steuern, wie häufig die Änderungen, die Sie an der Timeline des Projekts vornehmen, für die übergeordneten Aufgaben oder das Projekt gespeichert werden.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# Wählen Sie den Projektaktualisierungstyp aus

Durch die Auswahl eines Aktualisierungstyps für ein Projekt können Sie steuern, wie häufig die Änderungen, die Sie an der Timeline des Projekts vornehmen, für die übergeordneten Aufgaben oder das Projekt gespeichert werden.

Wenn die Projekt-Timeline aktualisiert wird, wird sie anhand von Änderungen am Projekt, seinen Aufgaben oder Änderungen an einem anderen Projekt, von dem die Timeline abhängig ist, neu berechnet.

Beispielsweise können die folgenden Änderungen an den Aufgaben auf dem Projekt-Trigger eine Aktualisierung der Timeline des Projekts bewirken:

* Datum der Aufgaben aktualisieren
* Ändern von Vorgängerbeziehungen von Aufgaben
* Ändern Sie die Beziehungen zwischen über- und untergeordneten Elementen, fügen Sie Zuweisungen hinzu oder entfernen Sie sie, und ändern Sie darüber hinaus die Aufgabenbegrenzung oder den Dauertyp.

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aktualisierungstyp eines Projekts aktualisieren

Wenn die Aufgaben aktualisiert werden, werden ihre übergeordneten Objekte (übergeordnete Aufgaben oder das Projekt) zu dem durch den Aktualisierungstyp angegebenen Zeitpunkt aktualisiert.  So legen Sie einen Aktualisierungstyp für Ihr Projekt fest:

1. Wechseln Sie zu dem Projekt, dessen Aktualisierungstyp Sie angeben möchten.
1. Klicken Sie auf das Menü Mehr . ![](assets/more-icon.png) neben dem Namen des Projekts klicken Sie auf **Bearbeiten** .

1. Klicken  **Projekt** **Einstellungen**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. Im **Aktualisierungstyp** auswählen, ob Workfront die Timeline des Projekts automatisch täglich berechnen soll, wenn eine Änderung eintritt oder ob der Projektmanager sie manuell berechnen soll.

   Wählen Sie aus den Optionen in der folgenden Liste aus. 

   >[!IMPORTANT]
   >
   >Wenn die Timeline eines Projekts länger als 15 Jahre ist, berechnet Workfront die Timeline nicht automatisch oder bei Änderung. Der Aktualisierungstyp eines Projekts, das länger als 15 Jahre dauert, ist immer Manuell.

   * **Automatisch und Bei Änderung:** Dies ist die Standardeinstellung. Die Projekt-Timeline wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem die Timeline abhängig ist. Die Projekt-Timeline wird auch jede Nacht aktualisiert. \
      Dies ist die empfohlene Einstellung, da sie sicherstellt, dass die Projekt-Timeline immer auf dem neuesten Stand ist.

      Wenn Sie eine Aufgabe oder das Projekt aktualisieren und eine Timeline-Neuberechnung Trigger haben, werden alle verfügbaren Daten sofort angezeigt, sodass Sie mit der Arbeit fortfahren können. Bei Projekten mit mehr als 100 Aufgaben werden Daten, die längere Berechnungen erfordern, abgeblendet dargestellt.

      ![](assets/dates-dimmed-when-insline-editing-350x146.png)

      Dies bedeutet, dass die Neuberechnung noch nicht abgeschlossen ist und sich die Daten ändern können.

   * **Nur ändern:** Die Projekt-Timeline wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem die Timeline abhängig ist. Geplante Aktualisierungen treten nicht auf.\
      Sie können diese Option auswählen, wenn Sie Bedenken hinsichtlich der Systemleistung haben und nur selten Änderungen am Projekt oder an anderen Projekten auftreten, von denen die Timeline abhängig ist.

   * **Nur Automatisch:** Die Projektzeitleiste wird jede Nacht aktualisiert. sie wird nicht sofort aktualisiert, nachdem Änderungen vorgenommen wurden.\
      Sie können diese Option auswählen, wenn Sie Bedenken hinsichtlich der Systemleistung haben und wenn täglich im Projekt oder in anderen Projekten, von denen die Timeline abhängig ist, viele Änderungen auftreten.

      >[!NOTE]
      >
      >Ein Projekt berechnet nicht automatisch jede Nacht neu, wenn es sich im Planungsstatus befindet. Es wird nur bei Veränderung neu berechnet.

   * **Nur manuell:** Die Projekt-Timeline wird nur aktualisiert, wenn Sie die Option zum **Zeitleisten neu berechnen**, wie im Abschnitt &quot;Manuelle Neuberechnung&quot;im Artikel beschrieben [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
      Sie können diese Option auswählen, wenn Sie gleichzeitig viele Änderungen am Projekt vornehmen und möchten, dass die Timeline-Neuberechnung erfolgt, nachdem alle Änderungen vorgenommen wurden (und nicht nach jeder einzelnen Änderung).

1. Klicken Sie auf **Speichern**.
