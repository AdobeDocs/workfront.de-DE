---
title: Überblick über Zugriffsebenen
user-type: administrator
content-type: reference
product-area: system-administration
keywords: Zugriff,Ebene,System,Admin,Standard,Light,Mitwirkende
navigation-topic: access-levels
description: Alle Benutzenden müssen über eine Zugriffsebene verfügen, um sich anmelden und in Workfront arbeiten zu können. Mithilfe der Zugriffsebene können Sie steuern, was Benutzende sehen und mit bestimmten Workfront-Objekten und -Bereichen tun können.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 627d59c8c8296e5b6c8b6da53705a1c3d7633751
workflow-type: tm+mt
source-wordcount: '1775'
ht-degree: 96%

---

# Überblick über Zugriffsebenen

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die aktuellen Zugriffsebenen. Informationen zu den alten Zugriffsebenen finden Sie unter [Überblick über Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Als Adobe Workfront-Admin weisen Sie einem Benutzer bzw. einer Benutzerin eine Zugriffsebene aus zwei Gründen zu:

* Alle Benutzenden müssen über eine Zugriffsebene verfügen, um sich anmelden und in Workfront arbeiten zu können.
* Mithilfe der Zugriffsebene können Sie steuern, was Benutzende sehen und mit bestimmten Workfront-Objekten und -Bereichen tun können.

## Neue integrierte Zugriffsebenen in Adobe Workfront {#built-in-access}

Workfront verfügt über fünf neue integrierte Zugriffsebenen:

* Systemadmin
* Standard
* Light
* Mitwirkende
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
>Es wird dringend empfohlen, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie sich nach der Einrichtung Ihrer Benutzenden darauf beziehen können.

### Zugriffsebene des Systemadmins

Diese integrierte Zugriffsebene ist mit der Standardlizenz verbunden und richtet sich an Benutzende, die für die Verwaltung des Adobe Workfront-Systems zuständig sind. Diese integrierte Zugriffsebene kann nicht geändert werden.

Benutzende mit der Zugriffsebene „Systemadmin“ können alle Funktionen in Workfront nutzen. Sie können alle Workfront-Objekte und -Informationen anzeigen und bearbeiten, die von allen anderen Benutzenden in Workfront eingegeben wurden.

Sie haben auch Zugriff auf den kompletten Setup-Bereich, wo sie jede Einstellung auf Systemebene ändern können, und sie können auf alle Bereiche im Hauptmenü zugreifen.

Weitere Informationen finden Sie unter [Gewähren des vollständigen Administratorzugriffs für Benutzende](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Zugriffsebene „Standard“

Diese Zugriffsebene ist auch an die Standardlizenz angefügt und richtet sich an Benutzende, die folgende Aktionen ausführen:

* Planen, Erstellen und Nachverfolgen aller Projekte an einem Ort
* Automatisieren von Routinevorgängen
* Verwalten von Ressourcen
* Nachverfolgen von und Zusammenarbeiten bei Anfragen
* Nachverfolgen und Erstellen von Berichten zu den Projektfinanzen
* Starten eingehender Arbeitsanfragen
* Zusammenarbeit an Projekten, Aufgaben und Problemen

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene „Standard“ erstellen und den Umfang des Zugriffs anpassen, den diese für die verschiedenen Workfront-Objekttypen zulässt. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Zugriffsebene „Standard“ verfügbar sind:

| Workfront-Objekttyp | Kein Zugriff | Zugriffsrecht „Anzeigen“ | Zugriffsrecht „Bearbeiten“ |
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
| Aufgabengebiete |   |   | ✓ |
| Teams |   |   | ✓ |
| Vorlagen |   |   | ✓ |
| Finanzdaten |   |   | ✓ |
| Ressourcen-Management |   |   | ✓ |
| Szenarienplaner |   |   | ✓ (Die Standardeinstellung ist „Kein Zugriff“.) |
| Ziele |   |   | ✓ |

{style="table-layout:auto"}

### Zugriffsebene „Light“

Diese Zugriffsebene ist Teil der Light-Lizenz und richtet sich an Benutzende, die folgende Aktionen ausführen:

* Anzeigen aller Elemente und Aktualisierungen im Zusammenhang mit der Arbeit
* Genehmigen von Projekten, Aufgaben und Problemen
* Anzeigen von Dashboards und Berichten
* Zeit für Projekte, Aufgaben und Probleme verfolgen und Arbeitszeittabellen genehmigen
* Erstellen und Verwalten von Problemen

Für Benutzende mit der Zugriffsebene „Light“ gilt Folgendes:

* Ihnen können Arbeitselementen zugewiesen werden, aber sie können diese nicht abschließen.
* Sie können im Hauptmenü auf Anfragen und Dokumente zugreifen.
* Sie haben eingeschränkte Möglichkeiten, Objekte zu erstellen. Sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.
* Die Zeit kann nur auf Projektebene protokolliert werden, wenn Bearbeitungszugriff aktiviert ist. Sie können keine Projekte erstellen, bearbeiten, löschen oder freigeben.
* Kann benutzerdefinierte Formulare nur zu Problemen und Dokumenten aktualisieren.

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene „Light“ erstellen und den Umfang der Zugriffsrechte für die verschiedenen Workfront-Objekttypen anpassen. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte in der Zugriffsebene „Light“ verfügbar sind:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront-Objekttyp</th> 
   <th>Kein Zugriff</th> 
   <th>Zugriffsrecht „Anzeigen“</th> 
   <th>Zugriffsrecht „Bearbeiten“</th> 
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
   <td>✓ (Die Standardeinstellung ist „Kein Zugriff“.)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist „Kein Zugriff“.)</td> 
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
   <td>Aufgabengebiete</td> 
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
   <td> <p>✓ (Die Standardeinstellung ist „Kein Zugriff“)</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ressourcen-Management</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Szenarienplaner </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist „Kein Zugriff“.)</td> 
  </tr>

