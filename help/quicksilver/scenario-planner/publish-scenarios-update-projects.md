---
product-area: enterprise-scenario-planner-product-area
keywords: publish,plans,projects,scenario,scenarios
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im Szenario-Planer
description: Sie können Projekte aus bereits bestehenden Initiativen erstellen und Projekte aktualisieren, die zuvor mit Initiativen verknüpft waren, indem Sie Szenarien im Adobe Workfront-Szenario-Planer veröffentlichen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: 9babe17ad862925440e555f881bf753fb443b67d
workflow-type: tm+mt
source-wordcount: '1722'
ht-degree: 0%

---

# Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]

Veröffentlichen eines Szenarios über [!DNL Adobe Workfront Scenario Planner] führt Folgendes aus:

* Erstellt Projekte aus den Initiativen für das Szenario und verknüpft sie miteinander.
* Aktualisiert bereits mit Initiativen im Zusammenhang stehende Projekte mit Informationen aus der verknüpften Initiative. Projekte können auch mit Initiativen verknüpft werden, wenn Sie sie in einen Plan importieren. Weitere Informationen finden Sie unter [Importieren von Projekten in Pläne in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td>[!UICONTROL Business] oder höher</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt </td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen.</p> <p>Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>Zugriffsstufe*</p> </td> 
   <td> 
    <ul> 
    <li>Zugriff auf [!UICONTROL bearbeiten] für [!DNL Scenario Planner] und Projekte</li></ul>

<p><b>NOTIZ</b>

Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen</p> </td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Verwalten] Berechtigungen für den Plan </li> 
     <li>[!UICONTROL Berechtigungen für veröffentlichte Projekte verwalten</li> 
    </ul> <p>Weitere Informationen zur Anforderung eines zusätzlichen Zugangs zu Projekten finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Weitere Informationen zum Zugriff auf die [!DNL Workfront Scenario Planner], siehe [Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

## Voraussetzungen

Bevor Sie beginnen:

* Sie müssen einen Plan erstellen und speichern, bevor Sie damit Initiativen veröffentlichen können.
* Die Einstellung Benutzern erlauben, Projekte ohne Verwendung einer Vorlageneinstellung zu erstellen, muss im Bereich &quot;Projektvoreinstellungen&quot;der Einrichtung aktiviert sein. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Überlegungen zur Veröffentlichung von Initiativen für Projekte

* Sie können nur ein Szenario aus einem Plan veröffentlichen.
* Eine Initiative kann nur mit einem Projekt verknüpft werden.
* Ein Projekt kann mit mehr als einer Initiative verknüpft werden, wenn die Initiativen zu unterschiedlichen Plänen gehören.

  >[!TIP]
  >
  >Wenn ein Projekt in mehreren Plänen vorhanden ist und Sie Informationen aus allen Plänen in das Projekt veröffentlichen, überschreibt die neueste Veröffentlichung die vorhandenen [!DNL Scenario Planner] Informationen zum Projekt.

* Wurden Initiativen für den Plan durch Importieren von Projekten in den Plan geschaffen, werden bei der Veröffentlichung der Initiative auch die verknüpften Projekte mit Initiativinformationen aktualisiert.

  >[!TIP]
  >
  >Sie können dasselbe Projekt in mehrere Pläne importieren. Durch die Veröffentlichung werden möglicherweise Initiativinformationen zu einem Projekt überschrieben, das mit mehreren Initiativen verknüpft ist.

  Informationen zum Erstellen von Initiativen durch Importieren von Projekten finden Sie unter [Importieren von Projekten in Pläne in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Änderungen am Projekt werden nicht auf die verknüpfte Initiative übertragen.



## Initiativen veröffentlichen

>[!IMPORTANT]
>
>Wenn Sie Änderungen an den Initiativen im Plan vornehmen, einschließlich der Lösung von Konflikten, müssen Sie die Initiative erneut veröffentlichen, damit die neuen Informationen im Projekt sichtbar sind. Diese Informationen werden nur bei der Veröffentlichung der entsprechenden Initiative zu den mit Initiativen verbundenen Projekten angezeigt. Informationen zur Lösung von Konflikten zwischen Initiativen finden Sie unter [Beheben von Initiativkonflikten im [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **[!UICONTROL Szenarien]**
1. (Optional und bedingt) Wenn Sie aus einem vorhandenen Plan veröffentlichen möchten, klicken Sie auf die **[!UICONTROL Filter]** icon ![](assets/filter-nwepng.png) in der oberen rechten Ecke des Plans eine der folgenden Optionen auswählen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Zeigt alle Pläne an, deren Inhaber Sie sind oder die für Sie freigegeben wurden. Dies ist die Standardeinstellung. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Meine Pläne]</td> 
      <td>Zeigt die von Ihnen erstellten Pläne an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Für mich freigegeben]</td> 
      <td> <p>Zeigt Pläne an, die Sie nicht erstellt, aber für Sie freigegeben haben.</p> <p>Wichtig: Sie müssen über [!UICONTROL Manager]-Berechtigungen verfügen, um für Sie freigegebene Pläne veröffentlichen zu können. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Optional) Klicken Sie auf die **[!UICONTROL Suche]** icon ![](assets/search-icon.png) und beginnen Sie mit der Eingabe des Namens eines Plans, um ihn schnell in der Liste zu finden.
1. (Bedingt) Um aus einem neuen Plan zu veröffentlichen, erstellen Sie einen Plan.

   Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. (Optional) Klicken Sie auf den Namen eines bestehenden Plans und erstellen Sie neue Szenarien für den Plan.

   Informationen zum Erstellen von Szenarien für einen Plan finden Sie unter [Erstellen und Vergleichen von Planszenarien in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Optional) Aktualisieren Sie die Initiativen eines bestehenden oder neuen Plans oder erstellen Sie neue.

   Informationen zum Erstellen von Initiativen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Klicks **[!UICONTROL Plan speichern]**.
1. Wählen Sie das Szenario, das Sie veröffentlichen möchten, aus dem **[!UICONTROL Ursprüngliches Szenario]** Dropdown-Menü, und klicken Sie auf **[!UICONTROL Zu Veröffentlichen wechseln]** ![](assets/go-to-publish-button-icon.png) in der oberen rechten Ecke.

   Oder

   Klicks **[!UICONTROL Szenarien vergleichen]**, bewegen Sie den Mauszeiger über die Szenariokarte, von der Sie die Veröffentlichung vornehmen möchten, und klicken Sie auf **[!UICONTROL Zu Veröffentlichen wechseln]** ![](assets/go-to-publish-button-icon.png).

   Die [!UICONTROL Initiativen veröffentlichen] angezeigt, auf der eine Liste aller Initiativen im Szenario angezeigt wird. Wenn eine der Initiativen zuvor veröffentlicht wurde, wird das Projektsymbol ![](assets/project-icon-sp.png) nach ihrem Namen angezeigt und **[!UICONTROL Zuletzt veröffentlicht]** Datum wird in der Liste ausgefüllt.

   >[!TIP]
   >
   >Auf Initiativen, die durch den Import von Projekten erstellt wurden, wird auch das Projektsymbol angezeigt ![](assets/project-icon-sp.png) rechts von ihrem Namen

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Optional und bedingt) Wenn Sie aus einem vorhandenen Plan veröffentlichen möchten, klicken Sie auf die **[!UICONTROL Filter]** icon ![](assets/filter-nwepng.png) in der oberen rechten Ecke des Plans eine der folgenden Optionen auswählen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Zeigt alle Initiativen des ausgewählten Szenarios an. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Publiziert]</td> 
      <td>Zeigt Initiativen an, die Sie oder ein anderer Benutzer zuvor veröffentlicht haben. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Veröffentlichung rückgängig gemacht]</td> 
      <td> <p>Zeigt nicht veröffentlichte Initiativen an. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Optional) Klicken Sie auf die **[!UICONTROL Suche]** icon ![](assets/search-icon.png) und beginnen Sie mit der Eingabe des Namens einer Initiative, um sie schnell in der Liste zu finden.
