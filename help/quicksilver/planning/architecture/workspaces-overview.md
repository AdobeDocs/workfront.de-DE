---
title: Arbeitsbereiche - Übersicht
description: Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitszyklus des Teams darstellen. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig an die Workflows Ihrer Organisationseinheiten anpassen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
TQID: https://experienceleague.adobe.com/Hh1Gh4ex1dLrPhsmqiLv3x5NAU0yKzIwcsV4hEogXTo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 4ac828444e49213cdc4e00a5f92e404899e2225d
workflow-type: tm+mt
source-wordcount: 608
ht-degree: 3%

---

# Überblick über Arbeitsbereiche

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einer Organisationseinheit verwendet werden. Er stellt den Arbeitszyklus und die Prozesse der Einheit dar. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig anpassen.

<!--update screenshot with production, it was broken at Preview-->

![Workspaces Landingpage-Administratorkonto](assets/workspaces-landing-page-admin-account.png)

## Überlegungen zu Arbeitsbereichen

* Sie können Arbeitsbereiche für bestimmte Organisationseinheiten innerhalb Ihrer Organisation erstellen, die der Funktionsweise jeder Einheit entsprechen.
* Workfront Planning verfügt über keine vorkonfigurierten Arbeitsbereiche. Sie müssen sie entsprechend den Anforderungen Ihres Unternehmens erstellen.
* Sie können Arbeitsbereiche wie folgt erstellen:

   * Neu
   * Verwenden einer Vorlage. Vorlagen enthalten eine vorkonfigurierte Anzahl von Datensatztypen und deren Feldern.
   * Verwenden der KI-gestützten Planungs-Designer. Diese Funktion befindet sich derzeit in Beta.
   * Verwenden eines Vorlagenpakets für mehrere Arbeitsbereiche.

  Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

* Arbeitsbereiche sind Frameworks, in denen Ihre Organisationseinheiten (ein Team, eine Gruppe, eine Abteilung oder ein Unternehmensbereich) arbeiten. Sie können nicht mit Feldern verknüpft werden. Nur die Datensatztypen innerhalb eines Arbeitsbereichs können Feldern zugeordnet werden.

  Weitere Informationen finden Sie unter [Datensatztypen - Übersicht](/help/quicksilver/planning/architecture/overview-of-record-types.md).
* Arbeitsbereiche werden auf den folgenden Registerkarten im Bereich Planung angezeigt:

   * **Arbeitsbereiche, an denen ich mitwirke**: Zeigt von Ihnen erstellte Arbeitsbereiche oder Arbeitsbereiche an, die für Sie freigegeben sind.
   * **Andere Arbeitsbereiche**: Zeigt alle anderen Arbeitsbereiche im System an. Dies ist nur für Systemadministratoren verfügbar.
   * <span class="preview">**Beispiel-Arbeitsbereiche**: Zeigt integrierte Beispiele für Best Practice-Arbeitsbereiche an. Sie können die Arbeitsbereiche, Datensatztypen oder Datensätze oder Felder nicht bearbeiten, aber Sie können Ansichten hinzufügen, bearbeiten und für andere freigeben.</span>

  >[!NOTE]
  >
  ><span class="preview">Es wird empfohlen, die Beispiel-Arbeitsbereiche nicht zu bearbeiten, sondern sie als Referenz zum Erstellen eigener Arbeitsbereiche zu verwenden. Verwenden Sie das Vorlagenpaket für mehrere Arbeitsbereiche , um Arbeitsbereiche zu erstellen, die mit den auf der Registerkarte Beispiel-Arbeitsbereiche aufgeführten Arbeitsbereichen identisch sind. Weitere Informationen finden Sie im Abschnitt „Erstellen mehrerer Arbeitsbereiche mithilfe eines Best-Practice-Vorlagenpakets für mehrere Arbeitsbereiche“ im Artikel [Erstellen von &#x200B;](/help/quicksilver/planning/architecture/create-workspaces.md)&quot; </span>

<!--
No longer the case - they match now: 

* For all other users:

* **Workspaces I'm on**: Workspaces they created (for Standard-license users) and workspaces others shared with them display in the Workspaces area.

<div class="preview"> 

* **Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.

</div>
-->



* Die Datensatztypen, die ein Arbeitsbereich enthält, sollten den Arbeitszyklus und die Konzepte einer Organisationseinheit widerspiegeln.

  Wenn es sich bei den Arbeitsobjekten einer Einheit beispielsweise um Kampagnen, Produkte und Regionen handelt, sollte der Arbeitsbereich dieser Einheit die Datensatztypen von Kampagne, Produkt und Region enthalten.
* Wenn Sie einen Arbeitsbereich erstellen, sind nur Sie berechtigt, auf Ihren Arbeitsbereich zuzugreifen und ihn zu verwalten. Sie müssen sie für andere Benutzer freigeben, damit diese im selben Bereich mit Ihnen zusammenarbeiten können.

  Weitere Informationen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md).

  Systemadministratoren können alle Arbeitsbereiche verwalten, auch die, die sie nicht erstellt haben.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Es gibt Beschränkungen für die Anzahl der Workspace-Objekte, die Sie in Ihrer Instanz von Workfront Planning erstellen können. Weitere Informationen finden Sie unter [Übersicht über Adobe Workfront Planning-Objektbeschränkungen](/help/quicksilver/planning/general/limitations-overview.md).

## Überblick über die globale Suche

Auf der Landingpage Planning können Sie mithilfe des globalen Suchfelds nach den folgenden Planning-Objekten suchen:

* Arbeitsbereiche
* Eintragstypen
* Ansichten

![Globales Suchfeld](assets/global-search-box.png)

Beachten Sie Folgendes zur Verwendung der globalen Suche:

* Sie können die Suche über die Planning-Landingpage oder über eine beliebige Planning-Seite aufrufen, indem Sie die folgende Tastenkombination drücken:

   * STRG+K für Windows
   * ⌘+K für Mac
* Die letzten 7 Ergebnisse von jedem Objekt werden im Suchfeld angezeigt.
* Sie können eine allgemeine Suche durchführen oder ein Objekt auswählen und einzelne Listen durchsuchen.


