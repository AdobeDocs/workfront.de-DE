---
navigation-topic: business-case-and-scorecards
title: Budgetressourcen im Geschäftsfall mit dem Szenario-Planer
description: Im Rahmen der Ressourcenplanung können Sie den Adobe Workfront-Szenario-Planer verwenden, um beim Erstellen des Geschäftsszenarios die für das Abschließen der Arbeit in einem Projekt erforderlichen Vorgangsrollen zu planen.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Budgetressourcen im Geschäftsfall mit dem Szenario-Planer

Im Rahmen der Ressourcenplanung können Sie den Adobe Workfront-Szenario-Planer verwenden, um beim Erstellen des Geschäftsszenarios die für das Abschließen der Arbeit in einem Projekt erforderlichen Vorgangsrollen zu planen.

Weitere Informationen zum Erstellen eines Geschäftsfalls finden Sie unter [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Die Informationen zur Rolle &quot;Job&quot;für die mit dem Projekt verknüpfte Initiative, die Sie im Szenario-Planer auf Systemebene eingeben, sind beim Veröffentlichen der Initiative im Bereich &quot;Ressourcenbudgetierung&quot;des Projektfalls sichtbar. Der Szenario-Planer ist nur im neuen Adobe Workfront-Erlebnis verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Übersicht über den Szenario-Planer](../../../scenario-planner/scenario-planner-overview.md).

Sie können Ressourcen im Geschäftsfall auch mit dem Resource Planer einplanen. Weitere Informationen finden Sie unter folgenden Themen:

* [Haushaltsmittel im Geschäftsfall](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Es wird empfohlen, bei der Arbeit an einem Projekt zu entscheiden, ob Sie den Ressourcen-Planer oder den Szenario-Planer verwenden möchten. Ein häufiger Wechsel zwischen den beiden während der Laufzeit des Projekts kann zu Inkonsistenzen in der Art und Weise führen, wie Sie Ihre Ressourcen für das Projekt einsetzen.

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
   <td> <p>Sie müssen eine zusätzliche Lizenz für den Adobe Workfront-Szenario-Planer erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können.</p> <p>Informationen zum Abrufen des Workfront-Szenario-Players finden Sie unter <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des Szenario-Planers benötigter Zugriff</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf Folgendes: </p> 
    <ul> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Finanzielle Daten</p> </li> 
     <li> <p>Szenarienplaner </p> </li> 
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

* Erstellen Sie einen Plan mit dem Szenario-Planer.

   Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Plänen im Szenario-Planer](../../../scenario-planner/create-and-edit-plans.md).

* Erstellen Sie eine Initiative für den Plan und verknüpfen Sie sie mit einem Projekt.

   Stellen Sie sicher, dass Sie die für die Initiative erforderlichen Informationen zu den Stellenrollen angeben und das verknüpfte Projekt mit diesen Informationen aktualisieren.

   Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Erstellen und Bearbeiten von Initiativen im Szenario-Planer](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importieren von Projekten in Pläne im Szenario-Planer](../../../scenario-planner/import-projects-to-plans.md)
   * [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im Szenario-Planer](../../../scenario-planner/publish-scenarios-update-projects.md).

* Obwohl dies keine Voraussetzungen sind, empfehlen wir auch Folgendes:

   * Weisen Sie Aufgaben für das Projekt den im Szenario-Planer vorgesehenen Auftragsrollen zu.
   * Geben Sie die Anzahl der geplanten Stunden für die Aufgaben im Projekt an.

      Auf diese Weise können Sie den Arbeitsaufwand für eine Aufgabe nachvollziehen, was bei der Entscheidung hilfreich ist, für wie viel Zeit die Ressourcen für die Erfüllung der Aufgabe in den Haushalt eingestellt werden sollen.

      Informationen zum Verknüpfen von Aufgaben mit geplanten Stunden finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Budgetressourcen im Geschäftsfall unter Verwendung des Szenario-Planers für Projekte in Verbindung mit Initiativen

>[!IMPORTANT]
Sie können Ihre Ressourcen für einen Zeitraum von 15 Jahren einplanen. Wenn Sie Ressourcen für ein Projekt mit einer Dauer von mehr als 15 Jahren einsetzen, sind die Budgetierungsinformationen möglicherweise nicht korrekt.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Wechseln Sie zu dem Projekt, für das Sie Ressourcen planen möchten.

   >[!TIP]
   Dies ist ein Projekt, das mit einer Initiative im Szenario-Planer verbunden ist, deren verknüpfte Initiative mindestens einmal veröffentlicht wurde.

1. Klicken **Geschäftsfall** im linken Bereich.
1. (Bedingt) Im **Ressourcen-Budgetierung** führen Sie einen der folgenden Schritte aus:

   * Wenn Sie gerade Informationen aus dem Szenario-Planer veröffentlicht haben, wählen Sie im **Wählen Sie aus, welche Stunden für die Berechnung der budgetierten Arbeitskosten des Projekts verwendet werden sollen** im Bereich &quot;Ressourcenbudgetierung&quot;ein und klicken Sie dann auf **Auswählen**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Wenn Sie den Ressourcen-Planer bereits für die Budgetplanung für das Projekt ausgewählt haben, klicken Sie auf **Änderung** > **Szenario-Planer** > **Auswählen**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront verwendet die erforderlichen Arbeitsstunden aus der verknüpften Initiative, um die budgetierten Arbeitskosten und die geplanten Arbeitszeiten des Projekts zu berechnen. Dies ist die empfohlene Option. Kosten werden im Geschäftsfall in der Währung des Projekts angezeigt.

      Wenn Sie ein Projekt kopieren und die budgetierten Stunden in das neue Projekt kopieren, werden die mit dem Szenario-Planer geplanten Stunden nicht in das neue Projekt kopiert. Nur Stunden, die im Ressourcenplaner veranschlagt sind, werden kopiert. Weitere Informationen finden Sie unter [Projekt kopieren](../manage-projects/copy-project.md).

      >[!IMPORTANT]
      Wenn Sie mit dem Szenario-Planer Haushaltsmittel für das Projekt einsetzen, werden die budgetierten Arbeitskosten in den folgenden Bereichen von Workfront angezeigt:
      * Ressourcen-Budgeting-Bereich des Geschäftsfalles
      * Der Scenario-Planer auf Systemebene als die People-Kosten der mit dem Projekt verknüpften Initiative. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Initiativen im Szenario-Planer](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Optional) Klicken Sie auf **Im Szenario-Planer anzeigen** den Plan, der die mit dem Projekt verbundene Initiative enthält, zu öffnen. Dadurch wird der Szenario-Planer in einer neuen Browser-Registerkarte geöffnet.
1. (Optional) Aktualisieren Sie die Informationen zur Initiative. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Initiativen im Szenario-Planer](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   Sie müssen die Initiative nach jeder Änderung veröffentlichen, damit der Bereich Ressourcenbudgetierung im Projekt aktualisiert werden kann.
