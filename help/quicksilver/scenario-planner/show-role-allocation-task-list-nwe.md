---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen
description: Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie deren Ressourcenzuweisung nebeneinander verwalten, um sicherzustellen, dass sie übereinstimmen. Dadurch wird eine Überallokation oder Unterauslastung vermieden.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen

<!--Audited: 07/2024-->

Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie deren Ressourcenzuweisung nebeneinander verwalten, um sicherzustellen, dass sie übereinstimmen. Dadurch wird eine Überallokation oder Unterauslastung vermieden.

In diesem Artikel wird beschrieben, wie Sie Ressourcen mithilfe des Bedienfelds [!UICONTROL Rollenzuweisung] in der Aufgabenliste eines Projekts abstimmen können.

Allgemeine Informationen zur Abstimmung von Ressourcen zwischen Projekten und Initiativen, einschließlich Voraussetzungen, finden Sie [Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Plan*</p> </td> 
   <td> <ul></li>
   <li><p>Neu: Ultimate </p></li>
   <p>Der Szenario-Planer ist für die neuen Workfront Select- oder Workfront Prime-Pläne nicht verfügbar. </p>
   <li><p>Aktuell: [!UICONTROL Business] oder höher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Lizenz*</p> </td> 
   <td> <p>Neu: Licht oder höher</p> 
   <p>Aktuell: [!UICONTROL Überprüfen] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> <ul><li><p>Für die neuen Workfront-Pläne:</p><p> Adobe Workfront</li></p>
   <li><p>Für die aktuellen Workfront-Pläne: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront-Szenarioplaner</p></li></ul>

<p>Weitere Informationen finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich, um die [!DNL Scenario Planner]</a> verwenden zu können. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Zugriffsebene </td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p> Berechtigung zum Anzeigen oder Erhöhen eines Projekts.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Dokumentation zu Zugriffsanforderungen für Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen

Wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] Lizenz erworben hat, können Sie die Ressourcenzuteilungen zwischen der Initiative und dem mit ihr verknüpften Projekt im Abschnitt [!UICONTROL Aufgaben] des Projekts abstimmen.

1. (Bedingt) Ein Projekt muss mit einer Initiative verbunden sein, indem eine der Methoden verwendet wird, die im Abschnitt [Zuweisung der Rollen für Projekte und Initiativen in der Aufgabenliste anzeigen](#show-role-allocation-for-projects-and-initiatives-in-the-task-list) dieses Artikels beschrieben sind.

   >[!IMPORTANT]
   >
   >Wenn Sie Änderungen an den Ressourcen der Initiative vornehmen, müssen Sie das Szenario, zu dem die Initiative gehört, erneut veröffentlichen, damit die neuesten Ressourceninformationen der Initiative im Projekt aktualisiert werden.

1. Wechseln Sie zu dem Projekt, in dem Sie die Zuordnung der Aufgabengebiete für das Projekt sowie für die zugehörige Initiative überprüfen möchten.
1. Klicken Sie **[!UICONTROL linken]** auf „Aufgaben“.
1. Klicken Sie oben **[!UICONTROL in der Symbolleiste auf]** Symbol „Rollenzuweisung anzeigen![](assets/show-role-allocation-icon.png) .

   Das Bedienfeld [!UICONTROL Rollenzuweisung] wird angezeigt.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Überprüfen Sie die folgenden Informationen im Bereich **[!UICONTROL Projektsummen]** des Bedienfelds [!UICONTROL Rollenzuweisung]:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aufgabengebiet]</td> 
      <td> <p>Die Namen der Aufgabengebiete, die mit einem der folgenden Elemente verknüpft sind:</p> 
       <ul> 
        <li> <p>Aufgaben im Projekt</p> </li> 
        <li> <p>Probleme im Projekt</p> </li> 
        <li> <p>Dem Projekt zugeordnete Initiative</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>Die Anzahl der erforderlichen Stunden für jedes Aufgabengebiet auf der Initiative während der Gesamtdauer der Initiative. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Geplante Stunden]</td> 
      <td>Die Anzahl der geplanten Stunden, die mit jedem Aufgabengebiet in den Aufgaben oder Problemen des Projekts für die Gesamtdauer des Projekts verknüpft sind. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Varianz]</td> 
      <td> <p>Die Differenz zwischen den für die Initiative erforderlichen Stunden und den geplanten Stunden für die Arbeit am Projekt. [!DNL Workfront] berechnet die [!UICONTROL Variance] anhand der folgenden Formel:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Wenn Ressourcen für mehr Stunden als auf Initiative erforderlich eingeplant sind, ist die [!UICONTROL-Varianz] negativ und wird rot angezeigt. Das bedeutet, dass Ihre Ressourcen überlastet sind. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Die geplanten Stunden aus dem Projekt werden in den folgenden Szenarien nicht angezeigt:
   >
   >   
   >   
   >   * Wenn Aufgaben oder Probleme keinen Aufgabengebieten bzw. Benutzern mit einem ihnen zugeordneten Aufgabengebiet zugewiesen werden.
   >   * Wenn Aufgaben oder Probleme eine Dauer von null haben.
   >   
   >



1. (Optional) Wenn die Spalte [!UICONTROL Varianz] anzeigt, dass Ihre Ressourcen überlastet sind, passen Sie einen der folgenden Schritte an:

   * Reduzieren Sie die Anzahl der geplanten Stunden für ein Aufgabengebiet, das überlastet ist, oder fügen Sie den Aufgaben weitere Ressourcen hinzu und verteilen Sie mehr geplante Stunden auf die neuen Ressourcen. Sie können bei Aufgaben oder Problemen Zuweisungen oder die Anzahl der geplanten Stunden aktualisieren, wenn Sie sie bearbeiten. Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Aufgaben bearbeiten](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Probleme bearbeiten](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Sie müssen über zusätzliche Zugriffsrechte und Berechtigungen verfügen, um Aufgaben und Probleme zu bearbeiten.

   * Erhöhen Sie die Anzahl der erforderlichen Stunden für die Rolle, die die Überallokation für die Initiative anzeigt. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Sie müssen über zusätzliche Zugriffsrechte und Berechtigungen verfügen, um Pläne zu bearbeiten.


