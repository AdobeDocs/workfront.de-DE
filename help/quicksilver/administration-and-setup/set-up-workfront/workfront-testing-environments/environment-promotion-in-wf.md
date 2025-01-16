---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Verschieben von Objekten von einer Umgebung in eine andere innerhalb von Workfront
description: Die Funktion Umgebungsförderung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Das Verschieben von Transaktionsobjekten wird nicht unterstützt (mit wenigen Ausnahmen).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 8b4c04f5-f519-44e9-8429-0ce80c2d7c5b
source-git-commit: 9a588df1ef48b40056c5228c8ff03b5819eb4410
workflow-type: tm+mt
source-wordcount: '1041'
ht-degree: 2%

---

# Übersicht über das Verschieben von Objekten zwischen Workfront-Umgebungen (Umgebungs-Promotion)

Mit der Funktion zum Hochstufen der Umgebung können Sie Objekte von einer Workfront-Umgebung in eine andere verschieben. Sie können beispielsweise eine Vorlage erstellen und in Ihrer Sandbox-Umgebung konfigurieren, in dem Wissen, dass Tests, die Sie durchführen, keine Auswirkungen auf die tatsächlichen Daten Ihrer Organisation haben. Nachdem die Vorlage konfiguriert und getestet wurde, können Sie sie in Ihre Produktionsumgebung verschieben, sodass sie verwendet werden kann.

Dieser Prozess wird als „Umgebungsförderung“ bezeichnet.

Sie können diesen Prozess in Workfront durchführen, indem Sie ein Paket von zu verschiebenden Objekten erstellen und dieses Paket dann in der neuen Umgebung installieren.

* Spezifische Anweisungen zum Ausführen dieses Prozesses in Workfront finden Sie unter:

   * [Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-create-package.md)
   * [Installieren eines Umgebungs-Promotion-Pakets](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-install-package.md)

* Anweisungen zum Ausführen dieses Prozesses über die Workfront-API finden Sie unter [Verschieben von Objekten zwischen  [!DNL Workfront]  mithilfe der  [!DNL Workfront] -API](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion.md).

