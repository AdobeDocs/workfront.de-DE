---
navigation-topic: business-case-and-scorecards
title: Budgetressourcen im Business Case mithilfe des Resource Planers
description: Im Rahmen der Ressourcenplanung können Sie den Ressourcen-Planer auf Projektebene verwenden, um beim Erstellen des Geschäftsfalls die für das Abschließen der Arbeit in einem Projekt erforderlichen Arbeitsplatzrollen zu planen.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# Budgetressourcen im Business Case mithilfe des Resource Planers

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Im Rahmen der Ressourcenplanung können Sie den Ressourcen-Planer auf Projektebene verwenden, um beim Erstellen des Geschäftsfalls die für das Abschließen der Arbeit in einem Projekt erforderlichen Arbeitsplatzrollen zu planen.

Weitere Informationen zum Erstellen eines Geschäftsfalls finden Sie unter [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Die Informationen, die Sie im Ressourcenplaner auf Projektebene eingeben, sind auch im Ressourcenplaner auf Systemebene sichtbar. Das Gegenteil ist auch der Fall. Informationen zum Ressourcen-Planer finden Sie unter [Übersicht über den Ressourcenplaner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Sie können Ressourcen im Geschäftsfall auch mit dem Adobe Workfront-Szenario-Planer einplanen. Weitere Informationen finden Sie unter [Budgetressourcen im Geschäftsfall mit dem Szenario-Planer](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-Abo</a>*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>*</td> 
   <td> <p>Überprüfen oder höher</p> <p>Wichtig: Sie müssen über eine Planungslizenz verfügen, um die Informationen zur Ressourcenbudgetierung zu ändern. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Folgendes: </p> 
    <ul> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Finanzielle Daten</p> </li> 
    </ul> <p>Informationen über den benötigten Zugriff auf Budgetressourcen finden Sie auch unter <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Erforderlicher Zugriff auf Budgetressourcen in Adobe Workfront</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Adobe Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie Folgendes tun:

* Erfüllen Sie alle Voraussetzungen für die Ressourcenplanung in Adobe Workfront. Weitere Informationen finden Sie unter [Übersicht über den Ressourcenplaner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Verknüpfen Sie Ressourcenpools mit dem Projekt.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   Sie können keine Ressourcen für Probleme im Geschäftsfall einplanen. Sie können sie im Ressourcenplaner auf Systemebene einplanen. Weitere Informationen zum Ressourcen-Planer finden Sie unter [Übersicht über den Ressourcenplaner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Obwohl dies keine Voraussetzung ist, empfehlen wir auch, für die Aufgaben im Projekt &quot;Geplante Stunden&quot;anzugeben. Auf diese Weise können Sie nachvollziehen, wie viel Arbeit eine Aufgabe möglicherweise benötigt, was wiederum bei der Entscheidung hilft, für viel Zeit die Ressourcen in den Haushalt eingestellt werden müssen, um die Aufgabe abzuschließen. Informationen zum Verknüpfen von Aufgaben mit geplanten Stunden finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Anwenden von Ressourcen-Pools auf ein Projekt und Budgetressourcen im Geschäftsfall

>[!IMPORTANT]
Sie können Ihre Ressourcen für einen Zeitraum von 15 Jahren einplanen. Wenn Sie Ressourcen für ein Projekt mit einer Dauer von mehr als 15 Jahren einsetzen, sind die Budgetierungsinformationen möglicherweise nicht korrekt.

So wenden Sie Ressourcenpools und Budgetprojektressourcen im Geschäftsfall für ein Projekt ohne Ressourcenpool an:

1. Wechseln Sie zu dem Projekt, für das Sie Ressourcen planen möchten.
1. Klicken **Geschäftsfall** im linken Bereich.
1. (Bedingt) Wenn Ihr Unternehmen keine Lizenz für den Workfront-Szenario-Planer besitzt, klicken Sie auf **Ressourcen-Budgetierung bearbeiten** im **Ressourcen-Budgetierung** und fahren Sie dann mit Schritt 5 fort.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Optional und bedingt) Wenn die Projektinformationen aus einer Initiative im Szenario-Planer veröffentlicht wurden, führen Sie einen der folgenden Schritte aus:

   * Wählen Sie Ressourcenplaner im **Wählen Sie aus, welche Stunden für die Berechnung der budgetierten Arbeitskosten des Projekts verwendet werden sollen** und klicken Sie auf **Auswählen > Ressourcen-Budgetierung bearbeiten**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Wenn Sie den Szenario-Planer für die Budgetierungsressourcen für das Projekt ausgewählt haben, klicken Sie auf **Änderung** > **Ressourcen-Budgetierung bearbeiten**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   Hierbei werden die budgetierten Stunden des Projekts verwendet, um die für das Projekt veranschlagten Arbeitskosten zu berechnen.

   Der Szenario-Planer ist nur im neuen Adobe Workfront-Erlebnis verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Übersicht über den Szenario-Planer](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   Es wird empfohlen, bei der Arbeit an einem Projekt zu entscheiden, ob Sie den Ressourcen-Planer oder den Szenario-Planer verwenden möchten. Ein häufiger Wechsel zwischen den beiden während der Laufzeit des Projekts kann zu Inkonsistenzen in der Art und Weise führen, wie Sie Ihre Ressourcen für das Projekt einsetzen.

1. Im **Ressourcenpool auswählen** ein oder mehrere **Ressourcen-Pools**.

   Sie dürfen nur Ressourcen-Pools angeben, die mit aktiven Benutzern gefüllt sind.

   >[!TIP]
   Wenn das Projekt bereits mit Ressourcenpools verknüpft ist, wird der Ressourcen-Planer standardmäßig angezeigt. Um dem Projekt weitere Ressourcen-Pools hinzuzufügen, bearbeiten Sie das Projekt. Weitere Informationen zum Bearbeiten eines Projekts finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicken **Anwenden**.

   Der Ressourcen-Planer wird für das ausgewählte Projekt angezeigt.

   Standardmäßig sind die ersten 20 mit diesem Projekt verknüpften Auftragsrollen im Abschnitt Ressourcenbudgeting in alphabetischer Reihenfolge aufgelistet. 

   Weitere Informationen zum Ressourcen-Planer finden Sie unter [Übersicht über den Ressourcenplaner](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Optional und bedingt) Erweitern Sie die Auftragsrollen, um die ihnen zugeordneten Benutzer anzuzeigen.

   >[!NOTE]
   Aktive Benutzer werden nur dann unter den ihnen zugeordneten Vorgangsrollen angezeigt, wenn sie die folgenden Kriterien erfüllen:
   * Sie gehören zu einem der Ressourcen-Pools des Projekts.
   * Sie haben ihnen Budgetzeit zugewiesen.
   * Sie sind mit einer der Vorgangsrollen des Projekts verknüpft.


    

1. Klicken **Heute** , um zum heutigen Zeitrahmen zurückzukehren.
1. (Optional) Klicken Sie auf **Woche**, **Monat** oder **Quartal** , um Informationen für das Projekt in verschiedenen Zeitrahmen anzuzeigen.
1. (Optional) Klicken Sie auf die **Stunden** und wählen Sie **Stunden**,**FTE** oder **Kosten** , um zu ändern, wie Informationen im Ressourcenplaner angezeigt werden. Stunden werden standardmäßig angezeigt.

1. (Optional) Klicken Sie auf **Export** , um den Ressourcen-Planer in eine Excel-Datei zu exportieren.

   >[!NOTE]
   Sie können Daten für bis zu 12 Zeiträume gleichzeitig exportieren.

1. (Optional) Klicken Sie auf die **Vollbild** icon ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) , um den Ressourcen-Planer im Vollbildmodus anzuzeigen.

1. Aktualisieren Sie die **BDG** (Budgeting Hours) mit Stunden-, FTE- oder Kostenwerten für die Benutzer, Rollen oder das Projekt, indem Sie einen der folgenden Schritte ausführen:

   * Schätzen Sie manuell die Höhe der Stunden-, FTE- oder Kostenwerte für Rollen, Benutzer oder das Projekt.

      Oder

   * Klicken Sie auf **Optionen** für das Projekt oder die Auftrags-Rollen und wählen Sie eine Option aus, um die Stunden automatisch für Rollen, Benutzer oder das Projekt zu planen.
   Weitere Informationen zum Budgeting in der Projektansicht des Ressourcen-Planers finden Sie unter [Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Rollenansicht](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   Sie können Stunden, FTEs oder Kosten für Ihre Ressourcen für jeden beliebigen Zeitrahmen, der im Bereich Ressourcenbudgetierung angezeigt wird, unabhängig von der Zeitleiste des Projekts einplanen. Wenn Sie beispielsweise angeben möchten, dass Ihre Ressourcen während der Planung des Projekts möglicherweise nicht verfügbar sind (wo sie mit geplanten Stunden verknüpft sind), aber zu einem anderen Zeitpunkt verfügbar sein können, können Sie dies tun, indem Sie sie für Zeiträume mit null geplanten Stunden in den Haushaltsplan einbeziehen, sofern diese zur Verfügung stehen.

1. (Optional) Um zu verstehen, ob Sie die geplanten Stunden, FTEs oder Kosten in einen anderen Zeitrahmen verschieben können, klicken Sie auf die Schaltfläche **Optionen** Symbol, dann **Anpassen der Budgetierungsdaten**.

   Weitere Informationen über die Anpassung der budgetierten Datumsangaben finden Sie unter [Anpassen der Budgetierungsdaten im Ressourcenplaner](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Klicken Sie auf **Speichern**.

   Wenn Sie mit Ihren Arbeitsplatzrollen Kosten pro Stunde verbunden sind, berechnet das Budgetieren der Ressourcen im Bereich Ressourcenbudgetierung die **Geplante Arbeitskosten** des Projekts. Die budgetierten Arbeitskosten werden im Bereich Ressourcenbudgetierung des Geschäftsszenarios und in der Zusammenfassung der Geschäftsfälle angezeigt.

   >[!TIP]
   Kosten werden im Geschäftsfall in der Währung des Projekts angezeigt.

   Die im Geschäftsszenario angegebenen Budgetierungsinformationen werden auch im Ressourcen-Planer angezeigt.

   <!--drafted for Budgeted Hours: 
   <span class="preview">When you copy a project, you have the option to also copy the Budgeted Hours to the new project. Only hours budgeted in the Resource Planner are copied. For more information, see [Copy a project](../manage-projects/copy-project.md)</span>
   -->
