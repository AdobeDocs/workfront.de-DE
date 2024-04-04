---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Objekte von einer Umgebung in eine andere in Workfront verschieben
description: Die Funktion zur Umgebungsförderung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Die Möglichkeit zum Verschieben von Transaktionsobjekten wird nicht unterstützt (mit eingeschränkten Ausnahmen).
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 5d84d50b8984bbff7bbc02ffc0ce86ec1f486742
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 1%

---

# Übersicht über das Verschieben von Objekten zwischen Workfront-Umgebungen (Umgebungsförderung)

Die Umgebungsförderungsfunktion soll die Möglichkeit bieten, Objekte von einer Workfront-Umgebung in eine andere zu verschieben. Sie können beispielsweise eine Vorlage erstellen und in Ihrer Sandbox-Umgebung konfigurieren, in dem Wissen, dass sich Tests, die Sie durchführen, nicht auf die tatsächlichen Daten Ihrer Organisation auswirken. Nachdem die Vorlage konfiguriert und getestet wurde, können Sie sie in Ihre Produktionsumgebung verschieben, damit sie einsatzbereit ist.

Dieser Prozess wird als &quot;Umweltförderung&quot;bezeichnet.

Sie können diesen Vorgang in Workfront durchführen, indem Sie ein Objekt-Package erstellen, das verschoben werden soll, und dieses Package dann in der neuen Umgebung installieren.

