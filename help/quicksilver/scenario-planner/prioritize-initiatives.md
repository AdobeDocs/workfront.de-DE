---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Aktualisieren der Initiativen-Prioritäten im Szenario-Planer
description: Die Priorisierung von Initiativen ist wichtig, da Initiativen Aufgabengebiete und Budgetressourcen aus dem Plan in der Reihenfolge erhalten, in der sie im Plan aufgeführt sind.
author: Alina
feature: Workfront Scenario Planner
exl-id: 45f019de-b29c-477b-8bd1-f32ef21c1015
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Aktualisierung der [!DNL Scenario Planner]

Die Priorisierung von Initiativen ist wichtig, da Initiativen Aufgabengebiete und Budgetressourcen aus dem Plan in der Reihenfolge erhalten, in der sie im Plan aufgeführt sind.

Sie können Initiativen nach einem von Ihnen erstellten Plan oder nach einem Plan priorisieren, den jemand für Sie freigegeben hat.

Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Informationen zum Erstellen von Initiativen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Packstück</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTIZ</b></p>
<p>Wenden Sie sich an Ihren Workfront-Support-Mitarbeiter, wenn Sie ein anderes Workfront-Paket haben.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Lizenz</p> </td> 
   <td> <p>[!UICONTROL light] oder höher</p> 
   <p>[!UICONTROL Überprüfung] oder höher</p> </td> 
  </tr> 
    <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für einen Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zum Zugriff auf den Szenario-Planer finden Sie unter [Zugriff für die Verwendung des erforderlich [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen für Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Aktualisieren der Prioritäten der Initiative

Wenn Sie die Priorität von Initiativen ändern, ändern Sie deren Listenreihenfolge im Plan.

Wir empfehlen, dringendere Initiativen an die Spitze eines Plans zu stellen und die fließenderen - die jederzeit und nur möglich wären, wenn Ressourcen zur Verfügung stünden - am Ende des Plans.

>[!NOTE]
>
>[!DNL Workfront] ordnet den Initiativen Planressourcen in der Reihenfolge zu, in der sie im Plan aufgeführt sind.
>
>Wenn beispielsweise im Plan drei Techniker verfügbar sind und für Initiative 1 und Initiative 2 jeweils zwei Techniker erforderlich sind und beide für denselben Zeitraum geplant sind, verknüpft Workfront zwei Techniker mit Initiative 1 und einen verbleibenden verfügbaren Techniker mit Initiative 2. In diesem Fall zeigt Initiative 2 einen Konflikt an, da ein Ingenieur fehlt. Manchmal ist die Änderung der Priorität Ihrer Initiativen der einzige Weg, Konflikte auf einem Plan zu vermeiden.

So aktualisieren Sie die Priorität der Initiative:

{{step1-to-scenario-planner}}

Eine Liste mit Plänen wird angezeigt.

1. Klicken Sie auf den Namen eines Plans, um ihn zu öffnen, und suchen Sie dann die Initiativen, die Sie priorisieren möchten.
1. Klicken Sie links neben dem Namen einer oder mehrerer Initiativen auf das Kästchen und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie links neben dem Namen einer der ausgewählten Initiativen auf den Ziehgriff und ziehen Sie sie dann in der Liste nach oben oder unten, um die Priorität der Initiative zu ändern.

     Workfront zeigt die Anzahl der ausgewählten Initiativen an.

     ![Multi-Select-](assets/multi-select-initiative-number.png)

   * Klicken Sie **[!UICONTROL unten im Plan auf]** Priorisieren) und wählen Sie dann eine der folgenden Optionen aus:

      * **[!UICONTROL Oben]**: Verschiebt die ausgewählten Initiativen an den Anfang der Liste. Die ausgewählten Initiativen werden im Plan an erster Stelle aufgeführt.
      * **[!UICONTROL Unten]**: Verschiebt die ausgewählten Initiativen an das Ende der Liste. Die ausgewählten Initiativen werden im Plan als letzte aufgeführt.
      * **[!UICONTROL Eine Zahl auswählen]**: Verschiebt die ausgewählten Initiativen nach der hier angegebenen Initiative.

        ![Initiativen priorisieren](assets/prioritize-initiatives-expanded-highlighted-350x171.png)

     [!DNL Workfront] platziert die ausgewählten Initiativen sofort an die angegebene Stelle und die Anzahl aller Initiativen wird entsprechend aktualisiert.

1. Klicken Sie **[!UICONTROL Plan speichern]** um Ihre Änderungen zu speichern.
