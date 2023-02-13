---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Übersicht über den Lastenausgleich
description: Nachdem die Projektmanager die Arbeit an Projekten geplant und Aufgaben erstellt haben, können Sie den Arbeitslastausgleich verwenden, um diese Arbeit den Benutzern in Ihren Teams zuzuweisen.
author: Alina
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 11c87d8a97261c24d063fbc824f2e907d07f8217
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---

# Übersicht über den Lastenausgleich

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Nachdem die Projektmanager die Arbeit an Projekten geplant und Aufgaben erstellt haben, können Sie den Arbeitslastausgleich verwenden, um diese Arbeit Benutzern zuzuweisen.

>[!IMPORTANT]
>
>Sie können den Lastenausgleich verwenden, um Benutzern tatsächliche Arbeit (Aufgaben und Probleme) zuzuweisen.
>
>Sie müssen den Ressourcen-Planer und nicht den Arbeitslast-Balancer verwenden, um die Auftragsrollenzuweisungen für Ihre Projekte auf hoher Ebene zu schätzen. Weitere Informationen zum Ressourcen-Planer finden Sie unter [Übersicht über den Ressourcenplaner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

In diesem Artikel werden der allgemeine Zweck des Workload Balancer und einige der Best Practices für die Einrichtung Ihrer Projekte und Ressourcen für die erfolgreiche Verwendung beschrieben.

## Suchen Sie den Lastenausgleich .

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Es wird empfohlen, den Workflow-Lastenausgleich in den folgenden Bereichen für die Planung von Ressourcen zu verwenden:

* Auf Systemebene im Bereich Ressourcen .
* Auf Projektebene im Abschnitt Lastenausgleich eines Projekts.
* Auf Teamebene im Bereich Lastenausgleich eines Teams.

Weitere Informationen zum Auffinden des Lastenausgleichs finden Sie unter [Suchen Sie den Lastenausgleich .](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Vorteile des Lastenausgleichs

Beachten Sie bei der Verwendung des Workload Balancers die folgenden Vorteile:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Greifen Sie auf eine klare visuelle Zuordnung von Ressourcenüberzuteilung und unzureichender Nutzung zu, die für alle Beteiligten transparent ist.
* Als Personalverantwortlicher können Sie Ihre Menschen vor Burnout schützen und sie in die Lage versetzen, ihre beste Arbeit mit besserer Konzentration, Qualität und Interaktion zu erledigen. Sie können ihre volle Nutzung sicherstellen, Silos unterbrechen und die Abstimmung der Arbeit zwischen Teams ermöglichen.
* Wenn Sie Arbeiten auf Aufgaben- oder Problemebene zuweisen, können Sie nicht erkennen, wie beschäftigt ein Benutzer sein könnte. Wenn Sie den Lastenausgleich verwenden, können Sie sehen, welche Benutzer in ihrer Arbeitslast verfügbar sind, um die Aufgabe oder das Problem rechtzeitig abzuschließen. Dazu gehören die Zeitdauer und Details zur Planung von Ausnahmen.

   Weitere Informationen finden Sie unter [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

   Sie können Arbeitselemente auch stapelweise zuweisen, was die gleichzeitige Verteilung einer großen Anzahl von Arbeitselementen über mehrere Projekte hinweg erleichtert. Weitere Informationen finden Sie unter [Stapelweises Zuweisen von Arbeiten mithilfe des Lastenausgleichs](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Führungskräfte können durch Transparenz in der Art und Weise, wie Menschen in ihrer Organisation genutzt werden, zeitnahe Personalentscheidungen treffen.
* Teammitglieder profitieren von einer besseren Zusammenarbeit, da sie alle jederzeit sehen können, woran ihre Mitarbeiter arbeiten. Informationen über den Zugriff, der zum Anzeigen oder Verwalten von Ressourcen im Lastenausgleich erforderlich ist, finden Sie unter [Zugriff erforderlich für die Verwaltung von Ressourcen im Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Geben Sie ihn für alle Benutzer frei, die keinen Zugriff auf den Bereich &quot;Ressourcen&quot;haben, indem Sie einen Link dazu in eine benutzerdefinierte Registerkarte einbetten. Weitere Informationen finden Sie unter [Den Lastenausgleich über einen Link freigeben](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* Visualisieren und verwalten Sie die Arbeitslasten und Anforderungen von Personen in einer Ansicht auf globaler, Projekt- oder Teamebene, je nach Ihrer Rolle. Bei der Projektverwaltung umfasst dies nicht nur die Ressourcenzuweisung für das Projekt, sondern auch die Visualisierung der Ressourcenzuordnung über den Adobe Workfront-Szenario-Planer. Manager von Personen verwenden den Workfront-Szenario-Planer, um die beruflichen Fertigkeiten in der gesamten Organisation zu verwalten. Der Szenario-Planer ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

   >[!NOTE]
   >
   >  Für den Szenario-Planer ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Übersicht über den Szenario-Planer](../../scenario-planner/scenario-planner-overview.md).


## Best Practices für die Verwendung des Lastenausgleichs

Wir empfehlen die folgenden Best Practices für die Planung von Projekten, die Konfiguration von Benutzern und die Verwendung von Filtern, bevor Sie mit der Planung Ihrer Ressourcen mit dem Workload Balancer beginnen.

* [Best Practices für die Anzeige von Informationen im Arbeitslastausgleich](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Best Practices zum Einrichten von Benutzern](#best-practices-for-setting-up-users)
* [Best Practices zum Einrichten von Aufgaben und Problemen](#best-practices-for-setting-up-tasks-and-issues)

### Best Practices für die Anzeige von Informationen im Arbeitslastausgleich {#best-practices-for-displaying-information-in-the-workload-balancer}

Es wird empfohlen, Filter zu verwenden, damit Sie nur die Informationen anzeigen können, die für nicht zugewiesene und zugewiesene Arbeitselemente relevant sind.

Informationen zum Erstellen und Verwenden von Filtern im Arbeitslastausgleich finden Sie unter [Filtern von Informationen im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Best Practices zum Einrichten von Benutzern

* Da der Benutzer, der Zeitpläne einplant, für andere Benutzer funktioniert, müssen Sie über die richtigen Zugriffsrechte und Berechtigungen verfügen, um Ressourcen für die Arbeit planen zu können.

   Informationen über den Zugriff, der für die Verwaltung der Arbeitslast Ihrer Ressourcen im Workload-Balancer erforderlich ist, finden Sie unter [Zugriff erforderlich für die Verwaltung von Ressourcen im Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Die Benutzer, deren Arbeitsaufwand Sie verwalten möchten, müssen die folgenden Kriterien erfüllen, damit die Informationen über ihre Verfügbarkeit und Fähigkeiten korrekt sind:

   * Mit ihrem Profil verknüpfen Sie Zeitpläne und Vorgangsrollen.
   * Weitere Informationen zum Verknüpfen von Zeitplänen und Auftragsrollen mit Benutzern finden Sie unter [Benutzer hinzufügen](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Wenn einem Benutzer kein Zeitplan zugeordnet ist, wird der Standardzeitplan Ihres Workfront-Systems dem Benutzer standardmäßig zum Zwecke der Ressourcenverwaltung zugeordnet.
   * Lassen Sie Ausnahmen planen in ihren Zeitplänen aktualisiert.\
      Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter [Zeitplan erstellen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Lassen Sie den Kalender in ihrem Profil aktualisiert.\
      Weitere Informationen zum Aktualisieren des Zeitlimitkalenders eines Benutzers finden Sie unter [Persönliche Abwesenheit in Adobe Workfront konfigurieren](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

      <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* Der Workfront-Administrator muss bestimmen, wie Workfront die Benutzerverfügbarkeit berechnet. Sie können entscheiden, ob Workfront entweder den Standardzeitplan des Systems oder den Zeitplan des Benutzers verwendet, um die Zeit zu berechnen, für die der Benutzer zur Verfügung steht. Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Best Practices zum Einrichten von Aufgaben und Problemen {#best-practices-for-setting-up-tasks-and-issues}

Stellen Sie sicher, dass die folgende Aufgabe und das Einrichten von Problemen vorhanden sind, bevor Sie mit der Zuweisung von Aufgaben an Benutzer im Arbeitslastausgleich beginnen:

* Übergeordnete Aufgaben werden Benutzern oder Rollen nicht zugewiesen. Sie werden nicht im Lastenausgleich angezeigt.
* Aufgaben und Probleme haben einen Wert für &quot;Geplante Stunden&quot;, der größer als null ist.

* Aufgaben und Probleme haben einen Wert für ihre Dauer, der größer als null ist.
* Die geplanten Daten der Probleme entsprechen dem Zeitrahmen des Projekts.

## Bevor Sie mit der Verwendung des Lastenausgleichs beginnen

* Sie können den Lastenausgleich verwenden, um Arbeitsaufgaben zuzuweisen und tägliche Zuordnungen für Benutzer in Ihrer Organisation zu verwalten.

   In diesem Artikel erfahren Sie, wie Sie im Arbeitslastausgleich navigieren, um die folgenden Aktionen durchzuführen: [Navigieren Sie zum Lastenausgleich .](../workload-balancer/navigate-the-workload-balancer.md).

   In den folgenden Artikeln erfahren Sie, wie Sie Arbeit zuweisen und Benutzerzuweisungen verwalten:

   * [Übersicht über die Zuweisung von Aufgaben im Arbeitslastausgleich](../workload-balancer/assign-work-in-workload-balancer.md).
   * [Verwalten von Benutzerzuordnungen im Lastenausgleich](../workload-balancer/manage-user-allocations-workload-balancer.md).

* Der Lastenausgleich kann sich in verschiedenen Bereichen von Workfront befinden. Informationen darüber, wo Sie den Lastenausgleich finden können, finden Sie unter [Suchen Sie den Lastenausgleich .](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Zugriff erforderlich, um den Lastenausgleich zu verwenden

Sie müssen über den richtigen Workfront-Zugriff und die richtigen Berechtigungen für bestimmte Projekte verfügen, um den Workload Balancer in Workfront anzeigen und verwenden zu können. Informationen über den für die Verwendung des Workload Balancer benötigten Zugriff finden Sie im Artikel [Zugriff erforderlich für die Verwaltung von Ressourcen im Workload Balancer](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
