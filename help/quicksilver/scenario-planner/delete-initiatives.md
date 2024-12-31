---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Löschen von Initiativen im Szenario-Planer
description: Sie können Initiativen in einem von Ihnen erstellten Plan oder in einem Plan löschen, den jemand für Sie freigegeben hat. Sie können gelöschte Initiativen nicht wiederherstellen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%

---

# Initiativen im [!DNL Scenario Planner] löschen

Sie können Initiativen in einem von Ihnen erstellten Plan oder in einem Plan löschen, den jemand für Sie freigegeben hat. Sie können gelöschte Initiativen nicht wiederherstellen.

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
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für einen Plan</p> <p>Informationen zum Anfordern zusätzlichen Zugriffs auf einen Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Dokumentation zu Zugriffsanforderungen für Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Initiativen löschen

Beachten Sie beim Löschen von Initiativen Folgendes:

* Durch das Löschen einer Initiative werden die erforderliche Anzahl von Aufgabengebieten und die mit der Initiative verbundenen Kosteninformationen aus dem Plan entfernt.
* Beim Löschen einer Initiative, die durch den Import eines Projekts erstellt wurde, wird das mit der Initiative verknüpfte Projekt nicht gelöscht.
* Das Löschen einer Initiative, die mindestens einmal in einem Projekt veröffentlicht wurde, führt zu Folgendem:

   * Die Initiative wird aus dem Szenario gelöscht, der [!DNL Scenario Planner] Bereich verbleibt jedoch im Abschnitt [!UICONTROL Projektdetails].
   * Wenn die Initiative, die Sie löschen, die einzige veröffentlichte Initiative im Szenario ist, wird der Indikator, dass der Plan veröffentlicht wurde, ebenfalls entfernt.

     Informationen zur Veröffentlichung von Initiativen in Projekten finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     Informationen zum Erstellen von Initiativen durch Importieren von Projekten finden Sie [Projekte in Pläne importieren in der [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Sie können jeweils nur eine Initiative löschen oder mehrere Initiativen gleichzeitig löschen.

* [Löschen Sie eine Initiative](#delete-one-initiative)
* [Initiativen stapelweise löschen](#delete-initiatives-in-bulk)

### Eine Initiative löschen {#delete-one-initiative}

{{step1-to-scenario-planner}}

Eine Liste mit Plänen wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiative, die Sie löschen möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Mehr]** ![](assets/more-menu.png) rechts neben dem Namen der Initiative und klicken Sie dann auf **[!UICONTROL Löschen]** > **[!UICONTROL Ja, löschen]**.

   * Aktivieren Sie das Kästchen links von der Initiative und klicken Sie dann im unverankerten ]**, das unten im Plan angezeigt wird, auf**[!UICONTROL  Löschen und dann auf **[!UICONTROL Ja, löschen]**.

   Die Initiative und ihre Aufgabengebiete sowie Kosteninformationen werden aus dem Plan gelöscht.

1. Klicken Sie **[!UICONTROL Plan speichern]** um Ihre Änderungen zu speichern.

### Initiativen stapelweise löschen {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

Eine Liste mit Plänen wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiative, die Sie löschen möchten.
1. Markieren Sie die Kästchen links neben den Initiativen, die Sie löschen möchten, und klicken Sie dann im unten im Plan angezeigten ]**auf**[!UICONTROL  Löschen und anschließend auf **[!UICONTROL Ja, löschen]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Die Initiativen und ihre Aufgabengebiete sowie Kosteninformationen werden aus dem Plan gelöscht.

1. Klicken Sie **[!UICONTROL Plan speichern]** um Ihre Änderungen zu speichern.