<tr>   
   <td>Ziele </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist „Kein Zugriff“)</td> 
 </tbody> 
</table>

### Zugriffsebene „Mitwirkende“

Diese Zugriffsebene ist Teil der Lizenz für Mitwirkende und ist für Benutzende gedacht, die folgende Aktionen ausführen:

* Senden von Anfragen
* Nachverfolgen von Anfragen
* Aktualisieren und Überprüfen von Anfragen
* Genehmigen von Anfragen

Für Benutzende mit dieser integrierten Zugriffsebene gilt:

* Sie können Anfragen stellen und diese aktualisieren
* Sie können Dokumente hochladen und genehmigen
* Sie können Projekte, Aufgaben und Probleme genehmigen

  >[!NOTE]
  >
  >Mitwirkende können an Genehmigungen teilnehmen, aber nicht auf die Registerkarte „Genehmigungen“ zugreifen, um Genehmigungsvorgänge anzuzeigen oder zu verwalten.

* Sie können den Status der von ihnen gesendeten Probleme überprüfen
* Kann benutzerdefinierte Formulare nur zu Problemen und Dokumenten aktualisieren.
* Sie können Arbeitselementen zugewiesen werden, können diese aber nicht abschließen
* Sie können nur über das Hauptmenü auf Anfragen zugreifen. Weitere Informationen zu Anfrage-Warteschlangen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene „Mitwirkende“ erstellen und den Umfang des Zugriffs anpassen, den diese für die verschiedenen Workfront-Objekttypen zulässt. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Zugriffsebene „Mitwirkende“ verfügbar sind:

