---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Kopieren von Initiativen im Szenario-Planer
description: Sie können Initiativen erstellen, indem Sie bestehende kopieren. Sie können Initiativen kopieren, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein anderer für Sie freigegeben hat.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# Kopieren Sie die Initiativen in [!DNL Scenario Planner]

Sie können Initiativen erstellen, indem Sie bestehende kopieren. Sie können Initiativen kopieren, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein anderer für Sie freigegeben hat.

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
   <td> <p>[!DNL Adobe Workfront]<b> Lizenz</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen.</p> <p>Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] oder höher auf die [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Kopieren von Initiativen

Beachten Sie beim Kopieren von Initiativen Folgendes:

* Durch das Kopieren einer Initiative wird die Kopie auf denselben Plan wie die ursprüngliche Initiative gesetzt.
* Durch das Kopieren einer Initiative werden die folgenden Informationen aus der ursprünglichen Initiative kopiert und der neuen Initiative hinzugefügt:

   * [!UICONTROL Dauer]
   * [!UICONTROL Aufgabengebiete]
   * [!UICONTROL Personen] und [!UICONTROL Feste Kosten]
   * [!UICONTROL Geplanter Gewinn]

* Durch das Kopieren einer Initiative können die folgenden Informationen für den Plan geändert werden, sofern die Informationen auf der ursprünglichen Initiative vorhanden sind:

   * Erforderliche Anzahl von Vorgangsrollen
   * [!UICONTROL Kosten]
   * [!UICONTROL Nutzung planen]
   * Vorgangsrollenauslastung
   * [!UICONTROL Nettowert]

* Das Kopieren einer Initiative, die durch Importieren eines Projekts erstellt oder mindestens einmal in ein Projekt veröffentlicht wurde, hat folgende Auswirkungen:

   * Das mit der Initiative verbundene Projekt wird nicht dupliziert.
   * Die kopierte Initiative wird nicht mit dem Projekt verbunden.
   * Die [!DNL Scenario Planner] für Projekte, die mindestens einmal veröffentlicht wurden.

   Informationen zu Veröffentlichungsinitiativen für Projekte finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

   Informationen zum Erstellen von Initiativen durch Importieren von Projekten finden Sie unter [Importieren von Projekten in Pläne in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Kopieren von Initiativen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png)Klicken Sie auf [!UICONTROL Szenarien].

   Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiativen, die Sie kopieren möchten.
1. Markieren Sie das Kontrollkästchen links neben der Initiative bzw. den Initiativen, die Sie kopieren möchten, und klicken Sie auf **[!UICONTROL Kopieren]** aus dem Menü, das unten im Plan angezeigt wird.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] kopiert die Initiativen sofort und fügt sie unter die zuletzt ausgewählte Initiative ein.

   Der Name der kopierten Initiative lautet *[!UICONTROL Kopie von]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Je nachdem, wo Sie die neuen Initiativen einfügen, kann sich die Anzahl der vorhandenen Initiativen ändern.

1. Aktualisieren Sie den Namen der kopierten Initiative.

   >[!TIP]
   >
   >Es wird empfohlen, den Namen der Initiative immer zu aktualisieren, um Verwirrung zu vermeiden, falls Sie sie erneut kopieren möchten.

1. (Optional) Aktualisieren Sie die Priorität Ihrer neu erstellten Initiativen.

   Informationen zur Priorisierung von Initiativen finden Sie unter [Aktualisierung der Prioritäten der Initiative in [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klicken **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.
