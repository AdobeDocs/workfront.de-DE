---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: Überblick über den Workload Balancer
description: Nachdem das Projekt-Management die Arbeit an Projekten durch Erstellen von Aufgaben geplant hat und nachdem das Ressourcen-Management den Projekten im Ressourcenplaner Ressourcen für Aufgabengebiete zugewiesen hat, können Projektbesitzer bzw. -besitzerinnen und das Team-Management Benutzenden im Workload Balancer Arbeitselemente zuweisen.
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 9e217d36d5aeb36761a9a433b84e73ac2b7a114b
workflow-type: tm+mt
source-wordcount: '1202'
ht-degree: 100%

---

# Überblick über den Workload Balancer {#workload-balancer-overview}

>[!CONTEXTUALHELP]
>id="wf-resourcing-workload-balancer"
>title="Workload Balancer"
>abstract="Projektverantwortliche und Team-Mangement können den Workload Balancer verwenden, um Benutzenden Arbeitselemente zuzuweisen."

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

Nachdem das Projekt-Management die Arbeit an Projekten durch Erstellen von Aufgaben geplant hat und nachdem das Ressourcen-Management den Projekten im Ressourcenplaner Ressourcen für Aufgabengebiete zugewiesen hat, können Projektbesitzer bzw. -besitzerinnen und das Team-Management Benutzenden im Workload Balancer Arbeitselemente zuweisen.

