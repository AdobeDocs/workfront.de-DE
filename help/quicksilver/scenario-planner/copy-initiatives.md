---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Kopieren von Initiativen im Szenario-Planer
description: Sie können Initiativen durch Kopieren vorhandener Initiativen erstellen. Sie können Initiativen in einen von Ihnen erstellten Plan oder in einen Plan kopieren, den jemand für Sie freigibt.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Kopieren von Initiativen im [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Sie können Initiativen durch Kopieren vorhandener Initiativen erstellen. Sie können Initiativen in einen von Ihnen erstellten Plan oder in einen Plan kopieren, den jemand für Sie freigibt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Packstück</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTIZ</b></p>
<p>Wenden Sie sich an Ihren Workfront-Support-Mitarbeiter, wenn Sie ein anderes Workfront-Paket haben.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Lizenz</p> </td> 
   <td> <p>[!UICONTROL light] oder höher</p> 
   <p>[!UICONTROL Überprüfung] oder höher</p> </td> 
  </tr> 
    <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für einen Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zum Zugriff auf den Szenario-Planer finden Sie unter [Zugriff für die Verwendung des erforderlich [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen für Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Initiativen kopieren

Beachten Sie beim Kopieren von Initiativen Folgendes:

* Durch Kopieren einer Initiative wird die Kopie auf denselben Plan wie die ursprüngliche Initiative gesetzt.
* Beim Kopieren einer Initiative werden die folgenden Informationen aus der ursprünglichen Initiative kopiert und der neuen Initiative hinzugefügt:

   * [!UICONTROL Dauer]
   * [!UICONTROL Aufgabengebiete]
   * [!UICONTROL Personen] und [!UICONTROL Fixkosten]
   * [!UICONTROL Geplanter Nutzen]

* Durch Kopieren einer Initiative können die folgenden Informationen für den Plan geändert werden, sofern die Informationen für die ursprüngliche Initiative vorhanden sind:

   * Erforderliche Anzahl von Aufgabengebieten
   * [!UICONTROL Kosten]
   * [!UICONTROL Planauslastung]
   * Nutzung des Aufgabengebiets
   * [!UICONTROL Nettowert]

* Das Kopieren einer Initiative, die durch den Import eines Projekts erstellt wurde oder in einem Projekt veröffentlicht wurde, hat mindestens einmal die folgenden Auswirkungen:

   * Das mit der Initiative verknüpfte Projekt wird nicht dupliziert.
   * Die kopierte Initiative wird nicht mit dem Projekt verbunden.
   * Bei Projekten, die mindestens einmal veröffentlicht wurden, wird der [!DNL Scenario Planner] des Projekts nicht geändert.

  Informationen zur Veröffentlichung von Initiativen in Projekten finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Informationen zum Erstellen von Initiativen durch Importieren von Projekten [&#x200B; Sie unter „Projekte in Pläne importieren“ im  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Initiativen kopieren

{{step1-to-scenario-planner}}

Eine Liste mit Plänen wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiativen, die Sie kopieren möchten.
1. Aktivieren Sie das Kästchen links neben der Initiative bzw. den Initiativen, die Sie kopieren möchten, und klicken Sie dann **[!UICONTROL Kopieren]** aus dem Menü, das unten im Plan angezeigt wird.

   ![Initiative kopieren](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] kopiert die Initiativen sofort und platziert sie unter der zuletzt ausgewählten Initiative.

   Der Name der kopierten Initiative lautet *[!UICONTROL Kopie von]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Je nachdem, wo Sie die neuen Initiativen einfügen, kann sich die Anzahl der bestehenden Initiativen ändern.

1. Aktualisieren Sie den Namen der kopierten Initiative.

   >[!TIP]
   >
   >Es wird empfohlen, den Namen der Initiative immer zu aktualisieren, um Verwirrungen zu vermeiden, falls Sie sie erneut kopieren möchten.

1. (Optional) Aktualisieren Sie die Priorität Ihrer neu erstellten Initiativen.

   Informationen zur Prioritätensetzung für Initiativen finden Sie unter [Aktualisieren von Initiativprioritäten in der [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klicken Sie **[!UICONTROL Plan speichern]** um Ihre Änderungen zu speichern.
