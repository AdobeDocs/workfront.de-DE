---
title: Arbeitsbereiche - Übersicht
description: Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitszyklus des Teams darstellen. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig an die Workflows Ihrer Organisationseinheiten anpassen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
source-git-commit: 31aff197d6af521df2258f3f99fea6fb5785b9e3
workflow-type: tm+mt
source-wordcount: '388'
ht-degree: 4%

---

# Überblick über Arbeitsbereiche

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einer Organisationseinheit verwendet werden. Er stellt den Arbeitszyklus und die Prozesse der Einheit dar. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig anpassen.


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
* Abhängig von Ihrer Workfront-Lizenz werden Arbeitsbereiche auf den folgenden Registerkarten im Bereich Planung angezeigt:

   * Für Systemadministratoren werden Arbeitsbereiche auf den folgenden Registerkarten angezeigt:

      * **Arbeitsbereiche, an denen ich mitwirke**: Zeigt von Ihnen erstellte Arbeitsbereiche oder Arbeitsbereiche an, die für Sie freigegeben sind.
      * **Andere Arbeitsbereiche**: Zeigt alle anderen Arbeitsbereiche im System an.

   * Für alle anderen Benutzer werden die von ihnen erstellten Arbeitsbereiche und die von anderen für sie freigegebenen Arbeitsbereiche im Arbeitsbereich angezeigt.

* Die Datensatztypen, die ein Arbeitsbereich enthält, sollten den Arbeitszyklus und die Konzepte einer Organisationseinheit widerspiegeln.

  Wenn es sich bei den Arbeitsobjekten einer Einheit beispielsweise um Kampagnen, Produkte und Regionen handelt, sollte der Arbeitsbereich dieser Einheit die Datensatztypen von Kampagne, Produkt und Region enthalten.
* Wenn Sie einen Arbeitsbereich erstellen, sind nur Sie berechtigt, auf Ihren Arbeitsbereich zuzugreifen und ihn zu verwalten. Sie müssen sie für andere Benutzer freigeben, damit diese im selben Bereich mit Ihnen zusammenarbeiten können.

  Weitere Informationen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md).

  Systemadministratoren können alle Arbeitsbereiche verwalten, auch die, die sie nicht erstellt haben.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Es gibt Beschränkungen für die Anzahl der Workspace-Objekte, die Sie in Ihrer Instanz von Workfront Planning erstellen können. Weitere Informationen finden Sie unter [Übersicht über Adobe Workfront Planning-Objektbeschränkungen](/help/quicksilver/planning/general/limitations-overview.md).
