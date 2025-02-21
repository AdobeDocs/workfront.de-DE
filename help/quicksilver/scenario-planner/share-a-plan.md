---
product-area: enterprise-scenario-planner-product-area
keywords: Plan,Berechtigungen,Freigabe,Initiativen,Szenarien,Szenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Freigeben eines Plans im Szenario-Planer
description: Sie können einen Plan, den Sie im Adobe Workfront-Szenarioplaner erstellt haben, für andere Benutzer freigeben.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 1%

---

# Plan im [!DNL Scenario Planner] freigeben

<!--Audited: 07/2024-->

Sie können einen Plan in der [!DNL Adobe Workfront Scenario Planner] für andere Benutzer freigeben, damit diese an derselben Arbeit zusammenarbeiten können wie Sie.

>[!TIP]
>
>Wenn Sie einen Link zu einem Plan an andere senden, müssen Sie den Plan auch für diese Personen freigeben, damit sie ihn anzeigen können.

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

## Voraussetzungen

* Die Benutzenden, denen Berechtigungen für den Plan erteilt wurden, müssen Zugriff auf den [!DNL Scenario Planner] in ihren Zugriffsebenen haben, wie sie von Ihrem [!DNL Workfront]-Administrator gewährt wurden, um Berechtigungen für einen Plan zu erhalten.

  Beispielsweise können [!UICONTROL Anforderer] keine Pläne anzeigen, erstellen oder bearbeiten. Dies sollten Sie beachten, wenn Sie einen Plan für einen Benutzer freigeben, der über eine Antragstellerlizenz verfügt.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Weitere Informationen zum Zugriff auf die [!DNL Scenario Planner] für verschiedene Lizenztypen finden Sie unter [Zugriff auf gewähren [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Überlegungen zur Planfreigabe

* Alle Benutzer, einschließlich Systemadministratoren, haben nur Zugriff auf von ihnen erstellte Pläne.
* Sie können einen Plan gemeinsam nutzen oder mehrere Pläne gleichzeitig nutzen.
* Sie können keine Pläne anzeigen, die Sie nicht erstellt haben oder die nicht für Sie freigegeben wurden.
* Sie können einen Plan nur für andere Benutzer freigeben. Pläne können nicht für Gruppen, Teams oder Unternehmen freigegeben werden.
* Sie müssen zuerst einen Plan speichern, bevor Sie ihn freigeben können.
* Sie können eine URL zu einem Plan für einen anderen Benutzer freigeben. Wenn der/die Benutzende nicht die Berechtigung hat, zumindest den Plan anzuzeigen, kann er/sie von einem/r anderen Benutzenden Zugriff auf den Plan anfordern, wenn er/sie die URL erhält. Informationen zum Anfordern des Zugriffs auf einen Plan finden Sie unter [Anfordern des Zugriffs auf einen Plan in der [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Bei der Freigabe mehrerer Pläne, die bereits für andere freigegeben wurden, ersetzen die Benutzer, für die Sie sie freigeben, nicht, sondern werden den vorhandenen Benutzern in jedem ausgewählten Plan hinzugefügt.

## Planberechtigungsoptionen

In der folgenden Tabelle sind die Berechtigungen aufgeführt, die Sie bei der Freigabe eines Plans gewähren können. Weitere Informationen dazu, welchen Zugriff Benutzer auf ihrer Lizenz erhalten, finden Sie unter [Zugriff auf gewähren [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aktionen</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Manage]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL view]</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Plan anzeigen </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Initiativen anzeigen </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Szenarien anzeigen</td> 
   <td>✓</td> 
   <td><span style="font-weight: normal;">✓</span> </td> 
  </tr> 
  <tr> 
   <td>Aufgabengebiete anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Kosten- und Budgetinformationen anzeigen*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Verwalten von Kosten- und Budgetinformationen*</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Initiativen erstellen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Erstellen von Szenarien</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Initiativen oder Szenarien löschen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Szenarien kopieren</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Szenarien veröffentlichen**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

* Sie müssen Zugriff auf Finanzdaten haben, um Finanzinformationen zu Plänen anzeigen oder verwalten zu können, auch wenn Sie über Verwaltungsberechtigungen für Pläne verfügen. Informationen zum Zugriff auf Finanzdaten finden Sie unter [Zugriff auf Finanzdaten gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Um Szenarien veröffentlichen zu können, benötigen Sie Zugriff auf die Erstellung und Berechtigungen zum Verwalten von Projekten.

Informationen zur Zugriffsebene von Projekten finden Sie unter [Zugriff auf Projekte gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

## Pläne freigeben

{{step1-to-scenario-planner}}

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen

   Oder

   Wählen Sie mehrere Pläne aus, um sie stapelweise freizugeben.

   >[!TIP]
   >
   >Sie können einen Plan freigeben, indem Sie oben rechts in der Kopfzeile des Plans auf die Avatare der Benutzer klicken, für die der Plan freigegeben ist.

1. (Bedingt) Wenn Sie einen Plan geöffnet haben, klicken Sie auf das Symbol **[!UICONTROL Mehr]** ![Mehr](assets/more-icon.png) rechts neben dem Namen [!UICONTROL Plan] und klicken Sie dann auf **[!UICONTROL Freigeben]**

   Oder

   Wenn Sie mehrere Pläne ausgewählt haben, um sie zusammen freizugeben, klicken Sie auf das **[!UICONTROL Freigeben]**-Symbol oben ![](assets/share-icon-26x26.png) in der Liste der Pläne, um das [!UICONTROL Plan]-Zugriffsfeld zu öffnen.

   >[!TIP]
   >
   >* Benutzende, die über Berechtigungen für alle ausgewählten Pläne verfügen, werden im [!UICONTROL Plan] angezeigt.
   >* Alle zusätzlichen Benutzer werden hinzugefügt und ersetzen nicht die vorhandenen Benutzer in allen ausgewählten Plänen.

1. Beginnen Sie im Feld **[!UICONTROL Planzugriff erteilen an]** mit der Eingabe des Namens der Benutzer, für die Sie den Plan freigeben möchten, und wählen Sie sie aus, wenn sie in der Liste angezeigt werden.
1. Wählen Sie aus dem Dropdown-Menü Berechtigungen rechts neben dem Benutzernamen die Berechtigungsstufe aus, die Sie ihm für den Plan gewähren möchten.
1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL-Ansicht]</td> 
      <td>Benutzer, für die Sie den Plan freigeben, sind berechtigt, den Plan anzuzeigen. Sie können keine Informationen zum Plan bearbeiten, keine Initiativen hinzufügen, keine Szenarien erstellen und keine Szenarien veröffentlichen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL verwalten]</td> 
      <td> <p>Benutzer, für die Sie den Plan freigeben, sind berechtigt, den Plan zu verwalten, der Bearbeitungsinformationen enthält, Initiativen hinzuzufügen, Szenarien zu erstellen und den Plan zu veröffentlichen. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Sie können einen Plan nur löschen, wenn Sie ihn erstellt haben. Mit Ihnen geteilte Pläne können nicht gelöscht werden.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Der Plan ist jetzt für die von Ihnen angegebenen Benutzer freigegeben.

   Sie können Benutzer mit Berechtigungen für den Plan in der Spalte „Für mich freigegeben“ in einer Liste von Plänen oder in der oberen rechten Ecke der Kopfzeile des Plans anzeigen.

   >[!TIP]
   >
   >Sie können Pläne anzeigen, die für Sie freigegeben sind, indem Sie den Filter [!UICONTROL Für mich freigegeben] in einer Liste von Plänen anwenden.


