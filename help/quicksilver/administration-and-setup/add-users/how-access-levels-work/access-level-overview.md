---
title: Übersicht über Zugriffsebenen
user-type: administrator
content-type: reference
product-area: system-administration
keywords: Zugriff,Ebene,System,Administrator,Standard,Licht,Mitwirkende
navigation-topic: access-levels
description: Jeder Benutzer muss über eine Zugriffsebene verfügen, um sich anmelden und in Workfront arbeiten zu können. Mithilfe der Zugriffsebene können Sie steuern, was ein Benutzer mit bestimmten Workfront-Objekten und -Bereichen sehen und machen kann.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1747'
ht-degree: 6%

---

# Übersicht über Zugriffsebenen

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die aktuellen Zugriffsebenen. Informationen zu den alten Zugriffsebenen finden Sie unter [Zugriffsebenen - Übersicht](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Als Adobe Workfront-Administrator weisen Sie einem Benutzer eine Zugriffsebene zu zwei Zwecken zu:

* Jeder Benutzer muss über eine Zugriffsebene verfügen, um sich anmelden und in Workfront arbeiten zu können.
* Mithilfe der Zugriffsebene können Sie steuern, was ein Benutzer mit bestimmten Workfront-Objekten und -Bereichen sehen und machen kann.

## Neue integrierte Zugriffsebenen in Adobe Workfront {#built-in-access}

Workfront verfügt über fünf neue integrierte Zugriffsebenen:

* Systemadministrator
* Standard
* Leicht
* Mitwirkender oder Mitwirkende
* Extern

Je nach Zugriffsebene sind für die meisten Workfront-Objekttypen bis zu drei Berechtigungen verfügbar:

<table style="table-layout:auto">
    <tr>
        <td>Bearbeiten</td>
        <td>Benutzende können das Workfront-Objekt erstellen, bearbeiten, löschen und freigeben</td>
    </tr>
    <tr>
        <td>Ansicht</td>
        <td>Benutzende können das Workfront-Objekt überprüfen und freigeben</td>
    </tr>
    <tr>
        <td>Kein Zugriff</td>
        <td>Benutzende können nicht auf das Workfront-Objekt zugreifen</td>
    </tr>
</table>

Wenn Sie eine benutzerdefinierte Zugriffsebene benötigen, können Sie die integrierte Zugriffsebene kopieren und den gewünschten Zugriffsbereich an die verschiedenen Workfront-Objekttypen anpassen. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Es wird dringend empfohlen, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können.

### Zugriffsebene des Systemadministrators

Diese integrierte Zugriffsebene ist mit der Standardlizenz verbunden und richtet sich an Benutzende, die für die Verwaltung des Adobe Workfront-Systems zuständig sind. Diese integrierte Zugriffsebene kann nicht geändert werden.

Benutzende mit der Zugriffsebene „Systemadministrator“ können alles in Workfront tun. Sie können alle Workfront-Objekte und -Informationen anzeigen und bearbeiten, die von allen anderen Benutzenden in Workfront eingegeben wurden.

Sie haben auch Zugriff auf den kompletten Setup-Bereich, wo sie jede Einstellung auf Systemebene ändern können, und sie können auf alle Bereiche im Hauptmenü zugreifen.

Weitere Informationen finden Sie unter [Gewähren des vollständigen Administratorzugriffs für einen Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Standard-Zugriffsebene

Diese Zugriffsebene ist auch an die Standardlizenz angehängt und richtet sich an Benutzer, die:

* Alle Projekte an einem Ort planen, erstellen und verfolgen
* Automatisieren von Routineprozessen
* Verwalten von Ressourcen
* Nachverfolgen und Zusammenarbeiten bei Anfragen
* Verfolgen und Erstellen von Berichten zu den Projektfinanzen
* Starten eingehender Arbeitsaufträge
* Zusammenarbeit bei Projekten, Aufgaben und Problemen

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der standardmäßigen integrierten Zugriffsebene erstellen und den Umfang des Zugriffs anpassen, den diese für die verschiedenen Workfront-Objekttypen zulässt. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Standardzugriffsebene verfügbar sind:

| Workfront-Objekttyp | Kein Zugriff | Ansichtszugriff | Zugriff bearbeiten |
|---|---|---|---|
| Projekte |   |   | ✓ |
| Aufgaben |   |   | ✓ |
| Probleme |   |   | ✓ |
| Portfolios |   |   | ✓ |
| Programme |   |   | ✓ |
| Berichte (einschließlich Dashboards und Kalenderberichte) |   |   | ✓ |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokumente |   |   | ✓ |
| Benutzende |   |   | ✓ |
| Vorlagen |   |   | ✓ |
| Finanzdaten |   |   | ✓ |
| Ressourcenverwaltung |   |   | ✓ |
| Szenarienplaner |   |   | ✓ (Die Standardeinstellung ist Kein Zugriff.) |
| Ziele |   |   | ✓ |

{style="table-layout:auto"}

### Lichteingangsebene

Diese Zugriffsebene ist an die Light-Lizenz angehängt und richtet sich an Benutzende, die:

* Alle Elemente und Aktualisierungen im Zusammenhang mit der Arbeit anzeigen
* Projekte, Aufgaben und Probleme genehmigen
* Anzeigen von Dashboards und Berichten
* Zeit für Projekte, Aufgaben und Probleme verfolgen und Arbeitszeittabellen genehmigen
* Probleme erstellen und verwalten

Benutzende mit der Zugriffsebene Light:

* Kann Arbeitselementen zugewiesen werden, sie können jedoch nicht abgeschlossen werden.
* Kann im Hauptmenü auf Anfragen und Dokumente zugreifen.
* Die Möglichkeit, Objekte zu erstellen, ist eingeschränkt. Sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.
* Die Zeit kann nur auf Projektebene protokolliert werden, wenn Bearbeitungszugriff aktiviert ist. Sie können keine Projekte erstellen, bearbeiten, löschen oder freigeben.

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene Light erstellen und den Zugriffsbereich für die verschiedenen Workfront-Objekttypen anpassen. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte in der Zugriffsebene „Licht“ verfügbar sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront-Objekttyp</th> 
   <th>Kein Zugriff</th> 
   <th>Ansichtszugriff</th> 
   <th>Zugriff bearbeiten</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekte</td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (für die Protokollierung der Zeit auf Projektebene)</td> 
  </tr> 
  <tr> 
   <td>Aufgaben</td> 
   <td> </td> 
   <td></td> 
   <td>✓ (eingeschränkt)</td> 
  </tr> 
  <tr> 
   <td>Probleme</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist Kein Zugriff.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist Kein Zugriff.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Berichte (einschließlich Dashboards und Kalenderberichte)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filter, Ansichten und Gruppierungen</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokumente</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Benutzende</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
    <tr> 
   <td>Teams</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr>
  <tr> 
   <td>Vorlagen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Finanzdaten</td> 
   <td></td> 
   <td> <p>✓(Standardeinstellung ist Kein Zugriff)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ressourcenverwaltung</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Szenarienplaner </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist Kein Zugriff.)</td> 
  </tr>

<tr>   
   <td>Ziele </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Standardeinstellung ist Kein Zugriff)</td> 
 </tbody> 
