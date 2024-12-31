---
product-area: projects
navigation-topic: manage-issues
title: Problemstatus von „Auf Feedback warten“ automatisch auf „In Bearbeitung“ aktualisieren
description: Wenn der Primäre Kontaktperson eines Problems das Problem aktualisiert, indem entweder ein Feld aktualisiert (einschließlich eines benutzerdefinierten Felds) oder ein Kommentar hinzugefügt wird, wird der Problemstatus automatisch auf „In Bearbeitung“ aktualisiert.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: 948cd81908df3174eb985d1c65533077d3ef5d49
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Problemstatus von „Auf Feedback warten“ automatisch auf „In Bearbeitung“ aktualisieren

Wenn der Primäre Kontaktperson eines Problems das Problem aktualisiert, indem entweder ein Feld aktualisiert (einschließlich eines benutzerdefinierten Felds) oder ein Kommentar hinzugefügt wird, wird der Problemstatus automatisch auf „In Bearbeitung“ aktualisiert.

Damit diese automatische Statusänderung erfolgt, ist Folgendes erforderlich:

* Das Problem muss über eine Anfrage-Warteschlange eingegeben werden.

  Informationen zum Erstellen von Anfrage-Warteschlangen finden Sie [ Abschnitt „Erstellen und Verwalten ](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) Anfrage-Warteschlangen“. Informationen zum Erstellen von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Die Warteschlangendetails in der Anfrage-Warteschlange müssen über die folgenden Einstellungen verfügen:
   * **Wenn jemand eine Anfrage stellt, wird** automatisch erteilt. ist auf **Contribute-Zugriff eingestellt**
   * **Status ändern** wird unter „Erweiterte Einstellungen“ ausgewählt

  ![Warteschlangendetails gewähren Contribute Zugriff, und der Änderungsstatus ist ausgewählt.](assets/queuedetails-contributeaccess-changestatus.png)

  >[!IMPORTANT]
  >
  >  Beim Einrichten einer Anfrage-Warteschlange können Sie den Zugriff definieren, den primäre Kontakte auf die von ihnen gesendeten Probleme haben.
  >
  >Wenn Sie die Auswahl der Einstellung „Status ändern“ beim Einrichten der Anfrage-Warteschlange aufheben, denken Sie daran, dass Systemadministratoren immer Zugriff haben, um den Status von Problemen zu ändern, auch wenn die Option „Status ändern“ in den Anfrage-Warteschlangeneinstellungen deaktiviert ist.

  Weitere Informationen zu Warteschlangendetails finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Das Problem muss den Status „Feedback ausstehend“ aufweisen.
* Für Probleme auf Systemebene muss der Status Ausstehendes Feedback (AWF) verfügbar sein.

  Weitere Informationen zum Status auf Systemebene finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
