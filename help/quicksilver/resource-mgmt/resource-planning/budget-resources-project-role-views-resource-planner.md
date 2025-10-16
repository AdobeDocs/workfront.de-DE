---
product-area: resource-management
navigation-topic: resource-planning
title: Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Aufgabenansichten
description: Sie können Ressourcen im Adobe Workfront-Ressourcenplaner mithilfe der Projekt- und Rollenansichten budgetieren. Mit der Ansicht „Benutzer“ im Ressourcenplaner können Sie keine Ressourcen budgetieren.
author: Lisa
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '2098'
ht-degree: 0%

---

# Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Rollenansichten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

Die Hauptaufgabe des Ressourcenplaners besteht darin, Ihre Ressourcen für die Arbeit zu budgetieren, die an Projekten durchgeführt werden muss.

>[!IMPORTANT]
>
>Sie können Ressourcen nur budgetieren, wenn Sie die Ansichten **Nach Projekt anzeigen** oder **Nach Funktion anzeigen** auf den Ressourcenplaner anwenden.

Bevor Sie mit der Budgetplanung im Ressourcenplaner beginnen, lesen Sie die folgenden Artikel:

* [Ressourcenplaner - Übersicht](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Zugriff zum Budgetressourcen in Adobe Workfront erforderlich](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf das Ressourcenmanagement bearbeiten, der den Zugriff auf die Bearbeitung von Prioritäten und Budgetstunden im Ressourcenplaner beinhaltet</p> <p>Zugriff auf Finanzdaten bearbeiten, um Ressourcen nach Kosten zu budgetieren</p> <p>Zugriff auf Projekte und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für die Projekte, für die Sie Informationen budgetieren möchten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Budgetressourcen im Ressourcenplaner

* [Budgetressourcen in der Projektansicht](#budget-resources-in-the-project-view)
* [Budgetressourcen in der Rollenansicht](#budget-resources-in-the-role-view)
* [Gesamtbudget](#budget-resources-in-bulk)

### Budgetressourcen in der Projektansicht {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

{{step1-to-resourcing}}

1. Der **Planer** wird standardmäßig angezeigt.
1. (Bedingt) Wählen Sie die Ansicht **Nach Projekt anzeigen**.
1. Erweitern Sie die Projekte und Aufgabengebiete, um die Zuordnung für das Projekt, die Aufgabengebiete oder die Benutzer zu verwalten.
1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für Benutzer vorzunehmen:

   * Geben **in der Spalte** BDG) manuell die Anzahl der budgetierten Stunden, VZÄ oder Kosten für die Benutzer an.

   * Klicken Sie auf das **Mehr**-Menü für das Aufgabengebiet des Benutzers und dann auf **Geplante Stunden der Benutzer als „Budgetiert“**.\
     Die budgetierten Stunden der einzelnen Benutzer werden anhand der folgenden Formel berechnet:

     `User Budgeted Hours = User Planned Hours`

1. Führen Sie einen der folgenden Schritte aus, um eine Budgetzuweisung für Aufgabengebiete vorzunehmen:

   * Geben **in der Spalte** BDG) manuell die Anzahl der budgetierten Stunden, VZÄ oder Kosten für das Aufgabengebiet an.

     >[!NOTE]
     >
     >Die Funktion „Budgetierte Stunden“ wird den budgetierten Stunden des Projekts hinzugefügt.

   * (Bedingt) Wenn Sie budgetierte Stunden für Benutzer haben, klicken Sie auf das Menü **Mehr** für das Aufgabengebiet und dann auf **Budgetierte Stunden für Funktion gesamt für Benutzer**.\
     Die budgetierten Stunden für jede Funktion werden anhand der folgenden Formel berechnet:

     `Role Budgeted Hours = SUM(User Budgeted Hours)`

   * Klicken Sie auf das **Mehr**-Menü für das Projekt und dann auf **Geplante Stunden für Funktionen als „Budgetiert“**.\
     Die budgetierten Stunden für jede Funktion werden anhand der folgenden Formel berechnet:\
     *

     `Role Budgeted Hours = Role Planned Hours`

     >[!NOTE]
     >   
     >* Die Funktion „Budgetierte Stunden“ wird den budgetierten Stunden des Projekts hinzugefügt.
     >* Benutzer können sowohl für Primäre als auch für andere (oder sekundäre) Funktionen budgetiert werden.
     >* Der **Prozentsatz der FTE-Verfügbarkeit** für die Rollen des Benutzers muss eine Zahl sein, die sich von 0 % für die verfügbaren Stunden unterscheidet, um einen Wert für ein Aufgabengebiet im Ressourcenplaner anzuzeigen. Wenn ein(e) Benutzende(r) einer Funktion mit einer 0 % **Prozentsatz der FTE-Verfügbarkeit** zugeordnet ist, ist der Wert Verfügbare Stunden für dieses Aufgabengebiet null. In diesem Fall kann die Rolle einen negativen **Nettowert“**.\
     >Weitere Informationen zum **Prozentsatz der FTE-Verfügbarkeit** für Aufgabengebiete finden Sie im Artikel [Bearbeiten des Benutzerprofils](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   * Geben **in der Spalte** BDG) manuell die Anzahl der budgetierten Stunden, VZÄ oder Kosten für das Projekt an. Dadurch wird die Anzahl der vom Projekt budgetierten Stunden auf die einzelnen Funktionen unter dem Projekt verteilt. Die folgenden Szenarien sind vorhanden:

      * Wenn die von Ihnen angegebene Anzahl von budgetierten Stunden des Projekts den geplanten Stunden des Projekts entspricht, entsprechen die budgetierten Stunden des Aufgabengebiets den geplanten Stunden des Aufgabengebiets.
      * Wenn die von Ihnen angegebene Anzahl von budgetierten Projektstunden nicht mit den geplanten Projektstunden übereinstimmt, werden die budgetierten Stunden der Funktion entsprechend dem Prozentsatz der für jede Funktion erforderlichen geplanten Stunden verteilt.\
        Beispiel: Wenn ein Projekt 20 geplante Stunden hat und diese auf zwei Aufgabengebiete aufgeteilt sind (Berater benötigt 12 geplante Stunden und Ingenieur benötigt 8 geplante Stunden) und Sie für das Projekt 30 Stunden budgetieren, werden die Stunden wie folgt aufgeteilt: Die Funktion Berater erhält 18 budgetierte Stunden und die Funktion Ingenieur erhält 12 budgetierte Stunden.

1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für das Projekt vorzunehmen:

   * Budgetieren Sie die Rollen unter dem Projekt, wie in Schritt 7 beschrieben.\
     Die budgetierten Stunden des Projekts werden anhand der folgenden Formel berechnet:

     `Project Budgeted Hours = SUM(Role Budgeted Hours)`

   * Geben **in der Spalte** BDG) manuell die Anzahl der budgetierten Stunden, VZÄ oder Kosten für das Projekt an.\
     Dadurch werden die für die Funktion budgetierten Stunden aktualisiert, wie in Schritt 7 beschrieben.\
     ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. Klicken Sie auf **Speichern**.\
   Nachdem Sie die Ressourcen im Ressourcenplaner budgetiert haben, werden die budgetierten Stunden für die Ressourcen und die damit verbundenen Kosten im Business Case jedes Projekts aufgeführt.\
   Weitere Informationen zum Verständnis des Bereichs „Ressourcenbudgetierung“ des Business Case finden Sie im Abschnitt „Ressourcenbudgetierung“ im Artikel [Überblick über die Bereiche des Business Case](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) Wählen Sie die Benutzeransicht aus, um Benutzerüberallokationen oder eine unzureichende Auslastung zwischen der verfügbaren und der geplanten Stunde für jeden Benutzer zu bemerken. Budgetierte Stunden sind in der Benutzeransicht nicht sichtbar.

   Weitere Informationen dazu, wie Workfront die Verfügbarkeit von Benutzenden berechnet, finden Sie unter [Konfigurieren von Ressourcenverwaltungseinstellungen](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Budgetressourcen in der Rollenansicht {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

Sie müssen Bearbeitungszugriff auf die Ressourcen-Management- und Finanzdaten sowie Finanzverwaltungsberechtigungen für die Projekte haben, um Ressourcen im Ressourcenplaner zu budgetieren. Wenn Sie nur Ansichtszugriff auf mindestens ein Projekt haben, das unter einem Aufgabengebiet aufgeführt ist, können Sie in der Ansicht „Funktion“ keine Zuteilungen für das Aufgabengebiet budgetieren. Sie können weiterhin Budgetzuweisungen für die Projekte durchführen, für die Sie über Verwaltungsberechtigungen verfügen.

Informationen zum Zugriff, der für die Budgetierung von Ressourcen erforderlich ist, finden Sie im Artikel [Zugriff auf die Budgetierung von Ressourcen in Adobe Workfront erforderlich](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

So budgetieren Sie Zuteilungen im Ressourcenplaner in der ****:

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken Sie auf **Ressourcen**.
1. Der **Planer** wird standardmäßig angezeigt.
1. (Bedingt) Wählen Sie die Ansicht **Nach Rolle anzeigen** aus.
1. Erweitern Sie die Aufgabengebiete und Projekte, um die Zuordnung für das Projekt, die Aufgabengebiete oder die Benutzer zu verwalten.
1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für Benutzer vorzunehmen:

   * Geben **in der Spalte** BDG) manuell die Anzahl der budgetierten Stunden, VZÄ oder Kosten für die Benutzer an.
   * Klicken Sie auf das **Mehr**-Menü für das Projekt und dann auf **Geplante Stunden der Benutzer als „Budgetiert“**.\
     Die budgetierten Stunden der einzelnen Benutzer werden anhand der folgenden Formel berechnet:

     `User Budgeted Hours = User Planned Hours`

1. Führen Sie einen der folgenden Schritte aus, um eine Budgetzuweisung für Aufgabengebiete vorzunehmen:

   * Geben **in der Spalte** BDG) manuell die Anzahl der budgetierten Stunden, VZÄ oder Kosten für die Aufgabengebiete an.\
     Dadurch werden die für die Funktion budgetierten Stunden auf die budgetierten Stunden des Projekts für die Projekte verteilt, auf die Sie Zugriff haben.

   * Klicken Sie auf das **Mehr**-Menü für das Aufgabengebiet und dann auf **Geplante Stunden für Projekte als „Budgetiert“ festlegen.**Die für die Funktion budgetierten Stunden werden anhand der folgenden Formel berechnet:\
     *

     `Role Budgeted Hours = SUM(Project Budgeted Hours)`

     *Die budgetierten Stunden des Projekts werden anhand der folgenden Formel berechnet:

     `Project Budgeted Hours = Project Planned Hours`

   * Geben **in der Spalte** BDG) manuell die Anzahl der budgetierten Stunden, FTEs oder Kosten für die Projekte an, die unter dem Aufgabengebiet aufgeführt sind.\
     Dadurch wird der Funktion die Anzahl der vom Projekt budgetierten Stunden hinzugefügt.

   >[!NOTE]
   >
   >Benutzer können sowohl für Primäre als auch für andere (oder sekundäre) Funktionen budgetiert werden. Der **Prozentsatz der FTE-Verfügbarkeit** für die Rollen des Benutzers muss eine Zahl sein, die sich von 0 % für die verfügbaren Stunden unterscheidet, um einen Wert für ein Aufgabengebiet im Ressourcenplaner anzuzeigen. Wenn ein(e) Benutzende(r) einer Funktion mit einer 0 % **Prozentsatz der FTE-Verfügbarkeit** zugeordnet ist, ist der Wert Verfügbare Stunden für dieses Aufgabengebiet null. In diesem Fall kann die Rolle einen negativen **Nettowert“**.\
   >Weitere Informationen zum **Prozentsatz der FTE-Verfügbarkeit** für Aufgabengebiete finden Sie im Artikel [Bearbeiten des Benutzerprofils](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für das Projekt vorzunehmen:

   * Geben **in der Spalte** BDG) manuell die Anzahl der budgetierten Stunden, VZÄ oder Kosten für die Projekte an.\
     Dadurch werden auch die budgetierten Stunden für die Funktionen aktualisiert, unter denen das Projekt aufgeführt ist.

   * Klicken Sie auf das **Mehr** für das Aufgabengebiet und dann auf **Geplante Stunden für Projekte als budgetiert festlegen**.\
     Die budgetierten Stunden des Projekts werden anhand der folgenden Formel berechnet:

     `Project Budgeted Hours = Project Planned Hours`

     Die budgetierten Stunden des Projekts werden der Funktion „Budgetierte Stunden“ hinzugefügt.

   * (Bedingt) Wenn Sie die Stunden für die Benutzer budgetiert haben, klicken Sie auf das Menü **Mehr** für das Projekt und dann auf **Budgetierte Stunden der Benutzer insgesamt für Projekt**.\
     Die budgetierten Stunden des Projekts werden anhand der folgenden Formel berechnet:

     `Project Budgeted Hours = SUM(User Budgeted Hours)`

     ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. Klicken Sie auf **Speichern**.\
   Nachdem Sie die Ressourcen im Ressourcenplaner budgetiert haben, werden die budgetierten Stunden für die Ressourcen und die damit verbundenen Kosten im Business Case jedes Projekts aufgeführt.
Weitere Informationen zum Thema Ressourcenbudgetierung im Business Case finden Sie im Artikel [Budgetressourcen im Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Optional) Wählen Sie die Ansicht **Nach Benutzer anzeigen**, um Benutzerüberallokationen oder eine unzureichende Auslastung zwischen den verfügbaren und den geplanten Stunden für jeden Benutzer zu bemerken. Budgetierte Stunden werden in der Ansicht Nach Benutzer anzeigen nicht angezeigt.

### Gesamtbudget {#budget-resources-in-bulk}

Bei Verwendung von Schnellverknüpfungen können Sie die Zuteilung von Budgets für Ihre Ressourcen stapelweise budgetieren. Die Schnelllinks sind nur für die Projekt- und Rollenansichten verfügbar.

![Optionen für die automatische Budgetierung](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Bei Verwendung der Schnellverknüpfungen zu Budgetzuweisungen für Ressourcen wird die Budgetierung automatisch nur auf die auf dem Bildschirm angezeigten Zeiträume angewendet. Wenn sich die Zeitleiste eines Projekts über einen längeren Zeitraum als den auf dem Bildschirm angezeigten erstreckt, müssen Sie von links nach rechts scrollen und dann die Schnelllinks verwenden, um Ihre Ressourcen automatisch zu budgetieren.

So budgetieren Sie Ressourcen stapelweise:

1. Navigieren Sie zu .\
   Weitere Informationen zum Zugriff auf den Ressourcenplaner finden Sie im Abschnitt „Zugriff auf den Ressourcenplaner“ im Artikel [Ressourcenplaner - Übersicht](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   In der Liste wird eine Liste der Projekte angezeigt, die Sie verwalten können.

1. (Optional) Erweitern Sie jedes Projekt, um eine Liste der damit verbundenen Aufgabengebiete anzuzeigen.\
   Oder
1. (Optional) Wählen Sie **Nach Rolle anzeigen** und erweitern Sie dann jede Rolle, um eine Liste der damit verbundenen Projekte anzuzeigen.
1. Bewegen Sie den Mauszeiger über den Namen eines Projekts oder Aufgabengebiets.
1. Klicken Sie auf das **Mehr**-Symbol ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png), das ganz rechts neben dem Projekt- oder Rollennamen angezeigt wird.

1. Klicken Sie auf eine der verfügbaren Optionen, um den Betrag der budgetierten Stunden (BDG) für andere Objekte automatisch anzugeben.

   Je nachdem, ob Sie auf das Symbol Mehr in einem Projekt oder einer Rolle geklickt haben, unterscheiden sich die Optionen für die Massenbudgetierung. Die nachstehende Tabelle zeigt die für Projekte und Rollen verfügbaren Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>Projektansicht</strong> </td> 
      <td><strong>Rollenansicht</strong> </td> 
     </tr> 
     <tr> 
      <td>Projektoptionen</td> 
      <td> 
       <ul> 
        <li><strong>Geplante Stunden der Funktionen als budgetiert festlegen</strong>: Wählen Sie diese Option, damit die budgetierten Stunden der Funktion mit ihren geplanten Stunden identisch werden. Die Summe der budgetierten Stunden für die Funktionen wird für die budgetierten Stunden des Projekts angezeigt. </li> 
        <li><strong>Budgetierungsdaten anpassen</strong> : Wählen Sie diese Option, um die budgetierten Stunden in einen anderen Zeitrahmen zu verschieben.<br>Weitere Informationen zum Anpassen von Budgetierungsdaten finden Sie <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Anpassen von Budgetierungsdaten im Ressourcenplaner</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Geplante Stunden der Benutzer als budgetiert festlegen</strong>: Wählen Sie diese Option, damit die budgetierten Stunden der Benutzer mit ihren geplanten Stunden identisch werden. </li> 
        <li><strong>Budgetierte Stunden der Benutzer insgesamt für Projekt</strong>: Wählen Sie diese Option, um alle budgetierten Stunden der Benutzer hinzuzufügen und die Summe als budgetierte Stunden für das Projekt und für die Funktion anzuzeigen. Es wird empfohlen, diese Option zu verwenden, nachdem Sie entweder Ihre Benutzer manuell budgetiert haben oder Sie die vorherige Option zuerst verwendet haben. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Rollenoptionen</td> 
      <td> 
       <ul> 
        <li><strong>Geplante Stunden der Benutzer als budgetiert festlegen</strong>: Wählen Sie diese Option, damit die budgetierten Stunden der Benutzer mit den geplanten Stunden identisch werden. </li> 
        <li><strong>Summe der budgetierten Stunden der Benutzer für Funktion</strong>: Wählen Sie diese Option, um alle budgetierten Stunden der Benutzer zusammenzufassen und die Summe als budgetierte Stunden für die Funktion und das Projekt anzuzeigen. Es wird empfohlen, diese Option zu verwenden, nachdem Sie entweder Ihre Benutzer manuell budgetiert haben oder Sie die vorherige Option zuerst verwendet haben. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Geplante Stunden der Projekte als budgetiert festlegen</strong>: Wählen Sie diese Option, damit die budgetierten Stunden des Projekts mit den geplanten Stunden des Projekts identisch werden. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Einige der Optionen werden möglicherweise nicht angezeigt, wenn einige der Voraussetzungen für die Arbeit im Ressourcenplaner fehlen.
   >
   >
   >Weitere Informationen zu den Voraussetzungen, die für eine präzise Budgetierung im Ressourcenplaner erfüllt sein müssen, finden Sie im Abschnitt „Voraussetzungen für die Arbeit im Ressourcenplaner“ im Artikel [Ressourcenplaner - Übersicht](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   >Beispielsweise werden einige der Optionen in den folgenden Szenarien möglicherweise nicht angezeigt:
   >
   >   
   >   
   >   * Wenn Projekte nicht mit dem Ressourcenpool verknüpft sind
   >   * Wenn Ressourcenpools, die mit Projekten verknüpft sind, keine Benutzer enthalten
   >   * Wenn Ressourcenpools, die mit Projekten verknüpft sind, Benutzer enthalten, denen kein Aufgabengebiet zugeordnet ist.
   >   
   >
