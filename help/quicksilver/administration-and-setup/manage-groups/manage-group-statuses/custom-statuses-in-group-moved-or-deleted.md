---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Benutzerdefinierte Status in einer Gruppe, die verschoben oder gelöscht wird
description: In diesem Artikel wird erläutert, was mit der Gruppe benutzerdefinierter Status passiert, wenn Sie eine Gruppe verschieben oder löschen.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Benutzerdefinierte Status in einer Gruppe, die verschoben oder gelöscht wird

In diesem Artikel wird erläutert, was mit der Gruppe benutzerdefinierter Status passiert, wenn Sie eine Gruppe verschieben oder löschen.

## Benutzerdefinierte Status in einer verschobenen Gruppe

Beachten Sie die folgenden Szenarien, in denen beschrieben wird, was mit der Gruppe benutzerdefinierter Status passiert, wenn Sie eine Gruppe unter einer anderen Gruppe an eine neue Position verschieben.

Informationen zum Verschieben einer Gruppe finden Sie unter [Verschieben einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Wenn Sie eine Gruppe unter eine andere Gruppe verschieben </td> 
   <td> <p>Alle Status der verschobenen Gruppe bleiben dabei. Sie werden nicht zum Status der neuen übergeordneten Gruppe der Gruppe hinzugefügt.</p> <p>Die verschobene Gruppe erbt jedoch alle gesperrten Status in der Gruppe oder Gruppen, die nun höher in ihrer Hierarchie sind. Wenn ein Administrator von nun an einen höheren Status in der Hierarchie sperrt, erbt die verschobene Gruppe diesen Status.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Wenn der Status in beiden Gruppen denselben Schlüssel, aber unterschiedliche Attribute aufweist</td> 
   <td> <p>Angenommen, zwei verschiedene Untergruppen übernehmen denselben entsperrten Status von einer übergeordneten Gruppe. Die Gruppenadministratoren der 2 Gruppen passen dann den Status für ihre Gruppen auf unterschiedliche Weise an.</p> <p>Später wird eine der beiden Gruppen unter die andere verschoben. Jetzt haben beide einen Status mit demselben Schlüssel, aber es hat unterschiedliche Attribute in den beiden Gruppen.</p> <p>In diesem Fall ist einer der folgenden Punkte wahr:</p> 
    <ul> 
     <li>Wenn der Status in der neuen übergeordneten Gruppe entsperrt ist, behält der Status in der verschobenen Gruppe seine Attribute bei, die von der Verschiebung nicht betroffen sind.</li> 
     <li>Wenn der Status in der neuen übergeordneten Gruppe gesperrt ist, überschreiben die Attribute des Status in der übergeordneten Gruppe die Attribute des Status in der verschobenen Gruppe.</li> 
    </ul> <p>Weitere Informationen zu Statusschlüsseln finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Wenn eine verschobene Gruppe Status von ihrer vorherigen übergeordneten Gruppe hat </td> 
   <td> <p>Alle benutzerdefinierten Status, die von der vorherigen übergeordneten Gruppe übernommen wurden, werden mit der verschobenen Gruppe übernommen und zu ihren eigenen benutzerdefinierten Status. Sie sind nicht mehr mit der vorherigen übergeordneten Gruppe verbunden.</p> 
    <ul> 
     <li>Wenn die vorherige übergeordnete Gruppe einen gesperrten benutzerdefinierten Status nach dem Verschieben bearbeitet, wirken sich die Änderungen nicht auf den Status der verschobenen Untergruppe aus.</li> 
     <li>Wenn die vorherige übergeordnete Gruppe einen benutzerdefinierten Status sperrt, der beim Verschieben der Gruppe entsperrt wurde, wird der Status der verschobenen Untergruppe nicht gesperrt.</li> 
     <li>Die verschobene Gruppe kann jetzt Status entsperren, die gesperrt waren, als sie sie von der vorherigen übergeordneten Gruppe übernommen hat.</li> 
    </ul> 
     <p><b>BEISPIEL</b><p> 
     <p>Olivia, der Gruppenadministrator für die Marketing-Gruppe, erstellt zwei Status für die Gruppe. Sie benennt einen First Review mit dem Schlüssel ABC und sperrt ihn. Sie nennt die andere Final Review mit dem Schlüssel XYZ und sperrt sie nicht.</p> 
     <p>Sie erstellt außerdem eine Untergruppe unter der Marketing-Gruppe namens Produktmarketing. Zum Zeitpunkt der Erstellung übernimmt sie automatisch die Erstüberprüfung und die Endgültige Überprüfung von der Marketing-Gruppe.</p> 
     <p>Später verschiebt Olivia die Produktmarketing-Untergruppe unter die Produktgruppe. Sowohl die erste Überprüfung als auch die endgültige Überprüfung gehen mit der Produktmarketinggruppe an ihren neuen Speicherort unter der Produktgruppe.</p> 
     <p>Obwohl die erste Überprüfung vor der Verschiebung gesperrt war, kann der Produktmarketing-Gruppenadministrator sie jetzt bearbeiten, da es sich nicht mehr um einen von der übergeordneten Gruppe, aus der sie stammt, verwalteten Status handelt.</p> 
     <p>Die abschließende Überprüfung ist entsperrt und kann wie immer bearbeitet werden.</p> 
     <p>Für die Marketing-Gruppe ändert Olivia die Farben von First Review und Final Review und benennt sie in First Review-Edited und Final Review-Edited um. Sie sperrt auch Final Review-Edited. In der Produktmarketing-Gruppe ändern sich die Farben und Namen der Status First Review und Final Review nicht.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerdefinierte Status in einer Gruppe, die gelöscht wird

Wenn Sie eine Gruppe oder Untergruppe löschen, weisen Sie die ihr zugeordneten Informationen, einschließlich ihrer benutzerdefinierten Status, einer anderen Gruppe oder Untergruppe zu. Die Status der gelöschten Gruppe werden zu denen der Zielgruppe hinzugefügt.

Wenn einer der Status der gelöschten Gruppe auch von der Zielgruppe verwendet wurde (der Status in beiden Gruppen hat denselben Schlüssel) und die Zielgruppe den Status auf unterschiedliche Weise angepasst hat, überschreiben die Einstellungen der Version der Zielgruppe die Einstellungen der Version der verschobenen Gruppe.

>[!INFO]
>
>**BEISPIEL:**
>
>Der Gruppenadministrator von Gruppe A benennt einen entsperrten Systemstatus für ihre Gruppe um. Der Gruppenadministrator einer Gruppe B benennt diesen Status auch für seine Gruppe um. Obwohl der Status in den beiden Gruppen unterschiedliche Namen hat, hat er denselben Schlüssel.
>
>Später wird Gruppe A gelöscht und alle zugehörigen Informationen werden Gruppe B zugewiesen.
>
>* Der Name der Version Gruppe B des Status überschreibt den Namen der Version Gruppe A.
>* Wenn der Status von einer Person in Gruppe A auf ein Objekt angewendet wurde, bevor diese Gruppe gelöscht wurde, wird der Statusname des Objekts in den Namen für den von Gruppe B verwendeten Status aktualisiert.
>
>Informationen zum Schlüssel für einen Status finden Sie in der Tabelle in diesem Artikel unter [Erstellen oder Bearbeiten eines benutzerdefinierten Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Erstellen oder Bearbeiten eines Status für eine Gruppe](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Informationen zum Löschen einer Gruppe finden Sie unter [Löschen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
