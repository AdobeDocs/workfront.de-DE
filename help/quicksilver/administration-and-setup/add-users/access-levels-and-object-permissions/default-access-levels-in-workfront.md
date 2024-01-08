---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,chart,levels,permissions
navigation-topic: access-levels
title: Integrierte Zugriffsebenen
description: Jede der sechs aktuellen integrierten Zugriffsebenen wurde für einen bestimmten Benutzertyp entwickelt, einschließlich Systemadministrator, Planer, Worker, Reviewer, Anforderer und externer Benutzer. Mit diesen Zugriffsebenen können Sie steuern, welche Benutzer im System bearbeitet und angezeigt werden können. Wenn Sie eine benutzerdefinierte Zugriffsebene benötigen, können Sie eine integrierte Zugriffsebene kopieren und entsprechend der Zugriffsmenge ändern, die Sie benötigen, um sie für die verschiedenen Workfront-Objekttypen zuzulassen.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 9d2165cdc9399273a4f79b90d4049f50097cadee
workflow-type: tm+mt
source-wordcount: '1685'
ht-degree: 5%

---

# Integrierte Zugriffsebenen

<!--Audited: 01/2024-->

>[!NOTE]
>
>In diesem Artikel werden die aktuellen integrierten Zugriffsebenen in Adobe Workfront beschrieben. Informationen zu den neuen integrierten Zugriffsebenen finden Sie unter [Übersicht über die neuen Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).


Jede der sechs aktuellen integrierten Zugriffsebenen wurde für einen bestimmten Benutzertyp entwickelt. Mit diesen Zugriffsebenen können Sie steuern, welche Benutzer im System bearbeitet und angezeigt werden können.

Jede der sechs integrierten Zugriffsebenen ist für die folgenden Benutzertypen ausgelegt:

* Systemadministrator
* Planer
* Arbeitskraft
* Prüfende Person
* Anfragender
* Externer Benutzer

Je nach Zugriffsebene sind für die meisten Workfront-Objekttypen bis zu drei Einstellungen verfügbar:

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

Wenn Sie eine benutzerdefinierte Zugriffsebene für Planer, Worker, Anforderer oder Überprüfer benötigen, können Sie die integrierte Zugriffsebene kopieren und den Umfang des Zugriffs bestimmen, der für die verschiedenen Workfront-Objekttypen zulässig sein soll.

>[!TIP]
>
>Sie können die Zugriffsebene des Systemadministrators oder des externen Benutzers nicht ändern.

Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene oder Ändern einer der integrierten Zugriffsebenen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen und ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Wir empfehlen dringend, die integrierten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können.

