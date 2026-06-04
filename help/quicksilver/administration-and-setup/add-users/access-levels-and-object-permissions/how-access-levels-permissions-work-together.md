---
title: Zusammenarbeiten von alten Zugriffsebenen und Berechtigungen
user-type: administrator
content-type: reference
product-area: system-administration
keywords: Zugriff,Modell,funnel,Diagramm,Ebenen,Berechtigungen
navigation-topic: access-levels
description: Der Adobe Workfront-Administrator legt fest, welche Zugriffsebene jede Benutzerin bzw. jeder Benutzer haben soll. Diese Zugriffsebene definiert, was Benutzende mit Objekttypen und Bereichen im System sehen und tun können.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
TQID: https://experienceleague.adobe.com/yO-2iQdJUwZgAE93N-7Tqw3V8j3-JfYv0PrKohb-3o8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: d3382524-5489-431b-bde9-271ab257bc37
  - id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 908
ht-degree: 48%

---

# Zusammenarbeiten von alten Zugriffsebenen und Berechtigungen

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die alten Zugriffsebenen. Informationen zu den aktuellen Zugriffsebenen finden Sie unter [Überblick über die neuen Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Der Adobe Workfront-Administrator legt fest, welche Zugriffsebene jede Benutzerin bzw. jeder Benutzer haben soll. Diese Zugriffsebene definiert, was Benutzende mit Objekttypen und Bereichen im System sehen und tun können.

Benutzer erhalten auch Zugriff auf einzelne Objekte, wenn andere Benutzer bestimmte Berechtigungen für diese Objekte freigeben und gewähren.


![Sicherheitsmodellhierarchie](assets/security-model-hierachy.png)

Wenn Ihre Zugriffsebene beispielsweise besagt, dass Sie Aufgaben erstellen können, die Berechtigungen, die Sie für ein bestimmtes Projekt erhalten, jedoch nicht zulassen, dass Sie ihm Aufgaben hinzufügen, können Sie keine Aufgaben zum Projekt hinzufügen, obwohl Sie Aufgaben an einer anderen Stelle in Workfront erstellen können.

In diesem Artikel wird erläutert, wie diese Kombination funktioniert.

## Zugriffsebene

Die Zugriffsebene, die jedem Benutzer von einem Workfront-Administrator zugewiesen wurde, ist für die Anmeldung bei Workfront erforderlich.

Die standardmäßigen Zugriffsebenen sind:

* Systemadministrator (der Planlizenz beigefügt)
* Planer (der Planlizenz beigefügt)
* Worker (der Arbeitslizenz beigefügt)
* Reviewer (der Revisionslizenz beigefügt)
* Antragsteller (der Anfragelizenz beigefügt)
* Externer Benutzer (an die Lizenz für externe E-Mails angehängt)

Die Workfront-Lizenz für jede standardmäßige Zugriffsebene bestimmt, was auf der Zugriffsebene verfügbar und konfigurierbar ist. Informationen zu den Workfront-Lizenzen finden Sie unter [Adobe Workfront-Lizenzen - Übersicht](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Für die Benutzenden, die ihr zugewiesen sind, definiert eine Zugriffsebene, was sie mit den folgenden Objekttypen und Bereichen in Workfront sehen und tun können:

* Projekte
* Aufgaben
* Probleme
* Portfolios
* Berichte, Dashboards und Kalender
* Filter, Ansichten und Gruppierungen
* Dokumente
* Andere Benutzer
* Vorlagen
* Finanzielle Daten
* Ressourcenverwaltung
* Szenarienplaner
* Workfront-Ziele

In einer benutzerdefinierten Zugriffsebene können Sie die Einstellungen für diese Objekte und Bereiche konfigurieren, um zu ändern, wie viel Zugriff Benutzerinnen und Benutzer auf sie haben. Je nach der mit der Zugriffsebene verknüpften Lizenz sowie dem Typ des Objekts oder Bereichs können Sie die Zugriffsebene so konfigurieren, dass kein Zugriff auf ein Objekt oder Bereich zulässig ist, dass kein Zugriff angezeigt wird oder dass der Zugriff auf ein Objekt oder einen Bereich bearbeitet wird.

>[!IMPORTANT]
>
>Es wird dringend empfohlen, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie sich nach der Einrichtung Ihrer Benutzenden darauf beziehen können. Um eine Zugriffsebene anzupassen, kopieren Sie die standardmäßige Zugriffsebene und ändern Sie die Kopie. (Dies ist für jede Zugriffsebene möglich, mit Ausnahme von Systemadministrator und externem Benutzer.)

Eine ausführliche Erläuterung der Standardzugriffsebenen finden Sie unter [Integrierte Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Anweisungen zum Zuweisen einer Zugriffsebene zu einem Benutzer finden Sie unter [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Berechtigungen

Wenn ein Objekt für eine Person im System freigegeben wird, kann ein Benutzer dem Empfänger eine der folgenden Berechtigungen für das Objekt gewähren.

* **Anzeigen**: Mit dieser Berechtigungsstufe kann der Empfänger bzw. die Empfängerin das Objekt auf eine der folgenden Arten freigeben:

   * Systemweit, sodass alle Benutzenden es sehen können (nicht für alle Objekte verfügbar)
   * Für externe Benutzende, die keine Workfront-Lizenz haben (nicht für alle Objekte verfügbar)
   * Mit einer E-Mail-Adresse (nur für Dokumente verfügbar)

* **Mitwirken**: (nicht für alle Objekte verfügbar)
* **Verwalten**: Wenn jemand ein Objekt freigibt, werden die Rechte des Empfängers bzw. der Empfängerin am Objekt durch eine Kombination aus der Zugriffsebene der empfangenden Person und den von der freigebenden Person gewährten Berechtigungen für das Objekt bestimmt. Der niedrigste verfügbare Zugriffsgrad in dieser Kombination bestimmt, was der Empfänger bzw. die Empfängerin mit dem Objekt tun kann.

  >[!INFO]
  >
  >**Beispiel** Wenn die Zugriffsebene des Empfängers keine Projektbearbeitung zulässt, kann diese Person ein Projekt nicht bearbeiten oder löschen, selbst wenn der Teilende die Berechtigung zur Verwaltung erteilt hat.
  >
  >Wenn die Zugriffsebene des Empfängers bzw. der Empfängerin die Bearbeitung eines Projekts zulässt, die freigebende Person jedoch schreibgeschützte Berechtigungen für ein Projekt erteilt hat, kann der Benutzer bzw. die Benutzerin das Projekt nicht bearbeiten oder löschen.

In der folgenden Tabelle wird der allgemeine Zugriff eines Benutzers bzw. einer Benutzerin auf Objekte (definiert durch die Zugriffsebene der Benutzenden) mit den Berechtigungen für ein bestimmtes freigegebenes Objekt verglichen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Zugriffsebene </th> 
   <th>Berechtigungen </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Wird von einem Workfront-Admin in der Zugriffsebene eines Benutzers bzw. einer Benutzerin gewährt</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Wird durch einen Benutzer bzw. eine Benutzerin gewährt, der bzw. die ein Objekt auf Objektebene freigibt</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Wird von einem höherrangigen freigegebenen Objekt übernommen 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Wenn ein Benutzer bzw. eine Benutzerin ein Objekt mit bestimmten Berechtigungen teilt und dieses Objekt untergeordnete Objekte hat, übernimmt der Empfänger bzw. die Empfängerin dieselben Berechtigungen für diese untergeordneten Objekte.
>* Wenn eine Zugriffsebene Benutzende daran hindert, bestimmte Objekte zu löschen, verhindert dies nicht, dass sie untergeordnete Objekte löschen, die in diesen Objekten enthalten sind.
>

## Weitere Beispielszenarien

Wenn Olivia ein Workfront-Projekt für Tony freigibt, hängt es von einer Kombination aus zwei Dingen ab, welchen Zugriff Tony auf das Projekt hat:

* Die Zugriffsebene von Tony, zugewiesen durch den bzw. die Workfront-Admin
* Die Berechtigungen von Tony für das Projekt, angegeben von Olivia

Die Aktionen, die Tony am Projekt ausführen kann, können weiter eingeschränkt werden, Einschränkungen können jedoch nicht über das hinaus aufgehoben werden, was seine Zugriffsebene zulässt:

* Wenn seine Zugriffsebene es Tony nicht gestattet, Aufgaben zu erstellen, kann er keine Aufgaben zum Projekt hinzufügen, selbst wenn Olivia ihm die Berechtigung zum Hinzufügen von Aufgaben erteilt hat.
* Wenn seine Zugriffsebene es Tony gestattet, Aufgaben zu erstellen, Olivia jedoch keine Berechtigungen zum Hinzufügen von Aufgaben zu dem Projekt erteilt hat, kann er diesem Projekt keine Aufgaben hinzufügen, aber er kann Aufgaben zu anderen Projekten hinzufügen, für die ihm entsprechende Berechtigungen erteilt wurden.
