---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Für die Verwendung des Szenario-Planers benötigter Zugriff
description: Der Szenario-Planer benötigt eine separate Lizenz von Adobe Workfront und zusätzlichen Zugriff.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: f0f6c2bee98c6cebf8ea9e18bf34262f3c1d6e3a
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Zugriff erforderlich für die Verwendung des [!DNL Scenario Planner]

Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Weitere Informationen zum [!DNL Workfront Scenario Planner] finden Sie unter [Überblick [!DNL Scenario Planner] 3}.](../scenario-planner/scenario-planner-overview.md)

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Ohne korrekten Zugriff oder ohne entsprechende Berechtigungen können Sie möglicherweise den Bereich [!UICONTROL Szenarien] von [!DNL  Adobe Workfront] nicht anzeigen und keine Pläne oder Initiativen für Ihr Unternehmen verwalten. Die Verwaltung von Plänen und Initiativen umfasst das Erstellen, Bearbeiten und Löschen.

>[!IMPORTANT]
>
>Beim Zugriff auf [!UICONTROL Szenarien] können Sie nur von Ihnen erstellte Pläne anzeigen und verwalten. Wenn Sie anderen Benutzern erlauben möchten, die von Ihnen erstellten Pläne anzuzeigen oder zu verwalten, müssen Sie Folgendes tun:
>
>* Link zu Ihrem Plan an andere Benutzer senden
>* Plan für andere Benutzer freigeben
>
>  Informationen zum Freigeben eines Plans finden Sie unter [Planen in der  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md) freigeben.
>
>Wenn ein Benutzer deaktiviert wird, haben seine Pläne keinen Eigentümer und können nicht aufgerufen werden, es sei denn, sie wurden zuvor über einen Link freigegeben.

## Zugriff erforderlich, um die [!DNL Adobe Workfront Scenario Planner] anzuzeigen und zu verwenden

Sie müssen sicherstellen, dass alle folgenden Bedingungen erfüllt sind, bevor Sie auf den [!DNL Workfront Scenario Planner] zugreifen können:

