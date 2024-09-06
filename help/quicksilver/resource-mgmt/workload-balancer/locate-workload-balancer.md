---
product-area: resource-management
keywords: arbeiten, Team, personal, ressourcen
navigation-topic: the-workload-balancer
title: Suchen Sie den Workload Balancer
description: Sie können den Workload Balancer verwenden, um Ressourcen für die Arbeit zu planen oder ihre Verfügbarkeit und aktuelle Zuordnungen zu überprüfen.
author: Lisa
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: db0aab0e6e7e896a8e7c0afe2da709de7c3c2a4e
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Suchen Sie den Workload Balancer

Sie können den Lastenausgleich verwenden, um Ressourcen für die Arbeit zu planen oder deren Verfügbarkeit und aktuelle Zuordnungen zu überprüfen.

Sie können auf folgende Weise auf den Workload Balancer zugreifen:

* Aus mehreren Bereichen, die von Adobe Systems Workfront vordefiniert wurden
* Durch Hinzufügen zu einem benutzerspezifischen Abschnitt

In diesem Artikel werden die Bereiche beschrieben, in denen Sie auf den Workload Balancer zugreifen können.

>[!NOTE]
>
>Unabhängig von der Methode, die Sie für den Zugriff auf den Workload Balancer verwenden, ist die Navigation darin und die Verwaltung von Ressourcen identisch.
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
   <td><p>Neu: Standardmäßig</p>
       <p>oder</p>
       <p>Aktuell: Abo-Option, bei Verwendung des Workload Balancer im Ressourcenbereich;</br>
       Arbeit, wenn der Workload Balancer eines Team oder Projekts verwendet wird</p></td>
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
   <td role="rowheader">Objekt Berechtigungen</td> 
   <td>Ansicht Berechtigungen oder höher für die Projekte, Aufgaben und Probleme</td> 
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

    Klicken Sie im linken Fensterbereich auf &quot;Workload Balancer&quot;.
    
    ![](assets/nwe-balancer-team-350x172.png)
    
    Der Lastenausgleich eines Teams zeigt standardmäßig die folgenden Informationen an:
    
    * **Nicht zugewiesene Arbeit**: Dem Team zugewiesene Elemente, die Benutzern nicht zugewiesen sind.
    * **Zugewiesene Arbeit**: Alle Mitglieder der Team mit all ihren Aufgaben.
    
    >[!TIP]
    >
    >Team-Mitglieder können Aufgaben zugewiesen werden, die auch dem Team zugewiesen sind, oder anderen Teams oder Rollen zugewiesen werden.

### Zugriff auf den Lastenausgleich für ein Projekt

{{step1-to-projects}}

1. Klicken Sie auf den Namen eines Projekts, um die Projektseite zu öffnen.
1. Klicken Sie im linken Fensterbereich auf &quot; **Workload Balancer** &quot;. Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Lastenausgleich** klicken.

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

   * Der Ressourcenbereich
   * Ein Team
   * Ein Projekt

1. Rufen Sie eine gemeinsam nutzbare verknüpfen ab, und kopieren Sie sie in Ihre Zwischenablage, wie unter [Freigeben des Workload Balancer für eine verknüpfen](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md) beschrieben.
1. Erstellen ein Dashboard mit einem externen Seite, wie unter [Einbetten eines externen Web-Seite in ein Dashboard](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md) beschrieben. Verwenden Sie den freigebbaren Link, den Sie in Schritt 2 für die externe Seite erhalten haben.

   <!--
      (NOTE: ensure this stays correct)
      -->

1. Erstellen einen benutzerdefinierten Abschnitt, wie in [Erstellen benutzerdefinierte Registerkarten oder Abschnitte](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) beschrieben, um die Dashboard auf der benutzerdefinierten Tab zu platzieren.

   Wenn Sie über den Abschnitt &quot;Benutzerdefiniert&quot; auf den Workload Balancer zugreifen, können Sie ihn so Ansicht, als würden Sie direkt von einem der ursprünglichen Bereiche aus zugreifen, die in Schritt 1 aufgeführt sind.

   <!--
      (NOTE: ensure this stays correct)
     -->

1. (Optional) Geben Sie die benutzerdefinierten Tab in einem Layout Vorlage frei, wie unter  [Anpassen des linken Bedienfelds mithilfe eines Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) beschrieben.


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