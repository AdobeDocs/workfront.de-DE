---
product-area: resource-management
keywords: Arbeitsbereich,Team,Personal,Ressourcen
navigation-topic: the-workload-balancer
title: Suchen Sie den Lastenausgleich .
description: Sie können den Lastenausgleich verwenden, um Ressourcen für die Arbeit zu planen oder deren Verfügbarkeit und aktuelle Zuordnungen zu überprüfen.
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 2375cf5d7ae817340ce9552994d87cb5af9a054b
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Suchen Sie den Lastenausgleich .

Sie können den Lastenausgleich verwenden, um Ressourcen für die Arbeit zu planen oder deren Verfügbarkeit und aktuelle Zuordnungen zu überprüfen.

Sie können auf den Lastenausgleich wie folgt zugreifen:

* Aus mehreren von Adobe Workfront vordefinierten Bereichen
* Durch Hinzufügen zu einem benutzerdefinierten Abschnitt

In diesem Artikel werden die Bereiche beschrieben, in denen Sie auf den Lastenausgleich zugreifen können.

>[!NOTE]
>
>Unabhängig von der Methode, die Sie für den Zugriff auf den Lastenausgleich verwenden, ist die Navigation und Verwaltung von Ressourcen identisch.
>
>Weitere Informationen zum Arbeitslastausgleich und dessen Verwendung für die Verwaltung und Planung Ihrer Ressourcen für die Arbeit finden Sie in den folgenden Artikeln:
>
>* [Übersicht über den Lastenausgleich](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [Navigieren Sie zum Arbeitsladeausgleich](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [Übersicht über die Zuweisung von Arbeit im Arbeitslastausgleich](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [Verwalten von Benutzerzuweisungen im Arbeitslade-Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Planen Sie bei Verwendung des Workload-Balancers im Ressourcenbereich;</br>
       Arbeiten bei Verwendung des Workload Balancers für ein Team oder Projekt</p></td>
  </tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zeigen Sie den Zugriff auf Folgendes an oder höher:</p> 
    <ul> 
     <li>Ressourcenverwaltung</li> 
     <li>Projekte</li> 
     <li>Aufgaben</li> 
     <li>Probleme</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Anzeigen von Berechtigungen oder höher für die Projekte, Aufgaben und Probleme</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Auf den Lastenausgleich in vordefinierten Bereichen zugreifen

Die folgenden Abschnitte veranschaulichen, wo Sie auf den Lastenausgleich in Workfront zugreifen können.

### Zugriff auf den Lastenausgleich für mehrere Projekte im Bereich &quot;Ressourcen&quot;

{{step1-to-resourcing}}

1. Klicken Sie im linken Bereich auf **Lastenausgleich** .

   ![](assets/nwe-balancer-global.png)

   Der Lastenausgleich zeigt standardmäßig Folgendes anhand von Informationen im Bereich &quot;Ressourcen&quot;an:

   * **Nicht zugewiesene Arbeit**: Keine nicht zugewiesenen Arbeitselemente.
   * **Zugewiesene Arbeit**: Alle aktiven Benutzer im System.

     Es wird empfohlen, beim Anzeigen von Benutzern im Bereich &quot;Zugewiesene Arbeit&quot;Filter zu verwenden. Weitere Informationen finden Sie unter [Filtern von Informationen im Arbeitslastausgleich](../workload-balancer/filter-information-workload-balancer.md).

### Zugriff auf den Lastenausgleich für ein Team

{{step1-to-team}}

Die Seite Ihres Startseiten-Teams wird angezeigt.

1. Klicken Sie im linken Bereich auf **Lastenausgleich** .

   ![](assets/nwe-balancer-team-350x172.png)

   Der Lastenausgleich eines Teams zeigt standardmäßig die folgenden Informationen an:

   * **Nicht zugewiesene Arbeit**: Dem Team zugewiesene Elemente, die Benutzern nicht zugewiesen sind.
   * **Zugewiesene Arbeit**: Alle Mitglieder des Teams mit allen ihren Zuweisungen.

     >[!TIP]
     >
     >Team-Mitglieder können Aufgaben zugewiesen werden, die auch dem Team zugewiesen sind, oder anderen Teams oder Rollen zugewiesen werden.

### Zugriff auf den Lastenausgleich für ein Projekt

{{step1-to-projects}}

1. Klicken Sie auf den Namen eines Projekts, um die Projektseite zu öffnen.
1. Klicken Sie im linken Bereich auf **Lastenausgleich** . Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Lastenausgleich** klicken.

   Der Lastenausgleich für das Projekt wird angezeigt.

   ![](assets/nwe-balancer-project-350x152.png)

   Der Lastenausgleich eines Projekts zeigt standardmäßig Folgendes nach Informationen an:

   * **Nicht zugewiesene Arbeit**: Elemente aus dem Projekt, die Auftrags- oder Teams zugewiesen sind und Benutzern nicht zugewiesen sind.
   * **Zugewiesene Arbeit**: Benutzer, die Elementen im Projekt zugewiesen sind.

     >[!TIP]
     >
     >Sie können alle Benutzer im System anstelle nur der Benutzer im Projekt (im Bereich &quot;Zugewiesene Arbeit&quot;) anzeigen, indem Sie die Option Alle Benutzer anzeigen aktivieren. Weitere Informationen finden Sie unter [Navigieren im Arbeitslastausgleich](../workload-balancer/navigate-the-workload-balancer.md).


## Den Lastenausgleich zu einem benutzerdefinierten Abschnitt hinzufügen

Sie können den Lastenausgleich zu jedem benutzerdefinierten Abschnitt hinzufügen.

Die meisten Anpassungen, die Sie bereits auf den Lastenausgleich angewendet haben, bleiben erhalten, wenn Sie ihn zu einem benutzerdefinierten Abschnitt hinzufügen.

1. Greifen Sie auf den Lastenausgleich zu, indem Sie einen der folgenden Bereiche aufrufen:

   * Ressourcenbereich
   * Ein Team
   * Ein Projekt

1. Rufen Sie einen freigebbaren Link ab und kopieren Sie ihn in die Zwischenablage, wie unter [Den Lastenausgleich mit einem Link teilen](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md) beschrieben.
1. Erstellen Sie ein Dashboard mit einer externen Seite, wie in [Einbetten einer externen Webseite in ein Dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md) beschrieben. Verwenden Sie den freigebbaren Link, den Sie in Schritt 2 für die externe Seite erhalten haben.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Erstellen Sie einen benutzerdefinierten Abschnitt wie in [Erstellen Sie benutzerdefinierte Registerkarten oder Abschnitte](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) beschrieben, um das Dashboard auf der benutzerdefinierten Registerkarte zu platzieren.

   Beim Zugriff auf den Lastenausgleich über den benutzerdefinierten Abschnitt können Sie ihn so anzeigen, als ob Sie direkt über einen der in Schritt 1 aufgelisteten ursprünglichen Bereiche darauf zugegriffen hätten.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Optional) Geben Sie die benutzerdefinierte Registerkarte in einer Layout-Vorlage frei, wie unter [Anpassen des linken Bedienfelds mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) beschrieben.


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->