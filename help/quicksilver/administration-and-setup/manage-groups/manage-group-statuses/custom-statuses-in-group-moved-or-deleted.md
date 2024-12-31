---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Benutzerdefinierte Status in einer Gruppe, die verschoben oder gelöscht wird
description: In diesem Artikel wird erläutert, was mit der Gruppierung benutzerdefinierter Status geschieht, wenn Sie eine Gruppe verschieben oder löschen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Benutzerdefinierte Status in einer Gruppe, die verschoben oder gelöscht wird

In diesem Artikel wird erläutert, was mit der Gruppierung benutzerdefinierter Status geschieht, wenn Sie eine Gruppe verschieben oder löschen.

## Angepasste Status in einer verschobenen Gruppe

Betrachten Sie die folgenden Szenarien, die beschreiben, was mit benutzerdefinierten Gruppenstatus geschieht, wenn Sie eine Gruppe an einen neuen Speicherort unter einer anderen Gruppe verschieben.

Informationen zum Verschieben einer Gruppe finden Sie unter [Verschieben einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wenn Sie eine Gruppe in eine andere Gruppe verschieben </td> 
   <td> <p>Alle Status der verschobenen Gruppe bleiben bei ihr. Sie werden nicht zum Status der neuen übergeordneten Gruppe der Gruppe hinzugefügt.</p> <p>Die verschobene Gruppe übernimmt jedoch alle gesperrten Status in der Gruppe oder den Gruppen, die jetzt höher in ihrer Hierarchie sind. Wenn ein Administrator einen Status in der Hierarchie weiter oben sperrt, erbt die verschobene Gruppe diesen Status von nun an.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wenn ein Status in beiden Gruppen denselben Schlüssel, aber unterschiedliche Attribute aufweist</td> 
   <td> <p>Angenommen, zwei verschiedene Untergruppen erben denselben entsperrten Status von einer übergeordneten Gruppe. Die Gruppenadministratoren der beiden Gruppen passen dann den Status für ihre Gruppen auf unterschiedliche Weise an.</p> <p>Später wird eine der beiden Gruppen unter die andere verschoben. Jetzt haben beide einen Status mit demselben Schlüssel, aber er hat verschiedene Attribute in den beiden Gruppen.</p> <p>In diesem Fall trifft eine der folgenden Bedingungen zu:</p> 
    <ul> 
     <li>Wenn der Status in der neuen übergeordneten Gruppe entsperrt ist, behält der Status in der verschobenen Gruppe seine Attribute bei, ohne vom Verschieben betroffen zu sein.</li> 
     <li>Wenn der Status in der neuen übergeordneten Gruppe gesperrt ist, überschreiben die Attribute des Status in der übergeordneten Gruppe die des Status in der verschobenen Gruppe.</li> 
    </ul> <p>Informationen zu Statusschlüsseln finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Wenn eine verschobene Gruppe Status von der vorherigen übergeordneten Gruppe übernommen hat </td> 
   <td> <p>Alle benutzerdefinierten Status, die von der vorherigen übergeordneten Gruppe übernommen wurden, enthalten die verschobene Gruppe und werden zu eigenen benutzerdefinierten Status. Sie sind nicht mehr mit der vorherigen übergeordneten Gruppe verbunden.</p> 
    <ul> 
     <li>Wenn die vorherige übergeordnete Gruppe nach dem Verschieben einen gesperrten benutzerdefinierten Status bearbeitet, wirken sich die Änderungen nicht auf den Status der verschobenen Untergruppe aus.</li> 
     <li>Wenn die vorherige übergeordnete Gruppe einen benutzerdefinierten Status sperrt, der beim Verschieben der Gruppe entsperrt wurde, ist der Status der verschobenen Untergruppe nicht gesperrt.</li> 
     <li>Die verschobene Gruppe kann jetzt Status entsperren, die gesperrt wurden, als sie sie von der vorherigen übergeordneten Gruppe geerbt hat.</li> 
    </ul> 
     <p><b>BEISPIEL:</b><p> 
     <p>Olivia, die Gruppenadministratorin der Marketing-Gruppe, erstellt zwei Status für die Gruppe. Sie nennt einen First Review mit dem Schlüssel ABC und sperrt ihn. Sie nennt die andere Final Review mit dem Schlüssel XYZ und sperrt sie nicht.</p> 
     <p>Sie erstellt auch eine Untergruppe unter der Marketing-Gruppe namens „Produktmarketing“. Im Moment der Erstellung übernimmt sie automatisch sowohl die erste als auch die letzte Überprüfung von der Marketing-Gruppe.</p> 
     <p>Später verschiebt Olivia die Untergruppe „Produkt-Marketing“ in die Produktgruppe. Sowohl die erste als auch die abschließende Überprüfung gehen mit der Produktmarketing-Gruppe an den neuen Speicherort unter der Produktgruppe.</p> 
     <p>Obwohl die erste Überprüfung vor dem Verschieben gesperrt wurde, kann der Administrator der Marketing-Produktgruppe sie jetzt bearbeiten, da es sich nicht mehr um einen geerbten Status handelt, der von der übergeordneten Gruppe gesteuert wird, aus der sie stammt.</p> 
     <p>Die endgültige Überprüfung ist entsperrt und kann wie immer bearbeitet werden.</p> 
     <p>Für die Marketing-Gruppe ändert Olivia die Farben von First Review und Final Review und benennt sie in First Review Edited und Final Review Edited um. Sie sperrt auch Final Review-Edited. In der Produkt-Marketing-Gruppe ändern sich die Farben und Namen der Status „Erste Überprüfung“ und „Abschließende Überprüfung“ nicht.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Angepasste Status in einer Gruppe, die gelöscht wird

Wenn Sie eine Gruppe oder Untergruppe löschen, weisen Sie die mit ihr verknüpften Informationen, einschließlich ihres benutzerdefinierten Status, einer anderen Gruppe oder Untergruppe zu. Die Status der gelöschten Gruppe werden zu denen der Zielgruppe hinzugefügt.

Wenn einer der Status der gelöschten Gruppe auch von der Zielgruppe verwendet wurde (der Status in beiden Gruppen hat denselben Schlüssel) und die Zielgruppe den Status auf unterschiedliche Weise angepasst hat, überschreiben die Einstellungen der Version der Zielgruppe die Einstellungen der Version der verschobenen Gruppe.

>[!INFO]
>
>**BEISPIEL:**
>
>Der Gruppenadministrator der Gruppe A benennt einen entsperrten Status auf Systemebene in seine Gruppe um. Der Gruppenadministrator einer Gruppe B benennt diesen Status ebenfalls in seine Gruppe um. Obwohl der Status in den beiden Gruppen unterschiedliche Namen hat, hat er denselben Schlüssel.
>
>Später wird Gruppe A gelöscht und alle zugehörigen Informationen werden Gruppe B zugewiesen.
>
>* Der Name der Gruppe B-Version des Status überschreibt den Namen der Gruppe A-Version.
>* Wenn der Status von einer Person der Gruppe A auf ein Objekt angewendet wurde, bevor diese Gruppe gelöscht wurde, wird der Statusname auf dem Objekt auf den Namen für den Status aktualisiert, der von Gruppe B verwendet wird.
>
>Informationen zum Schlüssel für einen Status finden Sie in der Tabelle in diesem Artikel unter [Erstellen oder Bearbeiten eines benutzerdefinierten Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Erstellen oder Bearbeiten eines Status für eine Gruppe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Informationen zum Löschen einer Gruppe finden Sie unter [Löschen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
