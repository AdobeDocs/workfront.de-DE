---
title: Übersicht über die neuen Zugriffsebenen
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,level,system,administrator,standard,light,contributor
navigation-topic: access-levels
description: Jeder Benutzer muss über eine Zugriffsstufe verfügen, um sich in Workfront anmelden und arbeiten zu können. Mit der Zugriffsebene können Sie steuern, was ein Benutzer mit bestimmten Workfront-Objekten und -Bereichen sehen und tun kann.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d297d8a4-5a4e-418f-983a-19545aeb0668
source-git-commit: 681d3b74eec1388f3b6cc7edf51422e0019cc318
workflow-type: tm+mt
source-wordcount: '1636'
ht-degree: 4%

---

# Übersicht über die neuen Zugriffsebenen

Als Adobe Workfront-Administrator weisen Sie einem Benutzer für zwei Zwecke eine Zugriffsstufe zu:

* Jeder Benutzer muss über eine Zugriffsstufe verfügen, um sich in Workfront anmelden und arbeiten zu können.
* Mit der Zugriffsebene können Sie steuern, was ein Benutzer mit bestimmten Workfront-Objekten und -Bereichen sehen und tun kann.

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
        <td>Benutzer können das Workfront-Objekt erstellen, bearbeiten, löschen und freigeben</td>
    </tr>
    <tr>
        <td>Anzeigen</td>
        <td>Benutzer können das Workfront-Objekt überprüfen und freigeben</td>
    </tr>
    <tr>
        <td>Kein Zugriff</td>
        <td>Benutzer können nicht auf das Workfront-Objekt zugreifen</td>
    </tr>
</table>

Wenn Sie eine benutzerdefinierte Zugriffsebene benötigen, können Sie die integrierte Zugriffsebene kopieren und die gewünschte Zugriffsmenge entsprechend den verschiedenen Workfront-Objekttypen anpassen. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Wir empfehlen dringend, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können.

### Zugriffsstufe für Systemadministrator

Diese integrierte Zugriffsstufe, die an die Standardlizenz angehängt ist, wurde für einen Benutzer entwickelt, der für die Verwaltung des Adobe Workfront-Systems zuständig ist. Sie können diese integrierte Zugriffsebene nicht ändern.

Benutzer mit der Zugriffsebene &quot;Systemadministrator&quot;können alles in Workfront tun. Sie können alle Workfront-Objekte und Informationen anzeigen und bearbeiten, die von allen anderen Benutzern in Workfront eingegeben wurden.

Sie haben außerdem Zugriff auf den gesamten Bereich &quot;Setup&quot;, in dem sie jede Einstellung auf Systemebene ändern können und auf alle Bereiche im Hauptmenü zugreifen können.

Weitere Informationen finden Sie unter [Gewähren eines vollen Administratorzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

### Standardzugriffsstufe

Diese Zugriffsstufe, die ebenfalls mit der Standardlizenz verbunden ist, richtet sich an Benutzer, die:

* Alle Projekte an einem Ort planen, erstellen und verfolgen
* Automatisieren von Routineprozessen
* Ressourcen verwalten
* Tracking und Zusammenarbeit bei Anforderungen
* Verfolgen und Berichte zu den Projektfinanzen
* Starten eingehender Arbeitsanfragen
* Zusammenarbeit bei Projekten, Aufgaben und Problemen

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der integrierten Standard-Zugriffsebene erstellen und den Umfang des Zugriffs anpassen, der dies für die verschiedenen Workfront-Objekttypen zulässt. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte in der Zugriffsebene &quot;Standard&quot;:

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekte |   |   | ✓ |
| Aufgaben |   |   | ✓ |
| Probleme |   |   | ✓ |
| Portfolios |   |   | ✓ |
| Programme |   |   | ✓ |
| Berichte (einschließlich Dashboards und Kalenderberichten) |   |   | ✓ |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokumente |   |   | ✓ |
| Benutzende |   |   | ✓ |
| Vorlagen |   |   | ✓ |
| Finanzdaten |   |   | ✓ |
| Ressourcenverwaltung |   |   | ✓ |
| Szenarienplaner |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |
| Pinnwände |   |   | ✓ |
| Startseite |   |   | ✓ |
| Ziele |   |   | ✓ |

{style="table-layout:auto"}

### Geringfügige Zugangsstufe

Diese Zugriffsstufe ist an die Light-Lizenz angehängt und richtet sich an Benutzer, die:

* Alle Elemente und Updates anzeigen, die für die Arbeit erforderlich sind
* Projekte, Aufgaben und Probleme genehmigen
* Anzeigen von Dashboards und Berichten
* Zeitverlauf verfolgen und Timesheets genehmigen
* Erstellen und Verwalten von Problemen
* Aktualisierungen der Arbeit vornehmen

Benutzer mit der Zugriffsebene Light :

* Arbeitselemente können zugewiesen werden, können jedoch nicht abgeschlossen werden.
* Kann auf Anfragen und Dokumente im Hauptmenü zugreifen.
* Sie haben nur begrenzte Möglichkeiten, Objekte zu erstellen - sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene von Light erstellen und den Umfang des Zugriffs anpassen, der dies für die verschiedenen Workfront-Objekttypen zulässt. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte in der Zugriffsebene für Light :

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Workfront-Objekttyp</th> 
   <th>Kein Zugriff</th> 
   <th>Zugriff anzeigen</th> 
   <th>Zugriff bearbeiten</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekte</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgaben</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
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
   <td>✓ (Die Standardeinstellung ist "Kein Zugriff".)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Programme</td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist "Kein Zugriff".)</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Berichte (einschließlich Dashboards und Kalenderberichten)</td> 
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
   <td>✓</td> 
   <td> <p> </p> </td> 
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
   <td>✓ (Die Standardeinstellung ist "Kein Zugriff".)</td> 
  </tr> 
  <tr> 
   <td>Pinnwände </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
     <tr> 
   <td>Startseite </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr>   
   <td>Ziele </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
 </tbody> 
