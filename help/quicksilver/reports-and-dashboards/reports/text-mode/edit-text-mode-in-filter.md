---
product-area: reporting
navigation-topic: text-mode-reporting
title: Filter im Textmodus bearbeiten
description: '"HINWEIS: fügen Sie in diesem Artikel einen Abschnitt hinzu: /content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Entwerfen Sie diesen Bereich auch im Artikel Textmodus - Übersicht )'''
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: be47bc4da5e3921a7c36e19831acde91aad55db1
workflow-type: tm+mt
source-wordcount: '1031'
ht-degree: 0%

---

# Filter im Textmodus bearbeiten

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

Sie können Filter in einer Liste oder in einem Bericht im Textmodus bearbeiten, um auf Felder zuzugreifen, die in der Standardoberfläche nicht verfügbar sind, und komplexere Filter zu erstellen.

Weitere Textmodusbeispiele beim Erstellen eines Filters finden Sie im Artikel unter &quot;Beispiele für benutzerdefinierte Filter&quot; [Beispiele für benutzerdefinierte Ansicht, Filter und Gruppierung](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um Berichterstellungselemente in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten von Filtern in einem Bericht verwalten</p> <p>Berechtigungen für einen Filter verwalten und ihn bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie mit der Verwendung des Textmodus in einem Bericht oder einer Liste beginnen, sollten Sie stets sicherstellen, dass Sie mit der Syntax des Workfront-Textmodus vertraut sind.

Weitere Informationen finden Sie unter:

* [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Übersicht über die Syntax der Textmodi](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Beispiele für benutzerdefinierte Ansicht, Filter und Gruppierung](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Textmodus in einem Filter bearbeiten

Die Bearbeitung eines Filters im Textmodus ist für Berichte und Listen identisch. Der Zugriff auf den Filter erfolgt über einen Bericht oder eine Liste.

>[!TIP]
>
>Es wird empfohlen, möglichst viele Filter im Standardmodus zu erstellen und den Filter in den Textmodus zu konvertieren, um ihn zu bearbeiten.

Weitere Informationen zum Erstellen von Filtern finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Führen Sie einen der folgenden Schritte aus:

   1. Um auf den Filter eines Berichts zuzugreifen, gehen Sie zum Bericht und klicken Sie auf **Berichtaktionen** > **Bearbeiten** > **Filter** Registerkarte.
   1. Um von einer Liste aus auf den Filter zuzugreifen, navigieren Sie zur Liste und wählen Sie die **Filter** im Dropdown-Menü den Mauszeiger über den zu ändernden Filter und klicken Sie auf **Bearbeiten** icon ![](assets/edit-icon.png).

      Der Filter-Builder wird geöffnet.

1. Klicken **Filterregel hinzufügen** um die Filterbedingungen hinzuzufügen, klicken Sie auf **In den Textmodus wechseln** in der rechten oberen Ecke des Builders.
1. Fügen Sie Filteranweisungen mithilfe des Textmodus hinzu. Jede Filteranweisung kann die folgenden Zeilen und zusätzlichen Informationen enthalten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Filterzeile/Informationen</b></td> 
      <td><b>Beispiel</b></td> 
     </tr> 
     <tr> 
      <td> <p>Feldname und der Wert, der dem Wert entspricht, der in der Workfront-Datenbank angezeigt wird.</p> <p>Diese Zeile ist obligatorisch.</p> <p> Weitere Informationen dazu, wie Objekte und Felder in der Datenbank angezeigt werden, finden Sie unter <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Um nach Aufgaben mit dem Status In Bearbeitung zu filtern, verwenden Sie die folgende Zeile:</p> <p><code>status=INP</code> </p> <p><b>TIPP</b>

   Beim Filtern nach Status müssen Sie den aus drei Buchstaben bestehenden Code des Status und nicht den Namen verwenden.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Modifikator für Feldnamen und dem entspricht der Modifikator . Dies gibt an, welche Bedingungen das Feld, nach dem Sie filtern, erfüllen muss.</p> <p>Diese Zeile ist obligatorisch.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Um anzugeben, dass der Status der Aufgaben, nach denen Sie filtern, gleich In Bearbeitung sein muss, verwenden Sie zusätzlich zur oben stehenden Zeile die folgende Zeile:</p> <p><code>status_Mod=in</code> </p> <p>Wenn der Modifikator ein Bereich ist, gibt es zwei Zeilen, die den Modifikator angeben.</p> 
       <div> <span class="autonumber"><span><b>BEISPIEL </b></span></span> 
        <p>Dies ist ein Textmodusfilter, der nach Aufgaben sucht, die in Bearbeitung sind, die innerhalb des aktuellen Monats über ein geplantes Abschlussdatum verfügen und einem Benutzer mit einer bestimmten GUID zugewiesen sind:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Eine vollständige Liste der Filter-Modifikatoren im Textmodus finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- und Bedingungs-Modifikatoren</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Anweisungsoperator. Standardmäßig ist jede Filteranweisung durch den Operator "AND"verbunden. Dies wird nicht in der Textmodus-Oberfläche angezeigt. Sie können auch einen "OR"-Operator zwischen zwei Anweisungen hinzufügen, um anzugeben, dass Sie nach Objekten filtern möchten, die eine oder die andere von zwei Bedingungen erfüllen können.</p> <p>Filteroperatoren sind nur für Filter mit mehr als einer Anweisung erforderlich.</p> <p>Tipp:   
        <ul> 
         <li> <p>"OR"unterscheidet zwischen Groß- und Kleinschreibung und muss immer großgeschrieben werden.</p> </li> 
         <li> <p>Wenn Sie Ihren Operator von AND in OR ändern, kann sich die Anzahl der Listenelemente erhöhen.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>BEISPIEL </b></span></span> 
        <p>Um nach Aufgaben mit dem Status "Wird ausgeführt"oder mit dem geplanten Abschlussdatum "Heute"zu filtern, verwenden Sie Folgendes: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Ein Platzhalter, mit dem Sie die Informationen in einem Filter generalisieren und auf die aktuelle Zeit oder den angemeldeten Benutzer verweisen können.</p> <p>Platzhalter sind optional.</p> <p>Tipp:   <p>Es wird empfohlen, nach Möglichkeit Platzhalter zu verwenden, um Ihre Filter dynamischer zu gestalten und nicht dieselben Filter für jeden Benutzer oder ähnliche Zeitrahmen zu duplizieren.</p> <p>Weitere Informationen zu Filtern von Platzhaltern finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Platzhalterfiltervariablen</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>BEISPIEL</b></span></span> 
        <p>Um nach Aufgaben zu filtern, die dem aktuell angemeldeten Benutzer zugewiesen sind, verwenden Sie Folgendes:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Gehen Sie wie folgt vor, um eine Filteranweisung hinzuzufügen, die mit dem Operator &quot;OR&quot;verbunden ist:

   1. Fügen Sie eine neue Codezeile hinzu und geben Sie OR ein.:1: gefolgt von dem Objekt oder Attribut, nach dem Sie filtern möchten, und dem Wert, mit dem Sie ihn vergleichen möchten. Verwenden Sie die folgende Zeile, um auf Aufgaben zu verweisen, die sich in einem beliebigen Status außer Neu befinden:

      ```
      OR:1:status=NEW
      ```

   1. Fügen Sie eine zweite Zeile hinzu und geben Sie OR ein.:1: gefolgt vom Objekt, dem Modifikator und dem Modifikatorcode. Um den Modifikator für die Codezeile zu definieren, die auf alle Aufgabenstatus mit Ausnahme von New verweist, verwenden Sie die folgende Modifikatorzeile:

      ```
      OR:1:status_Mod=notin
      ```

      Jeder Zeile der neuen Anweisung muss &quot;OR:`<number>`:&quot;.

      Informationen zum Erstellen von &quot;OR&quot;-Anweisungen in einem Filter finden Sie unter [Erstellen von &quot;OR&quot;-Anweisungen in Textmodusfiltern](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>Sie können mehrere &quot;OR&quot;-Anweisungen im selben Filter haben. Jedes Mal, wenn Sie eine neue &quot;OR&quot;-Anweisung haben, erhöht sich die Zahl nach &quot;OR:&quot;.
Um nach Aufgaben zu filtern, die den Status &quot;In Bearbeitung&quot;aufweisen oder dem angemeldeten Benutzer zugewiesen sind oder die das geplante Abschlussdatum heute aufweisen, verwenden Sie Folgendes:
`status=INP`
`status_Mod=in`
`OR:1:assignedToID=$$USER.ID`
`OR:1:assignedToID_Mod=in`
`OR:2:plannedCompletionDate=$$TODAY`
`OR:2:plannedCompletionDate_Mod=eq`

1. Klicken **Fertig** wenn Sie Ihre Änderungen speichern und den Bericht oder Filter weiter bearbeiten möchten.
1. Klicken **Speichern und schließen** , um Ihren Bericht zu speichern, oder **Filter speichern** , um den Filter in der Liste zu speichern.