>[!IMPORTANT]
>
>Sie können den Workload Balancer verwenden, um Benutzenden die tatsächliche Arbeit (Aufgaben und Probleme) zuzuweisen.
>
>Sie müssen jedoch den Ressourcenplaner, nicht den Workload Balancer, verwenden, um die Zuteilungen der Aufgabengebiete für Ihre Projekte auf einer allgemeinen Ebene zu schätzen. Weitere Informationen zum Ressourcenplaner finden Sie unter [Überblick über den Ressourcenplaner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

In diesem Artikel werden der allgemeine Zweck des Workload Balancers und einige der Best Practices für die Einrichtung Ihrer Projekte und Ressourcen beschrieben, damit Sie ihn erfolgreich einsetzen können.

Die Video-Tutorials zum Workload Balancer können Sie sich auf der Seite [Workfront-Tutorials](https://experienceleague.adobe.com/de/docs/workfront-learn/tutorials-workfront/home) ansehen. Wählen Sie im linken Menü **Ressourcen verwalten** > **Workload Balancer** aus und wählen Sie dann ein Tutorial aus.

## Auffinden des Workload Balancers

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

Es wird empfohlen, den Workload Balancer in den folgenden Bereichen für die Planung von Ressourcen zu verwenden:

* Auf Systemebene im Bereich „Ressourcenplanung“.
* Auf Projektebene im Abschnitt „Workload Balancer“ eines Projekts.
* Auf Team-Ebene im Abschnitt „Workload Balancer“ eines Teams.

Weitere Informationen zum Auffinden des Workload Balancers finden Sie unter [Auffinden des Workload Balancers](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Vorteile des Workload Balancers

Beachten Sie die folgenden Vorteile bei der Verwendung des Workload Balancers:

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* Greifen Sie auf eine übersichtliche visuelle Darstellung der Überallokation und Unterauslastung von Ressourcen zu, die für alle Beteiligten transparent ist.
* Als Person mit Personalverantwortung können Sie Ihre Mitarbeitenden vor Burnout schützen und sie in die Lage versetzen, mit besserer Fokussierung, höherer Qualität und größerem Engagement bestmögliche Arbeit zu leisten. Sie können ihre volle Auslastung sicherstellen, Silos aufbrechen und eine Team-übergreifende Abstimmung der Arbeit ermöglichen.
* Wenn Sie Arbeit auf Aufgaben- oder Problemebene zuweisen, haben Sie keinen Einblick in die potenzielle Auslastung eines Benutzers bzw. einer Benutzerin. Wenn Sie den Workload Balancer verwenden, können Sie sehen, welche Benutzenden in ihrem Workload Kapazitäten haben, um die Aufgabe oder das Problem termingerecht abzuschließen. Dazu gehören auch Angaben zu ihrer Ausfallzeit oder Zeitplanausnahmen.

  Weitere Informationen finden Sie unter [Überblick über die Zuweisung von Arbeit im Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  Sie können auch eine große Anzahl Arbeitselemente gleichzeitig zuweisen. Dadurch wird es einfacher, viele Arbeitselemente gleichzeitig über mehrere Projekte zu verteilen. Weitere Informationen finden Sie unter [Massenzuweisung von Arbeit im Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* Führungskräfte können zeitnahe Personalentscheidungen treffen, da sie wissen, wie die Mitarbeitenden in ihrer Organisation ausgelastet sind.
* Team-Mitglieder profitieren von einer besseren Zusammenarbeit, da alle sehen können, woran ihre Kollegen und Kolleginnen jeweils arbeiten. Informationen zu den Zugriffsrechten, die zum Anzeigen oder Verwalten von Ressourcen im Workload Balancer benötigt werden, finden Sie unter [Zur Verwaltung von Ressourcen im Workload Balancer benötigte Zugriffsrechte](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* Geben Sie die Option für alle frei, deren Hauptmenü die Ressourcenplanung nicht enthält, indem Sie einen entsprechenden Link in einer benutzerdefinierten Registerkarte einfügen. Weitere Informationen finden Sie unter [Freigeben des Workload Balancers mit einem Link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
* Stellen Sie die Workloads der Mitarbeitenden und den Bedarf entsprechend Ihrer Rolle in einer Ansicht auf globaler, Projekt- oder Team-Ebene dar und verwalten Sie sie. Bei der Verwaltung von Projekten umfasst dies nicht nur die Ressourcenzuteilung für das Projekt, sondern auch die Visualisierung der Ressourcenzuteilung über den Adobe Workfront-Szenarienplaner. Personalverantwortliche verwenden den Workfront-Szenarienplaner, um die beruflichen Fähigkeiten in der gesamten Organisation zu verwalten. Der Szenarienplaner ist nur in der neuen Adobe Workfront-Version verfügbar.

  >[!NOTE]
  >
  >  Für den Szenarienplaner ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zum Workfront-Szenarienplaner finden Sie unter [Überblick über den Szenarienplaner](../../scenario-planner/scenario-planner-overview.md).


## Best Practices für die Verwendung des Workload Balancers

Wir empfehlen die folgenden Best Practices für die Planung von Projekten, die Konfiguration von Benutzenden und die Verwendung von Filtern, bevor Sie mit der Planung Ihrer Ressourcen mit dem Workload Balancer beginnen.

* [Best Practices für die Anzeige von Informationen im Workload Balancer](#best-practices-for-displaying-information-in-the-workload-balancer)
* [Best Practices zum Einrichten von Benutzenden](#best-practices-for-setting-up-users)
* [Best Practices zum Einrichten von Aufgaben und Problemen](#best-practices-for-setting-up-tasks-and-issues)

### Best Practices für die Anzeige von Informationen im Workload Balancer {#best-practices-for-displaying-information-in-the-workload-balancer}

Es wird empfohlen, Filter zu verwenden, damit Sie nur die Informationen anzeigen können, die sowohl für nicht zugewiesene als auch für zugewiesene Arbeitselemente relevant sind.

Informationen zum Erstellen und Verwenden von Filtern im Workload Balancer finden Sie unter [Filtern von Informationen im Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### Best Practices für die Einrichtung von Benutzenden

* Als Person, die Arbeit für andere geplant hat, müssen Sie über die richtigen Zugriffsrechte und Berechtigungen verfügen, um Ressourcen für Arbeit zu planen.

  Informationen zu den Zugriffsrechten, die für die Verwaltung des Workloads Ihrer Ressourcen im Workload Balancer benötigt werden, finden Sie unter [Zur Verwaltung von Ressourcen im Workload Balancer benötigte Zugriffsrechte](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* Die Benutzenden, deren Workload Sie verwalten möchten, müssen die folgenden Kriterien erfüllen, damit die Informationen zu ihrer Verfügbarkeit und ihren Fähigkeiten korrekt sind:

   * Ihrem Profil müssen Zeitpläne und Aufgabengebiete zugewiesen sein.

     Weitere Informationen zum Verknüpfen von Zeitplänen und Aufgabengebieten mit Benutzenden finden Sie unter [Hinzufügen von Benutzenden](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * Wenn eine Person keinem Zeitplan zugeordnet ist, wird zum Ressourcen-Management der Person standardmäßig der Standardzeitplan Ihres Workfront-Systems zugeordnet.
   * Zeitplanausnahmen müssen in den entsprechenden Zeitplänen aktualisiert werden.

     Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * Der Kalender für Ausfallzeiten muss im Profil der jeweiligen Person aktualisiert werden.

     Informationen zum Aktualisieren des Kalenders für Ausfallzeiten einer Person finden Sie unter [Konfigurieren von persönlicher Ausfallzeit](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* Der bzw. die Workfront-Admin muss festlegen, wie Workfront die Benutzerverfügbarkeit ermittelt. Er bzw. sie kann entscheiden, ob Workfront den Standardzeitplan des Systems oder den Zeitplan der Person zur Ermittlung der Zeit verwendet, in der die Person für die Arbeit zur Verfügung steht. Dazu kann er bzw. sie die Einstellungen für das Ressourcen-Management im Bereich „Setup“ von Workfront anpassen.

  Weitere Informationen finden Sie unter [Konfigurieren von Voreinstellungen für das Ressourcen-Management](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Best Practices zum Einrichten von Aufgaben und Problemen {#best-practices-for-setting-up-tasks-and-issues}

Stellen Sie sicher, dass das folgende Setup für Aufgaben und Probleme vorhanden ist, bevor Sie damit beginnen, Benutzenden im Workload Balancer Arbeit zuzuweisen:

* Übergeordnete Aufgaben werden Benutzenden oder Rollen nicht zugewiesen. Übergeordnete Aufgaben werden im Workload Balancer nicht angezeigt.
* Aufgaben und Probleme haben einen Wert für „Geplante Stunden“, der größer als null ist.

* Aufgaben und Probleme haben einen Wert für ihre „Dauer“, der größer als null ist.
* Die geplanten Termine der Probleme befinden sich innerhalb der Timeline des Projekts.

## Bevor Sie mit der Verwendung des Workload Balancers beginnen

* Lesen Sie die folgenden Artikel, bevor Sie mit der Verwendung des Workload Balancers beginnen:

   * Dieser Artikel führt Sie durch die Navigation im Workload Balancer, um die folgenden Aktionen auszuführen: [Navigieren im Workload Balancer](../workload-balancer/navigate-the-workload-balancer.md).

   * In den folgenden Artikeln erfahren Sie, wie Sie Arbeit zuweisen und Benutzerzuordnungen verwalten:

      * [Überblick über die Zuweisung von Arbeit im Workload Balancer](../workload-balancer/assign-work-in-workload-balancer.md).
      * [Verwalten von Benutzerzuordnungen im Workload Balancer](../workload-balancer/manage-user-allocations-workload-balancer.md).

* Der Workload Balancer ist in verschiedenen Bereichen von Workfront zu finden. Informationen dazu, wo Sie den Workload Balancer finden, finden Sie unter [Auffinden des Workload Balancers](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## Für die Verwendung des Workload Balancers erforderliche Zugriffsrechte

Sie müssen über die richtigen Workfront-Zugriffsrechte und -Berechtigungen für bestimmte Projekte verfügen, um den Workload Balancer in Workfront anzeigen und verwenden zu können. Informationen zu den Zugriffsrechten, die für die Verwendung des Workload Balancers erforderlich sind, finden Sie im Artikel [Zur Verwaltung von Ressourcen im Workload Balancer benötigte Zugriffsrechte](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
