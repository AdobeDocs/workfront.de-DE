---
product-area: projects
navigation-topic: manage-issues
title: Anfragestatus von „Warten auf Feedback“ automatisch auf „In Bearbeitung“ aktualisieren
description: Wenn der Primäre Kontaktperson eines Problems das Problem aktualisiert, indem entweder ein Feld aktualisiert (einschließlich eines benutzerdefinierten Felds) oder ein Kommentar hinzugefügt wird, wird der Problemstatus automatisch auf „In Bearbeitung“ aktualisiert.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: dc4b6dc284c59281206a457395765e634067ba91
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Problemstatus von „Auf Feedback warten“ automatisch auf „In Bearbeitung“ aktualisieren

<!--Audited: 109/2025-->

Wenn der Primäre Kontaktperson eines Problems das Problem aktualisiert, indem entweder ein Feld aktualisiert (einschließlich eines benutzerdefinierten Felds) oder ein Kommentar hinzugefügt wird, wird der Problemstatus automatisch auf „In Bearbeitung“ aktualisiert.

Damit diese automatische Statusänderung erfolgt, sind folgende Schritte erforderlich:

* Das Problem muss mithilfe einer Anfrage-Warteschlange hinzugefügt werden.

  Informationen zum Erstellen von Anfrage-Warteschlangen finden Sie [&#x200B; Abschnitt „Erstellen und Verwalten &#x200B;](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) Anfrage-Warteschlangen“.

  Informationen zum Senden von Anfragen an eine Anfrage-Warteschlange finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Die Warteschlangendetails in der Anfrage-Warteschlange müssen über die folgenden Einstellungen verfügen:
   * **Wenn jemand eine Anfrage stellt, automatisch gewähren** ist auf **Beitragszugriff** eingestellt
   * **Status ändern** ist ausgewählt

  ![Warteschlangendetails gewähren Beitragszugriff, und der Änderungsstatus ist ausgewählt.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Beim Einrichten einer Anfrage-Warteschlange können Sie den Zugriff definieren, den primäre Kontakte auf die von ihnen gesendeten Probleme haben.
  >
  >Wenn Sie die Auswahl der Einstellung „Status ändern“ beim Einrichten der Anfrage-Warteschlange aufheben, denken Sie daran, dass Systemadministratoren immer Zugriff haben, um den Status von Problemen zu ändern, auch wenn die Option „Status ändern“ in den Anfrage-Warteschlangeneinstellungen deaktiviert ist.

  Weitere Informationen zu Warteschlangendetails finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Das Problem muss den Status „Feedback ausstehend“ aufweisen.
* Für Probleme auf Systemebene muss der Status Ausstehendes Feedback (AWF) verfügbar sein.

  Weitere Informationen zum Status auf Systemebene finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
