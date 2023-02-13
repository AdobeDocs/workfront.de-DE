---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Löschen von Plänen im Szenario-Planer
description: Sie können von Ihnen erstellte Pläne löschen. Sie können Pläne, die für Sie freigegeben wurden, nicht löschen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 1%

---

# Löschen von Plänen in [!DNL Scenario Planner]

Sie können von Ihnen erstellte Pläne löschen. Sie können Pläne, die für Sie freigegeben wurden, nicht löschen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

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
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen.</p> <p>Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] oder höher auf die [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

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
>* Alle mit dem Plan zusammenhängenden Informationen werden ebenfalls gelöscht. Dies umfasst alle mit dem Plan verbundenen Szenarien und Initiativen, einschließlich Informationen über die Rollen und Kosten bei der Arbeit. Diese Informationen können nicht abgerufen werden.
>* Wenn der Plan ein veröffentlichtes Szenario enthält, werden die mit den gelöschten Initiativen verknüpften Projekte beibehalten und die [!DNL Scenario Planner] verbleibt im Gebiet [!UICONTROL Projektdetails] Abschnitt.
>
>  Informationen zu Veröffentlichungsinitiativen für Projekte finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

So löschen Sie einen Plan:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png)Klicken Sie auf [!UICONTROL Szenarien].

   Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen.
1. Klicken Sie auf **[!UICONTROL Mehr Menü]** ![](assets/more-menu.png) rechts neben dem Namen des Plans klicken Sie auf **[!UICONTROL Löschen]** > **[!UICONTROL Ja, löschen]**.

   Der Plan wird gelöscht und Sie kehren zur Liste der Pläne zurück.

### Löschen von Szenarien {#delete-scenarios}

>[!IMPORTANT]
>
>Beachten Sie beim Löschen eines Szenarios Folgendes:
>
>* Beim Löschen eines Szenarios werden alle Initiativen und ihre Informationen aus dem Szenario gelöscht. Wenn sie in andere Szenarien kopiert werden, bleiben die Initiativen in den anderen Szenarien erhalten.
>* Beim Löschen eines Szenarios übernimmt das nachfolgende Szenario die Nummer des gelöschten Szenarios und die Zählreihenfolge wird beibehalten. Wenn Sie beispielsweise Szenario 4 löschen, wird Szenario 5 zu Szenario 4.
>* Wenn einige Initiativen zum Szenario veröffentlicht werden, wird das mit der Initiative verknüpfte Projekt beibehalten und der Bereich &quot;Szenario-Planer&quot;bleibt auf den verknüpften Projekten erhalten
>* Wenn die veröffentlichten Initiativen auf einem anderen Szenario vorhanden sind, bleiben sie auf diesem Szenario, einschließlich ihrer Verknüpfung zum Projekt. Durch die Veröffentlichung dieser Initiativen aus den anderen Szenarien werden die verknüpften Projekte mit neuen Informationen aus diesen Szenarien aktualisiert.
>
>  Informationen zu Veröffentlichungsinitiativen für Projekte finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

So löschen Sie ein Szenario:

1. Gehen Sie zu dem Plan, für den Sie ein Szenario löschen möchten.

   Standardmäßig wird das Szenario Anfänglich angezeigt.

1. Klicken **[!UICONTROL Szenarien vergleichen]**.
1. Klicken Sie oben rechts auf der Szenariokarte auf die **[!UICONTROL Mehr]** Menü ![](assets/more-menu.png)Klicken Sie auf **[!UICONTROL Löschen]**.

   Das Szenario wird gelöscht.

1. Klicken **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.

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


