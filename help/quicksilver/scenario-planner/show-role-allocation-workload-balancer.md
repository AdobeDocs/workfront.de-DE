---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Rollenzuweisung für Projekte und Initiativen im Arbeitslastausgleich anzeigen
description: Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie die Ressourcenzuordnung nebeneinander verwalten, um sicherzustellen, dass sie
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# Rollenzuweisung für Projekte und Initiativen im [!DNL Workload Balancer]

>[!IMPORTANT]
>
>Ihr Unternehmen muss eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , damit Sie Initiativinformationen zu einem Projekt anzeigen können. Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe [Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Nachdem Sie Projekte und Initiativen miteinander verbunden haben, können Sie die Ressourcenzuordnung nebeneinander verwalten, um sicherzustellen, dass sie übereinstimmen. Dadurch wird verhindert, dass sie überverteilt oder nicht verwendet werden.

In diesem Artikel wird beschrieben, wie Sie Ressourcen mithilfe des [!UICONTROL Rollenzuweisung] Bedienfeld in [!UICONTROL Lastenausgleich] eines Projekts.

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
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen.</p> <p>Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe <a href="../scenario-planner/access-needed-to-use-sp.md">Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf Projekte </p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für das Projekt</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Anforderung] des Zugriffs auf einen Plan im [!DNL Workfront Scenario Planner]</a>.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff auf ein Projekt finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Rollenzuweisung für Projekte und Initiativen im [!DNL Workload Balancer]

Wenn Ihr Unternehmen eine [!DNL Workfront Scenario Planner] -Lizenz können Sie die Ressourcenzuweisungen zwischen der Initiative und dem ihr zugeordneten Projekt auf Projektebene abstimmen. [!DNL Workload Balancer].

1. (Bedingt) Verbinden Sie ein Projekt mit einer Initiative mit einer der in den folgenden Artikeln beschriebenen Methoden:

   * [Importieren von Projekten in Pläne in [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Wenn Sie Änderungen an den Ressourcen der Initiative vornehmen, müssen Sie das Szenario, zu dem die Initiative gehört, erneut veröffentlichen, damit die neuesten Ressourceninformationen aus der Initiative über das Projekt aktualisiert werden.

1. Wechseln Sie zu dem Projekt, in dem Sie die Zuordnung von Stellenrollen für das Projekt und die damit verbundene Initiative überprüfen möchten.
1. Klicken [!DNL Workload Balancer] im linken Bereich.

   Möglicherweise müssen Sie auf **[!UICONTROL Planung]**, dann **[!UICONTROL Wechseln zum Lastenausgleich]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken **[!UICONTROL Monat]** Um den Lastenausgleich nach Monat anzuzeigen, klicken Sie auf das Dropdown-Menü neben einem Monat in der Timeline ![](assets/drop-down-next-to-month-month-view-wb.png)Klicken Sie auf **[!UICONTROL Mehr]**.
   * Klicken Sie auf **[!UICONTROL Rollenzuweisung anzeigen]** icon ![](assets/show-role-allocation-icon.png) in der oberen rechten Ecke der Symbolleiste.

   Die [!UICONTROL Rollenzuweisung] angezeigt.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Auch wenn die [!UICONTROL Rollenzuweisung] auch dann, wenn Ihr Unternehmen keine [!DNL Workfront Scenario Planner] -Lizenz können Sie keine Informationen zu den Stellenrollen von Initiativen anzeigen.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Überprüfen Sie die folgenden Informationen in der **[!UICONTROL Gesamtprojektsummen]** Bereich des Bereichs &quot;Rollenzuweisung&quot;:

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
   >   * Wenn Aufgaben oder Probleme [!UICONTROL Dauer] von null.




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


1. (Optional) Klicken Sie auf das Dropdownsymbol, um einen der Monate im [!UICONTROL Rollenzuweisung] oder in der Timeline des [!UICONTROL Lastenausgleich].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Derselbe Informationstyp wird in der [!UICONTROL Gesamtprojektsummen] wird auch für jeden Monat angezeigt.

   >[!TIP]
   >
   >Die in der [!UICONTROL Rollenzuweisung] -Bedienfeld die Monate in der Timeline, die auf dem Bildschirm im [!UICONTROL Lastenausgleich]. Scrollen Sie auf der Timeline zurück und weiter, um weitere Monate anzuzeigen.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


