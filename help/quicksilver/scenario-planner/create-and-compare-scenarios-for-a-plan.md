---
product-previous: enterprise-scenario-planner
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Erstellen und Vergleichen von Planszenarien im Szenario-Planer
description: Wenn Sie die langfristige Strategie Ihres Unternehmens planen, gibt es viele Informationen, über die Sie am Anfang vielleicht nicht verfügen oder an die Sie nicht denken. Es braucht Zeit und Experimente, um zu einer endgültigen Strategie zu gelangen, die Ihre Interessengruppen akzeptieren können. Die Durchführung einer "Was wäre wenn"-Analyse zur Erstellung mehrerer Szenarien für Ihren Plan kann Ihnen dabei helfen, potenzielle Umstände genau vorherzusagen und zu bewerten und letztendlich den bestmöglichen Plan zu entwickeln.
author: Alina
feature: Workfront Scenario Planner
exl-id: 9a79ef81-6271-4cc9-b701-3ba0aeafb324
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '949'
ht-degree: 2%

---

# Erstellen und Vergleichen von Planszenarien im [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Wenn Sie die langfristige Strategie Ihres Unternehmens planen, gibt es viele Informationen, über die Sie am Anfang vielleicht nicht verfügen oder an die Sie nicht denken. Es braucht Zeit und Experimente, um zu einer endgültigen Strategie zu gelangen, die Ihre Interessengruppen akzeptieren können. Die Durchführung einer &quot;Was wäre wenn&quot;-Analyse zur Erstellung mehrerer Szenarien für Ihren Plan kann Ihnen dabei helfen, potenzielle Umstände genau vorherzusagen und zu bewerten und letztendlich den bestmöglichen Plan zu entwickeln.

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
   <p>Der Szenario-Planer ist für den neuen Workfront Select- oder Workfront-Plan nicht verfügbar. </p>
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

## Erstellen von Szenarien

Ein Szenario ist eine Kopie eines Plans. Sie können beliebig viele Szenarien erstellen. Wir empfehlen jedoch, die Anzahl der Szenarien auf ein Minimum zu beschränken, damit Sie sie einfach vergleichen können.

{{step1-to-scenario-planner}}

1. Erstellen Sie einen Plan oder klicken Sie auf den Namen eines existierenden.

   Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Der erste Plan, den Sie erstellen, wird automatisch als &quot;[!UICONTROL Ursprüngliches Szenario]&quot;gespeichert.

1. Klicken Sie auf den nach unten zeigenden Pfeil neben einem vorhandenen Szenario und dann auf das Symbol **[!UICONTROL Kopieren]** .

   ![](assets/copy-scenarios-ui-and-highlighted-icon-350x95.png)

   Dadurch wird ein neues Szenario mit denselben Informationen wie das kopierte Szenario erstellt. Es erhält automatisch den Namen &quot;[!UICONTROL Szenario 2]&quot;, wenn es das zweite Szenario Ihres Plans ist, &quot;[!UICONTROL Szenario 3]&quot;, wenn es das dritte Szenario ist usw. Sie können Ihre Szenarien nicht umbenennen. Die Anzahl der Exemplare, die Sie erstellen können, ist unbegrenzt.

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

     Informationen zum Erstellen von Initiativen finden Sie unter [Erstellen und Bearbeiten von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   * Aktualisieren der Prioritäten Ihrer Initiativen
   * Personen- oder Budgetinformationen anpassen
   * Überprüfen und Anpassen von Initiativkonflikten in Ihrem Szenario

     Weitere Informationen zum Auflösen von Konflikten finden Sie unter [Beheben von Initiativkonflikten im  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. Klicken Sie auf **[!UICONTROL Plan speichern]** , um Ihre Änderungen zu speichern.

## Szenarios vergleichen

Nachdem Sie Ihre Szenarien erstellt haben, können Sie diese vergleichen, um die beste für Ihre Organisation zu finden.

1. Gehen Sie zu dem Plan, für den Sie Szenarien vergleichen möchten.
1. Klicken Sie auf **[!UICONTROL Szenarien vergleichen]**. Die Seite mit dem Szenario-Vergleich wird angezeigt.

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
      <td>Das in diesem Szenario für den Plan definierte Gesamtbudget. Budgetinformationen zu Plänen finden Sie unter <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Übersicht über Pläne in der [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Kosten</td> 
      <td>Die mit den Initiativen im Zusammenhang mit dem Szenario verbundenen Kosten. Informationen zu Kosten finden Sie unter <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Übersicht über Initiativen in der [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Nutzung</td> 
      <td>Der [!UICONTROL Prozentsatz der Budgetnutzung] für den Plan in diesem Szenario. Informationen zum Prozentsatz der [!UICONTROL Budgetnutzung] finden Sie unter <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Übersicht über Pläne in der [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Nettowert</td> 
      <td>Der [!UICONTROL Nettowert] des Plans in diesem Szenario. Informationen zum [!UICONTROL Nettowert] eines Plans finden Sie unter <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Übersicht über Pläne in der [!DNL Scenario Planner]</a>. </td> 
     </tr> 
     <tr> 
      <td>Initiativen</td> 
      <td>Die Anzahl der Initiativen für den Plan in diesem Szenario.</td> 
     </tr> 
     <tr> 
      <td>Konflikt</td> 
      <td>Die Anzahl der Initiativen, die im Plan für dieses Szenario jede Art von Konflikten zeigen. Informationen zu Initiativkonflikten finden Sie unter <a href="../scenario-planner/resolve-conflicts-in-sp.md" class="MCXref xref">Beheben von Initiativkonflikten im [!DNL Scenario Planner]</a>. </td> 
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

   Weitere Informationen finden Sie im Abschnitt [Szenarien erstellen](#create-scenarios) in diesem Artikel.

1. Klicken Sie auf **[!UICONTROL Beschreibung hinzufügen]** , um eine Beschreibung für das Szenario hinzuzufügen.

   Oder

   Klicken Sie auf das Beschreibungsfeld, um es zu aktualisieren, und klicken Sie dann auf eine beliebige Stelle auf dem Bildschirm, um Ihre Änderungen zu speichern.

1. (Optional) Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![](assets/more-icon.png), um das Szenario in **[!UICONTROL Kopieren]** oder in **[!UICONTROL Löschen]** zu kopieren.

   ![](assets/copy-or-delete-scenario-links-from-card-350x109.png)

   Wenn Sie ein Szenario kopieren, wird es automatisch auf der Kartenseite angezeigt und gemäß folgendem Muster umbenannt: &quot;[!UICONTROL Szenario] `<next number in order>`&quot;.

1. (Bedingt) Wenn Sie auf **[!UICONTROL Löschen]** geklickt haben, klicken Sie auf **[!UICONTROL Ja, löschen Sie es]**, um dies zu bestätigen.

   Gelöschte Szenarien können nicht wiederhergestellt werden.

   Informationen zum Löschen von Szenarien finden Sie unter [Löschpläne in der  [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

1. Klicken Sie auf **[!UICONTROL Plan speichern]** , um Ihre Szenarien und Ihren Plan zu speichern.
