---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Freigeben eines Ziels in Workfront-Zielen
description: Wenn Sie ein Ziel freigeben, gewähren Sie "Verwalten"Berechtigungen für ein Ziel für eine Person, die es nicht erstellt hat.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 4%

---

# Freigeben eines Ziels in Adobe Workfront-Zielen

Wenn Sie ein Ziel freigeben, gewähren Sie &quot;Verwalten&quot;Berechtigungen für ein Ziel für eine Person, die es nicht erstellt hat.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> 
   <p>Für den neuen Plan und die Lizenzstruktur:
  <ul><li>Ein ultimativer Plan </li>
  Oder
  <li>Eine zusätzliche Lizenz für Adobe Workfront Goals für die Prime- oder Select Adobe Workfront-Pläne. </li></ul> </p>
<p>Für den aktuellen Plan und die Lizenzstruktur: 
<ul><li> A Pro oder höher </li>
  <li>Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitarbeiter oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderungen, eine der folgenden: </p>
<ul>
<li>Ein Select- oder Prime-Adobe Workfront-Plan und eine zusätzliche Adobe Workfront Goals-Lizenz.</li>
<li>Ein Ultimate Workfront-Plan, der standardmäßig Workfront-Ziele enthält. </li></ul>
 <p>Oder</p>
 <p>Aktuelle Produktanforderungen: Ein Workfront-Plan und eine zusätzliche Lizenz für Adobe Workfront Goals. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen oder Anzeigen höherer Berechtigungen zum Ziel</p>
  <p>Berechtigungen für das Ziel verwalten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zur Freigabe von Zielen

* Benutzer können die folgenden Berechtigungen für ein Ziel haben:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Zielberechtigungen</b></p></td> 
      <td>
      <p><b>Beschreibung</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Anzeigen</p></td> 
      <td>
      <p>Benutzer sind berechtigt, das Ziel anzuzeigen, können jedoch keine Informationen für das Ziel bearbeiten, keine Informationen für Ergebnisse oder Aktivitäten hinzufügen oder bearbeiten, den Status nicht aktualisieren oder das Ziel löschen.</p>      
      <p>Standardmäßig können alle Benutzer mit Zugriff auf Ziele alle Ziele im System anzeigen. Benutzer können das Ziel kopieren, wenn sie in ihrer Zugriffsebene Zugriff auf Ziele bearbeiten haben.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Verwalten</p></td> 
      <td> <p>Benutzer können alle Informationen für das Ziel bearbeiten, einschließlich der Ergebnisse oder Aktivitäten, einschließlich Löschen.</p> 
      <p>Nur Zielersteller oder Benutzer, denen ausdrücklich die Berechtigung zum Verwalten eines Ziels erteilt wurde, können ein Ziel verwalten.</p> 
      Nur Benutzer mit Verwaltungsberechtigungen für ein Ziel können das Ziel für andere freigeben, um ihnen Berechtigungen zum Ziel zu erteilen. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Sie können die folgenden Arten von Zielen für andere freigeben:

   * Ein von Ihnen erstelltes Ziel
   * Ein Ziel, das von einer anderen Person erstellt wurde, der Sie die Berechtigung zum Verwalten erteilt haben.

* Wenn Sie über Verwaltungsberechtigungen für ein Ziel verfügen, können Sie die Berechtigungen für das Ziel für den Ersteller ändern. Standardmäßig verfügen sie über Verwaltungsberechtigungen, wenn sie das Ziel erstellen. Sie können ihre Berechtigungen jedoch ändern, um sie anzuzeigen.

## Teilen eines Ziels

1. Klicken Sie oben rechts auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png) > **Ziele** .

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Die Zielliste wird angezeigt.

1. Klicken Sie auf den Namen eines Ziels in der Liste. Die Zielseite wird geöffnet.

1. Klicken Sie auf das Symbol &quot;**Mehr&quot;** neben dem Zielnamen und dann auf &quot;**Freigeben**&quot;.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Das Feld &quot;Zielzugriff&quot;wird angezeigt.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie die Einstellung **Systemübergreifendes Verwalten** aus, um allen Systemadministratoren, die Zugriff auf Ziele bearbeiten in ihrer Zugriffsebene haben, Verwaltungsberechtigungen zu erteilen. Diese Option ist für alle neuen Ziele standardmäßig deaktiviert.
   * Beginnen Sie mit der Eingabe des Namens eines Benutzers, dem Sie &quot;Verwalten&quot;Berechtigungen erteilen möchten, in das Feld **Zugriff auf** gewähren. Wählen Sie den Namen aus, wenn er in der Liste angezeigt wird.

     >[!TIP]
     >
     >Sie können ein Ziel nur für andere Benutzer freigeben. Sie können keine Ziele für Gruppen, Teams oder Ihr Unternehmen freigeben.

1. Klicken Sie auf **Freigabe**.

   Das Ziel wird für die von Ihnen angegebenen Benutzer freigegeben. Eine systemweite Beschriftung oder der Name der Benutzer, die über Verwaltungsberechtigungen für das Ziel verfügen, wird im Feld Zugriff auf Verwalten im Bereich Zieldetails angezeigt.

## Optionen für Zielberechtigungen

In der folgenden Tabelle sind die Berechtigungen aufgeführt, die Sie beim Freigeben eines Ziels gewähren können. Weitere Informationen dazu, welche Zugriffsberechtigungen Benutzer auf der Grundlage ihrer Lizenz erhalten, finden Sie unter [Gewähren des Zugriffs auf Adobe Workfront-Ziele](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aktionen</strong> </p> </th> 
   <th> <p><strong>Verwalten</strong> </p> </th> 
   <th> <p><strong>Anzeigen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Ziel anzeigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ergebnisse oder Aktivitäten anzeigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Ziel kopieren* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konvertieren von Ergebnissen oder Aktivitäten in andere Ziele*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Als Aktivitäten hinzugefügte Projekte anzeigen* </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ziel bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeiten von Ergebnissen oder Aktivitäten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hinzufügen von Ergebnissen oder Aktivitäten für das Ziel</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Verknüpfen eines Projekts als Aktivität mit dem Ziel**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Ziel löschen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ergebnisse oder Aktivitäten löschen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projekte vom Ziel trennen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Sie müssen Zugriff auf Ziele bearbeiten in Ihrer Zugriffsebene haben, um Ergebnisse und Aktivitäten in Ziele konvertieren zu können.

**Sie müssen Zugriff auf die Berechtigungen Projekte anzeigen und anzeigen haben, die hinzugefügt wurden oder die Sie zum Ziel hinzufügen möchten, um sie anzuzeigen.

Weitere Informationen zur Zugriffsebene für Projekte finden Sie unter [Gewähren des Zugriffs auf Projekte](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Weitere Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
