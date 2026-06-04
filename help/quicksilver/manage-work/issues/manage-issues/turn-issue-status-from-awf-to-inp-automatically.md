---
product-area: projects
navigation-topic: manage-issues
title: Anfragestatus von „Warten auf Feedback“ automatisch auf „In Bearbeitung“ aktualisieren
description: Wenn der Primäre Kontaktperson eines Problems das Problem aktualisiert, indem entweder ein Feld aktualisiert (einschließlich eines benutzerdefinierten Felds) oder ein Kommentar hinzugefügt wird, wird der Problemstatus automatisch auf „In Bearbeitung“ aktualisiert.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
TQID: https://experienceleague.adobe.com/axgDUT8M6p79omHTSO8OrvM7qAM81AjG0Fug2JUl4ck
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 3%

---

# Automatisches Aktualisieren des Problemstatus von „Auf Feedback warten“ auf „In Bearbeitung“

<!--Audited: 109/2025-->

Wenn der Primäre Kontaktperson eines Problems das Problem aktualisiert, indem entweder ein Feld aktualisiert (einschließlich eines benutzerdefinierten Felds) oder ein Kommentar hinzugefügt wird, wird der Problemstatus automatisch auf „In Bearbeitung“ aktualisiert.

Damit diese automatische Statusänderung erfolgt, sind folgende Schritte erforderlich:

* Das Problem muss mithilfe einer Anfrage-Warteschlange hinzugefügt werden.

  Informationen zum Erstellen von Anfrage-Warteschlangen finden Sie [ Abschnitt „Erstellen und Verwalten ](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) Anfrage-Warteschlangen“.

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
