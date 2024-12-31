---
navigation-topic: business-case-and-scorecards
title: Budgetressourcen im Business Case mit dem Szenario-Planer
description: Im Rahmen der Ressourcenplanung können Sie mit dem Adobe Workfront-Szenario-Planer die Aufgabengebiete budgetieren, die zum Abschließen der Arbeit in einem Projekt erforderlich sind, wenn Sie den Business Case erstellen.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 0%

---

# Budgetressourcen im Business Case mit dem Szenario-Planer

Im Rahmen der Ressourcenplanung können Sie mit dem Adobe Workfront-Szenario-Planer die Aufgabengebiete budgetieren, die zum Abschließen der Arbeit in einem Projekt erforderlich sind, wenn Sie den Business Case erstellen.

Weitere Informationen zum Erstellen eines Business-Case finden Sie unter [Erstellen eines Business-Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Die Aufgabengebiet-Informationen für die mit dem Projekt verknüpfte Initiative, die Sie im Szenario-Planer auf Systemebene eingeben, werden bei der Veröffentlichung der Initiative im Bereich Ressourcenbudgetierung des Business Cases des Projekts angezeigt. Der Szenario-Planer ist nur in der neuen Adobe Workfront-Version verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter [Szenarioplaner - Übersicht](../../../scenario-planner/scenario-planner-overview.md).

Sie können Ressourcen auch im Business Case mit dem Ressourcenplaner budgetieren. Weitere Informationen finden Sie unter:

* [Budgetressourcen im Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)
  <!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Es wird empfohlen, dass Sie bei Beginn der Arbeit an einem Projekt entscheiden, ob Sie den Ressourcen- oder den Szenario-Planer verwenden. Wenn Sie während der Laufzeit eines Projekts häufig zwischen beiden wechseln, kann dies zu Inkonsistenzen in der Budgetierung Ihrer Ressourcen für das Projekt führen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Unternehmen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für den Adobe Workfront Scenario Planner erwerben, um auf die in diesem Artikel beschriebenen Funktionen zugreifen zu können.</p> <p>Informationen zum Abrufen des Workfront-Szenarioplaners finden Sie unter <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff für die Verwendung des Szenarioplaners erforderlich</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Folgendes bearbeiten: </p> 
    <ul> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Finanzielle Daten</p> </li> 
     <li> <p>Szenarienplaner </p> </li> 
    </ul> <p>Informationen zum Zugriff auf Budgetressourcen finden Sie auch unter <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Zugriff auf Budgetressourcen in Adobe Workfront erforderlich</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Adobe Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie Folgendes tun:

* Erstellen Sie einen Plan mit dem Szenario-Planer.

  Weitere Informationen finden Sie [Erstellen und Bearbeiten von Plänen im Szenario-Planer](../../../scenario-planner/create-and-edit-plans.md).

* Erstellen einer Initiative für den Plan und Verknüpfen mit einem Projekt.

  Stellen Sie sicher, dass Sie die erforderlichen Aufgabengebiet-Informationen für die Initiative angeben und das verknüpfte Projekt mit diesen Informationen aktualisieren.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Erstellen und Bearbeiten von Initiativen im Szenario-Planer](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Projekte in Pläne im Szenario-Planer importieren](../../../scenario-planner/import-projects-to-plans.md)
   * [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen im Szenario-Planer](../../../scenario-planner/publish-scenarios-update-projects.md).

* Obwohl dies keine Voraussetzungen sind, empfehlen wir auch Folgendes:

   * Weisen Sie Aufgaben im Projekt den im Szenario-Planer budgetierten Aufgabengebieten zu.
   * Geben Sie die Anzahl der geplanten Stunden für die Aufgaben im Projekt an.

     Auf diese Weise lässt sich erkennen, wie viel Arbeit eine Aufgabe ggf. abschließen muss. Dies erleichtert die Entscheidung, für wie viel Zeit die Ressourcen budgetiert werden sollen, um die Aufgabe abzuschließen.

     Informationen zum Verknüpfen von Aufgaben mit geplanten Stunden finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Budgetressourcen im Business Case unter Verwendung des Szenario-Planers für Projekte im Zusammenhang mit Initiativen

>[!IMPORTANT]
>
>Sie können Ihre Ressourcen für einen Zeitraum von 15 Jahren budgetieren. Wenn Sie Ressourcen für ein Projekt mit einer Laufzeit von mehr als 15 Jahren budgetieren, sind die Budgetierungsinformationen möglicherweise nicht korrekt.
><!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. Wechseln Sie zu dem Projekt, für das Sie Ressourcen budgetieren möchten.

   >[!TIP]
   >
   >Dies ist ein Projekt, das mit einer Initiative im Szenarioplaner verknüpft ist, deren verknüpfte Initiative mindestens einmal veröffentlicht wurde.

1. Klicken Sie **linken Bedienfeld** Business Case“.
1. (Bedingt) Führen Sie im **Ressourcenbudgetierung** einen der folgenden Schritte aus:

   * Wenn Sie soeben Informationen aus dem Szenario-Planer veröffentlicht haben, wählen Sie im Feld **Wählen Sie die Stunden, die zur Berechnung der budgetierten Lohnkosten des Projekts verwendet werden sollen** im Bereich Ressourcenbudgetierung die Option Szenario-Planer aus und klicken Sie dann auf **Auswählen**.

     ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Wenn der Ressourcenplaner zuvor für die Budgetierung von Ressourcen für das Projekt ausgewählt wurde, klicken Sie auf **Ändern** > **Szenario-Planer** > **Wählen**.

     ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     Workfront verwendet die erforderlichen Aufgabengebietsstunden aus der verknüpften Initiative, um die budgetierten Arbeitskosten und budgetierten Stunden des Projekts zu berechnen. Dies ist die empfohlene Option. Kosten werden im Business Case in der Währung des Projekts angezeigt.

     Wenn Sie ein Projekt kopieren und die budgetierten Stunden in das neue Projekt kopieren, werden die mit dem Szenario-Planer budgetierten Stunden nicht in das neue Projekt kopiert. Nur im Ressourcenplaner budgetierte Stunden werden kopiert. Weitere Informationen finden Sie unter [Kopieren eines Projekts](../manage-projects/copy-project.md).

     >[!IMPORTANT]
     >
     >Wenn Sie mit dem Szenario-Planer Ressourcen für das Projekt budgetieren, werden die budgetierten Lohnkosten in den folgenden Bereichen von Workfront angezeigt:
     >
     >   
     >   
     >   * Bereich „Ressourcenbudgetierung“ des Business Case
     >   * Der Szenario-Planer auf Systemebene als Personalkosten der mit dem Projekt verknüpften Initiative. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Initiativen im Szenario-Planer](../../../scenario-planner/create-and-edit-initiatives.md).
     >   
     >

1. (Optional) Klicken Sie auf **Im Szenario-Planer anzeigen**, um den Plan zu öffnen, der die mit dem Projekt verknüpfte Initiative enthält. Dadurch wird der Szenario-Planer in einer neuen Browser-Registerkarte geöffnet.
1. (Optional) Aktualisieren Sie die Informationen zur Initiative. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Initiativen im Szenario-Planer](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   >
   >Sie müssen die Initiative nach jeder Änderung im Bereich Ressourcenbudgetierung des zu aktualisierenden Projekts veröffentlichen.
