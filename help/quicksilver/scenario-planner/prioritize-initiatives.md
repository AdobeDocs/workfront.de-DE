---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Aktualisierung der Initiativprioritäten im Szenario-Planer
description: Die Priorisierung von Initiativen ist wichtig, da die Initiativen aus dem Plan in der Reihenfolge ihrer Aufgabenstellung und der Bereitstellung von Haushaltsmitteln finanziert werden, in der sie im Plan aufgeführt sind.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

# Aktualisieren der Initiativprioritäten im [!DNL Scenario Planner]

Die Priorisierung von Initiativen ist wichtig, da die Initiativen aus dem Plan in der Reihenfolge ihrer Aufgabenstellung und der Bereitstellung von Haushaltsmitteln finanziert werden, in der sie im Plan aufgeführt sind.

Sie können Initiativen anhand eines von Ihnen erstellten Plans oder eines Plans, den Sie von einer Person für Sie freigegeben haben, priorisieren.

Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Informationen zum Erstellen von Initiativen finden Sie unter [Erstellen und Bearbeiten von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Aktuell: [!UICONTROL Business] oder höher</p>
   <p>Neu: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>Neu: Licht oder höher</p> 
   <p>Aktuell: [!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> 
   <p>Für die aktuellen Workfront-Pläne: </p>
   <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können.</p> <p>Informationen zu Zugriff und Berechtigungen für den [!DNL Workfront Scenario Planner] finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des [!DNL Scenario Planner]</a> benötigten Zugriff. </p> </td> 
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

## Aktualisierung der Initiativprioritäten

Wenn Sie die Priorität von Initiativen ändern, ändern Sie deren Reihenfolge im Plan.

Wir empfehlen Ihnen, dringendere Initiativen ganz oben auf einen Plan zu setzen und die nahtloseren - die jederzeit und nur dann durchgeführt werden können, wenn Ressourcen zur Verfügung stehen - am Ende des Plans.

>[!NOTE]
>
>[!DNL Workfront] weist den Initiativen Planressourcen in der Reihenfolge zu, in der sie im Plan aufgeführt sind.
>
>Wenn beispielsweise für den Plan drei Ingenieure zur Verfügung stehen und für Initiative 1 und Initiative 2 jeweils zwei Ingenieure erforderlich sind und beide für den gleichen Zeitraum geplant sind, verknüpft Workfront zwei Ingenieure mit Initiative 1 und einen verbleibenden Ingenieur mit Initiative 2. In diesem Fall zeigt Initiative 2, dass ein Konflikt vorliegt, weil es einen Ingenieur verpasst. Manchmal ist es nur möglich, Konflikte innerhalb eines Plans zu vermeiden, indem Sie die Priorität Ihrer Initiativen ändern.

Aktualisierung der Initiativpriorität:

{{step1-to-scenario-planner}}

Eine Liste der Pläne wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiativen, die Sie priorisieren möchten.
1. Klicken Sie auf das Kästchen links neben dem Namen einer oder mehrerer Initiativen und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie links neben dem Namen einer der ausgewählten Initiativen auf den Ziehpunkt und ziehen Sie ihn dann nach oben oder unten in die Liste, um die Priorität der Initiative zu ändern.

     Workfront zeigt die Anzahl der ausgewählten Initiativen an.

     ![](assets/multi-select-initiative-number.png)

   * Klicken Sie unten im Plan auf das Feld **[!UICONTROL Priorize]** und wählen Sie dann aus den folgenden Optionen:

      * **[!UICONTROL Top]**: Verschiebt die ausgewählten Initiativen an den Anfang der Initiativliste. Die ausgewählten Initiativen werden zuerst im Plan aufgeführt.
      * **[!UICONTROL Unten]**: Verschiebt die ausgewählten Initiativen an den unteren Rand der Initiativliste. Die ausgewählten Initiativen werden zuletzt im Plan aufgeführt.
      * **[!UICONTROL Auswählen einer Zahl]**: Verschiebt die ausgewählten Initiativen nach der hier angegebenen Initiative.

        ![](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] platziert die ausgewählten Initiativen sofort an der Stelle, an der Sie angeben, und die Anzahl aller Initiativen wird entsprechend aktualisiert.

1. Klicken Sie auf **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.
