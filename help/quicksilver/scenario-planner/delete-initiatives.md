---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Löschen von Initiativen im Szenario-Planer
description: Sie können Initiativen löschen, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein Benutzer für Sie freigegeben hat. Sie können keine gelöschten Initiativen wiederherstellen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# Löschen von Initiativen in [!DNL Scenario Planner]

Sie können Initiativen löschen, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein Benutzer für Sie freigegeben hat. Sie können keine gelöschten Initiativen wiederherstellen.

## Zugriffsanforderungen

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
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen. </p> <p>Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich für die Verwendung des [!UICONTROL Szenario-Planers]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] oder höher auf die [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Löschen von Initiativen

Beachten Sie beim Löschen von Initiativen Folgendes:

* Durch das Löschen einer Initiative werden die erforderliche Anzahl von Arbeitsplatzrollen und die mit der Initiative verbundenen Kosteninformationen aus dem Plan entfernt.
* Durch Löschen einer durch Importieren eines Projekts erstellten Initiative wird das mit der Initiative verknüpfte Projekt nicht gelöscht.
* Das Löschen einer Initiative, die mindestens einmal in einem Projekt veröffentlicht wurde, führt zu folgenden Ergebnissen:

   * Die Initiative wird aus dem Szenario gestrichen, aber die [!DNL Scenario Planner] verbleibt im Gebiet [!UICONTROL Projektdetails] Abschnitt.
   * Wenn die Initiative, die Sie löschen, die einzige veröffentlichte Initiative für das Szenario ist, wird auch der Hinweis entfernt, dass der Plan veröffentlicht wurde.

      Informationen zu Veröffentlichungsinitiativen für Projekte finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

      Informationen zum Erstellen von Initiativen durch Importieren von Projekten finden Sie unter [Importieren von Projekten in Pläne in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Sie können eine Initiative gleichzeitig löschen oder mehrere Initiativen gleichzeitig löschen.

* [Eine Initiative löschen](#delete-one-initiative)
* [Massenlöschung von Initiativen](#delete-initiatives-in-bulk)

### Eine Initiative löschen {#delete-one-initiative}

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png)Klicken Sie auf [!UICONTROL Szenarien].

   Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiative, die Sie löschen möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **[!UICONTROL Mehr Menü]** ![](assets/more-menu.png) rechts neben dem Namen der Initiative klicken Sie auf **[!UICONTROL Löschen]** > **[!UICONTROL Ja, löschen]**.

   * Markieren Sie das Feld links neben der Initiative und klicken Sie auf **[!UICONTROL Löschen]** Klicken Sie im unverankerten Menü, das unten im Plan angezeigt wird, auf **[!UICONTROL Ja, löschen]**.

   Die Initiative und ihre Rolle und ihre Kosteninformationen werden aus dem Plan gestrichen.

1. Klicken **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.

### Massenlöschung von Initiativen {#delete-initiatives-in-bulk}

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png)Klicken Sie auf [!UICONTROL Szenarien].

   Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiative, die Sie löschen möchten.
1. Wählen Sie die Felder links neben den Initiativen aus, die Sie löschen möchten, und klicken Sie dann auf **[!UICONTROL Löschen]** aus dem Menü, das unten im Plan angezeigt wird, und klicken Sie dann auf **[!UICONTROL Ja, löschen Sie sie]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Die Initiativen und ihre Rolle und ihre Kosteninformationen werden aus dem Plan gestrichen.

1. Klicken **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.
