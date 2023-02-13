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
>Ihr Unternehmen muss eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , damit Sie Initiativinformationen zu einem Projekt anzeigen können. Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe [Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie die Ressourcenzuordnung nebeneinander verwalten, um sicherzustellen, dass sie übereinstimmen. Dadurch wird verhindert, dass sie überverteilt oder nicht verwendet werden.

In diesem Artikel wird beschrieben, wie Sie Ressourcen mithilfe des [!UICONTROL Rollenzuweisung] in der Aufgabenliste eines Projekts.

Allgemeine Informationen zur Abstimmung von Ressourcen zwischen Projekten und Initiativen, einschließlich Voraussetzungen, finden Sie unter [Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Zugriffsanforderungen

Sie müssen Folgendes tun:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> Plan*</b> </p> </td> 
   <td>[!UICONTROL Business] oder höher</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen.</p> <p>Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf Projekte </p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!UICONTROL Workfront]-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!UICONTROL Workfront]-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für das Projekt</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff auf ein Projekt finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen

Wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz verwenden, können Sie die Ressourcenzuweisungen zwischen der Initiative und dem ihr zugeordneten Projekt in der [!UICONTROL Aufgaben] des Projekts.

1. (Bedingt) Verbinden Sie ein Projekt mit einer Initiative, indem Sie eine der im Abschnitt [Rollenzuweisung für Projekte und Initiativen in der Aufgabenliste anzeigen](#Connect) dieses Artikels.

   >[!IMPORTANT]
   >
   >Wenn Sie Änderungen an den Ressourcen der Initiative vornehmen, müssen Sie das Szenario, zu dem die Initiative gehört, erneut veröffentlichen, damit die neuesten Ressourceninformationen aus der Initiative über das Projekt aktualisiert werden.

1. Wechseln Sie zu dem Projekt, in dem Sie die Zuordnung von Stellenrollen für das Projekt und die damit verbundene Initiative überprüfen möchten.
1. Klicken **[!UICONTROL Aufgaben]** im linken Bereich.
1. Klicken Sie auf **[!UICONTROL Rollenzuweisung anzeigen]** icon ![](assets/show-role-allocation-icon.png) in der oberen rechten Ecke der Symbolleiste.

   Die [!UICONTROL Rollenzuweisung] angezeigt.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Überprüfen Sie die folgenden Informationen in der **[!UICONTROL Gesamtprojektsummen]** der [!UICONTROL Rollenzuweisung] Bereich:

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
      <td> <p>Differenz zwischen den für die Initiative erforderlichen Stunden und den geplanten Arbeitszeiten für die Arbeit am Projekt. [!DNL Workfront] berechnet die [!UICONTROL Variante] anhand dieser Formel:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>Wenn Ressourcen für mehr Stunden geplant sind als für die Initiative erforderlich, ist die [!UICONTROL Varianz] negativ und wird rot angezeigt. Das bedeutet, dass Ihre Ressourcen überzugewiesen werden. </p> </td> 
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




1. (Optional) Wenn die Variable [!UICONTROL Abweichung] -Spalte zeigt an, dass Ihre Ressourcen überverteilt sind, passen Sie eine der folgenden Aktionen an:

   * Reduzieren Sie die Anzahl der geplanten Stunden für eine Auftragsrolle, die überzugeordnet ist, oder fügen Sie mehr Ressourcen zu den Aufgaben hinzu und verteilen Sie mehr geplante Stunden an die neuen Ressourcen. Sie können Zuweisungen oder die Anzahl der geplanten Stunden für Aufgaben oder Probleme bei der Bearbeitung aktualisieren. Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Aufgaben bearbeiten](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Probleme bearbeiten](../manage-work/issues/manage-issues/edit-issues.md)

      >[!NOTE]
      >
      >Sie benötigen zusätzlichen Zugriff und Berechtigungen, um Aufgaben und Probleme bearbeiten zu können.

   * Erhöhen Sie die Anzahl der erforderlichen Stunden für die Rolle, die die Überzuweisung auf die Initiative anzeigt. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

      >[!NOTE]
      >
      >Sie benötigen zusätzlichen Zugriff und Berechtigungen, um Pläne bearbeiten zu können.