| Workfront-Objekttyp | Kein Zugriff | Zugriffsrecht „Anzeigen“ | Zugriffsrecht „Bearbeiten“ |
|---|---|---|---|
| Projekt |   | ✓ (eingeschränkt) |   |
| Aufgabe |   | ✓ (eingeschränkt) |   |
| Problem |   |   | ✓ |
| Portfolios |   | ✓ |   |
| Programme |   | ✓ |   |
| Berichte (einschließlich Dashboards und Kalenderberichte) |   | ✓ (Nur die Registerkarte „Details“) |   |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokument |   |   | ✓ |
| Benutzende |   | ✓ |   |
| Aufgabengebiete |   | ✓ |   |
| Teams |   | ✓ |   |
| Vorlagen | ✓ |   |   |
| Finanzdaten | ✓ |   |   |
| Ressourcen-Management | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Ziele |   |   | ✓ (Die Standardeinstellung ist „Kein Zugriff“) |

{style="table-layout:auto"}

>[!IMPORTANT]
>
>Ab Version 24.7 haben Mitwirkende standardmäßig das Zugriffsrecht „Anzeigen“ für Programme und Portfolios.
>
> 
>Mitwirkende, die vor Version 24.7 eingebunden wurden, haben standardmäßig weiterhin keinen Zugriff auf Programme und Portfolios. Sie können die Zugriffsrechte dieser Personen manuell auf „Anzeigen“ aktualisieren.

### Zugriffsebene „Externe Benutzende“

Diese Zugriffsebene ist nicht an eine kostenpflichtige Workfront-Lizenz gebunden. Hierbei handelt es sich um die restriktivste Zugriffsebene. Sie wurde in erster Linie für Mitarbeitende wie externe Berater und Beraterinnen entwickelt, die sich nicht bei Workfront anmelden, aber gelegentlich Dokumente überprüfen, herunterladen oder anzeigen müssen.

Für Benutzende mit der Zugriffsebene „Externe Benutzende“ gilt Folgendes:

* Sie können nur Dokumente und Kalenderberichte anzeigen, die für sie freigegeben sind
* Sie können die Benutzenden anzeigen, die Dokumente und Kalenderberichte für sie freigeben
* Sie können Dokumente genehmigen, die für sie freigegeben wurden

Externe Benutzende können Arbeitselementen nicht zugewiesen werden.

Sie können diese Zugriffsebene nicht ändern.