Allgemeine Informationen zu diesen Zugriffsebenen finden Sie unter [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Zugriffsstufe für Systemadministrator

Die integrierte Systemadministratorzugriffsstufe, die an die Planungslizenz angehängt ist, ist für einen Benutzer ausgelegt, der für die Verwaltung des Adobe Workfront-Systems zuständig ist. Sie können diese integrierte Zugriffsebene nicht ändern.

Benutzer mit der Zugriffsebene &quot;Systemadministrator&quot;können alles in Workfront tun. Sie können alle Workfront-Objekte und Informationen anzeigen und bearbeiten, die von allen anderen Benutzern in Workfront eingegeben wurden.

Sie haben auch vollen Zugriff auf den Bereich Einrichtung , in dem sie jede Einstellung auf Systemebene ändern können. Und sie können auf alle Bereiche im Hauptmenü zugreifen ![](assets/main-menu-icon.png) oder im Hauptmenü ![](assets/lines-main-menu.png), falls verfügbar.

Weitere Informationen finden Sie unter [Gewähren eines vollen Administratorzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Planen der Zugriffsebene

Die Zugriffsstufe Planer ist ebenfalls mit der Planungslizenz verbunden und dient folgenden Zwecken:

* Manager von Gruppen, Teams, Projekten und Ressourcen
* Jeder, der für die Planung, Erstellung und Verwaltung von Aufgaben, Projekten, Portfolios und Programmen verantwortlich ist
* Jeder, der für die Zuweisung von Aufgaben (Aufgaben und Probleme) zu anderen Benutzern verantwortlich ist
* Benutzer, die Berichte erstellen und Timesheets, Arbeitselemente und Dokumente genehmigen
* Benutzer, die Zugriff auf alle Bereiche im Hauptmenü benötigen ![](assets/main-menu-icon.png) oder im Hauptmenü ![](assets/lines-main-menu.png), falls verfügbar

Sie können eine benutzerdefinierte Version der integrierten Zugriffsebene des Planers erstellen und den Umfang des Zugriffs für die verschiedenen Workfront-Objekttypen bestimmen. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen und ändern](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte in der Zugriffsebene &quot;Planer&quot;:

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
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
| Szenarienplaner |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |

{style="table-layout:auto"}

## Zugriffsstufe der Arbeitnehmer

Die an die Work-Lizenz angehängte Zugriffsstufe &quot;Worker&quot;wurde für Benutzer entwickelt, die die Arbeit in Workfront durchführen. Sie planen die Arbeit nicht; sie schließen sie ab.

Benutzer mit dieser Zugriffsstufe:

* den Arbeitselementen zugewiesen werden, in denen sie Beiträge und Protokollzeit einbringen können
* Kann Arbeiten und Dokumente genehmigen, jedoch keine Timesheets
* Berichte aufrufen und freigeben
* Kann mit anderen Benutzern im System kommunizieren
* Zugriff auf alle Bereiche im Hauptmenü nicht möglich ![](assets/main-menu-icon.png) oder im Hauptmenü ![](assets/lines-main-menu.png), sofern verfügbar, und ihr Bereich &quot;Benutzer&quot;heißt Teams. Im Bereich Teams können Benutzer mit dieser Zugriffsebene nur Teams anzeigen, denen sie angehören, sowie die diesen Teams zugewiesenen Aufgaben.
* Sie haben nur begrenzte Möglichkeiten, Objekte zu erstellen - sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.

Sie können eine benutzerdefinierte Version der integrierten Zugriffsstufe von Worker erstellen und den Umfang des Zugriffs bestimmen, der für die verschiedenen Workfront-Objekttypen zulässig ist. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen und ändern](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte in der Zugriffsebene von Worker:

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekte |   |   | ✓ (Eingeschränkt: Benutzer können nur das Projekt freigeben, Aufgaben und Probleme darin erstellen und Daten in benutzerdefinierten Formularen bearbeiten, die bereits angehängt sind.) |
| Aufgaben |   |   | ✓ |
| Probleme |   |   | ✓ |
| Portfolios |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |   |
| Programme |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |   |
| Berichte, Dashboards und Kalender |   | ✓ |   |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokumente |   |   | ✓ |
| Benutzende |   |   | ✓ |
| Teams |   |   | ✓ (eingeschränkter Zugriff) |
| Vorlagen | ✓ |   |   |
| Finanzielle Daten |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;. Mit der Einstellung Ansicht kann der Benutzer nur den Bereich Finanzen in den Projektdetails anzeigen.) |   |
| Ressourcenverwaltung |   | ✓ |   |
| Szenarienplaner |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |

{style="table-layout:auto"}

## Zugriffsebene der Prüfer

Die an die Überprüfungslizenz angehängte Zugriffsstufe ist für Führungskräfte gedacht, die Arbeiten von anderen Benutzern anfordern und die Arbeit überprüfen und genehmigen. Dies sind keine Projekteigentümer oder Teammitglieder, aber sie benötigen Zugriff auf Workfront, um die von ihnen überwachten Arbeitselemente anzuzeigen.

Beispielsweise könnte sich ein Verantwortlicher mit dieser Zugriffsebene bei Workfront anmelden, um an einer laufenden Überprüfung von Marketing-Materialien teilzunehmen, Arbeitsaktualisierungen zu sehen und Dokumente, Genehmigungen, Berichte und Kalender zu überprüfen.

Benutzer mit Zugriffsstufe &quot;Prüfer&quot;:

* Arbeitselemente können nicht zugewiesen oder Timesheets genehmigt werden
* Kann auf die Bereiche Anforderungen und Dokumente im Hauptmenü zugreifen ![](assets/main-menu-icon.png) oder im Hauptmenü ![](assets/lines-main-menu.png), falls verfügbar
* Sie haben nur begrenzte Möglichkeiten, Objekte zu erstellen - sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.

Sie können eine benutzerdefinierte Version der integrierten Zugriffsstufe des Prüfers erstellen und bestimmen, wie viel Zugriff es für die verschiedenen Workfront-Objekttypen ermöglicht. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen und ändern](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Die folgenden Zugriffseinstellungen sind für Projekte und Aufgaben, die über die Zugriffsebene von Worker hinausgehen, am höchsten und für Objekte auf der Zugriffsebene des Prüfers verfügbar:

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
   <td> <p>✓ (Die Standardeinstellung ist "Kein Zugriff". Mit der Einstellung Ansicht kann der Benutzer nur den Bereich Finanzen in den Projektdetails anzeigen.)</p> </td> 
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
   <td>Workfront-Ziele </td> 
   <td> </td> 
   <td> </td> 
   <td>✓ (Die Standardeinstellung ist "Kein Zugriff".)</td> 
  </tr> 
 </tbody> 
</table>

## Zugriffsstufe anfordern

Die Zugriffsstufe Anfordern ist an die Anforderungslizenz angehängt und wurde für Benutzer entwickelt, die einfache Arbeitsanfragen in Workfront erstellen und erhalten. Standardmäßig sind sie auf den Bereich Anforderungen beschränkt.

Beispielsweise kann ein Benutzer Probleme in der Anforderungswarteschlange Ihres Unternehmens protokollieren.

Benutzer mit dieser Zugriffsstufe:

* Kann Anforderungen stellen und diese Anforderungen aktualisieren
* Dokumente hochladen und genehmigen können
* Kann den Status der von ihnen eingereichten Probleme überprüfen
* Arbeitselemente können nicht zugewiesen werden
* Kann nur über den Bereich Anforderungen im Hauptmenü auf Anfragen zugreifen ![](assets/main-menu-icon.png) oder im Hauptmenü ![](assets/lines-main-menu.png), falls verfügbar. Weitere Informationen zu Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Sie können eine benutzerdefinierte Version der integrierten Zugriffsstufe &quot;Anforderer&quot;erstellen und den Umfang des Zugriffs bestimmen, der für die verschiedenen Workfront-Objekttypen zulässig ist. Weitere Informationen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen und ändern](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte in der Zugriffsebene &quot;Anforderer&quot;:

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekt |   | ✓ (nur die Seite &quot;Projektdetails&quot;) |   |
| Aufgabe |   | ✓ (nur Seite &quot;Aufgabendetails&quot;) |   |
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
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |

{style="table-layout:auto"}

## Zugriffsstufe für externe Benutzer

Die Zugriffsebene für externe Benutzer ist nicht an eine gebührenpflichtige Workfront-Lizenz gebunden. Es handelt sich dabei um die restriktivste Zugriffsstufe, die hauptsächlich für Mitarbeiter wie externe Berater konzipiert ist, die sich nicht bei Workfront anmelden, aber Dokumente gelegentlich überprüfen, herunterladen oder anzeigen müssen.

Workfront-Benutzer können externen Benutzern Aufgaben zuweisen, auch wenn sich externe Benutzer nicht beim System anmelden können. Es wird jedoch nicht empfohlen, externen Benutzern Aufgaben und Probleme zuzuweisen, da diese Arbeit im System nicht aufgelöst werden kann.

Benutzer mit der Zugriffsebene &quot;Externer Benutzer&quot;:

* Kann nur Dokumente und Kalenderberichte anzeigen, die für sie freigegeben wurden
* Können Benutzer sehen, die Dokumente und Kalenderberichte für sie freigeben?
* Kann die für sie freigegebenen Dokumente genehmigen

Sie können diese Zugriffsebene nicht ändern.

>[!IMPORTANT]
>
>Externer Benutzer ist nur verfügbar, wenn die Option &quot;Mit Personen ohne Workfront-Konten arbeiten, indem Sie deren E-Mail-Adresse verwenden&quot;im Bereich &quot;Systemeinstellungen&quot;unter &quot;Einrichtung&quot;aktiviert ist. Weitere Informationen finden Sie unter [Systemsicherheitsvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Diese Einstellungen sind zwar nicht im Bereich Zugriffsebenen für die Zugriffsebene &quot;Externer Benutzer&quot;sichtbar, ein Benutzer mit diesem Zugriff hat jedoch den höchsten Zugriff auf die Workfront-Objekttypen:

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Aufgabe | ✓ | |   |
| Problem | ✓ |   |   |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte, Dashboards und Kalender |   | ✓ (nur für Kalenderberichte; keine Möglichkeit, Berichte freizugeben) |   |
| Filter, Ansichten und Gruppierungen | ✓ |   |   |
| Dokumente |   | ✓ (ohne die Möglichkeit zur Freigabe von Dokumenten) |   |
| Benutzende |   | ✓ |   |
| Teams |   | ✓ |   |
| Vorlagen | ✓ |   |   |
| Finanzielle Daten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Workfront-Ziele | ✓ |   |   |
