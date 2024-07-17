---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen
description: Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie die Ressourcenzuordnung nebeneinander verwalten, um sicherzustellen, dass sie übereinstimmen. Dadurch wird verhindert, dass sie überverteilt oder nicht verwendet werden.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen

>[!IMPORTANT]
>
>Ihr Unternehmen muss eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] erwerben, damit Sie Informationen zur Initiative für ein Projekt anzeigen können. Informationen zum Abrufen des [!DNL Workfront Scenario Planner] finden Sie unter [Für die Verwendung des  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) benötigten Zugriffs.

Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie die Ressourcenzuordnung nebeneinander verwalten, um sicherzustellen, dass sie übereinstimmen. Dadurch wird verhindert, dass sie überverteilt oder nicht verwendet werden.

In diesem Artikel wird beschrieben, wie Sie Ressourcen mithilfe des Bereichs [!UICONTROL Rollenzuweisung] in der Aufgabenliste eines Projekts abstimmen können.

Allgemeine Informationen zur Abstimmung von Ressourcen zwischen Projekten und Initiativen, einschließlich Voraussetzungen, finden Sie unter [Überblick über die Abstimmung von Ressourcenzuweisungen zwischen Projekten und Initiativen](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Zugriffsanforderungen

Sie müssen Folgendes tun:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] oder höher</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können.</p> <p>Informationen zum Abrufen des [!DNL Workfront Scenario Planner] finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des [!DNL Scenario Planner]</a> benötigten Zugriffs. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf Projekte </p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!UICONTROL Workfront]-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!UICONTROL Workfront]-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für das Projekt</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff auf einen Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan in der [!DNL Scenario Planner]</a>.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff auf ein Projekt finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen

Wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz erworben hat, können Sie die Ressourcenzuweisungen zwischen der Initiative und dem mit ihr verknüpften Projekt im Abschnitt [!UICONTROL Aufgaben] des Projekts abstimmen.

1. (Bedingt) Verbinden Sie ein Projekt mit einer Initiative mit einer der Methoden, die unter [Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen](#Connect) dieses Artikels beschrieben sind.

   >[!IMPORTANT]
   >
   >Wenn Sie Änderungen an den Ressourcen der Initiative vornehmen, müssen Sie das Szenario, zu dem die Initiative gehört, erneut veröffentlichen, damit die neuesten Ressourceninformationen aus der Initiative über das Projekt aktualisiert werden.

1. Wechseln Sie zu dem Projekt, in dem Sie die Zuordnung von Stellenrollen für das Projekt und die damit verbundene Initiative überprüfen möchten.
1. Klicken Sie im linken Bereich auf **[!UICONTROL Aufgaben]** .
1. Klicken Sie oben rechts in der Symbolleiste auf das Symbol **[!UICONTROL Rollenzuweisung anzeigen]** ![](assets/show-role-allocation-icon.png) .

   Das Bedienfeld [!UICONTROL Rollenzuweisung] wird angezeigt.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Überprüfen Sie die folgenden Informationen im Bereich **[!UICONTROL Projektsummen]** im Bereich [!UICONTROL Rollenzuweisung] :

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
   >   * Wenn Aufgaben oder Probleme eine Dauer von null haben.
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