</table>

### Zugriffsebene des oder der Mitwirkenden

Diese Zugriffsebene ist der Lizenz für Mitwirkende beigefügt und ist für Benutzende gedacht, die:

* Anfragen senden
* Anforderungen tracken
* Aktualisierungs- und Überprüfungsanfragen
* Anfragen genehmigen

Benutzende mit dieser integrierten Zugriffsebene:

* Kann Anfragen stellen und diese aktualisieren
* Kann Dokumente hochladen und genehmigen
* Kann Projekte, Aufgaben und Probleme genehmigen

  >[!NOTE]
  >
  >Mitwirkende können an Genehmigungen teilnehmen, aber nicht auf die Registerkarte Genehmigungen zugreifen, um Genehmigungsprozesse anzuzeigen oder zu verwalten.

* Kann den Status der von ihnen gesendeten Probleme überprüfen
* Kann Arbeitselementen zugewiesen, aber nicht abgeschlossen werden
* Zugriff auf Anfragen nur über das Hauptmenü möglich. Weitere Informationen zu Anfrage-Warteschlangen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene von Mitwirkenden erstellen und den Umfang des Zugriffs anpassen, den sie für die verschiedenen Workfront-Objekttypen zulässt. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Zugriffsebene Mitwirkende verfügbar sind:

