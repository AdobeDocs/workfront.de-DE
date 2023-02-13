---
content-type: overview
product-area: resource-management
navigation-topic: resource-scheduling
title: Übersicht über die Planungsbereiche
description: In den folgenden Abschnitten wird beschrieben, wo Sie auf den Planungsbereich in Adobe Workfront zugreifen können und welche Funktionen im Planungsbereich verfügbar sind.
author: Alina
feature: Resource Management
exl-id: ed6f1db9-917d-4a19-9fd4-1ed5d2ca95fb
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '1790'
ht-degree: 0%

---

# Übersicht über die Planungsbereiche

>[!IMPORTANT]
>  
><span class="preview">Die in diesem Artikel beschriebene Planungsfunktion wird seit der Version 23.1 im Januar 2023 nicht mehr unterstützt und aus Adobe Workfront entfernt.   </span>
>  
> <span class="preview"> Dieser Artikel wird auch kurz nach der Version 23.1 (Anfang 2023) entfernt. Zu diesem Zeitpunkt empfehlen wir, alle Lesezeichen entsprechend zu aktualisieren. </span>
> 
><span class="preview"> Sie können jetzt den Lastenausgleich verwenden, um die Arbeit für Ihre Ressourcen zu planen. </span>
>  
> <span class="preview">Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie im Abschnitt [Der Lastenausgleich](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--  

>[!CAUTION] 
> 
> 
> <span class="preview">The information in this article refers to the Adobe Workfront's Scheduling tools. The Scheduling areas have been removed from the Preview environment and will be removed from the Production environment in **January 2023**. </span> 
> <span class="preview"> Instead, you can schedule resources in the Workload Balancer. </span> 
> 
>* <span class="preview"> For information about scheduling resources using the Workload Balancer, see the section [The Workload Balancer](../../resource-mgmt/workload-balancer/workload-balancer.md).</span> 
> 
>* <span class="preview"> For more information about the deprecation and removal of the Scheduling tools, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).</span> 

-->


In den folgenden Abschnitten wird beschrieben, wo Sie auf den Planungsbereich in Adobe Workfront zugreifen können und welche Funktionen im Planungsbereich verfügbar sind.

## Workfront-Bereiche, in denen Sie Ressourcen planen können

Sie können Ressourcen in den folgenden Bereichen in Workfront planen:

* **Für alle Projekte, für die Sie Ressourcen-Manager sind** (aus dem **Planung** Bereich) Der Bereich Planung in Workfront ermöglicht es Ressourcenmanagern, Ressourcenzuweisungen über mehrere Projekte hinweg vorzunehmen.

* **Für ein einzelnes Projekt, wenn Sie Mitglied des Projektteams sind** (aus dem **Planung** Bereich eines Projekts):

   Über den Bereich Planung innerhalb eines Projekts können Mitglieder des Projektteams den Benutzern im Projekt-Team Arbeit aus dem Projekt zuweisen.

* **Für ein einzelnes Team sind Sie Mitglied von** (aus dem **Zeitplan** -Bereich des Teams) Im Bereich Planung eines Teams können Team-Mitglieder dem Team bereits zugewiesene Aufgaben aus mehreren Projekten einzelnen Team-Mitgliedern zuweisen.

## Im Bereich Planung verfügbare Funktionen

Im Planungsbereich werden Aufgaben und Probleme sowie aktuelle Ressourcenzuweisungen angezeigt.\
![resource_scheduling_overview.png](assets/resource-scheduling-overview-350x237.png)

