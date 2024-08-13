---
title: Funktionsweise von Zugriffsebenen und Berechtigungen
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,chart,levels,permissions
navigation-topic: access-levels
description: Der Adobe Workfront-Administrator legt fest, welche Zugriffsebene die einzelnen Benutzer haben sollen. Diese Zugriffsebene definiert, was Benutzer mit Objekttypen und -bereichen im System sehen und tun können.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 2%

---

# Wie Zugriffsebenen und Berechtigungen zusammenarbeiten

Der Adobe Workfront-Administrator legt fest, welche Zugriffsebene die einzelnen Benutzer haben sollen. Diese Zugriffsebene definiert, was Benutzer mit Objekttypen und -bereichen im System sehen und tun können.

Benutzer erhalten auch Zugriff auf einzelne Objekte, wenn andere Benutzer diese Objekte freigeben und bestimmte Berechtigungen gewähren.


![](assets/security-model-hierachy.png)

Wenn beispielsweise auf Ihrer Zugriffsebene angegeben wird, dass Sie Aufgaben erstellen können, die Berechtigungen für ein bestimmtes Projekt jedoch nicht erlauben, Aufgaben hinzuzufügen, können Sie keine Aufgaben zum Projekt hinzufügen, auch wenn Sie Aufgaben an anderer Stelle in Workfront erstellen können.

In diesem Artikel wird erläutert, wie diese Kombination funktioniert.

## Zugriffsebene

Die von einem Workfront-Administrator jedem Benutzer zugewiesene Zugriffsebene ist für die Anmeldung bei Workfront erforderlich.

Die standardmäßigen Zugriffsebenen sind:

* Systemadministrator (an die Planungslizenz angehängt)
* Planer (an die Planungslizenz angehängt)
* Arbeitnehmer (an die Work-Lizenz angehängt)
* Überprüfer (an die Überprüfungslizenz angehängt)
* Anforderer (an die Anforderungslizenz angehängt)
* Externer Benutzer (an die externe E-Mail-Lizenz angehängt)