| Workfront-Objekttyp | Kein Zugriff | Ansichtszugriff | Zugriff bearbeiten |
|---|---|---|---|
| Projekt |   | ✓ (eingeschränkt) |   |
| Aufgabe |   | ✓(eingeschränkt) |   |
| Problem |   |   | ✓ |
| Portfolios |   | ✓ |   |
| Programme |   | ✓ |   |
| Berichte (einschließlich Dashboards und Kalenderberichte) |   | ✓ (Nur die Registerkarte Details ) |   |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokument |   |   | ✓ |
| Benutzerin oder Benutzer |   | ✓ |   |
| Teams |   | ✓ |   |
| Vorlagen | ✓ |   |   |
| Finanzdaten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Ziele |   |   | ✓ (Standardeinstellung ist Kein Zugriff) |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Ab Version 24.7 haben Mitwirkende standardmäßig Ansichtszugriff auf Programme und Portfolios.
>
> 
>Mitwirkende, die vor Version 24.7 eingebunden wurden, haben standardmäßig weiterhin keinen Zugriff auf Programme und Portfolios. Sie können den Zugriff dieser Personen auf die Anzeige bei Bedarf manuell aktualisieren.

### Zugriffsebene externer Benutzer

Diese Zugriffsebene ist nicht an eine gebührenpflichtige Workfront-Lizenz gebunden. Hierbei handelt es sich um die restriktivste Zugriffsebene. Sie wurde in erster Linie für Mitarbeiter wie externe Berater entwickelt, die sich nicht bei Workfront anmelden, aber Dokumente gelegentlich überprüfen, herunterladen oder anzeigen müssen.

Benutzer mit der Zugriffsebene Externer Benutzer:

* Kann nur Dokumente und Kalenderberichte anzeigen, die für sie freigegeben sind
* Anzeigen der Benutzer, die Dokumente und Kalenderberichte für sie freigeben
* Dokumente genehmigen, die für sie freigegeben wurden

Externe Benutzer können Arbeitselementen nicht zugewiesen werden.

Diese Zugriffsebene kann nicht geändert werden.