>[!IMPORTANT]
>
>Die Zugriffsebene „Externe Benutzende“ ist nur verfügbar, wenn die Option „Mit Personen ohne Workfront-Konten über deren E-Mail-Adresse zusammenarbeiten“ im Bereich „Systemeinstellungen“ im Setup aktiviert ist. Weitere Informationen finden Sie unter [Konfigurieren von Sicherheitseinstellungen für das System](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Zugriffsebene „Externe Benutzende“ verfügbar sind.

| Workfront-Objekttyp | Kein Zugriff | Zugriffsrecht „Anzeigen“ | Zugriffsrecht „Bearbeiten“ |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Aufgabe | ✓ |   |   |
| Problem | ✓ |   |   |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte (einschließlich Dashboards und Kalenderberichte) |   | ✓ (Nur für Kalenderberichte, keine Möglichkeit zur Freigabe von Berichten) |   |
| Filter, Ansichten und Gruppierungen | ✓ |   |   |
| Dokument |   | ✓ (Keine Möglichkeit zur Freigabe von Dokumenten) |   |
| Benutzende |   | ✓ |   |
| Aufgabengebiete | ✓ |   |   |
| Teams | ✓ |   |   |
| Vorlagen | ✓ |   |   |
| Finanzdaten | ✓ |   |   |
| Ressourcen-Management | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Ziele | ✓ |   |   |


## Zusammenarbeit zwischen Zugriffsebenen und Berechtigungen

Zugriffsebenen legen fest, was Benutzende bei allgemeinen Objekttypen und Bereichen im System, wie Projekten, Aufgaben und Problemen, sehen und damit tun können. Berechtigungen legen fest, worauf Sie bei bestimmten Objekten Zugriff haben, die von anderen Personen im System erstellt wurden. Dies kann beispielsweise ein Projekt zur Durchführung einer Marketing-Kampagne sein.

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

Die Aktivitäten, die Benutzende mit einem Objekt durchführen können, werden durch eine Kombination aus ihrer Zugriffsebene und den ihnen gewährten Berechtigungen definiert.

![Sicherheitsmodellhierarchie](assets/security-model-hierachy-copy.png)

### Erteilen von Berechtigungen über die Freigabe von Objekten

Benutzende erhalten Zugriff auf einzelne Objekte, wenn andere Benutzende bestimmte Berechtigungen für diese Objekte freigeben und gewähren.

>[!NOTE]
>
>* Wenn ein Benutzer bzw. eine Benutzerin ein Objekt mit bestimmten Berechtigungen teilt und dieses Objekt untergeordnete Objekte hat, übernimmt der Empfänger bzw. die Empfängerin dieselben Berechtigungen für diese untergeordneten Objekte.
>* Wenn eine Zugriffsebene Benutzende daran hindert, bestimmte Objekte zu löschen, verhindert dies nicht, dass sie untergeordnete Objekte löschen, die in diesen Objekten enthalten sind.

Ein Benutzer bzw. eine Benutzerin kann dem Empfänger bzw. der Empfängerin eine der folgenden Berechtigungen für das einzelne Objekt gewähren:

* **Anzeigen**: Mit dieser Berechtigungsstufe kann der Empfänger bzw. die Empfängerin das Objekt auf eine der folgenden Arten freigeben:

   * Systemweit, sodass alle Benutzenden es sehen können (nicht für alle Objekte verfügbar)
   * Für externe Benutzende, die keine Workfront-Lizenz haben (nicht für alle Objekte verfügbar)
   * Für eine E-Mail-Adresse (nur für Dokumente und Kalender verfügbar)

* **Mitwirken**: (nicht für alle Objekte verfügbar)
* **Verwalten**: Wenn jemand ein Objekt freigibt, werden die Rechte des Empfängers bzw. der Empfängerin am Objekt durch eine Kombination aus der Zugriffsebene der empfangenden Person und den von der freigebenden Person gewährten Berechtigungen für das Objekt bestimmt. Der niedrigste verfügbare Zugriffsgrad in dieser Kombination bestimmt, was der Empfänger bzw. die Empfängerin mit dem Objekt tun kann.

### Beispielszenarien

#### **Szenario 1**

Wenn die Zugriffsebene des Empfängers bzw. der Empfängerin die Projektbearbeitung nicht zulässt, kann diese Person ein Projekt nicht bearbeiten oder löschen, selbst wenn die freigebende Person die Berechtigung zur Verwaltung erteilt hat.

Wenn die Zugriffsebene des Empfängers bzw. der Empfängerin die Bearbeitung eines Projekts zulässt, die freigebende Person jedoch schreibgeschützte Berechtigungen für ein Projekt erteilt hat, kann der Benutzer bzw. die Benutzerin das Projekt nicht bearbeiten oder löschen.

#### **Szenario 2**

Wenn Olivia ein Workfront-Projekt für Tony freigibt, hängt es von einer Kombination aus zwei Dingen ab, welchen Zugriff Tony auf das Projekt hat:

* Die Zugriffsebene von Tony, zugewiesen durch den bzw. die Workfront-Admin
* Die Berechtigungen von Tony für das Projekt, angegeben von Olivia

Die Aktionen, die Tony am Projekt ausführen kann, können weiter eingeschränkt werden, Einschränkungen können jedoch nicht über das hinaus aufgehoben werden, was seine Zugriffsebene zulässt:

* Wenn seine Zugriffsebene es Tony nicht gestattet, Aufgaben zu erstellen, kann er keine Aufgaben zum Projekt hinzufügen, selbst wenn Olivia ihm die Berechtigung zum Hinzufügen von Aufgaben erteilt hat.
* Wenn seine Zugriffsebene es Tony gestattet, Aufgaben zu erstellen, Olivia jedoch keine Berechtigungen zum Hinzufügen von Aufgaben zu dem Projekt erteilt hat, kann er diesem Projekt keine Aufgaben hinzufügen, aber er kann Aufgaben zu anderen Projekten hinzufügen, für die ihm entsprechende Berechtigungen erteilt wurden.
