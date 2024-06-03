---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Für die Verwendung des Szenario-Planers benötigter Zugriff
description: Der Szenario-Planer benötigt eine separate Lizenz von Adobe Workfront und zusätzlichen Zugriff.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 330ee20ad14ea7409db1c6f627ed6aa0e0c5c014
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]

Die [!DNL Scenario Planner] erfordert eine zusätzliche Lizenz. Informationen zum [!DNL Workfront Scenario Planner], siehe [Die [!DNL Scenario Planner] Übersicht](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Ohne korrekten Zugriff oder ohne entsprechende Berechtigungen können Sie die [!UICONTROL Szenarien] Gebiet von[!DNL  Adobe Workfront] verwalten keine Pläne oder Initiativen für Ihre Organisation. Die Verwaltung von Plänen und Initiativen umfasst das Erstellen, Bearbeiten und Löschen.

>[!IMPORTANT]
>
>Beim Zugriff auf [!UICONTROL Szenarien]können Sie nur von Ihnen erstellte Pläne anzeigen und verwalten. Wenn Sie anderen Benutzern erlauben möchten, die von Ihnen erstellten Pläne anzuzeigen oder zu verwalten, müssen Sie Folgendes tun:
>
>* Link zu Ihrem Plan an andere Benutzer senden
>* Plan für andere Benutzer freigeben
>
>  Informationen zum Teilen eines Plans finden Sie unter [Freigeben eines Plans im [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Wenn ein Benutzer deaktiviert wird, haben seine Pläne keinen Eigentümer und können nicht aufgerufen werden, es sei denn, sie wurden zuvor über einen Link freigegeben.

## Der Zugriff, der erforderlich ist, um die [!DNL Adobe Workfront Scenario Planner]

Sie müssen sicherstellen, dass alle folgenden Bedingungen erfüllt sind, bevor Sie auf die [!DNL Workfront Scenario Planner]:

1. Ihr Unternehmen muss über einen der unten beschriebenen Workfront-Pläne verfügen.

   Je nachdem, ob Sie den neuen oder den aktuellen Workfront-Plan verwenden, muss Ihr Unternehmen über einen der folgenden Schritte verfügen:

   * Für die aktuellen Pläne muss Ihre Organisation über einen der folgenden Schritte verfügen:

      * Die [!UICONTROL Ultimate] [!DNL Workfront] Plan. Der Szenario-Planer ist im Ultimate-Plan enthalten.

        Oder

      * Die [!UICONTROL Auswählen] oder [!UICONTROL Prime] [!DNL Workfront] Plan, zusätzlich zum Kauf eines gesonderten [!DNL Scenario Planner] -Lizenz.

   * Für die aktuellen Workfront-Pläne muss Ihr Unternehmen über Folgendes verfügen:

      * Ihr Unternehmen muss eine [!DNL Workfront] [!UICONTROL Unternehmen] oder höher [!DNL Workfront] Plan. Informationen zum [!DNL Workfront] Pläne, siehe [Workfront-Pläne](https://workfront.com/plans).

      * Ihr Unternehmen muss eine [!DNL Workfront Scenario Planner] zusätzlich zu einer [!DNL Workfront] -Lizenz. Wenden Sie sich an [!DNL Workfront] Kundenbetreuer für weitere Informationen [!DNL Workfront Scenario Planner] Lizenzen.

1. Sie benötigen eine der unten beschriebenen Workfront-Lizenzen.

   Je nachdem, ob Sie die neuen oder die aktuellen Lizenzen verwenden, wird Ihr [!DNL Workfront] -Administrator muss Ihnen eine Lizenz der folgenden Typen zuweisen:

   * Für die neuen Lizenzen:
      * [!UICONTROL Standard]
      * [!UICONTROL hell]

   * Für die aktuellen Lizenzen:

      * [!UICONTROL Plan]
      * [!UICONTROL Arbeit]
      * [!UICONTROL Überprüfen]

   >[!NOTE]
   > 
   >* Bei Verwendung der neuen Lizenzen können Benutzer mit einer [!UICONTROL Mitarbeiter] oder [!UICONTROL Externe] Der Lizenztyp kann nicht auf die [!DNL Scenario Planner].
   >
   >* Bei der Verwendung der aktuellen Lizenzen können Benutzer mit dem Lizenztyp &quot;Anfrage&quot;oder &quot;Externe Lizenz&quot;nicht auf den Szenario-Planer zugreifen.

1. Ihre [!DNL Workfront] Administrator muss [!UICONTROL Ansicht] oder [!UICONTROL Bearbeiten] Zugriff auf [!DNL Scenario Planner] in Ihrer Zugriffsstufe.

   Informationen über die Gewährung des Zugriffs auf die [!DNL Workfront Scenario Planner], siehe [Zugriff auf gewähren [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Optional und empfohlen) Um finanzielle Informationen für Ihre Pläne und Initiativen anzuzeigen oder zu aktualisieren, benötigen Sie [!DNL Workfront] Außerdem muss der Administrator Ihnen Zugriff auf [!UICONTROL Finanzdaten] in Ihrer Zugriffsstufe. Informationen zur Bereitstellung von Finanzdaten auf Ihrer Zugriffsstufe finden Sie unter [Zugriff auf Finanzdaten gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Optional) Wenn Sie auf Pläne zugreifen müssen, die Sie nicht erstellt haben, muss Ihnen ein Planersteller die richtigen Berechtigungen für den Zugriff auf diesen Plan erteilen. Informationen zu den Berechtigungen, die für den Zugriff auf von Ihnen nicht erstellte Pläne und Initiativen erforderlich sind, finden Sie unter [Für den Zugriff auf Pläne und Initiativen erforderliche Berechtigungen](#permissions-needed-to-access-plans-and-initiatives) in diesem Artikel beschrieben.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Zugang erforderlich zur Anzeige von Plänen und Initiativen

Zusätzlich zu Ihrem Unternehmen, das die richtige Lizenz für die [!DNL Workfront Scenario Planner], Ihre [!DNL Workfront] -Administrator muss Ihnen außerdem den folgenden Zugriff und die folgende Einrichtung zuweisen, damit Sie die [!DNL Workfront Scenario Planner] und Informationen in diesem Bereich:

* Eine Zugriffsstufe mit mindestens [!UICONTROL Ansicht] Zugriff auf [!DNL Scenario Planner].

  Informationen über die Zugriffsstufe zu [!DNL Scenario Planner], siehe [Zugriff auf gewähren [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Eine Zugriffsstufe mit mindestens [!UICONTROL Ansicht] Zugriff auf [!UICONTROL Finanzdaten] wenn Sie auch finanzielle Informationen über den Plan und die Initiativen anzeigen müssen. Beispiele für Finanzinformationen sind Budgets, Kosten oder Arbeitsplatzraten.

  Informationen zum [!UICONTROL Finanzdaten] Zugriffsebene, siehe [Zugriff auf Finanzdaten gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Anforderer] und [!UICONTROL Externe] Benutzer haben keinen Zugriff auf die [!DNL Scenario Planner].

* Anzeigen von Berechtigungen für den Plan. Informationen zu den Berechtigungen, die für den Zugriff auf von Ihnen nicht erstellte Pläne und Initiativen erforderlich sind, finden Sie unter [Für den Zugriff auf Pläne und Initiativen erforderliche Berechtigungen](#permissions-needed-to-access-plans-and-initiatives) in diesem Artikel beschrieben.

## Für die Verwaltung von Plänen und Initiativen benötigter Zugriff

Ihre [!DNL Workfront] Der Administrator muss Ihnen den folgenden Zugriff zuweisen, damit Sie Pläne und deren Informationen im [!DNL Scenario Planner]:

* A [!UICONTROL Plan] oder [!UICONTROL Arbeit] Lizenztyp mit Bearbeitungszugriff auf die [!DNL Scenario Planner] in Ihrer Zugriffsstufe.

  Alle anderen Lizenztypen haben keinen Zugriff auf die Verwaltung von Plänen.

  Informationen über die Gewährung des Zugangs zu [!DNL Scenario Planner] auf der Zugriffsebene finden Sie unter [Zugriff auf gewähren [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] Lizenztyp mit [!UICONTROL Bearbeiten] Zugriff auf [!UICONTROL Finanzdaten] in Ihrer Zugriffsebene, wenn Sie auch Finanzinformationen über den Plan aktualisieren müssen.

  Beispiele für Finanzinformationen, die Sie bearbeiten können, sind [!UICONTROL Budget], [!UICONTROL Geplanter Vorteil], und [!UICONTROL Feste Kosten].

  >[!TIP]
  >
  >Nur [!UICONTROL Plan] Lizenzinhaber [!UICONTROL Bearbeiten] Zugriff auf [!UICONTROL Finanzdaten].

  Informationen zum [!UICONTROL Finanzdaten] Zugriffsebene, siehe [Zugriff auf Finanzdaten gewähren](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Verwalten Sie Berechtigungen für einen Plan, den Sie nicht erstellt haben. Informationen zu den Berechtigungen, die für den Zugriff auf von Ihnen nicht erstellte Pläne und Initiativen erforderlich sind, finden Sie unter [Für den Zugriff auf Pläne und Initiativen erforderliche Berechtigungen](#permissions-needed-to-access-plans-and-initiatives) in diesem Artikel beschrieben.

## Für den Zugriff auf Pläne und Initiativen erforderliche Berechtigungen

Zugriffsebenen arbeiten mit Berechtigungen in [!DNL Workfront] um Ihnen Einblick in Pläne und Initiativen zu geben, die Sie nicht erstellt haben. Zusätzlich zu der richtigen Zugriffsstufe für den Zugriff auf die [!DNL Scenario Planner]müssen Sie auch über die richtigen Berechtigungen für den Plan verfügen, den Sie anzeigen oder verwalten möchten, wenn Sie nicht der Ersteller dieser Pläne sind.

Standardmäßig haben Sie nur Zugriff auf von Ihnen erstellte Pläne. Um Pläne anzuzeigen, die andere Benutzer erstellt haben, müssen sie ihre Pläne für Sie freigeben. Weitere Informationen zu Freigabeplänen finden Sie unter [Freigeben eines Plans im [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Wenn ein Benutzer einen Link zu einem Plan teilt, ohne den Plan auch freizugeben, können Sie Berechtigungen für den Plan anfordern. Informationen zum Anfordern von Berechtigungen für Pläne finden Sie unter [Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

