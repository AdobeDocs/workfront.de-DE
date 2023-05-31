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
>Ihr Unternehmen muss eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , damit Sie Initiativinformationen zu einem Projekt anzeigen können. Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe [Für die Verwendung des Szenario-Planers benötigter Zugriff](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

Sie können Projekte mit Initiativen verbinden, um sicherzustellen, dass Ihre strategischen Pläne und die tatsächlichen Arbeiten synchron sind. Wenn Sie Ihre strategischen Pläne und Initiativen im Abschnitt [!DNL Scenario Planner] und Sie die tatsächliche Arbeit in einem Projekt planen, können Sie sicherstellen, dass Ihre Ressourcen für das Projekt und die Initiativen übereinstimmen, sodass Sie sie weder überzuordnen noch zu wenig nutzen.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie über Folgendes verfügen:

* Ein Plan im [!DNL Scenario Planner] mit einer Initiative im Zusammenhang mit einem Projekt.
* Erforderliche Stellenzuweisungen für die Initiative.
* Aufgaben oder Probleme im Projekt, für die Stunden geplant sind und die einer der folgenden Aufgaben zugewiesen sind:

   * Aufgabengebiete
   * Benutzer, die mit Auftragsrollen verknüpft sind

## Projekte und Initiativen verbinden

>[!NOTE]
>
>Initiativen können nur dann erstellt und mit Projekten verbunden werden, wenn Ihr Unternehmen eine zusätzliche Lizenz für die [!DNL Workfront Scenario Planner].

Sie können Projekte mit Initiativen verbinden, indem Sie einen der folgenden Schritte ausführen:

* Importieren von Projekten in einen Plan als neue Initiativen

   Weitere Informationen finden Sie unter [Importieren von Projekten in Pläne in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Veröffentlichen von Initiativen in Projekten

   Weitere Informationen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

Beide Prozesse stellen eine Verbindung zwischen den Projekten und den entsprechenden Initiativen her. Nachdem Sie sie verbunden haben, können Sie ihre Ressourcenzuweisungen verwalten, indem Sie sie vergleichen und sicherstellen, dass sie übereinstimmen.

## Überlegungen zur Abstimmung von Ressourcen auf verknüpfte Projekte und Initiativen

>[!NOTE]
>
>Sie können nur dann Initiativen anzeigen, sie mit Projekten verbinden und ihre Ressourcenzuweisungen in einem Projekt anzeigen, wenn Ihr Unternehmen eine zusätzliche Lizenz für die [!DNL Workfront Scenario Planner].

* Sie können Arbeitselementen an einem Projekt Benutzer-, Teams- und Stellenrollen zuweisen und Initiativen Jobrollen zuweisen. Daher können Sie nur die Rollen von Projekten und Initiativen miteinander in Einklang bringen.

   >[!TIP]
   >
   >Um die Zeit der Benutzer für ein Projekt mit Rollenzuweisungen für die Initiativen abzustimmen, müssen Sie Benutzer mit den Rollen &quot;Job&quot;verknüpfen.

* Sie können die Zuweisung von Initiativaufgaben zu einem verknüpften Projekt in den folgenden Bereichen des Projekts anzeigen:

   * [!DNL Scenario Planner] Abschnitt [!UICONTROL Projektdetails] -Bereich eines Projekts. Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [Verwalten von Informationen im Projekt [!UICONTROL Übersicht] area](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >Sie können keine Informationen über die Rolle des Arbeitsplatzes aus dem Projekt und der Initiative nebeneinander im [!DNL Scenario Planner] Abschnitt [!UICONTROL Projektdetails].

   * Die [!UICONTROL Rollenzuweisung] in den folgenden Bereichen:

      * [!UICONTROL Lastenausgleich] des Projekts

         Informationen dazu, wie Sie die Rollenverteilung zwischen der Initiative und dem verknüpften Projekt im [!UICONTROL Lastenausgleich], siehe [Rollenzuweisung für Projekte und Initiativen im [!UICONTROL Lastenausgleich]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL Aufgaben] Abschnitt

         Informationen darüber, wie die Rollenverteilung zwischen der Initiative und dem verknüpften Projekt in der [!UICONTROL Aufgaben] Abschnitt, siehe [Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >Sie können Informationen zu den Aufgaben vom Projekt und der Initiative nebeneinander in [!UICONTROL Rollenzuweisung] Bereich.



* Sie können die Zuordnung von Aufgaben für ein Projekt nicht auf einer verknüpften Initiative anzeigen. Weitere Informationen finden Sie unter [Importieren von Projekten in Pläne in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
