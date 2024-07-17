---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen
description: Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen

>[!IMPORTANT]
>
>Ihr Unternehmen muss eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] erwerben, damit Sie Informationen zur Initiative für ein Projekt anzeigen können. Informationen zum Abrufen des [!DNL Workfront Scenario Planner] finden Sie unter [Für die Verwendung des Szenario-Planers benötigter Zugriff](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Sie können Projekte mit Initiativen verbinden, um sicherzustellen, dass Ihre strategischen Pläne und die tatsächlichen Arbeiten synchron sind. Wenn Sie Ihre strategischen Pläne und Initiativen in der [!DNL Scenario Planner] skizzieren und die tatsächliche Arbeit in einem Projekt planen, können Sie sicherstellen, dass Ihre Ressourcen für das Projekt und die Initiativen übereinstimmen, sodass Sie sie weder überzuordnen noch zu wenig nutzen.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie über Folgendes verfügen:

* Ein Plan im [!DNL Scenario Planner] mit einer Initiative, die mit einem Projekt verbunden ist.
* Erforderliche Stellenzuweisungen für die Initiative.
* Aufgaben oder Probleme im Projekt, für die Stunden geplant sind und die einer der folgenden Aufgaben zugewiesen sind:

   * Aufgabengebiete
   * Benutzer, die mit Auftragsrollen verknüpft sind

## Projekte und Initiativen verbinden

>[!NOTE]
>
>Sie können nur dann Initiativen erstellen und diese mit Projekten verknüpfen, wenn Ihr Unternehmen eine zusätzliche Lizenz für die [!DNL Workfront Scenario Planner] erworben hat.

Sie können Projekte mit Initiativen verbinden, indem Sie einen der folgenden Schritte ausführen:

* Importieren von Projekten in einen Plan als neue Initiativen

  Weitere Informationen finden Sie unter [Importieren von Projekten in Pläne in der  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Publish-Initiativen für Projekte

  Weitere Informationen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Beide Prozesse stellen eine Verbindung zwischen den Projekten und den entsprechenden Initiativen her. Nachdem Sie sie verbunden haben, können Sie ihre Ressourcenzuweisungen verwalten, indem Sie sie vergleichen und sicherstellen, dass sie übereinstimmen.

## Überlegungen zur Abstimmung von Ressourcen auf verknüpfte Projekte und Initiativen

>[!NOTE]
>
>Sie können nur dann Initiativen anzeigen, sie mit Projekten verknüpfen und ihre Ressourcenzuweisungen in einem Projekt anzeigen, wenn Ihr Unternehmen eine zusätzliche Lizenz für [!DNL Workfront Scenario Planner] erworben hat.

* Sie können Arbeitselementen an einem Projekt Benutzer-, Teams- und Stellenrollen zuweisen und Initiativen Jobrollen zuweisen. Daher können Sie nur die Rollen von Projekten und Initiativen miteinander in Einklang bringen.

  >[!TIP]
  >
  >Um die Zeit der Benutzer für ein Projekt mit Rollenzuweisungen für die Initiativen abzustimmen, müssen Sie Benutzer mit den Rollen &quot;Job&quot;verknüpfen.

* Sie können die Zuweisung von Initiativaufgaben zu einem verknüpften Projekt in den folgenden Bereichen des Projekts anzeigen:

   * [!DNL Scenario Planner] des Bereichs [!UICONTROL Projektdetails] in einem Projekt. Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Verwalten von Informationen im Bereich &quot;Projekt&quot;[!UICONTROL Überblick]](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >Sie können keine Informationen zu den Aufgaben aus dem Projekt und der Initiative im Abschnitt [!DNL Scenario Planner] der [!UICONTROL Projektdetails] nebeneinander sehen.

   * Das Bedienfeld [!UICONTROL Rollenzuweisung] in den folgenden Bereichen:

      * [!UICONTROL Lastenausgleich] des Projekts

        Informationen zum Anzeigen und Abstimmen der Rollenzuweisungen zwischen der Initiative und dem verknüpften Projekt im [!UICONTROL Lastenausgleich] finden Sie unter [Rollenzuweisung für Projekte und Initiativen im [!UICONTROL Arbeitslastausgleich anzeigen]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * Abschnitt [!UICONTROL Aufgaben]

        Informationen dazu, wie Sie die Rollenzuweisungen zwischen der Initiative und dem verknüpften Projekt im Abschnitt [!UICONTROL Aufgaben] abstimmen, finden Sie unter [Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen](../scenario-planner/show-role-allocation-task-list-nwe.md).

     >[!TIP]
     >
     >Sie können Informationen zu Aufgabenrollen aus dem Projekt und der Initiative nebeneinander im Bedienfeld [!UICONTROL Rollenzuweisung] anzeigen.

* Sie können die Zuordnung von Aufgaben für ein Projekt nicht auf einer verknüpften Initiative anzeigen. Weitere Informationen finden Sie unter [Importieren von Projekten in Pläne in der  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
