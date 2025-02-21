---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Löschen von Plänen im Szenario-Planer
description: Sie können von Ihnen erstellte Pläne löschen. Mit Ihnen geteilte Pläne können nicht gelöscht werden.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 1%

---

# Löschen von Plänen in der [!DNL Scenario Planner]

Sie können von Ihnen erstellte Pläne löschen. Mit Ihnen geteilte Pläne können nicht gelöscht werden.

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

## Pläne löschen

>[!IMPORTANT]
>
>Gelöschte Pläne können nicht wiederhergestellt werden.

Sie können einen Plan löschen oder ein Szenario in einem Plan löschen.

* [Pläne löschen](#delete-plans)
* [Löschen von Szenarien](#delete-scenarios)

### Pläne löschen

>[!IMPORTANT]
>
>Beachten Sie beim Löschen von Plänen Folgendes:
>
>* Alle mit dem Plan zusammenhängenden Informationen werden ebenfalls gelöscht. Dies umfasst alle Szenarien und Initiativen, die mit dem Plan verbunden sind, einschließlich Informationen über Aufgabengebiete und Kosten. Diese Informationen können nicht wiederhergestellt werden.
>* Wenn der Plan ein veröffentlichtes Szenario enthält, werden die mit den gelöschten Initiativen verknüpften Projekte beibehalten und der [!DNL Scenario Planner] Bereich verbleibt im Abschnitt [!UICONTROL Projektdetails].
>
>  Informationen zur Veröffentlichung von Initiativen in Projekten finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Löschen eines Plans:

{{step1-to-scenario-planner}}

Eine Liste mit Plänen wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen.
1. Klicken Sie auf **[!UICONTROL Mehr]** ![Mehr ](assets/more-menu.png) rechts neben dem Plannamen und klicken Sie dann auf **[!UICONTROL Löschen]** > **[!UICONTROL Ja, löschen]**.

   Der Plan wird gelöscht und Sie kehren zur Liste der Pläne zurück.

### Löschen von Szenarien {#delete-scenarios}

>[!IMPORTANT]
>
>Beachten Sie beim Löschen eines Szenarios Folgendes:
>
>* Beim Löschen eines Szenarios werden alle Initiativen und deren Informationen aus dem Szenario gelöscht. Wenn sie in andere Szenarien kopiert werden, bleiben die Initiativen auf den anderen Szenarien.
>* Beim Löschen eines Szenarios übernimmt das nachfolgende Szenario die Nummer des gelöschten Szenarios und die Zählreihenfolge wird beibehalten. Wenn Sie beispielsweise Szenario 4 löschen, wird Szenario 5 zu Szenario 4.
>* Wenn einige Initiativen im Szenario veröffentlicht werden, wird das mit der Initiative verknüpfte Projekt beibehalten und der Bereich Szenario-Planer verbleibt in den verknüpften Projekten
>* Wenn die veröffentlichten Initiativen in einem anderen Szenario vorhanden sind, bleiben sie in diesem Szenario, einschließlich ihrer Verknüpfung mit dem Projekt. Durch die Veröffentlichung dieser Initiativen aus den anderen Szenarien werden die verknüpften Projekte mit neuen Informationen aus diesen Szenarien aktualisiert.
>
>  Informationen zur Veröffentlichung von Initiativen in Projekten finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

So löschen Sie ein Szenario:

1. Wechseln Sie zu dem Plan, für den Sie ein Szenario löschen möchten.

   Standardmäßig wird das anfängliche Szenario angezeigt.

1. Klicken Sie **[!UICONTROL Szenarien vergleichen]**.
1. Klicken Sie oben rechts auf der Szenariokarte auf das Menü **[!UICONTROL Mehr]** ![Mehr](assets/more-menu.png) und dann auf **[!UICONTROL Löschen]**.

   Das Szenario wird gelöscht.

1. Klicken Sie **[!UICONTROL Plan speichern]** um Ihre Änderungen zu speichern.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete initiatives</h2>
<p>(NOTE: moved this section to its own article about deleting initiatives) </p> <note type="important">
<p>Consider the following when deleting initiatives:</p>
<ul>
<li>Deleting an initiative deletes the job roles and cost information from the initiative.</li>
<li><span>When you delete an initiative that is published to a project, the initiative is removed from the scenario but the Scenario Planner area remains in the Project Details section.</span> </li>
<li> <p>If the initiative you delete is the only published initiative on the scenario, the indicator that the plan has been published is also removed. </p> <p>For information about publishing initiatives to projects, see <a href="../scenario-planner/publish-scenarios-update-projects.md" class="MCXref xref">Update or create projects by publishing initiatives in the Scenario Planner</a>.</p> </li>
</ul>
</note>
<p>To delete an initiative:</p>
<ol>
<li value="1"> <p> <p>Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png">, then click Scenarios.</p> </p> <p>A list of plans displays. </p> </li>
<li value="2">Click the name of a plan to open it, then locate the initiative you want to delete.</li>
<li value="3"> <p>Click the <strong>More menu</strong> <img src="assets/more-menu.png"> to the right of the initiative name, then click <strong>Delete</strong> > <strong>Yes, delete it</strong>. </p> <p>The initiative is deleted. </p> </li>
<li value="4">Click <strong>Save Plan</strong> to save your changes. </li>
</ol>
</div>
-->


