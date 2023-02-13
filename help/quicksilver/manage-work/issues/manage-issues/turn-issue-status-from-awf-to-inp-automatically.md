---
product-area: projects
navigation-topic: manage-issues
title: Automatische Aktualisierung des Problemstatus von "Warten auf Feedback"auf "In Bearbeitung"
description: Wenn der Primäre Kontakt eines Problems das Problem aktualisiert, indem entweder ein Feld (einschließlich eines benutzerdefinierten Felds) aktualisiert oder ein Kommentar hinzugefügt wird, wird der Problemstatus automatisch in In Bearbeitung aktualisiert.
author: Alina
feature: Work Management
exl-id: f94bb644-910f-4b46-80fd-fecbdf9cb18a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Automatische Aktualisierung des Problemstatus von &quot;Warten auf Feedback&quot;auf &quot;In Bearbeitung&quot;

Wenn der Primäre Kontakt eines Problems das Problem aktualisiert, indem entweder ein Feld (einschließlich eines benutzerdefinierten Felds) aktualisiert oder ein Kommentar hinzugefügt wird, wird der Problemstatus automatisch in In Bearbeitung aktualisiert.

Damit diese automatische Statusänderung eintritt, ist Folgendes erforderlich:

* Das Problem muss über eine Anforderungswarteschlange eingegeben werden.

   Informationen zum Erstellen von Anforderungswarteschlangen finden Sie in der [Erstellen und Verwalten von Anforderungswarteschlangen](../../../manage-work/requests/create-and-manage-request-queues/create-manage-request-queues.md) Abschnitt. Informationen zum Erstellen von Anforderungen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).

* Die Warteschlangendetails in der Anforderungswarteschlange müssen die folgenden Einstellungen aufweisen:
   * **Wenn jemand eine Anfrage stellt, gewähren Sie automatisch** auf **Beitragszugriff**
   * **Status ändern** ist unter Erweiterte Einstellungen ausgewählt

   ![Mit den Warteschlangendetails können Sie festlegen, dass der Status &quot;Beitragszugriff&quot;und &quot;Änderungsstatus&quot;ausgewählt ist.](assets/queuedetails-contributeaccess-changestatus.png)

   Weitere Informationen zu Warteschlangendetails finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

* Das Problem muss sich im Status Auf Feedback warten befinden.
* Für Probleme auf Systemebene muss der Status Await Feedback (AWF) verfügbar sein.

   Weitere Informationen zu den Status auf Systemebene finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
