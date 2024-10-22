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
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: a46c6d1f8a0ae58e07f0fb9d14ecdd06a856223f
workflow-type: tm+mt
source-wordcount: '1019'
ht-degree: 2%

---

# Übersicht über das Verschieben von Objekten zwischen Workfront-Umgebungen (Umgebungsförderung)

Mit der Umgebungsförderungsfunktion können Sie Objekte von einer Workfront-Umgebung in eine andere verschieben. Sie können beispielsweise eine Vorlage erstellen und in Ihrer Sandbox-Umgebung konfigurieren, in dem Wissen, dass sich Tests, die Sie durchführen, nicht auf die tatsächlichen Daten Ihrer Organisation auswirken. Nachdem die Vorlage konfiguriert und getestet wurde, können Sie sie in Ihre Produktionsumgebung verschieben, damit sie einsatzbereit ist.

Dieser Prozess wird als &quot;Umweltförderung&quot;bezeichnet.

Sie können diesen Vorgang in Workfront durchführen, indem Sie ein Objekt-Package erstellen, das verschoben werden soll, und dieses Package dann in der neuen Umgebung installieren.

* Spezifische Anweisungen zur Durchführung dieses Prozesses in Workfront finden Sie unter:

   * [Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Installieren eines Umgebungsförderungspakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Anweisungen zum Ausführen dieses Vorgangs über die Workfront-API finden Sie unter [Objekte mithilfe der API [!DNL Workfront] API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md) zwischen [!DNL Workfront] Umgebungen verschieben.

[Sehen Sie sich eine Videodemonstration für diese Funktion an](https://video.tv.adobe.com/v/3429735/){target=_blank}

## Unterstützte Objekte für die Umgebungsförderung

Die Umgebungsförderungsfunktion soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Dies sind Objekte, die konfiguriert werden können, z. B. Projekte, Teams oder benutzerdefinierte Formulare.

Da die Umgebungswerbung die Objektkonfiguration behandelt, sind Transaktionsobjekte (Objekte, die sich häufig ändern oder von Anwendungsfällen stark abhängig sind) nicht enthalten. Beispiele für Transaktionsobjekte sind Dokumente, Probleme, Anfragen, Aktualisierungen und Testentscheidungen.

* [Arbeitsobjekte](#work-objects)
* [Reporting-Objekte](#reporting-objects)
* [Benutzerdefinierte Datenobjekte](#custom-data-objects)
* [Organisationsobjekte](#organization-objects)
* [Andere Konfigurationsobjekte](#other-configuration-objects)


### Arbeitsobjekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Projekt (PROJ) | Projekt<br>Aufgabe<br>Zuweisung<br>Vorgänger<br>Firma<br>Überschreiben der Rate<br>Gruppe<br>Rolle<br>Team<br>Genehmigungsprozess<br>Genehmigungspfad<br>Genehmigungs-Schritt<br>Schritt-Genehmiger<br>Zeitplan<br>Nicht Arbeitstag<br>Warteschlangendefinition<br>Warteschlangenthementgruppe{1 6}Queue Topic<br>Routing Rule<br>Milestone Path<br>Milestone<br>Hour Type<br>Resource Pool<br>Category<br>Category Parameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik<br> |
| Vorlage (TMPL) | Vorlage<br>Vorlagenaufgabe<br>Vorlagenaufgabe-Zuweisung<br>Vorlagenaufgaben-Vorgänger<br>Firma<br>Überschreibungsrate<br>Gruppe<br>Rolle<br>Team<br>Genehmigungsprozess<br>Genehmigungspfad<br>Genehmigungsschritt<br>Schritt-Genehmiger<br>Zeitplan<br>Nicht-Arbeitstag<br>Warteschlangendefinition<br>Warteschlange ic group<br>Queue topic<br>Routing rule<br>Milestone path<br>milestone<br>Hour Type<br>Resource Pool<br>Category<br>Category Parameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |

### Reporting-Objekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Layout Template (UITMPL) | Layout template<br>Dashboard<br>Calendar<br>Calendar section<br>External Page<br>report<br>filter<br>Grouping<br>view<br>parameter<br>group |
| Dashboard (PTLTAB) | Dashboard<br>Kalender<br>Kalenderabschnitt<br>Externe Seite<br>Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter |
| Kalender (CALEND) | Calendar<br>Kalenderabschnitt |
| Externe Seite (EXTSEC) | Externe Seite |
| Bericht (PTLSEC) | Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter |
| Filter (UIFT) | Filter<br>Parameter |
| Gruppierung (UIGB) | Grouping<br>Parameter |
| Anzeigen (UIVW) | Parameter anzeigen<br> |

### Benutzerdefinierte Datenobjekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Kategorie (KG) | Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik<br>Gruppe |
| Parameter (PARAM) | Parameter<br>Parameteroption |
| Parametergruppe (PGRP) | Parametergruppe |

### Organisationsobjekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Gruppe (GRUPPE) | Gruppe <br>Untergruppen (bis zu 5 Ebenen) *<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Logik der Kategorieanzeige |
| Rolle (ROLE) | Funktion |
| Team (TEAM) | Team<br>group |
| Unternehmen (CMPY) | Unternehmen<br>Überschreibungsrate<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameter <br>Kategorieanzeigelogik<br>Gruppe |
| Portfolio (HAFEN) | Portfolio<br>Programm<br>Gruppe<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |
| Programm (PRGM) | Programm<br>Portfolio<br>Gruppe<br>Kategorie<br>Kategorieparameter<br>Parameter<br>Parametergruppe<br>Parameteroption<br>Kategorieanzeigelogik |

### Andere Konfigurationsobjekte

| Förderbares Objekt | Einbezogene förderfähige verknüpfte Objekte |
| --- | --- |
| Genehmigungsverfahren (ARVVR) | Genehmigungsprozess<br>Genehmigungspfad<br>Genehmigungsschritt<br>Schritt-Genehmiger<br>Rolle<br>Team<br>Gruppe |
| Zeitplan (SCHED) | Zeitplan<br>Nicht-Arbeitstag<br> Gruppe |
| Meilensteinpfad (MPATH) | Milestone Path<br>Milestone |
| Datenblatt-Profil (TSPRO) | Datenblatt-Profil<br>Stündentyp |
| Stundentyp (STUNDE) | Stundentyp |
| Ausgabentyp (EXPTYP) | Ausgabentyp |
| Risikotyp (RSKTYP) | Risikotyp |
| Ressourcen-Pool (RSPL) | Ressourcen-Pool |
| Zugriffsstufe (ACSLVL) | Zugriffsebene |
| Ratenkarte (RTCRD) | Tarifkarte |

\* Derzeit nicht verfügbar

<!--

>[!NOTE]
>
>Actions (ignore, select existing, and create new) are available on the following objects:
>
>* Role
>* Team
>* Company
>* Group

-->

## Status der Umgebungsförderung

Förderungspakete für die Umgebung durchlaufen mehrere Status, während sie erstellt und für den Wechsel zwischen Umgebungen vorbereitet werden. Sie können diese Status in Ihrer Paketliste innerhalb von Workfront oder in den API-Antworten sehen, wenn Sie die Workfront-API verwenden.

Zu diesen Status gehören:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>UNASSEMBLED</td> 
   <td><p>Dieser Status wird automatisch zugewiesen und stellt ein Paket dar, das gespeichert, aber noch nicht zusammengestellt wurde. </p><p>Dieser Status kann nicht direkt von einem Benutzer festgelegt werden.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING</td> 
   <td><p>Dieser Status wird automatisch zugewiesen, während Objekte assembliert werden. </p><p>Das Assemblieren bezieht sich auf den automatisierten Prozess zum Identifizieren von Objekten und Unterobjekten, die in ein Package aufgenommen werden sollen, und zum Hinzufügen dieser Objekte und ihrer Daten zum Paket.</p><p>Dieser Status kann nicht direkt von einem Benutzer festgelegt werden.</p></td> 
  </tr> 
  <tr> 
   <td>ENTWURF</td> 
   <td><p>Dieser Status wird beim Abschluss eines Assemblyprozesses oder beim Erstellen eines leeren Promotion-Pakets zugewiesen.</p><p>Es ist möglich, dass ein Benutzer das Promotion-Paket zurück in diesen Status verschiebt.</p><p>In diesem Status kann das Promotion-Paket in keiner Umgebung installiert werden.</p></td> 
  </tr> 
  <tr> 
   <td>TESTEN</td> 
   <td><p>Dieser Status ermöglicht die Installation eines Promotion-Pakets in jeder Vorschau- oder benutzerdefinierten Aktualisierungs-Sandbox. In diesem Status kann das Paket nicht in der Produktion installiert werden.</p></td> 
  </tr> 
  <tr> 
   <td>AKTIV</td> 
   <td><p>Dieser Status ermöglicht die Installation eines Promotion-Pakets in einer beliebigen Umgebung, einschließlich der Produktion.</p><p>Wenn ein Paketstatus auf AKTIV gesetzt ist, wird das Datum <code>publishedAt</code> automatisch auf den aktuellen Zeitstempel der Anfrage gesetzt.</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>Dieser Status wird verwendet, um zuvor verwendete Promotionspakete auszublenden, die in Zukunft in keiner Umgebung installiert werden.</p><p>Wenn ein Paket diesen Status aufweist, kann es in keiner Umgebung installiert werden.</p><p>Wenn ein Paketstatus auf DEAKTIVIERT gesetzt ist, wird das Datum <code>retiredAt</code> automatisch auf den aktuellen Zeitstempel der Anfrage gesetzt.</p><p>Die Verwendung dieses Status wird für die Verwendung des Endpunkts <code>DELETE /package</code> empfohlen, da dieser abgerufen werden kann und der Installationsverlauf für alle Implementierungen, die mit diesem Paket durchgeführt werden, beibehalten wird.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Wenn die ASSEMBLING-Phase fehlschlägt, wird das Promotionpaket automatisch in diesen Status versetzt.</p><p>Um das Package in die Phase der ASSEMBLING zurückzusetzen, müssen Sie den Assembling-Prozess erneut Trigger haben.</p><p>Weitere Informationen zum Zusammenstellen eines Pakets finden Sie im Abschnitt <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">Bearbeiten oder Zusammenführen eines vorhandenen Pakets</a> im Artikel Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets.</td> 
  </tr> 
  </tbody> 
</table>

