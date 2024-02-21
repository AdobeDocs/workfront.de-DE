---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Erstellen und Vergleichen von Planszenarien im Szenario-Planer
description: Wenn Sie die langfristige Strategie Ihres Unternehmens planen, gibt es viele Informationen, über die Sie am Anfang vielleicht nicht verfügen oder an die Sie nicht denken. Es braucht Zeit und Experimente, um zu einer endgültigen Strategie zu gelangen, die Ihre Interessengruppen akzeptieren können. Die Durchführung einer "Was wäre wenn"-Analyse zur Erstellung mehrerer Szenarien für Ihren Plan kann Ihnen dabei helfen, potenzielle Umstände genau vorherzusagen und zu bewerten und letztendlich den bestmöglichen Plan zu entwickeln.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: 296de69a1c444659c60bcf767bdacdd9e6e36830
workflow-type: tm+mt
source-wordcount: '966'
ht-degree: 1%

---

# Erstellen und Vergleichen von Planszenarien in [!DNL Scenario Planner]

Wenn Sie die langfristige Strategie Ihres Unternehmens planen, gibt es viele Informationen, über die Sie am Anfang vielleicht nicht verfügen oder an die Sie nicht denken. Es braucht Zeit und Experimente, um zu einer endgültigen Strategie zu gelangen, die Ihre Interessengruppen akzeptieren können. Die Durchführung einer &quot;Was wäre wenn&quot;-Analyse zur Erstellung mehrerer Szenarien für Ihren Plan kann Ihnen dabei helfen, potenzielle Umstände genau vorherzusagen und zu bewerten und letztendlich den bestmöglichen Plan zu entwickeln.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
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
   <td> <p>Zugriff bearbeiten oder höher auf [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Erstellen von Szenarien

Ein Szenario ist eine Kopie eines Plans. Sie können beliebig viele Szenarien erstellen. Wir empfehlen jedoch, die Anzahl der Szenarien auf ein Minimum zu beschränken, damit Sie sie einfach vergleichen können.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png)Klicken Sie auf [!UICONTROL Szenarien].

1. Erstellen Sie einen Plan.

   Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Der erste von Ihnen erstellte Plan wird automatisch als[!UICONTROL Ursprüngliches Szenario].&quot;

1. Klicken Sie auf den Nach-unten-Pfeil neben einem vorhandenen Szenario und dann auf das **[!UICONTROL Kopieren]** Symbol.

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Dadurch wird ein neues Szenario mit denselben Informationen wie das kopierte Szenario erstellt. Sie trägt automatisch den Namen[!UICONTROL Szenario 2]&quot;, wenn dies das zweite Szenario Ihres Plans ist, &quot;[!UICONTROL Szenario 3]&quot;, wenn es der dritte ist, und so weiter. Sie können Ihre Szenarien nicht umbenennen. Die Anzahl der Exemplare, die Sie erstellen können, ist unbegrenzt.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:this might change)
   </MadCap:conditionalText>
   -->

