---
product-area: enterprise-scenario-planner-product-area
keywords: plan,permissions,share,initiative,scenarios,scenario
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Plan im Szenario-Planer freigeben
description: Sie können einen Plan, den Sie im Adobe Workfront-Szenario-Planer erstellt haben, für andere Benutzer freigeben.
author: Alina
feature: Workfront Scenario Planner
exl-id: b8bbb533-4384-414c-8574-4e137962b8ca
source-git-commit: 82a5102d28700368a094502dcd6026462c149eb1
workflow-type: tm+mt
source-wordcount: '916'
ht-degree: 0%

---

# Freigeben eines Plans im [!DNL Scenario Planner]

Sie können einen Plan im [!DNL Adobe Workfront Scenario Planner] mit anderen Benutzern, damit sie an derselben Arbeit wie Sie zusammenarbeiten können.

>[!TIP]
>
>Wenn Sie einen Link zu einem Plan an andere senden, müssen Sie den Plan auch für diese freigeben, damit sie ihn anzeigen können.

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
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] [!DNL Scenario Planner]</p> <p>Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p> [!UICONTROL Verwalten] Berechtigungen für den Plan
     <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!UICONTROL Anforderung] des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

* Benutzer, denen Berechtigungen für den Plan erteilt wurden, müssen Zugriff auf die [!DNL Scenario Planner] -Bereich in ihren Zugriffsebenen, wie von Ihrer [!DNL Workfront] Administrator, um Berechtigungen für einen Plan zu erhalten.

   Beispiel: [!UICONTROL Anforderer] Pläne können nicht angezeigt, erstellt oder bearbeitet werden. Beachten Sie dies bei der Freigabe eines Plans für einen Benutzer, der über eine Requestor-Lizenz verfügt.

<!--
  NOTE: ensure this stays this way and they don't restrict Workers from SP as well?? OR ensure you can even SEE Requestors as an option or they are not grayed out??)
  -->

Weitere Informationen zum Zugriff auf die [!DNL Scenario Planner] Informationen zu verschiedenen Lizenztypen finden Sie unter [Zugriff auf gewähren [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

## Überlegungen zur Freigabe von Plänen

* Sie können einen einzelnen Plan oder mehrere Pläne gemeinsam nutzen.
* Sie können keine Pläne anzeigen, die Sie nicht erstellt haben oder die nicht für Sie freigegeben sind.
* Sie können einen Plan nur für andere Benutzer freigeben. Pläne können nicht für Gruppen, Teams oder Unternehmen freigegeben werden.
* Sie müssen zunächst einen Plan speichern, bevor Sie ihn freigeben können.
* Sie können eine URL für einen Plan für einen anderen Benutzer freigeben. Wenn der Benutzer nicht berechtigt ist, mindestens den Plan anzuzeigen, kann er den Zugriff auf den Plan von einem anderen Benutzer anfordern, wenn er die URL erhält. Informationen zum Anfordern des Zugangs zu einem Plan finden Sie unter [Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).
* Beim Freigeben mehrerer Pläne, die bereits für andere freigegeben wurden, ersetzen die Benutzer, für die Sie freigegeben haben, nicht, sondern werden für jeden ausgewählten Plan zu den vorhandenen Benutzern hinzugefügt.

## Pläne freigeben

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **[!UICONTROL Szenarien]**.
1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen.

   Oder

   Wählen Sie mehrere Pläne aus, um sie stapelweise freizugeben.

   >[!TIP]
   >
   >Sie können einen Plan freigeben, indem Sie auf die Avatare der Benutzer klicken, für die der Plan freigegeben ist, in der oberen rechten Ecke des Plan-Headers.

1. (Bedingt) Wenn Sie einen Plan geöffnet haben, klicken Sie auf die Schaltfläche **[!UICONTROL Mehr]** icon ![](assets/more-icon.png) rechts von der [!UICONTROL Plan] name und klicken Sie auf **[!UICONTROL Freigeben]**

   Oder

   Wenn Sie mehrere Pläne für die gemeinsame Nutzung ausgewählt haben, klicken Sie auf die Schaltfläche **[!UICONTROL Freigeben]** icon ![](assets/share-icon-26x26.png) oben in der Liste der Pläne zum Öffnen der [!UICONTROL Plan] Zugriffsfeld.

   >[!TIP]
   >
   >* Benutzer mit Berechtigungen für alle ausgewählten Pläne werden im [!UICONTROL Plan] Zugriffsfeld.
   >* Zusätzliche Benutzer werden zu den ausgewählten Plänen hinzugefügt und ersetzen nicht die vorhandenen Benutzer.


1. Im **[!UICONTROL Planen Sie Zugriff auf]** ein, geben Sie den Namen der Benutzer ein, für die Sie den Plan freigeben möchten, und wählen Sie sie aus, wenn sie in der Liste angezeigt werden.
1. Wählen Sie im Dropdown-Menü Berechtigungen rechts neben dem Benutzernamen die Berechtigungsebene aus, die Sie dem Plan gewähren möchten.
1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ansicht]</td> 
      <td>Benutzer, für die Sie den Plan freigeben, sind berechtigt, den Plan anzuzeigen. Sie können keine Informationen zum Plan bearbeiten, keine Initiativen, Szenarien oder Veröffentlichungsszenarien hinzufügen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Verwalten]</td> 
      <td> <p>Benutzer, für die Sie den Plan freigeben, haben die Berechtigung, den Plan zu verwalten. Dazu gehören die Bearbeitung von Informationen, das Hinzufügen von Initiativen, Szenarien und die Veröffentlichung des Plans. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Sie können einen Plan nur löschen, wenn Sie ihn erstellt haben. Sie können Pläne, die für Sie freigegeben wurden, nicht löschen.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Der Plan wird nun für die angegebenen Benutzer freigegeben.

   Sie können Benutzer mit Berechtigungen für den Plan in der Spalte Für mich freigegeben in einer Liste von Plänen oder in der oberen rechten Ecke der Planüberschrift anzeigen.

   >[!TIP]
   >
   >Sie können für Sie freigegebene Pläne anzeigen, indem Sie die Variable [!UICONTROL Freigegeben für mich] in einer Liste von Plänen.

## Berechtigungsoptionen planen

In der folgenden Tabelle sind die Berechtigungen aufgeführt, die Sie beim Freigeben eines Plans gewähren können. Weitere Informationen über den Zugriff, den Benutzer auf der Grundlage ihrer Lizenz erhalten, finden Sie unter [Zugriff auf gewähren [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aktionen</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Verwalten]</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Ansicht]</strong> </p> </th> 
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
   <td>Anzeigen von Vorgangsrollen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Kosten- und Budgetangaben anzeigen*</td> 
   <td>✓</td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td>Kosten- und Budgetdaten verwalten*</td> 
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
   <td> <p>Löschen von Initiativen oder Szenarien</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Szenarien kopieren</td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Veröffentlichungsszenarien**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Sie müssen Zugriff auf Finanzdaten haben, um finanzielle Informationen zu Plänen anzeigen oder verwalten zu können, selbst wenn Sie über Verwaltungsberechtigungen für Pläne verfügen. Informationen über den Zugang zu Finanzdaten finden Sie unter [Zugriff auf Finanzdaten gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

**Sie müssen Zugriff haben, um Projekte zu erstellen und zu verwalten, damit Sie Szenarien veröffentlichen können.

Informationen zur Zugriffsebene von Projekten finden Sie unter [Projektzugriff gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Weitere Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in [!DNL Adobe Workfront]](../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