[Sehen Sie sich eine Videodemonstration dieser Funktion an](https://video.tv.adobe.com/v/3429735/){target=_blank}

## Unterstützte Objekte für die Umgebungs-Promotion

Die Funktion zum Hochstufen der Umgebung soll die Möglichkeit bieten, konfigurationsbezogene Objekte von einer Umgebung in eine andere zu verschieben. Hierbei handelt es sich um Objekte, die konfiguriert werden können, z. B. Projekte, Teams oder benutzerdefinierte Formulare.

Da sich die Umgebungsförderung mit der Objektkonfiguration befasst, werden Transaktionsobjekte (Objekte, die sich häufig ändern oder stark vom Anwendungsfall abhängig sind) nicht einbezogen. Beispiele für Transaktionsobjekte sind Dokumente, Probleme, Anfragen, Aktualisierungen und Korrekturabzugsentscheidungen.

* [Arbeitsobjekte](#work-objects)
* [Berichterstellungsobjekte](#reporting-objects)
* [Benutzerdefinierte Datenobjekte](#custom-data-objects)
* [Organisationsobjekte](#organization-objects)
* [Andere Konfigurationsobjekte](#other-configuration-objects)


### Arbeitsobjekte

| Promotable-Objekt | Eingeschlossene werbefähige verknüpfte Objekte |
| --- | --- |
| Projekt (PROJ) | Projekt<br>Aufgabe<br>Zuweisung<br>Vorgänger<br>Unternehmen<br>Überschreibungsrate<br>Gruppe<br>Rolle<br>Team<br>Genehmigungsprozess<br>Genehmigungspfad<br>Genehmigungsschritt<br><br> Zeitplaner<br>Nicht-Arbeitstag<br><br> <br> <br> <br> <br> <br> <br> <br> <br> <br> <br> <br> <br> Warteschlangendefinition Logik |
| Vorlage (TMPL) | template<br>template task<br>template task assignment<br>template task precessor<br>company<br>override rate<br>group<br>role<br>team<br>approval path<br>approval step<br>step approver<br>scheduleday<br>queueDefinition<br>Themengruppe<br>queue e Topic<br>route<br><br><br><br><br><br><br><br><br> <br> <br> Option<br>Logik für Kategorieanzeige |

### Berichterstellungsobjekte

| Promotable-Objekt | Eingeschlossene werbefähige verknüpfte Objekte |
| --- | --- |
| Layoutvorlage (UTIMPL) | Layout-Vorlage<br>Dashboard<br>Kalender<br>Kalenderabschnitt<br>Externe Seite<br>Bericht<br>Filter<br>Gruppierung<br>Ansicht<br>Parameter<br>group |
| Dashboard (PTLTAB) | dashboard<br>calendar<br>calendar section<br>external page<br>report<br>filter<br>grouping<br>view<br>parameter |
| Kalender (KALENDER) | <br> |
| Externe Seite (EXTEC) | Externe Seite |
| Bericht (PTLSEC) | report<br>filter<br>grouping<br>view<br>parameter |
| Filter (UIFT) | <br> |
| Gruppierung (UIGB) | grouping<br>parameter |
| Ansicht (UIVW) | <br> |

### Benutzerdefinierte Datenobjekte

| Promotable-Objekt | Eingeschlossene werbefähige verknüpfte Objekte |
| --- | --- |
| Kategorie (CTG) | category<br>category Parameter<br>parameter<br>parameter group<br>parameter option<br>category display logic<br>group |
| Parameter (PARAM) | <br> |
| Parametergruppe (PGRP) | Parametergruppe |

### Organisationsobjekte

| Promotable-Objekt | Eingeschlossene werbefähige verknüpfte Objekte |
| --- | --- |
| Gruppe (GROUP) | Gruppe <br>Untergruppen (bis zu 5 Ebenen) *<br>Kategorie<br>Kategorie Parameter<br>Parameter<br>Parametergruppe<br>Parameter Option<br>Kategorie Anzeigelogik |
| Rolle (ROLE) | Funktion |
| Team (Team) | <br> |
| Firma (COMPY) | Firma<br>Überschreibungsrate<br>Kategorie<br>Kategorie Parameter<br>Parameter<br>Parametergruppe<br>Parameter <br>Kategorieanzeigelogik<br>Gruppe |
| Portfolio (PORT) | Portfolio <br>Programm<br>Gruppe<br>Kategorie<br>Kategorie Parameter<br>Parameter<br>Parametergruppe<br>Parameter Option<br>Kategorieanzeigelogik |
| Programm (PRGM) | Programm<br>Portfolio <br>Gruppe<br>Kategorie<br>Kategorie Parameter<br>Parameter<br>Parametergruppe<br>Parameter Option<br>Kategorieanzeigelogik |

### Andere Konfigurationsobjekte

| Promotable-Objekt | Eingeschlossene werbefähige verknüpfte Objekte |
| --- | --- |
| Genehmigungsprozess (ARVPRC) | Genehmigungsprozess<br>Genehmigungspfad<br>Genehmigungsschritt<br>Schritt Genehmiger<br>Rolle<br>Team<br>Gruppe |
| Zeitplan (SCHED) | Schedule<br>non-work day<br>group |
| Meilensteinpfad (MPATH) | Meilensteinpfad<br>Meilenstein |
| Arbeitszeittabellen-Profil (TSPRO) | Arbeitszeittabellen<br>Profil/Stundentyp |
| Stundentyp (STUNDE) | Stundentyp |
| Ausgabentyp (EXPTYP) | Ausgabentyp |
| Risikotyp (RSKTYP) | Risikotyp |
| Ressourcenpool (RSPL) | Ressourcen-Pool |
| Zugriffsebene (ACSLV) | Zugriffsebene |
| Tarifkarte (RTCR) | Tarifkarte |
| Speicherort/Klassifikator (CLSF) | Speicherort/Klassifikator |

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

## Umgebungsförderungsstatus

Umgebungs-Promotion-Pakete durchlaufen beim Erstellen und Vorbereiten des Wechsels zwischen Umgebungen mehrere Status. Sie können diese Status in Ihrer Paketliste in Workfront oder in den API-Antworten sehen, wenn Sie die Workfront-API verwenden.

Zu diesen Status gehören:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>NICHT MONTIERT</td> 
   <td><p>Dieser Status wird automatisch zugewiesen und stellt ein Paket dar, das gespeichert, aber noch nicht zusammengestellt wurde. </p><p>Dieser Status kann nicht direkt von einem Benutzer festgelegt werden.</p></td> 
  </tr> 
  <tr> 
   <td>ZUSAMMENSTELLEN</td> 
   <td><p>Dieser Status wird beim Zusammenfügen von Objekten automatisch zugewiesen. </p><p>Das Zusammenstellen bezieht sich auf den automatisierten Prozess der Identifizierung von Objekten und Unterobjekten, die in ein Paket aufgenommen werden sollen, und des Hinzufügens dieser Objekte und ihrer Daten zum Paket.</p><p>Dieser Status kann nicht direkt von einem Benutzer festgelegt werden.</p></td> 
  </tr> 
  <tr> 
   <td>ENTWURF</td> 
   <td><p>Dieser Status wird bei Abschluss eines Montageprozesses oder bei der Erstellung eines leeren Promotion-Pakets zugewiesen.</p><p>Ein Benutzer kann das Promotion-Paket zurück in diesen Status verschieben.</p><p>In diesem Status kann das Promotion-Paket in keiner Umgebung installiert werden.</p></td> 
  </tr> 
  <tr> 
   <td>TESTING</td> 
   <td><p>Mit diesem Status kann ein Promotion-Paket in jeder Vorschau- oder benutzerdefinierten Aktualisierungs-Sandbox installiert werden. In diesem Status kann das Paket nicht in der Produktion installiert werden.</p></td> 
  </tr> 
  <tr> 
   <td>AKTIV</td> 
   <td><p>Dieser Status ermöglicht die Installation eines Promotion-Pakets in jeder Umgebung, einschließlich Produktion.</p><p>Wenn der Status eines Pakets auf AKTIV gesetzt ist, wird das <code>publishedAt</code> automatisch auf den aktuellen Zeitstempel der Anfrage festgelegt.</p></td> 
  </tr> 
  <tr> 
   <td>DISABLED</td> 
   <td><p>Dieser Status wird verwendet, um zuvor verwendete Promotion-Pakete auszublenden, die in Zukunft in keiner Umgebung installiert werden.</p><p>Wenn sich ein Paket in diesem Status befindet, kann es in keiner Umgebung installiert werden.</p><p>Wenn ein Paketstatus auf DEAKTIVIERT gesetzt ist, wird das <code>retiredAt</code> automatisch auf den aktuellen Zeitstempel der Anfrage gesetzt.</p><p>Die Verwendung dieses Status wird anstelle des <code>DELETE /package</code>-Endpunkts empfohlen, da er abrufbar ist und der Installationsverlauf für alle Bereitstellungen mit diesem Paket beibehalten wird.</p></td> 
  </tr> 
  <tr> 
   <td>ASSEMBLING_FAILED</td> 
   <td><p>Das Promotion-Paket wird automatisch in diesen Status versetzt, wenn die MONTAGE fehlschlägt.</p><p>Um das Paket wieder in die MONTAGE-Phase einzubringen, muss der Zusammenstellungsprozess erneut Trigger werden.</p><p>Einzelheiten zum Zusammenstellen eines Pakets finden Sie im Abschnitt <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/testing-environments/environment-promotion-create-package#edit-or-assemble-an-existing-package">Bearbeiten oder Zusammenstellen eines vorhandenen Pakets</a> im Artikel Erstellen oder Bearbeiten eines Umgebungs-Promotion-Pakets.</td> 
  </tr> 
  </tbody> 
</table>

## Ressourcen

* Häufig gestellte Fragen zur Umgebungsförderung finden Sie unter [FAQ zur Umgebungsförderung](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-faq.md)
* Empfehlungen zur Fehlerbehebung finden Sie unter [Fehlerbehebung bei der Umgebungsförderung](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-troubleshooting.md)