1. Ihr Unternehmen muss über einen der unten beschriebenen Workfront-Pläne verfügen.

   Je nachdem, ob Sie den neuen oder den aktuellen Workfront-Plan verwenden, muss Ihr Unternehmen über einen der folgenden Schritte verfügen:

   * Für die neuen Pläne muss Ihre Organisation über einen der folgenden Schritte verfügen:

      * Der Plan [!UICONTROL Ultimate] [!DNL Workfront]. Der Szenario-Planer ist im Ultimate-Plan enthalten.

        Oder

      * Der Plan [!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] zusätzlich zum Kauf einer separaten [!DNL Scenario Planner] Lizenz.

   * Für die aktuellen Workfront-Pläne muss Ihr Unternehmen über Folgendes verfügen:

      * Ihr Unternehmen muss einen [!DNL Workfront] [!UICONTROL Business]- oder höheren [!DNL Workfront]-Plan erwerben. Weitere Informationen zu den [!DNL Workfront]-Plänen finden Sie unter [Workfront-Pläne](https://workfront.com/plans).

      * Ihr Unternehmen muss zusätzlich zu einer [!DNL Workfront] -Lizenz eine [!DNL Workfront Scenario Planner] -Lizenz erwerben. Wenden Sie sich an Ihren [!DNL Workfront] -Kundenbetreuer, um mehr über [!DNL Workfront Scenario Planner] -Lizenzen zu erfahren.

1. Sie benötigen eine der unten beschriebenen Workfront-Lizenzen.

   Je nachdem, ob Sie die neuen oder aktuellen Lizenzen verwenden, muss Ihr [!DNL Workfront] -Administrator Ihnen eine Lizenz der folgenden Typen zuweisen:

   * Für die neuen Lizenzen:
      * [!UICONTROL Standard]
      * [!UICONTROL Light]

   * Für die aktuellen Lizenzen:

      * [!UICONTROL Plan]
      * [!UICONTROL work]
      * [!UICONTROL Review]

   >[!NOTE]
   > 
   >* Bei Verwendung der neuen Lizenzen können Benutzer mit dem Lizenztyp [!UICONTROL Mitarbeiter] oder [!UICONTROL Externe ] nicht auf den Wert [!DNL Scenario Planner] zugreifen.
   >
   >* Bei der Verwendung der aktuellen Lizenzen können Benutzer mit dem Lizenztyp &quot;Anfrage&quot;oder &quot;Externe Lizenz&quot;nicht auf den Szenario-Planer zugreifen.

1. Ihr [!DNL Workfront] -Administrator muss Ihnen in Ihrer Zugriffsebene den Zugriff auf [!UICONTROL Ansicht] oder [!UICONTROL Bearbeiten] auf [!DNL Scenario Planner] gewähren.

   Weitere Informationen zum Gewähren des Zugriffs auf [!DNL Workfront Scenario Planner] finden Sie unter [Gewähren des Zugriffs auf  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Optional und empfohlen) Um Finanzinformationen für Ihre Pläne und Initiativen anzuzeigen oder zu aktualisieren, muss Ihr [!DNL Workfront] -Administrator Ihnen auch Zugriff auf [!UICONTROL Finanzdaten] in Ihrer Zugriffsebene gewähren. Informationen zur Gewährung von Finanzdaten auf Ihrer Zugriffsstufe finden Sie unter [Gewähren des Zugriffs auf Finanzdaten](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Optional) Wenn Sie auf Pläne zugreifen müssen, die Sie nicht erstellt haben, muss Ihnen ein Planersteller die richtigen Berechtigungen für den Zugriff auf diesen Plan erteilen. Informationen zu den Berechtigungen, die für den Zugriff auf von Ihnen nicht erstellte Pläne und Initiativen erforderlich sind, finden Sie im Abschnitt [Für den Zugriff auf Pläne und Initiativen benötigte Berechtigungen](#permissions-needed-to-access-plans-and-initiatives) in diesem Artikel.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Zugang erforderlich zur Anzeige von Plänen und Initiativen

Zusätzlich zum Erwerb der richtigen Lizenz für [!DNL Workfront Scenario Planner] muss Ihr [!DNL Workfront] -Administrator Ihnen auch den folgenden Zugriff und die folgende Einrichtung zuweisen, damit Sie die [!DNL Workfront Scenario Planner] und die Informationen in diesem Bereich anzeigen können:

* Eine Zugriffsebene mit mindestens [!UICONTROL View] Zugriff auf [!DNL Scenario Planner].

  Informationen zur Zugriffsebene auf [!DNL Scenario Planner] finden Sie unter [Gewähren des Zugriffs auf  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Eine Zugriffsebene mit mindestens [!UICONTROL Anzeigen] Zugriff auf [!UICONTROL Finanzdaten] , wenn Sie auch Finanzinformationen über den Plan und die Initiativen anzeigen müssen. Beispiele für Finanzinformationen sind Budgets, Kosten oder Arbeitsplatzraten.

  Informationen zur Zugriffsstufe [!UICONTROL Finanzdaten] finden Sie unter [Zugriff auf Finanzdaten gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Anforderer] und [!UICONTROL Externe ] Benutzer haben keinen Zugriff auf die Ansicht der [!DNL Scenario Planner].

* Anzeigen von Berechtigungen für den Plan. Informationen zu den Berechtigungen, die für den Zugriff auf von Ihnen nicht erstellte Pläne und Initiativen erforderlich sind, finden Sie im Abschnitt [Für den Zugriff auf Pläne und Initiativen benötigte Berechtigungen](#permissions-needed-to-access-plans-and-initiatives) in diesem Artikel.

## Für die Verwaltung von Plänen und Initiativen benötigter Zugriff

Ihr [!DNL Workfront] -Administrator muss Ihnen den folgenden Zugriff zuweisen, damit Sie Pläne und ihre Informationen in der [!DNL Scenario Planner] verwalten können:

* Ein Lizenztyp vom Typ [!UICONTROL Plan] oder [!UICONTROL Arbeit] mit Zugriff auf [!DNL Scenario Planner] in Ihrer Zugriffsebene bearbeiten .

  Alle anderen Lizenztypen haben keinen Zugriff auf die Verwaltung von Plänen.

  Informationen zum Gewähren des Zugriffs auf [!DNL Scenario Planner] über die Zugriffsebene finden Sie unter [Gewähren des Zugriffs auf  [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Ein [!UICONTROL Planen] -Lizenztyp mit [!UICONTROL Bearbeiten] -Zugriff auf [!UICONTROL Finanzdaten] in Ihrer Zugriffsebene, wenn Sie auch Finanzinformationen über den Plan aktualisieren müssen.

  Beispiele für Finanzinformationen, die Sie bearbeiten können, sind [!UICONTROL Budget], [!UICONTROL Geplanter Nutzen] und [!UICONTROL Feste Kosten].

  >[!TIP]
  >
  >Nur [!UICONTROL Planen] Lizenzinhaber haben [!UICONTROL Bearbeitungs] Zugriff auf [!UICONTROL Finanzdaten].

  Informationen zur Zugriffsstufe [!UICONTROL Finanzdaten] finden Sie unter [Zugriff auf Finanzdaten gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Verwalten Sie Berechtigungen für einen Plan, den Sie nicht erstellt haben. Informationen zu den Berechtigungen, die für den Zugriff auf von Ihnen nicht erstellte Pläne und Initiativen erforderlich sind, finden Sie im Abschnitt [Für den Zugriff auf Pläne und Initiativen benötigte Berechtigungen](#permissions-needed-to-access-plans-and-initiatives) in diesem Artikel.

## Für den Zugriff auf Pläne und Initiativen erforderliche Berechtigungen

Zugriffsebenen arbeiten mit Berechtigungen in [!DNL Workfront] zusammen, um Ihnen Einblick in Pläne und Initiativen zu geben, die Sie nicht erstellt haben. Zusätzlich zum Zugriff auf die [!DNL Scenario Planner] müssen Sie auch über die richtigen Berechtigungen für den Plan verfügen, den Sie anzeigen oder verwalten möchten, wenn Sie nicht der Ersteller dieser Pläne sind.

Standardmäßig haben Sie nur Zugriff auf von Ihnen erstellte Pläne. Um Pläne anzuzeigen, die andere Benutzer erstellt haben, müssen sie ihre Pläne für Sie freigeben. Weitere Informationen zu Freigabeplänen finden Sie unter [Planen in der  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md) freigeben.

Wenn ein Benutzer einen Link zu einem Plan teilt, ohne den Plan auch freizugeben, können Sie Berechtigungen für den Plan anfordern. Weitere Informationen zum Anfordern von Berechtigungen für Pläne finden Sie unter [Anfordern des Zugriffs auf einen Plan in der Datei [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

