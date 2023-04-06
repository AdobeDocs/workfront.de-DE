---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: access,model,funnel,chart,levels,permissions
navigation-topic: access-levels
title: Integrierte Zugriffsebenen in Adobe Workfront
description: Jede der sechs integrierten Zugriffsebenen ist für einen bestimmten Benutzertyp konzipiert, einschließlich Systemadministrator, Planer, Worker, Reviewer, Anforderer und externer Benutzer. Mit diesen Zugriffsebenen können Sie steuern, welche Benutzer im System bearbeitet und angezeigt werden können. Wenn Sie eine benutzerdefinierte Zugriffsebene benötigen, können Sie die integrierte Zugriffsebene kopieren und den Umfang des Zugriffs bestimmen, der für die verschiedenen Workfront-Objekttypen zulässig sein soll.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5cb42dd8-1557-4fa4-ab3d-8278ce9afd96
source-git-commit: 1bd454246419e199e5cfd0d8d1d73cd30c0b13b1
workflow-type: tm+mt
source-wordcount: '1515'
ht-degree: 5%

---

# Integrierte alte Zugriffsstufen in Adobe Workfront

Jede der sechs nativen Zugriffsstufen wurde für einen bestimmten Benutzertyp entwickelt:

* Systemadministrator
* Planer
* Arbeitskraft
* Prüfer
* Antragsteller
* Externer Benutzer

Je nach der bisherigen Zugriffsstufe sind für die meisten Workfront-Objekttypen bis zu drei Einstellungen verfügbar:

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

Wenn Sie eine benutzerdefinierte Zugriffsebene für Planer, Worker, Anforderer oder Überprüfer benötigen, können Sie die integrierte alte Zugriffsstufe kopieren und den Umfang des Zugriffs bestimmen, der für die verschiedenen Workfront-Objekttypen zulässig sein soll. Informationen zum Erstellen einer benutzerdefinierten Zugriffsebene oder Ändern einer der integrierten alten Zugriffsebenen finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

>[!IMPORTANT]
>
>Es wird dringend empfohlen, die integrierten alten Zugriffsebenen unverändert zu lassen, damit Sie nach der Einrichtung Ihrer Benutzer darauf verweisen können.

