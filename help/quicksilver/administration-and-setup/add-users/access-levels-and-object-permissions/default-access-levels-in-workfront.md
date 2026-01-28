---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: Zugriff,Modell,funnel,Diagramm,Ebenen,Berechtigungen
navigation-topic: access-levels
title: Integrierte Zugriffsebenen (veraltet)
description: Jede der sechs aktuellen integrierten Zugriffsebenen ist für einen bestimmten Benutzertyp konzipiert, einschließlich Systemadministrator, Planer, Sekundär, Prüfer, Antragsteller und externer Benutzer. Mit diesen Zugriffsebenen können Sie steuern, welche Benutzer im System bearbeiten und anzeigen können. Wenn Sie eine benutzerdefinierte Zugriffsebene benötigen, können Sie eine integrierte Zugriffsebene kopieren und entsprechend der gewünschten Zugriffsmenge ändern, um sie für die verschiedenen Workfront-Objekttypen zuzulassen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1656'
ht-degree: 7%

---

# Integrierte Zugriffsebenen (veraltet)

<!--Audited: 01/2024-->

>[!NOTE]
>
>Die Informationen in diesem Artikel beziehen sich auf die alten Zugriffsebenen. Informationen zu den aktuellen Zugriffsebenen finden Sie unter [Übersicht über neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Jede der sechs aktuellen integrierten Zugriffsebenen ist für einen bestimmten Benutzertyp konzipiert. Mit diesen Zugriffsebenen können Sie steuern, welche Benutzer im System bearbeiten und anzeigen können.

Jede der sechs integrierten Zugriffsebenen wurde für die folgenden Benutzertypen entwickelt:

* Systemadministrator
* Planerin oder Planer
* Arbeitskraft
* Prüfende Person
* Anfragenden
* Externer Benutzer

Je nach Zugriffsebene sind für die meisten Workfront-Objekttypen bis zu drei Einstellungen verfügbar:

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

Wenn Sie eine benutzerdefinierte Zugriffsebene für Planer, Sekundär, Auftraggeber oder Prüfer benötigen, können Sie die integrierte Zugriffsebene kopieren und die gewünschte Zugriffsmenge für die verschiedenen Workfront-Objekttypen bestimmen.

>[!TIP]
>
>Sie können weder die Zugriffsebenen des Systemadministrators noch des externen Benutzers ändern.

Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene oder zum Ändern einer der integrierten Zugriffsebenen finden Sie unter [Erstellen und Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Es wird dringend empfohlen, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können.

Allgemeine Informationen zu diesen Zugriffsebenen finden Sie unter [Zugriffsebenen - Übersicht](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Zugriffsebene des Systemadministrators

In Verbindung mit der Planlizenz richtet sich die integrierte Zugriffsebene „Systemadministrator“ an Benutzende, die für die Verwaltung des Adobe Workfront-Systems zuständig sind. Diese integrierte Zugriffsebene kann nicht geändert werden.

Benutzende mit der Zugriffsebene „Systemadministrator“ können alles in Workfront tun. Sie können alle Workfront-Objekte und -Informationen anzeigen und bearbeiten, die von allen anderen Benutzenden in Workfront eingegeben wurden.

Sie haben außerdem vollen Zugriff auf den Bereich Setup , in dem sie alle Einstellungen auf Systemebene ändern können. Und sie können auf alle Bereiche im Hauptmenü ![Hauptmenüsymbol](assets/main-menu-icon.png) oder Hauptmenü ![Hauptmenüsymbol](assets/main-menu-icon.png) zugreifen, falls verfügbar.

Weitere Informationen finden Sie unter [Gewähren des vollständigen Administratorzugriffs für einen Benutzer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Zugriffsebene des Planers

Die Zugriffsebene des Planers, die ebenfalls an die Planlizenz angehängt ist, ist für Folgendes ausgelegt:

* Manager von Gruppen, Teams, Projekten und Ressourcen
* Alle, die für die Planung, Erstellung und Verwaltung von Aufgaben, Projekten, Portfolios und Programmen verantwortlich sind
* Jeder, der für die Zuweisung von Arbeit (Aufgaben und Probleme) an andere Benutzer verantwortlich ist
* Benutzer, die Berichte erstellen und Arbeitszeittabellen, Arbeitselemente und Dokumente genehmigen
* Benutzer, die Zugriff auf alle Bereiche im Hauptmenü (![-Symbol) &#x200B;](assets/main-menu-icon.png) Hauptmenü (![-Symbol](assets/main-menu-icon.png) benötigen, falls verfügbar

Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene von Planer erstellen und den Umfang des Zugriffs festlegen, den sie für die verschiedenen Workfront-Objekttypen zulässt. Weitere Informationen finden Sie unter [Erstellen und Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Planerzugriffsebene verfügbar sind:

| Workfront-Objekttyp | Kein Zugriff | Ansichtszugriff | Zugriff bearbeiten |
|---|---|---|---|
| Projekte |   |   | ✓ |
| Aufgaben |   |   | ✓ |
| Probleme |   |   | ✓ |
| Portfolios |   |   | ✓ |
| Programme |   |   | ✓ |
| Berichte, Dashboards und Kalender |   |   | ✓ |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokumente |   |   | ✓ |
| Benutzende |   |   | ✓ |
| Teams |   |   | ✓ |
| Vorlagen |   |   | ✓ |
| Finanzielle Daten |   |   | ✓ |
| Ressourcenverwaltung |   |   | ✓ |
| Szenarienplaner |   |   | ✓ (Die Standardeinstellung ist Kein Zugriff.) |
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist Kein Zugriff.) |

{style="table-layout:auto"}

## Worker-Zugriffsebene

Im Anhang zur Arbeitslizenz ist die Worker-Zugriffsebene für Benutzende vorgesehen, die die Arbeit in Workfront ausführen. Sie planen die Arbeit nicht, sie schließen sie ab.

Benutzer mit dieser Zugriffsebene:

* Arbeitselementen zugewiesen werden, in denen sie einen Beitrag leisten und Zeit erfassen können
* Kann Arbeiten und Dokumente genehmigen, jedoch keine Arbeitszeittabellen
* Kann auf Berichte zugreifen und sie freigeben
* Kann mit anderen Benutzenden im System kommunizieren
* Es können nicht alle Bereiche im Hauptmenü (![-Symbol) &#x200B;](assets/main-menu-icon.png) Hauptmenü (![-Symbol) &#x200B;](assets/main-menu-icon.png), falls verfügbar, aufgerufen werden. Ihr Bereich „Benutzer“ heißt „Teams“. Im Bereich Teams können Benutzer mit dieser Zugriffsebene nur die Teams sehen, denen sie angehören, sowie die diesen Teams zugewiesenen Arbeiten.
* Die Möglichkeit, Objekte zu erstellen, ist eingeschränkt. Sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.

Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene von Worker erstellen und den Umfang des Zugriffs festlegen, der für die verschiedenen Workfront-Objekttypen zulässig ist. Weitere Informationen finden Sie unter [Erstellen und Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Worker-Zugriffsebene verfügbar sind:

| Workfront-Objekttyp | Kein Zugriff | Ansichtszugriff | Zugriff bearbeiten |
|---|---|---|---|
| Projekte |   |   | ✓ (Eingeschränkt: Benutzer können nur das Projekt freigeben, Aufgaben und Probleme darin erstellen und Daten in benutzerdefinierten Formularen bearbeiten, die bereits damit verbunden sind.) |
| Aufgaben |   |   | ✓ |
| Probleme |   |   | ✓ |
| Portfolios |   | ✓ (Die Standardeinstellung ist Kein Zugriff.) |   |
| Programme |   | ✓ (Die Standardeinstellung ist Kein Zugriff.) |   |
| Berichte, Dashboards und Kalender |   | ✓ |   |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokumente |   |   | ✓ |
| Benutzende |   |   | ✓ |
| Teams |   |   | ✓ (eingeschränkter Zugriff) |
| Vorlagen | ✓ |   |   |
| Finanzielle Daten |   | ✓ (Die Standardeinstellung ist Kein Zugriff. Mit der Einstellung Ansicht kann der Benutzer nur den Finanzbereich anzeigen   in den Projektdetails.) |   |
| Ressourcenverwaltung |   | ✓ |   |
| Szenarienplaner |   |   | ✓ (Die Standardeinstellung ist Kein Zugriff.) |
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist Kein Zugriff.) |

{style="table-layout:auto"}

## Zugriffsebene des Prüfers

Die Zugriffsebene des Reviewers ist an die Revisionslizenz angehängt und richtet sich an Führungskräfte, die Arbeit von anderen Benutzern anfordern und die Arbeit überprüfen und genehmigen. Dabei handelt es sich nicht um Projektbesitzer oder Teammitglieder, sie benötigen jedoch Zugriff auf Workfront, um die von ihnen überwachten Arbeitselemente anzeigen zu können.

Beispielsweise könnte sich ein Stakeholder mit dieser Zugriffsebene bei Workfront anmelden, um an einer fortlaufenden Überprüfung von Marketing-Materialien teilzunehmen, Arbeitsaktualisierungen zu Arbeiten anzuzeigen und Dokumente, Genehmigungen, Berichte und Kalender zu überprüfen.

Benutzer mit der Zugriffsebene des Reviewers:

* Kann keine Arbeitselemente zugewiesen oder Arbeitszeittabellen genehmigt werden
* Kann auf die Bereiche Anfragen und Dokumente im Hauptmenü (Hauptmenüsymbol![&#x200B; oder im Hauptmenü (Hauptmenüsymbol](assets/main-menu-icon.png) zugreifen, ![&#x200B; verfügbar](assets/main-menu-icon.png)
* Die Möglichkeit, Objekte zu erstellen, ist eingeschränkt. Sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.

Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene des Reviewers erstellen und den Umfang des Zugriffs festlegen, der für die verschiedenen Objekttypen von Workfront ermöglicht wird. Weitere Informationen finden Sie unter [Erstellen und Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Bei Projekten und Aufgaben, die stärker eingeschränkt sind als die Worker-Zugriffsebene, sind im Folgenden die höchsten Zugriffseinstellungen aufgeführt, die für Objekte auf der Reviewer-Zugriffsebene verfügbar sind:

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
   <td>Berichte, Dashboards, Kalender</td> 
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
   <td>Finanzielle Daten</td> 
   <td> </td> 
   <td> <p>✓ (Die Standardeinstellung ist Kein Zugriff. Mit der Einstellung Ansicht kann der Benutzer nur den Finanzbereich anzeigen   in den Projektdetails.)</p> </td> 
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
   <td>Workfront-Ziele </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist Kein Zugriff.)</td> 
  </tr> 
 </tbody> 
</table>

## Zugriffsebene des Antragstellers

Im Anhang zur Anfragelizenz ist die Zugriffsebene des Antragstellers für Benutzende konzipiert, die in Workfront Arbeitsanfragen stellen und empfangen. Standardmäßig sind sie auf den Bereich Anfragen beschränkt.

Beispielsweise kann ein Benutzer Probleme in der Helpdesk-Anfragewarteschlange Ihres Unternehmens protokollieren.

Benutzer mit dieser Zugriffsebene:

* Kann Anfragen stellen und diese aktualisieren
* Kann Dokumente hochladen und genehmigen
* Kann den Status der von ihnen gesendeten Probleme überprüfen
* Kann Arbeitselementen nicht zugewiesen werden
* Der Zugriff auf Anfragen ist nur über den Bereich Anfragen im Hauptmenü ![Hauptmenüsymbol](assets/main-menu-icon.png) oder über das Hauptmenü ![Hauptmenüsymbol](assets/main-menu-icon.png) möglich, falls verfügbar. Weitere Informationen zu Anfrage-Warteschlangen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene des Anforderers erstellen und den Umfang des Zugriffs festlegen, der für die verschiedenen Workfront-Objekttypen zulässig ist. Weitere Informationen finden Sie unter [Erstellen und Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Im Folgenden finden Sie die höchsten Zugriffseinstellungen, die für Objekte auf der Zugriffsebene des Anforderers verfügbar sind:

| Workfront-Objekttyp | Kein Zugriff | Ansichtszugriff | Zugriff bearbeiten |
|---|---|---|---|
| Projekt |   | ✓ (Nur die Seite mit den Projektdetails) |   |
| Aufgabe |   | ✓(Nur die Seite mit den Aufgabendetails) |   |
| Problem |   |   | ✓ |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte, Dashboards und Kalender |   | ✓ |   |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokumente |   |   | ✓ |
| Benutzerin oder Benutzer |   | ✓ |   |
| Teams |   | ✓ |   |
| Vorlagen | ✓ |   |   |
| Finanzielle Daten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist Kein Zugriff.) |

{style="table-layout:auto"}

## Zugriffsebene externer Benutzer

Die Zugriffsebene Externer Benutzer ist nicht an eine gebührenpflichtige Workfront-Lizenz gebunden. Dies ist die restriktivste Zugriffsebene, die hauptsächlich für Mitarbeiter wie externe Berater entwickelt wurde, die sich nicht bei Workfront anmelden, aber Dokumente gelegentlich überprüfen, herunterladen oder anzeigen müssen.

Workfront-Benutzende können externen Benutzenden Aufgaben zuweisen, auch wenn sich externe Benutzende nicht beim System anmelden können. Es wird jedoch nicht empfohlen, externen Benutzern Aufgaben und Probleme zuzuweisen, da diese Arbeit im System ungelöst bleiben würde.

Benutzer mit der Zugriffsebene Externer Benutzer:

* Kann nur Dokumente und Kalenderberichte anzeigen, die für sie freigegeben sind
* Kann die Benutzer sehen, die Dokumente und Kalenderberichte für sie freigeben
* Kann die Dokumente genehmigen, die für sie freigegeben wurden

Diese Zugriffsebene kann nicht geändert werden.

>[!IMPORTANT]
>
>Externer Benutzer ist nur verfügbar, wenn die Option „Mit Personen ohne Workfront-Konten über deren E-Mail-Adresse zusammenarbeiten“ im Bereich „Systemeinstellungen“ im Setup aktiviert ist. Weitere Informationen finden Sie unter [Systemsicherheitseinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Obwohl diese Einstellungen für die Zugriffsebene Externer Benutzer nicht im Bereich Zugriffsebenen sichtbar sind, hat ein Benutzer mit diesem Zugriff den folgenden Zugriff auf die Workfront-Objekttypen:

| Workfront-Objekttyp | Kein Zugriff | Ansichtszugriff | Zugriff bearbeiten |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Aufgabe | ✓ | |   |
| Problem | ✓ |   |   |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte, Dashboards und Kalender |   | ✓ (Nur für Kalenderberichte, keine Möglichkeit zur Freigabe von Berichten) |   |
| Filter, Ansichten und Gruppierungen | ✓ |   |   |
| Dokumente |   | ✓ (ohne die Möglichkeit, Dokumente freizugeben) |   |
| Benutzende |   | ✓ |   |
| Teams |   | ✓ |   |
| Vorlagen | ✓ |   |   |
| Finanzielle Daten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Workfront-Ziele | ✓ |   |   |