1. Wählen Sie eine oder mehrere Initiativen aus, um Projekte zu veröffentlichen und zu erstellen oder zu aktualisieren, und klicken Sie dann auf **[!UICONTROL Initiativen veröffentlichen]**.

   Dadurch wird aus jeder ausgewählten Initiative ein neues Projekt erstellt oder die vorhandenen verbundenen Projekte werden aktualisiert, wenn die veröffentlichten Initiativen bereits mit einem Projekt verknüpft waren.

   >[!TIP]
   >
   >Neue Projekte haben den gleichen Namen wie die veröffentlichten Initiativen.

1. (Bedingt) Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie eine Initiative veröffentlicht haben, klicken Sie auf **[!UICONTROL Siehe Verknüpftes Projekt]** , um das von der Initiative erstellte oder aktualisierte Projekt zu öffnen.
   * Wenn Sie mehrere Initiativen veröffentlicht haben, klicken Sie auf **[!UICONTROL Siehe Verknüpfte Projekte .]** um eine Liste der im Rahmen von Initiativen veröffentlichten Projekte zu öffnen. [!DNL Workfront] wendet die [!DNL Scenario Planner] Projekte werden standardmäßig nach der Projektliste gefiltert. Die zuletzt veröffentlichten Projekte werden oben in der Liste angezeigt.

     ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Gehen Sie zu den folgenden Bereichen, um Informationen über die Initiative zum Projekt zu erhalten:

   * **Die [!UICONTROL Updates] Abschnitt**: Eine Aktualisierung wird veröffentlicht, um anzugeben, dass das Projekt von der Initiative erstellt oder aktualisiert wurde. Die Aktualisierung enthält den Namen der Initiative, die das Projekt erstellt oder aktualisiert hat, und den verknüpften Namen des Plans, der die Initiative enthält. Sie können in der Aktualisierung auf den Namen des Plans klicken, um den Plan im [!DNL Scenario Planner].

     ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **Die [!UICONTROL Übersicht] der [!UICONTROL Projektdetails] Abschnitt**: Ein neuer [!DNL Scenario Planner] wird in diesem Bereich erstellt, der Informationen aus der verknüpften Initiative enthält.

     ![](assets/scenario-planner-on-project-details-350x135.png)

     Die folgenden Initiativinformationen werden im [!DNL Scenario Planner] der [!UICONTROL Projektdetails] Abschnitt:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Projektdauer]</span> </td> 
        <td><span>Die Dauer der entsprechenden Initiative, wenn das Projekt mit einer Initiative verbunden ist. Dieses Feld kann nicht bearbeitet werden.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Letztes Veröffentlichungsdatum]</span> </td> 
        <td><span>Das Datum, an dem das Projekt zuletzt aus einer entsprechenden Initiative veröffentlicht wurde.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Startdatum]</span> </td> 
        <td><span>Der erste Tag des Beginnmonats der Initiative, an dem das Projekt mit einer Initiative verbunden ist.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>Enddatum der [!UICONTROL Initiative]</span> </td> 
        <td><span>Der letzte Tag des Endmonats der Initiative, an dem das Projekt mit einer Initiative verbunden ist. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs und Stunden]</span> </td> 
        <td> <p>Informationen zu den damit verbundenen Stellenrollen und deren Zeitzuweisungen für die Initiative. Dazu gehören:</p> 
         <ul> 
          <li>Name der Auftragsrolle</li> 
          <li>Anzahl der FTE</li> 
          <li> <p>Stundenzahl für alle FTE</p> <p>Sie können die Anzahl der für Ihren Plan oder Ihre Initiative benötigten Arbeitsplatzrollen mithilfe von Stunden oder FTEs schätzen.</p> <p>Weitere Informationen finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen im Szenario-Planer</a>. </p> </li> 
         </ul> 
      <p><b>TIPP</b>

     Wenn die Anzahl der Arbeitsplätze für jeden Monat in der Initiative unterschiedlich ist, zeigt dieses Feld die maximale Anzahl der Rollen an, die für die Initiative benötigt werden. Wenn Sie beispielsweise 1 Berater für Januar und 2 für Februar benötigen, zeigt die Spalte 2 FTE und die entsprechende Anzahl von Stunden für 2 FTE für alle Monate an.</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >Alle Benutzer mit [!UICONTROL Ansicht] Der Zugriff auf das Projekt kann die [!DNL Scenario Planner] im Abschnitt [!UICONTROL Übersicht] Bereich. Sie können steuern, ob dieser Bereich im [!UICONTROL Details] mit einer Layout-Vorlage erstellen. Wenn Benutzern keine Layoutvorlage zugeordnet ist, wird dieser Bereich standardmäßig angezeigt.
     >
     >   
     >   
     >   * Informationen zum Hinzufügen oder Entfernen von Bereichen in der [!UICONTROL Details] Abschnitt mit einer Layoutvorlage finden Sie unter [Anpassen der [!UICONTROL Details] Ansicht mithilfe einer Layoutvorlage](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * Weitere Informationen zum Anzeigen von Informationen finden Sie unter [!UICONTROL Übersicht] der [!UICONTROL Projektdetails], siehe [[!UICONTROL Verwalten] Projektinformationen [!UICONTROL Übersicht] area](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **Die [!UICONTROL Rollenzuweisung] -Bedienfeld in [!UICONTROL Lastenausgleich] oder der Aufgabenliste des Projekts**: Informationen über die Rollenzuweisung für die Initiative werden in diesem Bereich zusätzlich zu den Rollenzuweisungen für das Projekt bereitgestellt.

     Weitere Informationen finden Sie unter [Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![](assets/role-allocation-panel-350x174.png)

     Änderungen an den Daten oder Ressourcen des Projekts wirken sich nicht auf die entsprechende Initiative oder auf einen der Bereiche des Projekts aus, die Informationen über die Initiative enthalten.

   * **Die [!UICONTROL Ressourcen-Budgetierung] der [!UICONTROL Geschäftsfall] des Projekts**: Eine neue Option zum Verwalten von Projektressourcen mit [!DNL Scenario Planner] Informationen werden im Abschnitt [!UICONTROL Ressourcen-Budgetierung] der [!UICONTROL Geschäftsfall] des Projekts.

     Weitere Informationen finden Sie unter [Haushaltsmittel in [!UICONTROL Geschäftsfall] mithilfe der [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![](assets/sp-in-business-case-selected-350x110.png)

1. (Optional) Überprüfen Sie die folgenden Informationen in der [!DNL Scenario Planner] nach der Veröffentlichung eines Szenarios:

   * Das veröffentlichte Szenario wird zum ersten Szenario, nachdem Sie daraus Initiativen veröffentlicht haben.
   * Sie können nach der Veröffentlichung eines Szenarios mindestens einmal in einem anderen Szenario nicht mehr veröffentlichen.
   * Die [!UICONTROL Zu Veröffentlichen wechseln] -Option aus allen anderen Szenarien entfernt, nachdem mindestens eine Initiative aus einem Szenario veröffentlicht wurde.
   * Neben den im Plan enthaltenen Projektsymbolen der veröffentlichten Initiativen wird ein grüner Indikator angezeigt.

     ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * Oben im Szenario wird ein grüner Indikator &quot;Veröffentlicht&quot;angezeigt, der auf der Szenariokarte und auf der Szenariokarte angezeigt wird. Das Feld Veröffentlicht wird auf der Szenariokarte ausgefüllt und gibt die Anzahl der Initiativen im Szenario an, die veröffentlicht wurden.

     ![](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >Wenn alle aus den Initiativen des Szenarios veröffentlichten Projekte gelöscht werden, wird der Hinweis, dass das Szenario veröffentlicht wurde, entfernt. Weitere Informationen finden Sie unter [Projekte löschen](../manage-work/projects/manage-projects/delete-projects.md).

1. (Optional) Aktualisieren Sie die Informationen über die Initiative und wiederholen Sie den oben beschriebenen Prozess, um die Initiative erneut zu veröffentlichen und die Initiativinformationen über das verknüpfte Projekt zu aktualisieren.

   Weitere Informationen zu Bearbeitungsinitiativen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