Allgemeine Informationen zu diesen Zugriffsebenen finden Sie unter [Übersicht über Zugriffsebenen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Zugriffsstufe für Systemadministrator

Diese integrierte Zugriffsstufe, die an die Planungslizenz angehängt ist, wurde für einen Benutzer entwickelt, der für die Verwaltung des Adobe Workfront-Systems zuständig ist. Sie können diese integrierte Zugriffsebene nicht ändern.

Benutzer mit der Zugriffsstufe &quot;Systemadministrator&quot;können alles in Workfront tun. Sie können alle Workfront-Objekte und Informationen anzeigen und bearbeiten, die von allen anderen Benutzern in Workfront eingegeben wurden.

Sie haben außerdem Zugriff auf den gesamten Bereich &quot;Einrichtung&quot;, in dem sie jede Einstellung auf Systemebene ändern können. Und sie können auf alle Bereiche im Hauptmenü zugreifen ![](assets/main-menu-icon.png).

Weitere Informationen finden Sie unter [Gewähren eines vollen Administratorzugriffs](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Planen der bisherigen Zugriffsstufe

Diese Zugriffsstufe, die ebenfalls an die Planungslizenz angehängt ist, wurde für Folgendes entwickelt:

* Manager von Gruppen, Teams, Projekten und Ressourcen
* Jeder, der für die Planung, Erstellung und Verwaltung von Aufgaben, Projekten, Portfolios und Programmen verantwortlich ist
* Jeder, der für die Zuweisung von Aufgaben (Aufgaben und Probleme) zu anderen Benutzern verantwortlich ist
* Benutzer, die Berichte erstellen und Timesheets, Arbeitselemente und Dokumente genehmigen
* Benutzer, die Zugriff auf alle Bereiche im Hauptmenü benötigen ![](assets/main-menu-icon.png)

Sie können eine benutzerdefinierte Version der integrierten alten Zugriffsstufe &quot;Planer&quot;erstellen und den Umfang des Zugriffs für die verschiedenen Workfront-Objekttypen bestimmen. Weitere Informationen finden Sie unter [Integrierte Zugriffsebenen in Adobe Workfront](#Customiz) in diesem Artikel.

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte in der bisherigen Zugriffsstufe Planer :

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
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |

{style="table-layout:auto"}

## Zugriffsstufe für ältere Arbeitskräfte

Diese Zugriffsstufe, die an die Work-Lizenz angehängt ist, richtet sich an Benutzer, die die Arbeit in Workfront durchführen. Sie planen die Arbeit nicht. sie vervollständigen sie.

Benutzer mit dieser Zugriffsstufe:

* den Arbeitselementen zugewiesen werden, in denen sie Beiträge und Protokollzeit einbringen können
* Kann Arbeiten und Dokumente genehmigen, jedoch keine Timesheets
* Berichte aufrufen und freigeben
* Kann mit anderen Benutzern im System kommunizieren
* Kann auf alle Bereiche im Hauptmenü zugreifen ![](assets/main-menu-icon.png), ihr &quot;Benutzer&quot;-Bereich jedoch heißt Teams. Im Bereich Teams können Benutzer mit dieser Zugriffsebene nur Teams anzeigen, denen sie angehören, sowie die diesen Teams zugewiesenen Aufgaben.
* Sie haben nur begrenzte Möglichkeiten, Objekte zu erstellen - sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.

Sie können eine benutzerdefinierte Version der integrierten Zugriffsstufe von Worker erstellen und den Umfang des Zugriffs für die verschiedenen Workfront-Objekttypen bestimmen. Weitere Informationen finden Sie unter [Integrierte Zugriffsebenen in Adobe Workfront](#Customiz) in diesem Artikel.

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte in der Zugriffsebene von Worker:

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekte |   |   | ✓ (Begrenzt) Benutzer können nur das Projekt freigeben, Aufgaben und Probleme darin erstellen und Daten in benutzerdefinierten Formularen bearbeiten, die bereits an das Projekt angehängt sind.) |
| Aufgaben |   |   | ✓ |
| Probleme |   |   | ✓ |
| Portfolios |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |   |
| Programme |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |   |
| Berichte (einschließlich Dashboards und Kalenderberichten) |   | ✓ |   |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokumente |   |   | ✓ |
| Benutzende |   |   | ✓ |
| Vorlagen | ✓ |   |   |
| Finanzdaten |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;. Mit der Einstellung Ansicht kann der Benutzer nur den Bereich Finanzen in den Projektdetails anzeigen.) |   |
| Ressourcenverwaltung |   | ✓ |   |
| Szenarienplaner |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |

{style="table-layout:auto"}

## Berechtigte Zugriffsstufe eines Prüfers

Diese Zugriffsstufe, die an die Überprüfungslizenz angehängt ist, richtet sich an Führungskräfte, die Arbeiten von anderen Benutzern anfordern und die Arbeit überprüfen und genehmigen. Dies sind keine Projekteigentümer oder Teammitglieder, aber sie benötigen Zugriff auf Workfront, um die von ihnen überwachten Arbeitselemente anzuzeigen.

Beispielsweise könnte sich ein Verantwortlicher mit dieser Zugriffsebene bei Workfront anmelden, um an einer laufenden Überprüfung von Marketing-Materialien teilzunehmen, Arbeitsaktualisierungen zu sehen und Dokumente, Genehmigungen, Berichte und Kalender zu überprüfen.

Benutzer mit Zugriffsstufe &quot;Prüfer&quot;:

* Arbeitselemente oder Genehmigungs-Zeitblätter können nicht zugewiesen werden
* Kann auf Anfragen und Dokumente im Hauptmenü zugreifen ![](assets/main-menu-icon.png).
* Sie haben nur begrenzte Möglichkeiten, Objekte zu erstellen - sie können keine Projekte, Portfolios, Programme oder Berichte erstellen.

Sie können eine benutzerdefinierte Version der integrierten Zugriffsstufe des Prüfers erstellen und bestimmen, wie viel Zugriff auf die verschiedenen Workfront-Objekttypen möglich ist. Weitere Informationen finden Sie unter [Integrierte Zugriffsebenen in Adobe Workfront](#Customiz) in diesem Artikel.

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
   <td>✓</td> 
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
   <td>Vorlagen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Finanzdaten</td> 
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

## Anfordern der bisherigen Zugriffsstufe

Diese Zugriffsstufe, die an die Anforderungslizenz angehängt ist, wurde für Benutzer entwickelt, die einfache Arbeitsanfragen in Workfront erstellen und erhalten. Standardmäßig sind sie auf den Bereich Anforderungen beschränkt.

Beispielsweise kann ein Benutzer Probleme in der Anforderungswarteschlange Ihres Unternehmens protokollieren.

Benutzer mit dieser Zugriffsstufe:

* Kann Anforderungen stellen und diese Anforderungen aktualisieren
* Dokumente hochladen und genehmigen können
* Kann den Status der von ihnen eingereichten Probleme überprüfen
* Arbeitselemente können nicht zugewiesen werden
* Kann nur über das Hauptmenü auf Anfragen zugreifen ![](assets/main-menu-icon.png). Weitere Informationen zu Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Sie können eine benutzerdefinierte Version der nativen Zugriffsstufe &quot;Anforderer&quot;erstellen und den Umfang des Zugriffs bestimmen, der für die verschiedenen Workfront-Objekttypen zulässig ist. Weitere Informationen finden Sie unter [Integrierte Zugriffsebenen in Adobe Workfront](#Customiz) in diesem Artikel.

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte in der Zugriffsebene &quot;Anforderer&quot;:

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekt |   | ✓ (nur die Seite &quot;Projektdetails&quot;) |   |
| Aufgabe |   | ✓ (nur die Detailseite) |   |
| Problem |   |   | ✓ |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte (einschließlich Dashboards und Kalenderberichten) |   | ✓ (nur die Detailseite) |   |
| Filter, Ansichten und Gruppierungen |   |   | ✓ |
| Dokument |   |   | ✓ |
| Benutzerin oder Benutzer |   | ✓ |   |
| Vorlage | ✓ |   |   |
| Finanzdaten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Workfront-Ziele |   |   | ✓ (Die Standardeinstellung ist &quot;Kein Zugriff&quot;.) |

{style="table-layout:auto"}

## Zugriffsstufe für externe Benutzer

Diese Zugriffsstufe ist nicht an eine gebührenpflichtige Workfront-Lizenz gebunden. Es handelt sich dabei um die restriktivste Zugriffsstufe, die hauptsächlich für Mitarbeiter wie externe Berater konzipiert ist, die sich nicht bei Workfront anmelden, aber Dokumente gelegentlich überprüfen, herunterladen oder anzeigen müssen.

Workfront-Benutzer können externen Benutzern Aufgaben zuweisen, auch wenn sich externe Benutzer nicht beim System anmelden können. Aber wir raten davon ab, weil diese Arbeit im System noch nicht gelöst sein würde.

Benutzer mit der Zugriffsebene &quot;Externer Benutzer&quot;:

* Kann nur Dokumente und Kalenderberichte anzeigen, die für sie freigegeben wurden
* Anzeigen der Benutzer, die Dokumente und Kalenderberichte für sie freigeben
* Genehmigen der Dokumente, die für sie freigegeben sind

Sie können diese Zugriffsebene nicht ändern.

>[!IMPORTANT]
>
>Externer Benutzer ist nur verfügbar, wenn die Option &quot;Mit Personen ohne Workfront-Konten arbeiten, indem Sie deren E-Mail-Adresse verwenden&quot;im Bereich &quot;Systemeinstellungen&quot;unter &quot;Einrichtung&quot;aktiviert ist. Weitere Informationen finden Sie unter [Systemsicherheitsvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md).

Im Folgenden finden Sie die höchsten verfügbaren Zugriffseinstellungen für Objekte auf Zugriffsebene externer Benutzer.

| Workfront-Objekttyp | Kein Zugriff | Zugriff anzeigen | Zugriff bearbeiten |
|---|---|---|---|
| Projekt | ✓ |   |   |
| Aufgabe | ✓ | ✓ |   |
| Problem | ✓ |   |   |
| Portfolios | ✓ |   |   |
| Programme | ✓ |   |   |
| Berichte (einschließlich Dashboards und Kalenderberichten) |   | ✓ (nur für Kalenderberichte; keine Möglichkeit zum Freigeben von Berichten) |   |
| Filter, Ansichten und Gruppierungen | ✓ |   |   |
| Dokument |   | ✓ (ohne die Möglichkeit, Dokumente freizugeben) |   |
| Benutzerin oder Benutzer |   | ✓ |   |
| Vorlage | ✓ |   |   |
| Finanzdaten | ✓ |   |   |
| Ressourcenverwaltung | ✓ |   |   |
| Szenarienplaner | ✓ |   |   |
| Workfront-Ziele | ✓ |   |   |