1. Aktualisieren Sie Ihr neues Szenario auf eine der folgenden Arten:

   * Erstellen, Aktualisieren oder Löschen von Initiativen

     >[!TIP]
     >
     >Wenn Sie eine Initiative in einem Szenario löschen, wird sie nur aus dem ausgewählten Szenario und nicht aus allen Szenarien entfernt.

     Informationen zum Erstellen von Initiativen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Aktualisieren der Prioritäten Ihrer Initiativen
   * Personen- oder Budgetinformationen anpassen
   * Überprüfen und Anpassen von Initiativkonflikten in Ihrem Szenario

     Informationen zur Konfliktlösung finden Sie unter [Beheben von Initiativkonflikten im [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Klicks **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.

## Szenarios vergleichen

Nachdem Sie Ihre Szenarien erstellt haben, können Sie diese vergleichen, um die beste für Ihre Organisation zu finden.

1. Gehen Sie zu dem Plan, für den Sie Szenarien vergleichen möchten.
1. Klicks **[!UICONTROL Szenarien vergleichen]**. Die Seite mit dem Szenario-Vergleich wird angezeigt.

   Alle vorhandenen Szenarien für den Plan werden im Kartenformat nebeneinander angezeigt. Das anfängliche Szenario wird immer zuerst aufgeführt und ist statisch.

   ![](assets/scenario-cards-overlapping-350x166.png)

1. (Optional) Scrollen Sie nach rechts, um alle Szenariokarten anzuzeigen.

   Die folgenden Informationen werden auf einer Szenariokarte angezeigt:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>Name des Szenarios</td> 
      <td> <p>Ein automatisch generierter Name von Workfront, der nicht bearbeitet werden kann. Beispiel: "[!UICONTROL Ursprüngliches Szenario]", "[!UICONTROL Szenario 2]"usw. </p> </td> 
     </tr> 
     <tr> 
      <td>Beschreibung des Szenarios</td> 
      <td>Ein manueller Eintrag, in dem Sie Details zum Szenario beschreiben können. </td> 
     </tr> 
     <tr> 
      <td>Verfügbare Auftragsrollen</td> 
      <td>Die Anzahl der im Budget des Plans für die Dauer des Plans verfügbaren Arbeitsplatzrollen. </td> 
     </tr> 
     <tr> 
      <td>Erforderliche Aufgabengebiete</td> 
      <td>Die Anzahl der erforderlichen Arbeitsplatzrollen basierend auf Ihren Initiativen. </td> 
     </tr> 
     <tr> 
      <td>Budget</td> 
      <td>Das in diesem Szenario für den Plan definierte Gesamtbudget. Budgetinformationen zu Plänen finden Sie unter <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Übersicht über Pläne im [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Kosten</td> 
      <td>Die mit den Initiativen im Zusammenhang mit dem Szenario verbundenen Kosten. Informationen zu Kosten finden Sie unter <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Übersicht über Initiativen im [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Nutzung</td> 
      <td>Der [!UICONTROL Prozentsatz der Budgetnutzung] für den Plan in diesem Szenario. Weitere Informationen zum Prozentsatz der [!UICONTROL Budgethilfe] finden Sie unter <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Übersicht über Pläne im [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Nettowert</td> 
      <td>Der [!UICONTROL Nettowert] des Plans in diesem Szenario. Informationen zum [!UICONTROL Nettowert] eines Plans finden Sie unter <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Übersicht über Pläne im [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Initiativen</td> 
      <td>Die Anzahl der Initiativen für den Plan in diesem Szenario.</td> 
     </tr> 
     <tr> 
      <td>Konflikt</td> 
      <td>Die Anzahl der Initiativen, die im Plan für dieses Szenario jede Art von Konflikten zeigen. Weitere Informationen zu Initiativkonflikten finden Sie unter <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Beheben von Initiativkonflikten im [!DNL Scenario Planner]</a>. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wenn sich die Informationen zwischen dem ursprünglichen Szenario und zusätzlichen Szenarien unterscheiden, wird neben dem Wert, der sich geändert hat, ein Nach-oben- oder Nach-unten-Pfeil angezeigt, der im Vergleich zum ursprünglichen Szenario einen Anstieg oder Rückgang dieses Werts angibt.
   >
   >
   >![](assets/arrows-on-scenario-cards-highlighted-350x70.png)
   >
   >Beispielsweise können sich das Budget, die Anzahl der Rollen und die Anzahl der Initiativen von einem Szenario zum anderen ändern.

1. Klicken Sie auf den Namen eines Szenarios, um darauf zuzugreifen und Änderungen daran vorzunehmen.

   Weitere Informationen finden Sie unter [Erstellen von Szenarien](#create-scenarios) in diesem Artikel beschrieben.

1. Klicks **[!UICONTROL Beschreibung hinzufügen]** , um eine Beschreibung für das Szenario hinzuzufügen

   Oder

   Klicken Sie auf das Beschreibungsfeld, um es zu aktualisieren, und klicken Sie dann auf eine beliebige Stelle auf dem Bildschirm, um Ihre Änderungen zu speichern.

1. (Optional) Klicken Sie auf die **[!UICONTROL Mehr]** Menü ![](assets/more-icon.png) nach **[!UICONTROL Kopieren]** oder **[!UICONTROL Löschen]** das Szenario.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Wenn Sie ein Szenario kopieren, wird es automatisch auf der Kartenseite angezeigt und nach folgendem Muster umbenannt: &quot;[!UICONTROL Szenario] `<next number in order>`.&quot;

1. (Bedingt) Wenn Sie auf **[!UICONTROL Löschen]** klicken **[!UICONTROL Ja, löschen]** zur Bestätigung.

   Gelöschte Szenarien können nicht wiederhergestellt werden.

   Informationen zum Löschen von Szenarien finden Sie unter [Löschen von Plänen in [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Klicks **[!UICONTROL Plan speichern]** um Ihre Szenarien und Ihren Plan zu speichern.