</table>

### Beitragende-Zugriffsebene

Diese Zugriffsstufe ist an die Mitarbeiter-Lizenz angehängt und richtet sich an Benutzer, die:

* Anfragen senden
* Anforderungen verfolgen
* Anforderungen aktualisieren und überprüfen
* Anforderungen genehmigen

Benutzer mit dieser integrierten Zugriffsstufe:

* Kann Anforderungen stellen und diese Anforderungen aktualisieren
* Dokumente hochladen und genehmigen können
* Kann den Status der von ihnen eingereichten Probleme überprüfen
* Arbeitselemente können zugewiesen werden, sie jedoch nicht abschließen
* Kann nur über das Hauptmenü auf Anfragen zugreifen. Weitere Informationen zu Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

>[!NOTE]
>
>Sie können eine benutzerdefinierte Version der integrierten Zugriffsstufe des Contributors erstellen und die zulässige Zugriffsmenge für die verschiedenen Workfront-Objekttypen anpassen. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte auf der Ebene des Contributor-Zugriffs:

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekt |   | ✓ (nur die Seite &quot;Projektdetails&quot;) |   |
| Aufgabe |   | ✓ (nur die Detailseite) |   |
| Problem |   |   | ✓ |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte (einschließlich Dashboards und Kalenderberichten) |   | ✓ (Registerkarte &quot;Nur Details&quot;) |   |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokument |   |   | ✓ |
| Benutzerin oder Benutzer |   | ✓ |   |
| Teams |   | ✓ |   |
| Vorlage | ✓ |   |   |
| Finanzdaten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Pinnwände |   |   | ✓ (einfache Karten) |
| Startseite |   | ✓ (Meine Aktualisierungen) |   |
| Ziele |   |   | ✓ |

{style="table-layout:auto"}

### Zugriffsstufe für externe Benutzer

Diese Zugriffsstufe ist nicht an eine gebührenpflichtige Workfront-Lizenz gebunden. Es handelt sich dabei um die restriktivste Zugriffsstufe, die hauptsächlich für Mitarbeiter wie externe Berater konzipiert ist, die sich nicht bei Workfront anmelden, aber gelegentlich Dokumente überprüfen, herunterladen oder anzeigen müssen.

Workfront-Benutzer können externen Benutzern Aufgaben zuweisen, auch wenn sich externe Benutzer nicht beim System anmelden können. Aber wir raten davon ab, weil diese Arbeit im System noch nicht gelöst sein würde.

Benutzer mit der Zugriffsebene &quot;Externer Benutzer&quot;:

* Kann nur Dokumente und Kalenderberichte anzeigen, die für sie freigegeben wurden
* Anzeigen von Benutzern, die Dokumente und Kalenderberichte für sie freigeben
* Genehmigen Sie die Dokumente, die für sie freigegeben wurden.

Sie können diese Zugriffsebene nicht ändern.

