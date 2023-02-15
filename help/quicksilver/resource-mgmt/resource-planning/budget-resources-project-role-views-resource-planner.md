---
product-area: resource-management
navigation-topic: resource-planning
title: Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Rollenansicht
description: Sie können Ressourcen im Adobe Workfront Resource Planer mithilfe der Projekt- und Rollenansicht einplanen. Sie können keine Ressourcen mit der Ansicht "User"im Ressourcenplaner einplanen.
author: Alina
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2160'
ht-degree: 0%

---

# Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Rollenansicht

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

Die Hauptfunktion des Ressourcenplaners besteht darin, Ihre Ressourcen für die Arbeit zu veranschlagen, die für Projekte durchgeführt werden muss.

>[!IMPORTANT]
>
>Sie können Ihre Ressourcen nur mit der **Anzeigen nach Projekt** oder **Ansicht nach Rolle** Ansichten zum Ressourcenplaner.

Bevor Sie mit Budgetinformationen im Ressourcenplaner beginnen, lesen Sie die folgenden Artikel:

* [Übersicht über den Ressourcenplaner](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Erforderlicher Zugriff auf Budgetressourcen in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf das Ressourcen-Management, das Zugriff auf die Option "Prioritäten bearbeiten"und die Budgetzeiten im Ressourcenplaner enthält.</p> <p>Zugriff auf Finanzdaten zu Budgetressourcen nach Kosten bearbeiten</p> <p>Zugriff auf Projekte und Benutzer bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für die Projekte, für die Sie Informationen zum Budget benötigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Budgetressourcen im Ressourcenplaner

* [Budgetressourcen in der Projektansicht](#budget-resources-in-the-project-view)
* [Budgetressourcen in der Rollenansicht](#budget-resources-in-the-role-view)
* [Massenbasierte Budgetmittel](#budget-resources-in-bulk)

### Budgetressourcen in der Projektansicht {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Ressourcen**.
1. Die **Planen** wird standardmäßig angezeigt.
1. (Bedingt) Wählen Sie die **Anzeigen nach Projekt** anzeigen.
1. Erweitern Sie die Projekte und die Auftragsrollen, um die Zuordnung für das Projekt, die Rollen oder Benutzer zu verwalten.
1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für Benutzer vorzunehmen:

   * Im **BDG** -Spalte manuell eine Anzahl von geplanten Stunden, FTE oder Kosten für die Benutzer angeben.

   * Klicken Sie auf **Mehr** Menü für die Auftragsrolle des Benutzers aus und klicken Sie auf **Festlegen der geplanten Benutzerzeiten als Budget**.\
      Die budgetierten Stunden eines jeden Benutzers werden anhand der folgenden Formel berechnet:

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für Stellenrollen vorzunehmen:

   * Im **BDG** -Spalte manuell eine Anzahl von geplanten Stunden, FTE oder Kosten für die Stellenfunktion angeben.

      >[!NOTE]
      >
      >Die Role Budgeted Hours werden zu den Projekt Budgeted Hours hinzugefügt.

   * (Bedingt) Wenn Sie die geplanten Stunden für Benutzer festgelegt haben, klicken Sie auf die Schaltfläche **Mehr** Menü für die Auftragsrolle aus und klicken Sie auf **Gesamtbesuchszeit in der Benutzerplanung für die Rolle**.\
      Die für die einzelnen Rollen veranschlagten Stunden werden anhand der folgenden Formel berechnet:

      ```
      Role Budgeted Hours = SUM(User Budgeted Hours)
      ```

   * Klicken Sie auf **Mehr** Menü für das Projekt aus und klicken Sie auf **Geplante Stunden für Rollen als Budget festlegen**.\
      Die für die einzelnen Rollen veranschlagten Stunden werden anhand der folgenden Formel berechnet:\
      *

      ```
      Role Budgeted Hours = Role Planned Hours
      ```

      >[!NOTE]
      >   
      >* Die Role Budgeted Hours werden zu den Projekt Budgeted Hours hinzugefügt.
      >* Benutzer können sowohl für Primäre als auch für andere (oder sekundäre) Rollen in den Budgets eingebunden werden.
      >* Die **Prozentsatz der VZÄ-Verfügbarkeit** für die Rollen des Benutzers muss eine Zahl sein, die sich von 0 % unterscheidet, damit die verfügbaren Stunden im Ressourcenplaner einen Wert für eine Auftragsrolle anzeigen. Wenn ein Benutzer einer Rolle mit einer 0 %-Marke zugeordnet ist **Prozentsatz der VZÄ-Verfügbarkeit**, ist der Wert Verfügbare Stunden für diese Auftragsrolle null. In diesem Fall zeigt die Rolle möglicherweise ein negatives **Nettowert**.\
         >Weitere Informationen zum **Prozentsatz der VZÄ-Verfügbarkeit** Informationen zu Vorgangsrollen finden Sie im Artikel . [Benutzerprofil bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).


   * Im **BDG** -Spalte manuell eine Anzahl an geplanten Stunden, FTE oder Kosten für das Projekt angeben. Dadurch wird die Anzahl der geplanten Stunden an jede Rolle im Rahmen des Projekts verteilt. Die folgenden Szenarien existieren:

      * Entspricht die Anzahl der für Ihr Projekt vorgesehenen Stunden der Anzahl der geplanten Projektstunden, entsprechen die für die Rolle vorgesehenen Stunden den für die geplanten Stunden.
      * Wenn die Anzahl der von Ihnen angegebenen projektbudgetierten Stunden nicht mit den geplanten Stunden des Projekts übereinstimmt, werden die Rollenbudgetierungsstunden entsprechend dem Prozentsatz der geplanten Stunden verteilt, der für jede Rolle benötigt wird.\
         Wenn ein Projekt beispielsweise 20 geplante Stunden umfasst und auf zwei Jobrollen verteilt ist (ein Berater benötigt 12 geplante Stunden und ein Ingenieur 8 geplante Stunden) und Sie 30 Stunden für das Projekt einplanen, werden die Stunden wie folgt verteilt: die Beraterrolle erhält 18 Budgetzeit und die Ingenieurrolle erhält 12 Budgetzstunden.

1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für das Projekt vorzunehmen:

   * Budget der Rollen im Rahmen des Projekts, wie in Schritt 7 beschrieben.\
      Die im Projekt veranschlagten Stunden werden nach folgender Formel berechnet:

      ```
      Project Budgeted Hours = SUM(Role Budgeted Hours)
      ```

   * Im **BDG** -Spalte manuell eine Anzahl an geplanten Stunden, FTE oder Kosten für das Projekt angeben.\
      Dadurch wird die Rolle der budgetierten Stunden aktualisiert, wie in Schritt 7 beschrieben.\
      ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. Klicken Sie auf **Speichern**.\
   Nachdem Sie Ihre Ressourcen im Ressourcen-Planer zusammengefasst haben, werden die budgetierten Stunden für Ihre Ressourcen und alle damit verbundenen Kosten im Business Case jedes Projekts aufgelistet.\
   Weitere Informationen zum Verständnis des Ressourcenbudgeting-Bereichs des Geschäftsfalls finden Sie im Abschnitt &quot;Ressourcenbudgeting&quot;im Artikel [Überblick über die Bereiche des Geschäftsfalles](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) Wählen Sie die Ansicht &quot;User&quot;aus, um festzustellen, ob die Benutzer für jeden Benutzer über die verfügbare und die geplante Stunde hinausreichen oder nicht genügend ausgelastet sind. Budgetierte Stunden sind in der Benutzeransicht nicht sichtbar.

   Informationen dazu, wie Workfront die Verfügbarkeit eines Benutzers berechnet, finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Budgetressourcen in der Rollenansicht {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

Sie müssen Zugriff auf Ressourcen-Management und Finanzdaten bearbeiten und Finanzberechtigungen für die Projekte verwalten haben, um im Ressourcenplaner über Budgetressourcen verfügen zu können. Wenn Sie nur Zugriff auf Anzeigen für mindestens ein Projekt haben, das unter einer Auftrags-Rolle aufgeführt ist, können Sie keine Zuweisung von Budgets für die Rolle in der Rollenansicht vornehmen. Sie können weiterhin die Budgetzuweisung für die Projekte vornehmen, für die Sie über Verwaltungsberechtigungen verfügen.

Informationen über den für Haushaltsmittel benötigten Zugriff finden Sie im Artikel [Erforderlicher Zugriff auf Budgetressourcen in Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

So weisen Sie Budgetzuweisungen im Ressourcenplaner in der Ansicht &quot;Rolle&quot;zu:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Ressourcen**.
1. Die **Planen** wird standardmäßig angezeigt.
1. (Bedingt) Wählen Sie die **Ansicht nach Rolle** anzeigen.
1. Erweitern Sie die Auftragsrollen und die Projekte, um die Zuordnung für das Projekt, die Jobrollen oder Benutzer zu verwalten.
1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für Benutzer vorzunehmen:

   * Im **BDG** -Spalte manuell eine Anzahl von geplanten Stunden, FTE oder Kosten für die Benutzer angeben.
   * Klicken Sie auf **Mehr** Menü für das Projekt aus und klicken Sie auf **Festlegen der geplanten Benutzerzeiten als Budget**.\
      Die budgetierten Stunden eines jeden Benutzers werden anhand der folgenden Formel berechnet:

      ```
      User Budgeted Hours = User Planned Hours
      ```

1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für Stellenrollen vorzunehmen:

   * Im **BDG** -Spalte manuell eine Anzahl von geplanten Stunden, FTE oder Kosten für die Stellenrollen angeben.\
      Dadurch werden die &quot;Role Budgeted Hours&quot;für die Projekte, auf die Sie Zugriff haben, auf die &quot;Project Budgeted Hours&quot;verteilt.

   * Klicken Sie auf **Mehr** -Menü für die Rolle &quot;Job&quot;aus und klicken Sie dann auf &quot;Planen Sie die Stunden der Projekte auf &quot;Geplant&quot;einstellen.**Die Rollenbudgetierungsstunden werden anhand der folgenden Formel berechnet:\
      *

      ```
      Role Budgeted Hours = SUM(Project Budgeted Hours)
      ```

      *Die budgetierten Projektstunden werden mit der folgenden Formel berechnet:

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

   * Im **BDG** -Spalte manuell eine Anzahl von geplanten Stunden, FTE oder Kosten für die Projekte angeben, die unter der Stellenfunktion aufgeführt sind.\
      Dadurch wird die Anzahl der geplanten Stunden zur Rolle hinzugefügt.
   >[!NOTE]
   >
   >Benutzer können sowohl für Primäre als auch für andere (oder sekundäre) Rollen in den Budgets eingebunden werden. Die **Prozentsatz der VZÄ-Verfügbarkeit** für die Rollen des Benutzers muss eine Zahl sein, die sich von 0 % unterscheidet, damit die verfügbaren Stunden im Ressourcenplaner einen Wert für eine Auftragsrolle anzeigen. Wenn ein Benutzer einer Rolle mit einer 0 %-Marke zugeordnet ist **Prozentsatz der VZÄ-Verfügbarkeit**, ist der Wert Verfügbare Stunden für diese Auftragsrolle null. In diesem Fall zeigt die Rolle möglicherweise ein negatives **Nettowert**.\
   >Weitere Informationen zum **Prozentsatz der VZÄ-Verfügbarkeit** Informationen zu Vorgangsrollen finden Sie im Artikel . [Benutzerprofil bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Führen Sie einen der folgenden Schritte aus, um die Budgetzuweisung für das Projekt vorzunehmen:

   * Im **BDG** -Spalte manuell eine Anzahl von geplanten Stunden, FTE oder Kosten für die Projekte angeben.\
      Dadurch werden auch die budgetierten Stunden für die Rollen aktualisiert, unter denen das Projekt aufgeführt ist.

   * Klicken Sie auf **Mehr** Menü für die Auftragsrolle aus und klicken Sie auf **Festlegen der geplanten Projektzeit als Budget**.\
      Die im Projekt veranschlagten Stunden werden nach folgender Formel berechnet:

      ```
      Project Budgeted Hours = Project Planned Hours
      ```

      Das Projekt Budgeted Hours wird den Role Budgeted Hours hinzugefügt.

   * (Bedingt) Wenn Sie die Stunden für die Benutzer in den Budgets festgelegt haben, klicken Sie auf die Schaltfläche **Mehr** Menü für das Projekt aus und klicken Sie auf **Gesamtbesuchszeit für das Projekt**.\
      Die im Projekt veranschlagten Stunden werden anhand der folgenden Formel berechnet:

      ```
      Project Budgeted Hours = SUM(User Budgeted Hours)
      ```

      ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. Klicken Sie auf **Speichern**.\
   Nachdem Sie Ihre Ressourcen im Ressourcen-Planer zusammengefasst haben, werden die budgetierten Stunden für Ihre Ressourcen und alle damit verbundenen Kosten im Business Case jedes Projekts aufgelistet.\
   Weitere Informationen zum Verständnis des Ressourcenbudgeting-Bereichs des Geschäftsfalls finden Sie im Artikel [Haushaltsmittel im Geschäftsfall](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Optional) Wählen Sie die **Ansicht nach Benutzer** um zu bemerken, dass die Benutzer für jeden Benutzer eine Überzuweisung oder Unterauslastung zwischen den verfügbaren und den geplanten Stunden vorgenommen haben. Budgetierte Stunden sind in der Ansicht &quot;View by User&quot;nicht sichtbar.

### Massenbasierte Budgetmittel {#budget-resources-in-bulk}

Bei Verwendung von Schnelllinks können Sie die Zuweisung von Ressourcen in großen Mengen vornehmen. Die Schnelllinks sind nur für Projekt- und Rollenansichten verfügbar.

![](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Bei Verwendung der Quick Links zu Budgetzuweisungen für Ressourcen wird die Budgetierung automatisch nur auf die auf dem Bildschirm angezeigten Zeiträume angewendet. Wenn sich die Timeline eines Projekts über einen längeren Zeitraum als den auf Ihrem Bildschirm angezeigten Zeitraum erstreckt, müssen Sie von links nach rechts blättern und dann die Quick Links verwenden, um Ihre Ressourcen automatisch zu budgetieren.

So planen Sie Ihre Ressourcen in großen Mengen:

1. Navigieren Sie zu .\
   Weitere Informationen zum Zugriff auf den Ressourcen-Planer finden Sie im Abschnitt &quot;Zugriff auf den Ressourcen-Planer&quot;im Artikel [Übersicht über den Ressourcenplaner](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   Eine Liste der Projekte, die Sie verwalten können, wird in der Liste angezeigt.

1. (Optional) Erweitern Sie jedes Projekt, um eine Liste der ihm zugeordneten Auftragsrollen anzuzeigen.\
   Oder
1. (Optional) Wählen Sie **Ansicht nach Rolle** und erweitern Sie dann jede Rolle, um eine Liste der ihr zugeordneten Projekte anzuzeigen.
1. Bewegen Sie den Mauszeiger über den Namen eines Projekts oder einer Auftragsrolle.
1. Klicken Sie auf **Mehr** icon ![options_icon_resource_planner.png](assets/options-icon-resource-planner.png)wird ganz rechts neben dem Projekt- oder Rollennamen angezeigt.

1. Klicken Sie auf eine der verfügbaren Optionen, um automatisch den Betrag der budgetierten Stunden (BDG) für andere Objekte anzugeben.

   Je nachdem, ob Sie in einem Projekt oder in einer Rolle auf das Symbol Mehr geklickt haben, unterscheiden sich die Optionen für das stapelweise Budgetieren. Die folgende Tabelle zeigt die für Projekte und Rollen verfügbaren Optionen:

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
        <li><strong>Geplante Stunden für Rollen als Budget festlegen</strong>: Wählen Sie diese Option, damit die budgetierten Stunden der Rolle mit den geplanten Stunden identisch werden. Die Gesamtdauer der geplanten Stunden für die Rollen wird für die geplanten Stunden angezeigt. </li> 
        <li><strong>Anpassen der Budgetierungsdaten</strong> : Wählen Sie diese Option aus, um die budgetierten Stunden in einen anderen Zeitrahmen zu verschieben.<br>Weitere Informationen zur Anpassung der Budgetierungsdaten finden Sie unter <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Anpassen der Budgetierungsdaten im Ressourcenplaner</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Festlegen der geplanten Benutzerzeiten als Budget</strong>: Wählen Sie diese Option, damit die Budgetierungszeiten des Benutzers mit den geplanten Stunden identisch werden. </li> 
        <li><strong>Gesamtbesuchszeit für das Projekt</strong>: Wählen Sie diese Option aus, um alle Benutzer mit der Option "Budgetierte Stunden"hinzuzufügen und die Gesamtsumme als die budgetierten Stunden für das Projekt und die Rolle anzuzeigen. Es wird empfohlen, diese Option zu verwenden, nachdem Sie entweder Ihre Benutzer manuell in den Haushalt eingebunden haben oder zuvor die vorherige Option verwendet haben. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Rollenoptionen</td> 
      <td> 
       <ul> 
        <li><strong>Festlegen der geplanten Benutzerzeiten als Budget</strong>: Wählen Sie diese Option, damit die Budgetierungszeiten des Benutzers mit den geplanten Stunden identisch werden. </li> 
        <li><strong>Gesamtbesuchszeit in der Benutzerplanung für die Rolle</strong>: Wählen Sie diese Option aus, um alle Budgetzeit des Benutzers hinzuzufügen und die Gesamtsumme als die budgetierten Stunden für die Rolle und das Projekt anzuzeigen. Es wird empfohlen, diese Option zu verwenden, nachdem Sie entweder Ihre Benutzer manuell in den Haushalt eingebunden haben oder zuvor die vorherige Option verwendet haben. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Festlegen der geplanten Projektzeit als Budget</strong>: Wählen Sie diese Option, damit die budgetierten Stunden des Projekts mit den geplanten Stunden identisch werden. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Einige der Optionen werden möglicherweise nicht angezeigt, wenn einige der Voraussetzungen für die Arbeit im Ressourcenplaner fehlen.
   >
   >
   >Weitere Informationen zu den Voraussetzungen, die für eine korrekte Budgetierung im Ressourcen-Planer erfüllt sein müssen, finden Sie im Abschnitt &quot;Voraussetzungen für die Arbeit im Ressourcen-Planer&quot;im Abschnitt [Übersicht über den Ressourcenplaner](../../resource-mgmt/resource-planning/get-started-resource-planner.md) Artikel.\
   >Einige der Optionen werden beispielsweise in den folgenden Szenarien möglicherweise nicht angezeigt:
   >
   >   
   >   
   >   * Wenn Projekte nicht mit Resource Pool verknüpft sind
   >   * Wenn Ressourcenpools, die mit Projekten verknüpft sind, keine Benutzer enthalten
   >   * Wenn Ressourcen-Pools, die mit Projekten verknüpft sind, Benutzer enthalten, denen keine Auftragsrolle zugeordnet ist.

