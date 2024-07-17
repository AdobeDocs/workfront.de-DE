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
ht-degree: 0%

---

# Kopieren von Initiativen in den [!DNL Scenario Planner]

Sie können Initiativen erstellen, indem Sie bestehende kopieren. Sie können Initiativen kopieren, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein anderer für Sie freigegeben hat.

## Zugriffsanforderungen

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] oder höher</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können.</p> <p>Informationen zum Abrufen des [!DNL Workfront Scenario Planner] finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des [!DNL Scenario Planner]</a> benötigten Zugriffs. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] oder höher auf die [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff auf einen Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan in der [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Kopieren von Initiativen

Beachten Sie beim Kopieren von Initiativen Folgendes:

* Durch das Kopieren einer Initiative wird die Kopie auf denselben Plan wie die ursprüngliche Initiative gesetzt.
* Durch das Kopieren einer Initiative werden die folgenden Informationen aus der ursprünglichen Initiative kopiert und der neuen Initiative hinzugefügt:

   * [!UICONTROL Dauer]
   * [!UICONTROL Vorgangsrollen]
   * [!UICONTROL Personen] und [!UICONTROL Feste Kosten]
   * [!UICONTROL Geplanter Vorteil]

* Durch das Kopieren einer Initiative können die folgenden Informationen für den Plan geändert werden, sofern die Informationen auf der ursprünglichen Initiative vorhanden sind:

   * Erforderliche Anzahl von Vorgangsrollen
   * [!UICONTROL Kosten]
   * [!UICONTROL Nutzung planen]
   * Vorgangsrollenauslastung
   * [!UICONTROL Nettowert]

* Das Kopieren einer Initiative, die durch Importieren eines Projekts erstellt oder mindestens einmal in ein Projekt veröffentlicht wurde, hat folgende Auswirkungen:

   * Das mit der Initiative verbundene Projekt wird nicht dupliziert.
   * Die kopierte Initiative wird nicht mit dem Projekt verbunden.
   * Der Abschnitt &quot;[!DNL Scenario Planner]&quot;im Projekt wird nicht geändert, wenn Projekte mindestens einmal veröffentlicht wurden.

  Informationen zu Veröffentlichungsinitiativen für Projekte finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Weitere Informationen zum Erstellen von Initiativen durch Importieren von Projekten finden Sie unter [Importieren von Projekten in Pläne in den [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

## Kopieren von Initiativen

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) und dann auf [!UICONTROL Szenarien].

   Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiativen, die Sie kopieren möchten.
1. Markieren Sie das Kästchen links neben der Initiative bzw. den Initiativen, die Sie kopieren möchten, und klicken Sie dann im Menü, das unten im Plan angezeigt wird, auf **[!UICONTROL Kopieren]** .

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] kopiert die Initiativen sofort und platziert sie unter der zuletzt ausgewählten Initiative.

   Der Name der kopierten Initiative lautet *[!UICONTROL Kopie von ]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Je nachdem, wo Sie die neuen Initiativen einfügen, kann sich die Anzahl der vorhandenen Initiativen ändern.

1. Aktualisieren Sie den Namen der kopierten Initiative.

   >[!TIP]
   >
   >Es wird empfohlen, den Namen der Initiative immer zu aktualisieren, um Verwirrung zu vermeiden, falls Sie sie erneut kopieren möchten.

1. (Optional) Aktualisieren Sie die Priorität Ihrer neu erstellten Initiativen.

   Weitere Informationen zur Priorisierung von Initiativen finden Sie unter [Aktualisieren der Initiativprioritäten in der [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klicken Sie auf **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.
