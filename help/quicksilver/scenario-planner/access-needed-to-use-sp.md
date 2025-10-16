---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Zugriff für die Verwendung des Szenario-Planers erforderlich
description: Für den Szenario-Planer sind eine separate Lizenz von Adobe Workfront und zusätzlicher Zugriff erforderlich.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 1b06589a705cf218239ff1273b865c05e4ceb96f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Zugriff für die Verwendung des [!DNL Scenario Planner] erforderlich

<!--Audited: 04/2024-->

<!--The [!DNL Scenario Planner] has additional license requirements. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).-->

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Ohne korrekte Zugriffsrechte oder Berechtigungen können Sie möglicherweise den Bereich [!UICONTROL Szenarien] von nicht anzeigen [!DNL  Adobe Workfront] Pläne oder Initiativen für Ihr Unternehmen verwalten. Die Verwaltung von Plänen und Initiativen umfasst das Erstellen, Bearbeiten und Löschen.

## Zugriff zum Anzeigen und Verwenden der [!DNL Adobe Workfront Scenario Planner] erforderlich

Sie müssen sicherstellen, dass alle folgenden Bedingungen erfüllt sind, bevor Sie auf die [!DNL Workfront Scenario Planner] zugreifen können:

1. Ihr Unternehmen muss über ein Workfront Ultimate-Paket verfügen.

   Der Szenario-Planer ist nicht für Workfront Workflow-Pakete verfügbar.

   Wenden Sie sich an Ihren Workfront-Kundenbetreuer, wenn Sie derzeit Workfront erneuern und den Szenarioplaner beibehalten möchten.

   Wenn Sie Neukunde sind, kann der Szenario-Planer nicht mehr erworben werden.

   <!--Old: 
    Depending on whether you use the new or the current Workfront plan, your organization must have one of the following:
    * For the new plans, your organization must have the  [!UICONTROL Ultimate] [!DNL Workfront] plan. The Scenario Planner is included only in the [!UICONTROL Ultimate] plan. 
    * For the current Workfront plans, your organization must have both of the following: 
      * Your organization must purchase a [!DNL Workfront] [!UICONTROL Business] or higher [!DNL Workfront] plan. 
      
      * Your organization must purchase a [!DNL Workfront Scenario Planner] license, in addition to a [!DNL Workfront] license. Contact your [!DNL Workfront] Account Representative to learn about [!DNL Workfront Scenario Planner] licenses. -->

1. Sie müssen über eine der folgenden Workfront-Lizenzen verfügen:

   * [!UICONTROL Licht] oder höher
   * [!UICONTROL Prüfer] oder höher

   <!--Old: 
      * For the current licenses: 
        * [!UICONTROL Plan]
        * [!UICONTROL Work]
        * [!UICONTROL Review]-->
   <!--Old: 
      >[!NOTE]
      > 
      >* When using the new licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
      >
      >* When using the current licenses, users with a Request or External license type cannot access the Scenario Planner. -->

1. Ihr [!DNL Workfront]-Administrator muss Ihnen [!UICONTROL Anzeigen] oder [!UICONTROL Bearbeiten] Zugriff auf [!DNL Scenario Planner] Ihrer Zugriffsebene gewähren.

   Informationen zum Gewähren des Zugriffs auf den [!DNL Workfront Scenario Planner] finden Sie unter [Gewähren des Zugriffs auf [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Optional und empfohlen) Um Finanzinformationen für Ihre Pläne und Initiativen anzuzeigen oder zu aktualisieren, muss Ihnen Ihr [!DNL Workfront]-Administrator auch Zugriff auf [!UICONTROL Finanzdaten] in Ihrer Zugriffsebene gewähren. Informationen zum Gewähren von Finanzdaten auf Ihrer Zugriffsebene finden Sie unter [Gewähren des Zugriffs auf Finanzdaten](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).


<!--1. (Optional) If you need to access plans you didn't create, a plan creator must give you the correct permissions to their plan to access it. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.-->

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

<!--Repetitive from above?? 

## Access needed to view plans and initiatives

In addition to your company acquiring the correct license for the [!DNL Workfront Scenario Planner], your [!DNL Workfront] administrator must also assign you the following access and setup so you can view the [!DNL Workfront Scenario Planner] and the information in this area:

* An access level with at least [!UICONTROL View] access to [!DNL Scenario Planner].

  For information about the access level to [!DNL Scenario Planner], see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* An access level with at least [!UICONTROL View] access to [!UICONTROL Financial Data] if you need to also view financial information about the plan and the initiatives. Some examples of financial information are budgets, costs, or job role rates.

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] and [!UICONTROL External] Users do not have access to view the [!DNL Scenario Planner].

* View permissions to the plan. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

## Access needed to manage plans and initiatives

Your [!DNL Workfront] administrator must assign you the following access so you can manage plans and their information in the [!DNL Scenario Planner]:

* A [!UICONTROL Plan] or [!UICONTROL Work] license type with Edit access to the [!DNL Scenario Planner] in your access level.

  All other license types do not have access to manage plans.

  For information about granting access to [!DNL Scenario Planner] from the Access Level, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] license type with [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level, if you need to also update financial information about the plan.

  Some examples of financial information that you can edit are [!UICONTROL Budget], [!UICONTROL Planned Benefit], and [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Only [!UICONTROL Plan] license holders have [!UICONTROL Edit] access to [!UICONTROL Financial Data].

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Manage permissions to a plan that you didn't create. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

-->

## Für den Zugriff auf Pläne und Initiativen erforderliche Berechtigungen

Zugriffsebenen arbeiten mit Berechtigungen in zusammen, [!DNL Workfront] Ihnen Einblicke in Pläne und Initiativen zu geben, die Sie nicht erstellt haben. Sie müssen nicht nur über die richtige Zugriffsebene für den Zugriff auf die [!DNL Scenario Planner] verfügen, sondern auch über die richtigen Berechtigungen für die Pläne verfügen, die Sie anzeigen oder verwalten möchten, wenn Sie nicht der Ersteller dieser Pläne sind.

Alle Benutzer, einschließlich Systemadministratoren, haben nur Zugriff auf von ihnen erstellte Pläne.

Um Pläne anzuzeigen, die von anderen Benutzern erstellt wurden, müssen diese ihre Pläne wie folgt mit Ihnen teilen:

* Plan für Sie freigeben

  Weitere Informationen zu Freigabeplänen finden Sie unter [Freigeben eines Plans in der [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

* Link zu einem von ihnen erstellten Plan senden

  Wenn ein(e) Benutzende(r) einen Link zu einem Plan freigibt, ohne auch den Plan freizugeben, können Sie Berechtigungen für den Plan anfordern. Informationen zum Anfordern von Berechtigungen für Pläne finden Sie unter [Anfordern von Zugriff auf einen Plan in der [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

>[!NOTE]
>
>Wenn ein Benutzer deaktiviert wird, hat sein Plan keinen Eigentümer und kann nur aufgerufen werden, wenn er zuvor mit einem Link geteilt wurde.