Die Workfront-Lizenz für die einzelnen Standardzugriffsebenen bestimmt, welche Zugriffsebene verfügbar und konfigurierbar ist. Informationen zu den Workfront-Lizenzen finden Sie unter [Übersicht über Adobe Workfront-Lizenzen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Eine Zugriffsebene definiert für die Benutzer, die ihr zugewiesen sind, die folgenden Objekttypen und -bereiche in Workfront:

* Projekte
* Aufgaben
* Probleme
* Portfolios
* Berichte, Dashboards und Kalender
* Filter, Ansichten und Gruppierungen
* Dokumente
* Sonstige Benutzer
* Vorlagen
* Finanzielle Daten
* Ressourcenverwaltung
* Szenarienplaner
* Workfront-Ziele

Auf einer benutzerdefinierten Zugriffsebene können Sie die Einstellungen für diese Objekte und Bereiche konfigurieren, um zu ändern, wie viel Zugriff Benutzer darauf haben. Je nach der mit der Zugriffsebene verknüpften Lizenz sowie dem Typ des Objekts oder Bereichs können Sie die Zugriffsebene so konfigurieren, dass kein Zugriff möglich ist, Sie können den Zugriff anzeigen oder den Zugriff auf ein Objekt oder einen Bereich bearbeiten.

>[!IMPORTANT]
>
>Wir empfehlen dringend, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können. Um eine Zugriffsebene anzupassen, kopieren Sie die standardmäßige Zugriffsebene und ändern Sie die Kopie. (Sie können dies für jede Zugriffsstufe mit Ausnahme von &quot;Systemadministrator&quot;und &quot;Externer Benutzer&quot;tun.)

Eine ausführliche Erläuterung der einzelnen Standardzugriffsebenen finden Sie unter [Integrierte Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Anweisungen zum Zuweisen einer Zugriffsebene zu einem Benutzer finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Berechtigungen

Beim Freigeben eines Objekts für eine Person im System kann ein Benutzer dem Empfänger eine der folgenden Berechtigungen für das Objekt gewähren.

* **Ansicht**: Diese Berechtigungsebene ermöglicht es dem Empfänger, das Objekt auf eine der folgenden Arten freizugeben:

   * Systemweit, damit alle Benutzer ihn sehen können (nicht für alle Objekte verfügbar)
   * Bei externen Benutzern ohne Workfront-Lizenz (nicht für alle Objekte verfügbar)
   * Mit einer E-Mail-Adresse (nur für Dokumente verfügbar)

* **Contribute**: (nicht für alle Objekte verfügbar)
* **Verwalten**: Wenn jemand ein Objekt freigegeben, werden die Rechte des Empfängers für das Objekt durch eine Kombination aus der Zugriffsebene des Empfängers und den Berechtigungen für das Objekt bestimmt, die vom Freigebende erteilt wurden. Der geringste in dieser Kombination verfügbare Zugriff bestimmt, was der Empfänger mit dem Objekt tun kann.

  >[!INFO]
  >
  >**Beispiel:** Wenn die Zugriffsebene des Empfängers die Bearbeitung von Projekten nicht zulässt, kann diese Person ein Projekt nicht bearbeiten oder löschen, selbst wenn der Freigebende die Berechtigung zur Verwaltung erteilt hat.
  >
  >Oder wenn die Zugriffsebene des Empfängers die Bearbeitung von Projekten zulässt, der freigebende Benutzer jedoch schreibgeschützte Berechtigungen für ein Projekt erteilt hat, kann der Benutzer das Projekt nicht bearbeiten oder löschen.

In der folgenden Tabelle wird der allgemeine Zugriff eines Benutzers auf Objekte (definiert durch die Zugriffsebene des Benutzers) mit Berechtigungen für ein bestimmtes freigegebenes Objekt verglichen:

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
   <td>Von einem Workfront-Administrator auf Zugriffsebene eines Benutzers gewährt</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Wird von einem Benutzer gewährt, der ein Objekt auf Objektebene teilt</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Von einem übergeordneten freigegebenen Objekt geerbt 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Wenn ein Benutzer ein Objekt mit bestimmten Berechtigungen teilt und dieses Objekt untergeordnete Objekte darunter hat, erbt der Empfänger dieselben Berechtigungen für diese untergeordneten Objekte.
>* Wenn eine Zugriffsebene Benutzer daran hindert, bestimmte Objekte zu löschen, hindert dies sie nicht daran, untergeordnete Objekte zu löschen, die in diesen Objekten enthalten sind.
>

## Weitere Beispielszenarien

Wenn Olivia ein Workfront-Projekt mit Tony teilt, wird Tony sein Zugang dazu durch eine Kombination zweier Dinge bestimmt:

* Tony&#39;s Access Level, vom Workfront-Administrator zugewiesen
* Tonys Berechtigungen für das Projekt, spezifiziert von Olivia

Tonys Maßnahmen in Bezug auf das Projekt können weiter auf das Projekt beschränkt werden, doch dürfen sie nicht über das auf seiner Zugangsstufe zulässige Maß hinausgehen:

* Wenn Tony&#39;s Zugangsstufe ihm nicht erlaubt, Aufgaben zu erstellen, kann er dem Projekt keine Aufgaben hinzufügen, selbst wenn Olivia ihm die Berechtigung erteilt hat, ihm Aufgaben hinzuzufügen.
* Wenn Tony&#39;s Zugriffsebene es ihm ermöglicht, Aufgaben zu erstellen, aber Olivia keine Berechtigungen erteilt hat, Aufgaben zum Projekt hinzuzufügen, kann er diesem Projekt keine Aufgaben hinzufügen, aber er kann Aufgaben zu anderen Projekten hinzufügen, für die ihm entsprechende Berechtigungen erteilt wurden.
