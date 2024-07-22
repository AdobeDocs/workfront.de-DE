---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Kopieren von Initiativen im Szenario-Planer
description: Sie können Initiativen erstellen, indem Sie bestehende kopieren. Sie können Initiativen kopieren, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein anderer für Sie freigegeben hat.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Kopieren von Initiativen in den [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Sie können Initiativen erstellen, indem Sie bestehende kopieren. Sie können Initiativen kopieren, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein anderer für Sie freigegeben hat.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Aktuell: [!UICONTROL Business] oder höher</p>
   <p>Neu: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>Neu: Licht oder höher</p> 
   <p>Aktuell: [!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> 
   <p>Für die aktuellen Workfront-Pläne: </p>
   <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können.</p> <p>Informationen zu Zugriff und Berechtigungen für den [!DNL Workfront Scenario Planner] finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des [!DNL Scenario Planner]</a> benötigten Zugriff. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Zugriffsebene </td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff auf einen Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan in der [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen für die Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

  Informationen zum Erstellen von Initiativen durch Importieren von Projekten finden Sie unter [Importieren von Projekten in Pläne in der  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Kopieren von Initiativen

{{step1-to-scenario-planner}}

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
