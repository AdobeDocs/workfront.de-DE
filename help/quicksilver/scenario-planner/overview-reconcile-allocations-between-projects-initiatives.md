---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Übersicht über die Abstimmung der Ressourcenzuteilungen zwischen Projekten und Initiativen
description: Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 0%

---

# Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Sie können Projekte mit Initiativen verbinden, um sicherzustellen, dass Ihre strategischen Pläne und die tatsächliche Arbeit synchron sind. Wenn Sie Ihre strategischen Pläne und Initiativen in der [!DNL Scenario Planner] umreißen und die tatsächliche Arbeit in einem Projekt planen, können Sie sicherstellen, dass Ihre Ressourcen sowohl im Projekt als auch in den Initiativen übereinstimmen, sodass Sie sie weder übermäßig zuweisen noch unterschreiten.

## Voraussetzungen

Bevor Sie beginnen, benötigen Sie Folgendes:

* Ein Plan in der [!DNL Scenario Planner] mit einer Initiative, die mit einem Projekt verbunden ist.
* Erforderliche Aufgabengebiet-Zuweisungen für die Initiative.
* Aufgaben oder Probleme im Projekt, die über geplante Stunden verfügen und einem der folgenden Elemente zugewiesen sind:

   * Aufgabengebiete
   * Mit Aufgabengebieten verknüpfte Benutzer

## Projekte und Initiativen verbinden

>[!NOTE]
>
>Sie können Initiativen nur dann erstellen und sie mit Projekten verbinden, wenn Ihr Unternehmen eine zusätzliche Lizenz für die [!DNL Workfront Scenario Planner] erworben hat.

Sie können Projekte mit Initiativen verbinden, indem Sie einen der folgenden Schritte ausführen:

* Projekte als neue Initiativen in einen Plan importieren

  Weitere Informationen finden Sie unter [Projekte in Pläne importieren in der [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Initiativen in Projekten veröffentlichen

  Weitere Informationen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Beide Prozesse schaffen eine Verbindung zwischen den Projekten und den entsprechenden Initiativen. Nach dem Verbinden können Sie die Ressourcenzuteilungen verwalten, indem Sie sie vergleichen und sicherstellen, dass sie übereinstimmen.

## Überlegungen zur Abstimmung von Ressourcen für verknüpfte Projekte und Initiativen

>[!NOTE]
>
>Sie können nur dann Initiativen anzeigen, sie mit Projekten verbinden und ihre Ressourcenzuteilungen für ein Projekt anzeigen, wenn Ihr Unternehmen eine zusätzliche Lizenz für das [!DNL Workfront Scenario Planner] erworben hat.

* Sie können Benutzende, Teams und Aufgabengebiete zu Arbeitselementen in einem Projekt und Aufgabengebiete zu Initiativen zuweisen. Auf diese Weise können Sie Aufgabengebiete nur zwischen Projekten und Initiativen abstimmen.

  >[!TIP]
  >
  >Um die Zeit der Benutzenden in einem Projekt mit den Rollenzuweisungen für die Initiativen abzustimmen, müssen Sie Benutzende mit Aufgabengebieten verknüpfen.

* Sie können die Zuordnung der Aufgabengebiete für Initiativen zu einem verknüpften Projekt in den folgenden Projektbereichen anzeigen:

   * [!DNL Scenario Planner] Abschnitt des Bereichs [!UICONTROL Projektdetails] in einem Projekt. Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Verwalten von Informationen im Projektbereich [!UICONTROL Übersicht]](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >Aufgabengebiet-Informationen aus dem Projekt und der Initiative werden nicht nebeneinander im [!DNL Scenario Planner] Abschnitt der [!UICONTROL Projektdetails] angezeigt.

   * Das [!UICONTROL  &quot;]&quot; in den folgenden Bereichen:

      * [!UICONTROL Workload-] des Projekts

        Informationen zum Anzeigen und Abstimmung der Rollenzuweisungen zwischen der Initiative und dem verknüpften Projekt im [!UICONTROL Workload-Balancer] finden Sie unter [Anzeigen der Rollenzuweisung für Projekte und Initiativen im [!UICONTROL Workload-Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * Abschnitt [!UICONTROL Aufgaben]

        Informationen zur Abstimmung der Rollenzuweisungen zwischen der Initiative und dem verknüpften Projekt im Abschnitt [!UICONTROL Aufgaben] finden Sie unter [Rollenzuweisung für Projekte und Initiativen anzeigen in der Aufgabenliste](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >Sie können Aufgabenrolleninformationen aus dem Projekt und der Initiative Seite an Seite im Bedienfeld [!UICONTROL Rollenzuweisung“ ].

* Sie können keine Aufgabengebiet-Zuordnung für ein Projekt für eine verknüpfte Initiative anzeigen. Weitere Informationen finden Sie unter [Projekte in Pläne importieren in der [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