>[!IMPORTANT]
>
>Externer Benutzer ist nur verfügbar, wenn die Option &quot;Mit Personen ohne Workfront-Konten arbeiten, indem Sie deren E-Mail-Adresse verwenden&quot;im Bereich &quot;Systemeinstellungen&quot;unter &quot;Einrichtung&quot;aktiviert ist. Weitere Informationen finden Sie unter [Systemsicherheitsvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

#### **Zugriffsdetails**

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte auf Zugriffsebene externer Benutzer.

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Aufgabe | ✓ |   |   |
| Problem | ✓ |   |   |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte (einschließlich Dashboards und Kalenderberichten) |   | ✓ (nur für Kalenderberichte; keine Möglichkeit, Berichte freizugeben) |   |
| Filter, Ansichten und Gruppierungen | ✓ |   |   |
| Dokument |   | ✓ (keine Möglichkeit zum Freigeben von Dokumenten) |   |
| Benutzerin oder Benutzer |   | ✓ |   |
| Teams | ✓ |   |   |
| Vorlage | ✓ |   |   |
| Finanzdaten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Pinnwände | ✓ |   |   |
| Startseite | ✓ |   |   |
| Ziele | ✓ |   |   |


## Wie Zugriffsebenen und Berechtigungen zusammenarbeiten

Zugriffsebenen definieren, was Benutzer mit allgemeinen Objekttypen und Bereichen im System sehen und tun können, z. B. Projekten, Aufgaben und Problemen. Berechtigungen definieren, worauf Sie Zugriff auf bestimmte Objekte haben, die von anderen Personen im System erstellt wurden, z. B. ein Projekt, das für eine Marketingkampagne erstellt wurde.

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

Die Aktivitäten, die ein Benutzer mit einem Objekt ausführen kann, werden durch eine Kombination seiner Zugriffsebene und der ihnen erteilten Berechtigungen definiert.

![](assets/security-model-hierachy-copy.png)

### Gewähren von Berechtigungen durch Freigeben von Objekten

Benutzer erhalten Zugriff auf einzelne Objekte, wenn andere Benutzer diese freigeben und bestimmte Berechtigungen für diese Objekte gewähren.

>[!NOTE]
>
>* Wenn ein Benutzer ein Objekt mit bestimmten Berechtigungen teilt und dieses Objekt untergeordnete Objekte darunter hat, erbt der Empfänger dieselben Berechtigungen für diese untergeordneten Objekte.
>* Wenn eine Zugriffsebene Benutzer daran hindert, bestimmte Objekte zu löschen, hindert dies sie nicht daran, untergeordnete Objekte zu löschen, die in diesen Objekten enthalten sind.

Ein Benutzer kann dem Empfänger eine der folgenden Berechtigungen für das einzelne Objekt gewähren:

* **Ansicht**: Mit dieser Berechtigungsstufe kann der Empfänger das Objekt auf eine der folgenden Arten freigeben:

   * Systemweit, damit alle Benutzer ihn sehen können (nicht für alle Objekte verfügbar)
   * Bei externen Benutzern ohne Workfront-Lizenz (nicht für alle Objekte verfügbar)
   * Mit einer E-Mail-Adresse (nur für Dokumente und Kalender verfügbar)

* **Beitragen**: (nicht für alle Objekte verfügbar)
* **Verwalten**: Wenn jemand ein Objekt freigegeben, werden die Rechte des Empfängers für das Objekt durch eine Kombination der Zugriffsebene des Empfängers und der Berechtigungen für das Objekt bestimmt, die vom Freigebende erteilt wurden. Der geringste in dieser Kombination verfügbare Zugriff bestimmt, was der Empfänger mit dem Objekt tun kann.

### Beispielszenarien

#### **Szenario 1**

Wenn die Zugriffsebene des Empfängers die Bearbeitung eines Projekts nicht zulässt, kann diese Person ein Projekt auch dann nicht bearbeiten oder löschen, wenn der Freigebende die Berechtigung zur Verwaltung erteilt hat.

Oder wenn die Zugriffsebene des Empfängers die Bearbeitung von Projekten zulässt, der freigebende Benutzer jedoch schreibgeschützte Berechtigungen für ein Projekt erteilt hat, kann der Benutzer das Projekt nicht bearbeiten oder löschen.

#### **Szenario 2**

Wenn Olivia ein Workfront-Projekt mit Tony teilt, wird Tony sein Zugang dazu durch eine Kombination zweier Dinge bestimmt:

* Tony&#39;s Access Level, vom Workfront-Administrator zugewiesen
* Tonys Berechtigungen für das Projekt, spezifiziert von Olivia

Tonys Maßnahmen in Bezug auf das Projekt können weiter auf das Projekt beschränkt werden, doch dürfen sie nicht über das auf seiner Zugangsstufe zulässige Maß hinausgehen:

* Wenn Tony&#39;s Zugangsstufe ihm nicht erlaubt, Aufgaben zu erstellen, kann er dem Projekt keine Aufgaben hinzufügen, selbst wenn Olivia ihm die Berechtigung erteilt hat, ihm Aufgaben hinzuzufügen.
* Wenn Tony&#39;s Zugriffsebene es ihm ermöglicht, Aufgaben zu erstellen, aber Olivia keine Berechtigungen erteilt hat, Aufgaben zum Projekt hinzuzufügen, kann er diesem Projekt keine Aufgaben hinzufügen, aber er kann Aufgaben zu anderen Projekten hinzufügen, für die ihm entsprechende Berechtigungen erteilt wurden.