* Spezifische Anweisungen zur Durchführung dieses Prozesses in Workfront finden Sie unter:

   * [Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Installieren eines Umgebungsförderungspakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Anweisungen zum Ausführen dieses Prozesses über die Workfront-API finden Sie unter [Objekte verschieben zwischen [!DNL Workfront] Umgebungen, die [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

## Unterstützte Objekte für die Umgebungsförderung

Die Funktion zur Umgebungsförderung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Die Möglichkeit zum Verschieben von Transaktionsobjekten wird nicht unterstützt (mit eingeschränkten Ausnahmen).

* [Arbeitsobjekte](#work-objects)
* [Reporting-Objekte](#reporting-objects)
* [Benutzerdefinierte Datenobjekte](#custom-data-objects)
* [Organisationsobjekte](#organization-objects)
* [Andere Konfigurationsobjekte](#other-configuration-objects)


### Arbeitsobjekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Projekt (PROJ) | Projekt<br>Aufgabe<br>Zuweisung<br>Vorgänger<br>Firma<br>Überschreibungsrate<br>Gruppe<br>Rolle<br>Team<br>Validierungsprozess<br>Validierungspfad<br>Validierungsschritt<br>Schritt-Genehmiger<br>Zeitplan<br>Nichtarbeitstag<br>Warteschlangendefinition<br>Themengruppe &quot;Warteschlange&quot;<br>Warteschlangenthema<br>Routing-Regel<br>Milestone-Pfad<br>Milestone<br>Stündentyp<br>Ressourcenpool<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |
| Vorlage (TMPL) | Vorlage<br>Vorlagenaufgabe<br>Vorlagenaufgaben zuweisen<br>VorlagenTask-Vorgänger<br>Firma<br>Überschreibungsrate<br>Gruppe<br>Rolle<br>Team<br>Validierungsprozess<br>Validierungspfad<br>Validierungsschritt<br>Schritt-Genehmiger<br>Zeitplan<br>Nichtarbeitstag<br>Warteschlangendefinition<br>Themengruppe &quot;Warteschlange&quot;<br>Warteschlangenthema<br>Routing-Regel<br>Milestone-Pfad<br>Milestone<br>Stündentyp<br>Ressourcenpool<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |

### Reporting-Objekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Layout Template (UITMPL) | Layout-Vorlage<br>Dashboard<br>Kalender<br>Kalenderabschnitt<br>Externe Seite<br>Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter |
| Dashboard (PTLTAB) | Dashboard<br>Kalender<br>Kalenderabschnitt<br>Externe Seite<br>Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter |
| Kalender (CALEND) | Kalender<br>Kalenderabschnitt |
| Externe Seite (EXTSEC) | Externe Seite |
| Bericht (PTLSEC) | Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter |
| Filter (UIFT) | Filter<br>Parameter |
| Gruppierung (UIGB) | Gruppierung<br>Parameter |
| Anzeigen (UIVW) | Ansicht<br>Parameter |

### Benutzerdefinierte Datenobjekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Kategorie (KG) | Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik<br>Gruppe |
| Parameter (PARAM) | Parameter<br>Parameteroption |
| Parametergruppe (PGRP) | Parametergruppe |

### Organisationsobjekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Gruppe (GRUPPE) | Gruppe <br>Untergruppen (bis zu 5 Stufen) *<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |
| Rolle (ROLE) | Funktion |
| Team (TEAM) | Team<br>Gruppe |
| Unternehmen (CMPY) | Firma<br>Überschreibungsrate<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameter <br>Kategorieanzeigelogik<br>Gruppe |
| Portfolio (HAFEN) | Portfolio<br>Programm<br>Gruppe<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |
| Programm (PRGM) | Programm<br>Portfolio<br>Gruppe<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |

### Andere Konfigurationsobjekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Genehmigungsverfahren (ARVVR) | Validierungsprozess<br>Validierungspfad<br>Validierungsschritt<br>Schritt-Genehmiger<br>Rolle<br>Team<br>Gruppe |
| Zeitplan (SCHED) | Zeitplan<br>Nichtarbeitstag<br>Gruppe |
| Meilensteinpfad (MPATH) | Milestone-Pfad<br>Milestone |
| Datenblatt-Profil (TSPRO) | Datenblatt-Profil<br>Stündentyp |
| Stundentyp (STUNDE) | Stundentyp |
| Ausgabentyp (EXPTYP) | Ausgabentyp |
| Risikotyp (RSKTYP) | Risikotyp |
| Ressourcen-Pool (RSPL) | Ressourcenpool |

\* Derzeit nicht verfügbar


## Status der Umgebungsförderung

Förderungspakete für die Umgebung durchlaufen mehrere Status, während sie erstellt und für den Wechsel zwischen Umgebungen vorbereitet werden. Sie können diese Status in Ihrer Paketliste innerhalb von Workfront oder in den API-Antworten sehen, wenn Sie die Workfront-API verwenden.

Zu diesen Status gehören:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>ASSEMBLING</td> 
   <td><p>Dieser Status wird automatisch zugewiesen, während Objekte assembliert werden. </p><p>Das Assemblieren bezieht sich auf den automatisierten Prozess zum Identifizieren von Objekten und Unterobjekten, die in ein Package aufgenommen werden sollen, und zum Hinzufügen dieser Objekte und ihrer Daten zum Paket.</p><p>Dieser Status kann nicht direkt von einem Kunden festgelegt werden.</p></td> 
  </tr> 
  <tr> 
   <td>ENTWURF</td> 
   <td><p>Dieser Status wird beim Abschluss eines Assemblyprozesses oder beim Erstellen eines leeren Promotion-Pakets zugewiesen.</p><p>Es ist möglich, dass ein Kunde das Promotion-Paket zurück in diesen Status verschiebt.</p><p>In diesem Status kann das Promotion-Paket in keiner Umgebung installiert werden.</p></td> 
  </tr> 
  <tr> 
   <td>TESTEN</td> 
   <td><p>Dieser Status ermöglicht die Installation eines Promotion-Pakets in jeder Vorschau- oder benutzerdefinierten Aktualisierungs-Sandbox. In diesem Status kann das Paket nicht in der Produktion installiert werden.</p></td> 
  </tr> 
  <tr> 
   <td>AKTIV</td> 
   <td><p>Dieser Status ermöglicht die Installation eines Promotion-Pakets in einer beliebigen Umgebung, einschließlich der Produktion.</p><p>Wenn ein Paketstatus auf "ACTIVE"gesetzt ist, wird die <code>publishedAt</code> Datum wird automatisch auf den aktuellen Zeitstempel der Anforderung gesetzt.</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>Dieser Status wird verwendet, um zuvor verwendete Promotionspakete auszublenden, die in Zukunft in keiner Umgebung installiert werden.</p><p>Wenn ein Paket diesen Status aufweist, kann es in keiner Umgebung installiert werden.</p><p>Wenn ein Paketstatus auf DEAKTIVIERT gesetzt ist, wird die <code>retiredAt</code> Datum wird automatisch auf den aktuellen Zeitstempel der Anforderung gesetzt.</p><p>Die Verwendung dieses Status wird empfohlen, da die<code>DELETE /package</code> -Endpunkt, da er abgerufen werden kann und der Installationsverlauf für alle Implementierungen, die mit diesem Paket vorgenommen werden, beibehalten wird.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Wenn die ASSEMBLING-Phase fehlschlägt, wird das Promotionpaket automatisch in diesen Status versetzt.</p><p>Um das Package in die Phase der ASSEMBLING zurückzusetzen, müssen Sie den Extraktionsvorgang erneut Trigger haben.</p></td> 
  </tr> 
  </tbody> 
</table>