* [Filter- und Tauschwerkzeuge](#filter-and-swap-tools)
* [Datumsauswahl](#date-selection)
* [Nicht zugewiesener Bereich](#unassigned-area)
* [Benutzer und Rollen](#users-and-roles)
* [Planung der Timeline](#scheduling-timeline)

### Filter- und Tauschwerkzeuge {#filter-and-swap-tools}

* **Filter-Tool:** Ermöglicht das Filtern des Inhalts, der in der Planung angezeigt wird. Weitere Informationen zur Verwendung des Filter-Tools finden Sie unter [Filtern von Informationen im Bereich &quot;Planung&quot;](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).
* **Tauschtool:** (Nur verfügbar, wenn Sie Ressourcen für Projekte auf der Registerkarte Planung oder Strukturierung planen) Ermöglicht Ihnen das schnelle Zuweisen, Austauschen oder Aufheben der Zuweisung von Benutzern zu Aufgaben in mehreren Projekten. Weitere Informationen finden Sie unter [Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen](../../resource-mgmt/resource-scheduling/manually-assign-items-scheduling-areas.md).

### Datumsauswahl {#date-selection}

Sie können den Datumsbereich anpassen, für den Daten in der Planung angezeigt werden. Standardmäßig beträgt der Datumsbereich 2 Wochen (14 aufeinander folgende Tage, einschließlich Wochenenden) ab dem aktuellen Tag.

### Nicht zugewiesener Bereich {#unassigned-area}

* [Bei der Planung von Ressourcen als Ressourcen-Manager (für mehrere Projekte im Bereich Planung )](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Beim Planen von Ressourcen als Mitglied des Projektteams (aus einem Projekt)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Beim Planen von Ressourcen als Teammitglied (aus einem Team)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Bei der Planung von Ressourcen als Ressourcen-Manager (für mehrere Projekte im Bereich Planung ) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area}

Die **Nicht zugewiesen** im Bereich der Planung nur die Aufgaben und Probleme angezeigt, die alle folgenden Kriterien erfüllen:

* Nicht einem Benutzer zugewiesen.
* Kein Team zugewiesen.\
   Wenn die Aufgabe oder das Problem einem Team zugewiesen wurde, wird sie weiterhin im **Nicht zugewiesen** Bereich, wenn die Aufgabe oder das Problem zusätzlich zur Teamzuweisung auch einer Rolle zugewiesen ist.\
   Wenn Aufgaben oder Probleme zusätzliche Aufgabenrollenzuweisungen haben, die von einem Benutzer nicht erfüllt werden, werden sie ebenfalls angezeigt.\
   Beispielsweise wird eine Aufgabe drei Aufgabenrollen zugewiesen: Designer, Produkt-Manager und Entwickler. Sie weisen diese Aufgabe Benutzer A mit der Rolle &quot;Designer&quot;zu und Benutzer B mit der Rolle &quot;Produkt-Manager&quot;. In diesem Szenario ist die Aufgabe weiterhin im Bereich Nicht zugewiesen in der Zeitplanung sichtbar, da die Rolle Entwicklerauftrag keinem Benutzer zugewiesen ist.

#### Beim Planen von Ressourcen als Mitglied des Projektteams (aus einem Projekt) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project}

Die **Nicht zugewiesen** im oberen Bereich der Planungszeitleiste werden Aufgaben und Probleme angezeigt, die die folgenden Kriterien erfüllen:

* Mit dem Projekt verknüpft, aber keinem Benutzer des Projekt-Teams zugewiesen.\
   Aufgaben, die mit dem Projekt verknüpft sind und einem Benutzer im Projektteam zugewiesen sind, werden in der Zeile des Benutzers angezeigt, dem die Aufgaben zugewiesen sind.
* Dem Projekt zugeordnet, aber einem Mitglied zugewiesen, das nicht im Projektteam ist.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;[! Is it even possible to have the task assigned to a member who is not part of the project team? If so, then would this end up in the Unassigned area?])</p>
  -->

#### **Beim Planen von Ressourcen als Teammitglied (aus einem Team)** {#when-scheduling-resources-as-a-team-member-from-a-team}

Die **Nicht zugewiesen** im oberen Bereich der Planungszeitleiste werden Aufgaben und Probleme angezeigt, die die folgenden Kriterien erfüllen:

* Dem Team und keinen anderen Benutzern im Team zugewiesen.\
   Aufgaben, die sowohl dem Team als auch einem Benutzer im Team zugewiesen sind, werden in der Zeile des Benutzers angezeigt, dem die Aufgaben zugewiesen sind.
* Dem Team und einem Benutzer zugewiesen, der nicht Mitglied des Teams ist.

### Benutzer und Rollen {#users-and-roles}

* [Bei der Planung von Ressourcen als Ressourcen-Manager (für mehrere Projekte im Bereich Planung )](#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area)
* [Beim Planen von Ressourcen als Mitglied des Projektteams (aus einem Projekt)](#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project)
* [Beim Planen von Ressourcen als Teammitglied (aus einem Team)](#when-scheduling-resources-as-a-team-member-from-a-team)

#### Bei der Planung von Ressourcen als Ressourcen-Manager (für mehrere Projekte im Bereich Planung ) {#when-scheduling-resources-as-the-resource-manager-for-multiple-projects-in-the-scheduling-area-1}

Alle Benutzer, denen eine der nicht zugewiesenen Aufgaben zugewiesen werden kann, befinden sich unter der **Nicht zugewiesen** Bereich. Benutzer können in der Planung eine Aufgabe oder ein Problem in folgenden Fällen zugewiesen werden:

* Standardmäßig werden Benutzer nur dann in der Planung angezeigt, wenn sie eine im System definierte Aufgabenrolle haben (entweder die Rolle des Hauptauftrags oder eines sekundären Auftrags) und diese Rolle mit der Auftragsrolle übereinstimmt, die einer Aufgabe oder einem Problem zugewiesen ist, die bzw. das derzeit in der **Nicht zugewiesen** auf der Zeitleiste der Planung. Sie können diese Funktion deaktivieren, damit jedem Benutzer Aufgaben und Probleme zugewiesen werden können, unabhängig davon, ob für diesen Benutzer in seinem Benutzerprofil eine Rolle definiert ist, die der Rollenzuweisung der Aufgabe oder des Problems entspricht, die ihm zugewiesen wird. Weitere Informationen finden Sie unter [Zulassen von Benutzerzuweisungen unabhängig von Rolle und Gruppenmitgliedschaft in den Planungsbereichen](../../resource-mgmt/resource-scheduling/assignments-regardless-of-role-or-group-scheduling-areas.md).\
   Ein Benutzer und die ihm zugewiesenen Aufgaben können mehrmals in der Zeitleiste der Planung angezeigt werden, wenn im Workfront-System mehrere Aufgabenrollen zugewiesen sind.\
   Benutzer verbleiben auf der Planung, nachdem ihnen eine Aufgabe oder ein Problem zugewiesen wurde, selbst wenn keine weiteren Aufgaben oder Probleme mit einer übereinstimmenden Rollenzuweisung vorhanden sind. Auf diese Weise können Sie alle erforderlichen Änderungen vornehmen, nachdem sie zugewiesen wurden.\
   Wenn die Aufgabe keiner Auftragsrolle zugewiesen ist, werden alle Benutzer angezeigt, die die Filteranforderungen erfüllen. Weitere Informationen zum Filter finden Sie unter [Filtern von Informationen im Bereich &quot;Planung&quot;](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

* Sie wurden im **Benutzer** im Feld **Filter** Registerkarte.\
   Weitere Informationen zum Filter finden Sie unter [Filtern von Informationen im Bereich &quot;Planung&quot;](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).\
   Bei der Planung von Ressourcen für ein Team (auf der Registerkarte &quot;Arbeiten am&quot;) wird auch die Teamzuweisung angezeigt.

Alle anderen diesen Benutzern zugewiesenen Aufgaben oder Probleme werden ebenfalls in der Timeline angezeigt.

Sie können die Ebene sehen, auf der Benutzer an einem bestimmten Tag zugewiesen werden, wie unter [Verwalten von Benutzerzuweisungen in den Planungsbereichen](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Aufgaben, für die Sie nicht mindestens Beitragsberechtigungen besitzen, werden in der Zeitleiste der Planung in grau dargestellt.

#### Beim Planen von Ressourcen als Mitglied des Projektteams (aus einem Projekt) {#when-scheduling-resources-as-a-member-of-the-project-team-from-a-project-1}

Jedes Mitglied des Teams wird immer in der Zeitleiste der Planung angezeigt, unabhängig von der Aufgabenrollenzuweisung der Benutzer und der Rollenzuweisung der Aufgaben im Bereich Nicht zugewiesen.

Wenn für einen Benutzer mehrere im System definierte Vorgangsrollen definiert sind, wird der Benutzer mehrmals in der Zeitplanungs-Timeline angezeigt, wenn eines der folgenden Kriterien erfüllt ist:

* Aufgaben oder Probleme werden im **Nicht zugewiesen** -Bereich, der den mit dem Benutzer verknüpften Auftragsrollen zugewiesen ist.
* Es gibt Aufgaben oder Probleme im Projekt mit zugewiesenen Auftragsrollen. Diese Aufgaben oder Probleme werden einem Benutzer zugewiesen, dessen Aufgabenrolle im System definiert ist.

#### Beim Planen von Ressourcen als Teammitglied (aus einem Team) {#when-scheduling-resources-as-a-team-member-from-a-team-1}

Jedes Mitglied des Teams wird immer in der Zeitleiste der Planung angezeigt, unabhängig von der Aufgabenrollenzuweisung der Benutzer und der Rollenzuweisung der Aufgaben im Bereich Nicht zugewiesen.

Sie können die Ebene sehen, auf der Benutzer an einem bestimmten Tag zugewiesen werden, wie unter [Verwalten von Benutzerzuweisungen in den Planungsbereichen](../../resource-mgmt/resource-scheduling/manage-allocations-scheduling-areas.md). Aufgaben, für die Sie nicht mindestens über Beitragsberechtigungen verfügen, um in der Zeitleiste der Planung als graue Leiste angezeigt zu werden.

### Planung der Timeline {#scheduling-timeline}

* **Standardinhalt:** Standardmäßig werden alle Aufgaben ausgeführt, die den im Abschnitt definierten Anforderungen entsprechen [Voraussetzungen für Aufgaben und Probleme](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md#task-and-issue-prerequisites) im [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md) Artikel zu allen Projekten mit dem Status Aktuell werden in der Zeitleiste der Planung angezeigt.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: [! true for teams? - Yes, but really we're focusing on tasks, and the team assignment.])
  </MadCap:conditionalText>
  -->

   Um anzupassen, was in der Timeline der Planung angezeigt wird, einschließlich der Anzeige von Problemen und Projekten mit einem anderen Status, verwenden Sie den Filter, wie unter [Filtern von Informationen im Bereich &quot;Planung&quot;](../../resource-mgmt/resource-scheduling/filter-scheduling-area.md).

   Für einen bestimmten Benutzer werden maximal 10 Aufgaben pro Tag angezeigt. Sie können die Liste erweitern, um alle Aufgaben anzuzeigen, die diesem Benutzer derzeit zugewiesen sind.

* **Übergeordnete Aufgaben:** Ob übergeordnete Aufgaben auf der Timeline angezeigt werden, hängt von mehreren Einstellungen ab. Weitere Informationen finden Sie im Abschnitt &quot;Konfigurieren, ob übergeordnete Aufgaben in der Planung angezeigt werden&quot;in der [Einstellungen in den Planungsbereichen konfigurieren](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) Artikel.

* **Farbcodierung:** Aufgaben und Probleme in der Zeitleiste der Planung sind je nach Projekt, zu dem sie gehören, farbkodiert. Sie können die Farbe, die mit einem bestimmten Projekt verknüpft ist, nicht anpassen.

   Beim Planen von Arbeitsaufgaben für Teams (auf der Registerkarte &quot;Staffing&quot;) werden Farben nur verwendet, wenn die **Alle Benutzeraufgaben anzeigen** aktiviert ist. Weitere Informationen finden Sie im Abschnitt &quot;Konfigurieren, ob übergeordnete Aufgaben in der Planung angezeigt werden&quot;in der [Einstellungen in den Planungsbereichen konfigurieren](../../resource-mgmt/resource-scheduling/configure-settings-scheduling-areas.md) Artikel.

* **Aufgabendauer:** Aufgabendauern werden in der Timeline für jede Aufgabe dargestellt (die Aufgabe erstreckt sich physisch über die Anzahl der Tage, die der Dauer entsprechen). Sie können die Dauer der Aufgabe nicht über die Planung anpassen.

* **Zeitlimit:** Die Zeitabnahme wird in der Planung durch eine hellgraue Anzeige in der Spalte des Tages dargestellt, für den die Zeitabstände für einen bestimmten Benutzer geplant sind.\
   Die Zeitlimit wird für jeden Benutzer auf der Grundlage der folgenden Informationen konfiguriert:

   Der persönliche Zeitablauf des Benutzers. Weitere Informationen zum persönlichen Zeitabschlusskalender finden Sie unter [Persönliche Abwesenheit in Adobe Workfront konfigurieren](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

   Der Zeitplan, der dem Benutzer zugewiesen ist. Dies kann der Standardzeitplan oder ein benutzerdefinierter Zeitplan sein. Weitere Informationen zu Zeitplänen finden Sie unter [Zeitplan erstellen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Wochenenden:** Wochenenden werden in der Planung samstags und sonntags als hellgraue Schattierung dargestellt. Wochentage, die in der Planung als Wochenenden festgelegt sind, können nicht konfiguriert werden. Sie können Benutzer für die Arbeit am Wochenende planen.
