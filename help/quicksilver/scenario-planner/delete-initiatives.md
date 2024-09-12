---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Löschen von Initiativen im Szenario-Planer
description: Sie können Initiativen löschen, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein Benutzer für Sie freigegeben hat. Sie können von Ihnen gelöschte Initiativen nicht wiederherstellen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 799ca02e-c513-4409-b327-1ce7d8eb19ae
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 2%

---

# Löschen von Initiativen im [!DNL Scenario Planner]

Sie können Initiativen löschen, die sich auf einen von Ihnen erstellten Plan oder auf einen Plan beziehen, den ein Benutzer für Sie freigegeben hat. Sie können von Ihnen gelöschte Initiativen nicht wiederherstellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Neu: Ultimate </p></li>
   <p>Der Szenario-Planer ist für den neuen Workfront Select- oder Workfront-Plan nicht verfügbar. </p>
   <li><p>Aktuell: [!UICONTROL Business] oder höher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>Neu: Licht oder höher</p> 
   <p>Aktuell: [!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> <ul><li><p>Für die neuen Workfront-Pläne:</p><p> Adobe Workfront</li></p>
   <li><p>Für die aktuellen Workfront-Pläne: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront-Szenario-Planer</p></li></ul>

<p>Weitere Informationen finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des [!DNL Scenario Planner]</a> erforderlichen Zugriff. </p> </td> 
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

## Löschen von Initiativen

Beachten Sie beim Löschen von Initiativen Folgendes:

* Durch das Löschen einer Initiative werden die erforderliche Anzahl von Arbeitsplatzrollen und die mit der Initiative verbundenen Kosteninformationen aus dem Plan entfernt.
* Durch Löschen einer durch Importieren eines Projekts erstellten Initiative wird das mit der Initiative verknüpfte Projekt nicht gelöscht.
* Das Löschen einer Initiative, die mindestens einmal in einem Projekt veröffentlicht wurde, führt zu folgenden Ergebnissen:

   * Die Initiative wird aus dem Szenario gelöscht, der Bereich [!DNL Scenario Planner] verbleibt jedoch im Abschnitt [!UICONTROL Projektdetails] .
   * Wenn die Initiative, die Sie löschen, die einzige veröffentlichte Initiative für das Szenario ist, wird auch der Hinweis entfernt, dass der Plan veröffentlicht wurde.

     Informationen zu Veröffentlichungsinitiativen für Projekte finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

     Weitere Informationen zum Erstellen von Initiativen durch Importieren von Projekten finden Sie unter [Importieren von Projekten in Pläne in den [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) .

Sie können eine Initiative gleichzeitig löschen oder mehrere Initiativen gleichzeitig löschen.

* [Eine Initiative löschen](#delete-one-initiative)
* [Massenlöschung von Initiativen](#delete-initiatives-in-bulk)

### Eine Initiative löschen {#delete-one-initiative}

{{step1-to-scenario-planner}}

Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiative, die Sie löschen möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das Menü &quot;**[!UICONTROL Mehr&quot;]** ![](assets/more-menu.png) rechts neben dem Namen der Initiative und klicken Sie dann auf &quot;**[!UICONTROL Löschen]**&quot;> &quot;**[!UICONTROL Ja&quot;, löschen Sie es &quot;]**&quot;.

   * Wählen Sie das Feld links neben der Initiative aus, klicken Sie dann auf **[!UICONTROL Löschen]** im schwebenden Menü, das unten im Plan angezeigt wird, und klicken Sie dann auf **[!UICONTROL Ja, löschen Sie es]**.

   Die Initiative und ihre Rolle und ihre Kosteninformationen werden aus dem Plan gestrichen.

1. Klicken Sie auf **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.

### Massenlöschung von Initiativen {#delete-initiatives-in-bulk}

{{step1-to-scenario-planner}}

Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiative, die Sie löschen möchten.
1. Wählen Sie die Felder links neben den Initiativen aus, die Sie löschen möchten, klicken Sie dann im Menü, das unten im Plan angezeigt wird, auf **[!UICONTROL Löschen]** und klicken Sie dann auf **[!UICONTROL Ja, löschen Sie sie]**.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   Die Initiativen und ihre Rolle und ihre Kosteninformationen werden aus dem Plan gestrichen.

1. Klicken Sie auf **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.
