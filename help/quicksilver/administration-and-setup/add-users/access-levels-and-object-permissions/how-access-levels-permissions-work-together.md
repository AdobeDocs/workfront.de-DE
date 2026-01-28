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
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 2%

---

# Zusammenarbeiten von alten Zugriffsebenen und Berechtigungen

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die alten Zugriffsebenen. Informationen zu den aktuellen Zugriffsebenen finden Sie unter [Übersicht über neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

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
>Es wird dringend empfohlen, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können. Um eine Zugriffsebene anzupassen, kopieren Sie die standardmäßige Zugriffsebene und ändern Sie die Kopie. (Dies ist für jede Zugriffsebene möglich, mit Ausnahme von Systemadministrator und externem Benutzer.)

Eine ausführliche Erläuterung der Standardzugriffsebenen finden Sie unter [Integrierte Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Anweisungen zum Zuweisen einer Zugriffsebene zu einem Benutzer finden Sie unter [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Berechtigungen

Wenn ein Objekt für eine Person im System freigegeben wird, kann ein Benutzer dem Empfänger eine der folgenden Berechtigungen für das Objekt gewähren.

* **Ansicht**: Mit dieser Berechtigungsstufe kann der Empfänger das Objekt auf eine der folgenden Arten freigeben:

   * Systemweit, sodass alle Benutzer es sehen können (nicht für alle Objekte verfügbar)
   * Bei externen Benutzern, die keine Workfront-Lizenz haben (nicht für alle Objekte verfügbar)
   * Mit einer E-Mail-Adresse (nur für Dokumente verfügbar)

* **Contribute**: (nicht für alle Objekte verfügbar)
* **Verwalten**: Wenn jemand ein Objekt freigibt, werden die Rechte des Empfängers am Objekt durch eine Kombination aus der Zugriffsebene des Empfängers und den vom Teilenden gewährten Berechtigungen für das Objekt bestimmt. Der niedrigste verfügbare Zugriffsgrad in dieser Kombination bestimmt, was der Empfänger mit dem Objekt tun kann.

  >[!INFO]
  >
  >**Beispiel** Wenn die Zugriffsebene des Empfängers keine Projektbearbeitung zulässt, kann diese Person ein Projekt nicht bearbeiten oder löschen, selbst wenn der Teilende die Berechtigung zur Verwaltung erteilt hat.
  >
  >Wenn die Zugriffsebene des Empfängers die Bearbeitung eines Projekts zulässt, der freigebende Benutzer jedoch schreibgeschützte Berechtigungen für ein Projekt erteilt hat, kann der Benutzer das Projekt nicht bearbeiten oder löschen.

In der folgenden Tabelle wird der allgemeine Zugriff eines Benutzers auf Objekte (definiert durch die Zugriffsebene des Benutzers) mit den Berechtigungen für ein bestimmtes freigegebenes Objekt verglichen:

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
   <td>Wird von einem Workfront-Administrator in der Zugriffsebene eines Benutzers gewährt</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Wird von einem Benutzer erteilt, der ein Objekt auf der Objektebene teilt</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Von einem höherrangigen freigegebenen Objekt geerbt 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Wenn ein Benutzer ein Objekt mit bestimmten Berechtigungen teilt und dieses Objekt untergeordnete Objekte hat, erbt der Empfänger dieselben Berechtigungen für diese untergeordneten Objekte.
>* Wenn eine Zugriffsebene Benutzer daran hindert, bestimmte Objekte zu löschen, verhindert dies nicht, dass sie untergeordnete Objekte löschen, die in diesen Objekten enthalten sind.
>

## Weitere Beispielszenarien

Wenn Olivia ein Workfront-Projekt mit Tony teilt, wird Tonys Zugang dazu durch eine Kombination zweier Dinge bestimmt:

* Tony&#39;s access level, zugewiesen von der Workfront-Administratorin bzw. dem -Administrator
* Tonys Berechtigungen für das Projekt, angegeben von Olivia

Tonys Aktionen im Projekt können im Projekt weiter eingeschränkt werden, sie können jedoch nicht über die auf seiner Zugriffsebene erlaubte Zugriffsebene hinausgehen:

* Wenn Tonys Zugriffsebene ihm nicht erlaubt, Aufgaben zu erstellen, kann er keine Aufgaben zum Projekt hinzufügen, selbst wenn Olivia ihm die Berechtigung zum Hinzufügen von Aufgaben erteilt hat.
* Wenn Tonys Zugriffsebene es ihm erlaubt, Aufgaben zu erstellen, Olivia jedoch keine Berechtigungen zum Hinzufügen von Aufgaben zu dem Projekt erteilt hat, kann er keine Aufgaben zu diesem Projekt hinzufügen, aber er kann Aufgaben zu anderen Projekten hinzufügen, für die ihm entsprechende Berechtigungen erteilt wurden.
