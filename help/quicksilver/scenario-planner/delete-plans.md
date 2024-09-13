---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Löschen von Plänen im Szenario-Planer
description: Sie können von Ihnen erstellte Pläne löschen. Sie können Pläne, die für Sie freigegeben wurden, nicht löschen.
author: Alina
feature: Workfront Scenario Planner
exl-id: 74515723-3822-425a-aa9e-970af63f9189
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 1%

---

# Löschen von Plänen in der [!DNL Scenario Planner]

Sie können von Ihnen erstellte Pläne löschen. Sie können Pläne, die für Sie freigegeben wurden, nicht löschen.

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
   <p>Der Szenario-Planer ist für die neuen Workfront Select- oder Workfront Prime-Pläne nicht verfügbar. </p>
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
>* Wenn der Plan ein veröffentlichtes Szenario enthält, werden die mit den gelöschten Initiativen verknüpften Projekte beibehalten und der Bereich &quot;[!DNL Scenario Planner]&quot;verbleibt im Abschnitt &quot;[!UICONTROL Projektdetails]&quot;.
>
>  Informationen zu Veröffentlichungsinitiativen für Projekte finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

So löschen Sie einen Plan:

{{step1-to-scenario-planner}}

Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen.
1. Klicken Sie auf das Menü &quot;**[!UICONTROL Mehr&quot;]** ![](assets/more-menu.png) rechts neben dem Planungsnamen und klicken Sie dann auf &quot;**[!UICONTROL Löschen]**&quot;> &quot;**[!UICONTROL Ja&quot;, löschen Sie es]**.

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
>  Informationen zu Veröffentlichungsinitiativen für Projekte finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

Löschen eines Szenarios:

1. Gehen Sie zu dem Plan, für den Sie ein Szenario löschen möchten.

   Standardmäßig wird das Szenario Anfänglich angezeigt.

1. Klicken Sie auf **[!UICONTROL Szenarien vergleichen]**.
1. Klicken Sie in der oberen rechten Ecke der Szenariokarte auf das Menü **[!UICONTROL Mehr]** Menü ![](assets/more-menu.png) und dann auf **[!UICONTROL Löschen]**.

   Das Szenario wird gelöscht.

1. Klicken Sie auf **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.

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


