---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Rollenzuweisung für Projekte und Initiativen im Arbeitslastausgleich anzeigen
description: Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie die Ressourcenzuordnung nebeneinander verwalten, um sicherzustellen, dass sie
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 1%

---

# Rollenzuweisung für Projekte und Initiativen im [!UICONTROL Arbeitslastausgleich] anzeigen

<!--Audited: 07/2024-->

Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie die Ressourcenzuordnung nebeneinander verwalten, um sicherzustellen, dass sie übereinstimmen. Dadurch wird verhindert, dass sie überverteilt oder nicht verwendet werden.

In diesem Artikel wird beschrieben, wie Sie Ressourcen mithilfe des Bedienfelds [!UICONTROL Rollenzuweisung] in [!UICONTROL Arbeitslast-Ausgleich] eines Projekts abstimmen können.

Allgemeine Informationen zur Abstimmung von Ressourcen zwischen Projekten und Initiativen, einschließlich Voraussetzungen, finden Sie unter [Überblick über die Abstimmung von Ressourcenzuweisungen zwischen Projekten und Initiativen](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Neu: Ultimate </p></li>
   <p>Der Szenario-Planer ist für den neuen Workfront Select- oder Workfront-Plan nicht verfügbar. </p>
   <li><p>Aktuell: [!UICONTROL Business] oder höher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>Neu: Licht oder höher</p> 
   <p>Aktuell: [!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> <ul><li><p>Für die neuen Workfront-Pläne:</p><p> Adobe Workfront</li></p>
   <li><p>Für die aktuellen Workfront-Pläne: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront-Szenario-Planer</p></li></ul>

<p>Weitere Informationen finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des [!DNL Scenario Planner]</a> erforderlichen Zugriff. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Zugriffsebene </td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p> Anzeigen oder höherer Berechtigungen für ein Projekt.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen für die Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rollenzuweisung für Projekte und Initiativen im [!UICONTROL Arbeitslastausgleich] anzeigen

Wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat, können Sie die Ressourcenzuweisungen zwischen der Initiative und dem mit ihr verknüpften Projekt auf Projektebene abstimmen [!UICONTROL Lastenausgleich].

1. (Bedingt) Verbinden Sie ein Projekt mit einer Initiative mit einer der in den folgenden Artikeln beschriebenen Methoden:

   * [Importieren Sie Projekte in Pläne in den  [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Aktualisieren oder erstellen Sie Projekte durch Veröffentlichen von Initiativen im  [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Wenn Sie Änderungen an den Ressourcen der Initiative vornehmen, müssen Sie das Szenario, zu dem die Initiative gehört, erneut veröffentlichen, damit die neuesten Ressourceninformationen aus der Initiative über das Projekt aktualisiert werden.

1. Wechseln Sie zu dem Projekt, in dem Sie die Zuordnung von Stellenrollen für das Projekt und die damit verbundene Initiative überprüfen möchten.
1. Klicken Sie im linken Bereich auf [!UICONTROL Lastenausgleich] .

   Möglicherweise müssen Sie auf **[!UICONTROL Planung]** und dann auf **[!UICONTROL Auf den Lastenausgleich wechseln]** klicken.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Monat]** , um den Lastenausgleich nach Monat anzuzeigen, klicken Sie auf das Dropdown-Menü neben einem Monat in der Timeline ![](assets/drop-down-next-to-month-month-view-wb.png) und dann auf **[!UICONTROL Mehr]**.
   * Klicken Sie oben rechts in der Symbolleiste auf das Symbol **[!UICONTROL Rollenzuweisung anzeigen]** ![](assets/show-role-allocation-icon.png) .

   Das Bedienfeld [!UICONTROL Rollenzuweisung] wird angezeigt.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Sie können zwar das Bedienfeld [!UICONTROL Rollenzuweisung] anzeigen, selbst wenn Ihr Unternehmen keine [!DNL Workfront Scenario Planner] -Lizenz erworben hat, können jedoch keine Informationen zu den Jobrollen von Initiativen angezeigt werden.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Überprüfen Sie die folgenden Informationen im Bereich **[!UICONTROL Projektsummen]** im Bereich &quot;Rollenzuweisung&quot;:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Auftragsrolle]</td> 
      <td> <p>Die Namen der Auftragsrollen, die mit einem der folgenden Elemente verknüpft sind:</p> 
       <ul> 
        <li> <p>Aufgaben im Projekt</p> </li> 
        <li> <p>Projektprobleme</p> </li> 
        <li> <p>mit dem Projekt in Zusammenhang stehende Initiative</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>Die Anzahl der erforderlichen Stunden, die mit jeder Rolle in der Initiative für die gesamte Dauer der Initiative verbunden sind. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Geplante Stunden]</td> 
      <td>Die Anzahl der geplanten Stunden, die mit jeder Rolle im Auftrag verknüpft sind, während der Gesamtdauer des Projekts in den Aufgaben oder Problemen im Projekt. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Abweichung]</td> 
      <td> <p>Differenz zwischen den für die Initiative erforderlichen Stunden und den geplanten Arbeitszeiten für die Arbeit am Projekt. [!DNL Workfront] berechnet die [!UICONTROL Varianz] anhand dieser Formel:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Wenn Ressourcen für mehr Stunden geplant sind als für die Initiative erforderlich, ist die [!UICONTROL Varianz] negativ und wird rot angezeigt. Das bedeutet, dass Ihre Ressourcen überzugewiesen werden. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Geplante Stunden aus dem Projekt werden in den folgenden Szenarien nicht angezeigt:
   >
   >   
   >   
   >   * Wenn Aufgaben oder Probleme nicht Auftragsrollen oder Benutzern mit einer ihnen zugeordneten Auftragsrolle zugewiesen sind.
   >   * Wenn Aufgaben oder Probleme eine [!UICONTROL Dauer] von null haben.
   >   
   >

1. (Optional) Wenn die Spalte [!UICONTROL Varianz] anzeigt, dass Ihre Ressourcen überverteilt sind, passen Sie eine der folgenden Aktionen an:

   * Reduzieren Sie die Anzahl der geplanten Stunden für eine Auftragsrolle, die überzugeordnet ist, oder fügen Sie mehr Ressourcen zu den Aufgaben hinzu und verteilen Sie mehr geplante Stunden an die neuen Ressourcen. Sie können Zuweisungen oder die Anzahl der geplanten Stunden für Aufgaben oder Probleme bei der Bearbeitung aktualisieren. Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Aufgaben bearbeiten](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Probleme bearbeiten](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Sie benötigen zusätzlichen Zugriff und Berechtigungen, um Aufgaben und Probleme bearbeiten zu können.

   * Erhöhen Sie die Anzahl der erforderlichen Stunden für die Rolle, die die Überzuweisung auf die Initiative anzeigt. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Initiativen in der [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Sie benötigen zusätzlichen Zugriff und Berechtigungen, um Pläne bearbeiten zu können.

1. (Optional) Klicken Sie auf das Dropdown-Symbol, um einen der Monate im Bedienfeld [!UICONTROL Rollenzuweisung] oder in der Timeline des [!UICONTROL Lastenausgleichs] zu erweitern.

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Für jeden Monat wird derselbe Informationstyp angezeigt, der im Bereich [!UICONTROL Gesamtsumme des Projekts] angezeigt wird.

   >[!TIP]
   >
   >Die im Bedienfeld [!UICONTROL Rollenzuweisung] aufgelisteten Monate sind die Monate in der Timeline, die auf dem Bildschirm im [!UICONTROL Arbeitsladeausgleich] angezeigt werden. Scrollen Sie auf der Timeline zurück und weiter, um weitere Monate anzuzeigen.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