>[!IMPORTANT]
>
>Externer Benutzer ist nur verfügbar, wenn die Option „Mit Personen ohne Workfront-Konten über deren E-Mail-Adresse zusammenarbeiten“ im Bereich „Systemeinstellungen“ im Setup aktiviert ist. Weitere Informationen finden Sie unter [Systemsicherheitseinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Zugriffsebene Externer Benutzer verfügbar sind.

| Workfront-Objekttyp | Kein Zugriff | Ansichtszugriff | Zugriff bearbeiten |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Aufgabe | ✓ |   |   |
| Problem | ✓ |   |   |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte (einschließlich Dashboards und Kalenderberichte) |   | ✓ (Nur für Kalenderberichte, keine Möglichkeit zur Freigabe von Berichten) |   |
| Filter, Ansichten und Gruppierungen | ✓ |   |   |
| Dokument |   | ✓ (keine Möglichkeit zur Freigabe von Dokumenten) |   |
| Benutzerin oder Benutzer |   | ✓ |   |
| Teams | ✓ |   |   |
| Vorlagen | ✓ |   |   |
| Finanzdaten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Ziele | ✓ |   |   |


## Zusammenarbeiten von Zugriffsebenen und Berechtigungen

Zugriffsebenen definieren, was Benutzer mit allgemeinen Objekttypen und Bereichen im System, wie Projekten, Aufgaben und Problemen, sehen und machen können. Berechtigungen definieren, auf was Sie Zugriff haben auf bestimmte Objekte, die von anderen Personen im System erstellt wurden, wie ein Projekt, das zum Ausführen einer Marketing-Kampagne erstellt wurde.

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

Die Aktivitäten, die ein Benutzer mit einem Objekt durchführen kann, werden durch eine Kombination aus seiner Zugriffsebene und den ihm gewährten Berechtigungen definiert.

![Sicherheitsmodellhierarchie](assets/security-model-hierachy-copy.png)

### Berechtigungen über die Freigabe von Objekten erteilen

Benutzer erhalten Zugriff auf einzelne Objekte, wenn andere Benutzer bestimmte Berechtigungen für diese Objekte freigeben und gewähren.

>[!NOTE]
>
>* Wenn ein Benutzer ein Objekt mit bestimmten Berechtigungen teilt und dieses Objekt untergeordnete Objekte hat, erbt der Empfänger dieselben Berechtigungen für diese untergeordneten Objekte.
>* Wenn eine Zugriffsebene Benutzer daran hindert, bestimmte Objekte zu löschen, verhindert dies nicht, dass sie untergeordnete Objekte löschen, die in diesen Objekten enthalten sind.

Ein Benutzer kann dem Empfänger eine der folgenden Berechtigungen für das einzelne Objekt gewähren:

* **Ansicht**: Mit dieser Berechtigungsstufe kann der Empfänger das Objekt auf eine der folgenden Arten freigeben:

   * Systemweit, sodass alle Benutzer es sehen können (nicht für alle Objekte verfügbar)
   * Bei externen Benutzern, die keine Workfront-Lizenz haben (nicht für alle Objekte verfügbar)
   * Mit einer E-Mail-Adresse (nur für Dokumente und Kalender verfügbar)

* **Contribute**: (nicht für alle Objekte verfügbar)
* **Verwalten**: Wenn jemand ein Objekt freigibt, werden die Rechte des Empfängers am Objekt durch eine Kombination aus der Zugriffsebene des Empfängers und den vom Teilenden gewährten Berechtigungen für das Objekt bestimmt. Der niedrigste verfügbare Zugriffsgrad in dieser Kombination bestimmt, was der Empfänger mit dem Objekt tun kann.

### Beispielszenarien

#### **Szenario 1**

Wenn die Zugriffsebene des Empfängers die Projektbearbeitung nicht zulässt, kann diese Person ein Projekt nicht bearbeiten oder löschen, selbst wenn der Teilende die Berechtigung zur Verwaltung erteilt hat.

Wenn die Zugriffsebene des Empfängers die Bearbeitung eines Projekts zulässt, der freigebende Benutzer jedoch schreibgeschützte Berechtigungen für ein Projekt erteilt hat, kann der Benutzer das Projekt nicht bearbeiten oder löschen.

#### **Szenario 2**

Wenn Olivia ein Workfront-Projekt mit Tony teilt, wird Tonys Zugang dazu durch eine Kombination zweier Dinge bestimmt:

* Tony&#39;s access level, zugewiesen von der Workfront-Administratorin bzw. dem -Administrator
* Tonys Berechtigungen für das Projekt, angegeben von Olivia

Tonys Aktionen im Projekt können im Projekt weiter eingeschränkt werden, sie können jedoch nicht über die auf seiner Zugriffsebene erlaubte Zugriffsebene hinausgehen:

* Wenn Tonys Zugriffsebene ihm nicht erlaubt, Aufgaben zu erstellen, kann er keine Aufgaben zum Projekt hinzufügen, selbst wenn Olivia ihm die Berechtigung zum Hinzufügen von Aufgaben erteilt hat.
* Wenn Tonys Zugriffsebene es ihm erlaubt, Aufgaben zu erstellen, Olivia jedoch keine Berechtigungen zum Hinzufügen von Aufgaben zu dem Projekt erteilt hat, kann er keine Aufgaben zu diesem Projekt hinzufügen, aber er kann Aufgaben zu anderen Projekten hinzufügen, für die ihm entsprechende Berechtigungen erteilt wurden.
