---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Benutzerdefinierte Status für eine Aufgabe oder ein Problem, die verschoben oder kopiert wird
description: Wenn Sie eine Aufgabe oder ein Problem in ein anderes Projekt verschieben oder kopieren, werden möglicherweise einige Status der Aufgabe oder des Problems aktualisiert, um den Status zu erhalten, der von der Gruppe des Zielprojekts verwendet wird.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4bd9b89d-9c66-4af7-97bf-f9518ad55d7c
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Benutzerdefinierter Status bei einer Aufgabe oder einem Problem, die/das verschoben oder kopiert wird

Wenn Sie eine Aufgabe oder ein Problem in ein anderes Projekt verschieben oder kopieren, werden möglicherweise einige Status der Aufgabe oder des Problems aktualisiert, um den Status zu erhalten, der von der Gruppe des Zielprojekts verwendet wird. Dies hängt davon ab, ob Status mit demselben Schlüssel in dieser Gruppe vorhanden sind:

* Wenn ein Status für die Aufgabe oder das Problem denselben Schlüssel wie ein Status hat, der von der Gruppe des Zielprojekts verwendet wird, bleibt der Status für die Aufgabe oder das Problem derselbe.

  Wenn die Bezeichnung dieser beiden Status nicht übereinstimmt, übernimmt der Status der Aufgabe oder des Problems die Bezeichnung des Status, der von der Gruppe des Zielprojekts verwendet wird.

* Wenn ein Status in der Aufgabe oder in einem Problem nicht denselben Schlüssel wie der entsprechende Status in der Gruppe des Zielprojekts hat, ändert sich der Status in der Aufgabe oder des Problems in den entsprechenden Standardstatus in der Gruppe des Zielprojekts.

Weitere Informationen zu Statusschlüsseln finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
