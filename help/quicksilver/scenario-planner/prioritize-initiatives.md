---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Aktualisierung der Initiativprioritäten im Szenario-Planer
description: Die Priorisierung von Initiativen ist wichtig, da die Initiativen aus dem Plan in der Reihenfolge ihrer Aufgabenstellung und der Bereitstellung von Haushaltsmitteln finanziert werden, in der sie im Plan aufgeführt sind.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Aktualisierung der Prioritäten der Initiative in [!DNL Scenario Planner]

Die Priorisierung von Initiativen ist wichtig, da die Initiativen aus dem Plan in der Reihenfolge ihrer Aufgabenstellung und der Bereitstellung von Haushaltsmitteln finanziert werden, in der sie im Plan aufgeführt sind.

Sie können Initiativen anhand eines von Ihnen erstellten Plans oder eines Plans, den Sie von einer Person für Sie freigegeben haben, priorisieren.

Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Informationen zum Erstellen von Initiativen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Zugriffsanforderungen

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
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] oder höher auf die [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aktualisierung der Initiativprioritäten

Wenn Sie die Priorität von Initiativen ändern, ändern Sie deren Reihenfolge im Plan.

Wir empfehlen Ihnen, dringendere Initiativen ganz oben auf einen Plan zu setzen und die nahtloseren - die jederzeit und nur dann durchgeführt werden können, wenn Ressourcen zur Verfügung stehen - am Ende des Plans zu platzieren.

>[!NOTE]
>
>[!DNL Workfront] weist den Initiativen Planressourcen in der Reihenfolge zu, in der sie im Plan aufgeführt sind.
>
>Wenn beispielsweise für den Plan drei Ingenieure zur Verfügung stehen und für Initiative 1 und Initiative 2 jeweils zwei Ingenieure erforderlich sind und beide für den gleichen Zeitraum geplant sind, verknüpft Workfront zwei Ingenieure mit Initiative 1 und einen verbleibenden Ingenieur mit Initiative 2. In diesem Fall zeigt Initiative 2, dass ein Konflikt vorliegt, weil es einen Ingenieur verpasst. Manchmal ist es nur möglich, Konflikte innerhalb eines Plans zu vermeiden, indem Sie die Priorität Ihrer Initiativen ändern.

Aktualisierung der Initiativpriorität:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png)Klicken Sie auf [!UICONTROL Szenarien].

   Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiativen, die Sie priorisieren möchten.
1. Klicken Sie auf das Kästchen links neben dem Namen einer oder mehrerer Initiativen und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie links neben dem Namen einer der ausgewählten Initiativen auf den Ziehpunkt und ziehen Sie ihn dann nach oben oder unten in die Liste, um die Priorität der Initiative zu ändern.

      Workfront zeigt die Anzahl der ausgewählten Initiativen an.

      ![](assets/multi-select-initiative-number.png)

   * Klicken Sie auf **[!UICONTROL Prioritize]** am Ende des Plans und wählen Sie dann aus den folgenden Optionen:

      * **[!UICONTROL Oben]**: Verschiebt die ausgewählten Initiativen ganz oben auf der Liste der Initiativen. Die ausgewählten Initiativen werden zuerst im Plan aufgeführt.
      * **[!UICONTROL Unten]**: Verschiebt die ausgewählten Initiativen an den Anfang der Initiativliste. Die ausgewählten Initiativen werden zuletzt im Plan aufgeführt.
      * **[!UICONTROL Auswählen einer Zahl]**: Verschiebt die ausgewählten Initiativen nach der hier angegebenen Initiative.

         ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)
      [!DNL Workfront] fügt die ausgewählten Initiativen, die Sie angeben, sofort ein und die Anzahl aller Initiativen wird entsprechend aktualisiert.


1. Klicken **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.
