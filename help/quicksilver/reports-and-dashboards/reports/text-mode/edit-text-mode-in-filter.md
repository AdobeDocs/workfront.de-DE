---
product-area: reporting
navigation-topic: text-mode-reporting
title: Bearbeiten eines Filters im Textmodus
description: Sie können einen Filter in einer Liste oder einem Bericht im Textmodus bearbeiten, um auf Felder zuzugreifen, die in der Standardschnittstelle nicht verfügbar sind, und komplexere Filter zu erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 1%

---

# Bearbeiten eines Filters im Textmodus

<!-- Audited: 1/2025 -->

Sie können einen Filter in einer Liste oder einem Bericht im Textmodus bearbeiten, um auf Felder zuzugreifen, die in der Standardschnittstelle nicht verfügbar sind, und komplexere Filter zu erstellen.

Weitere Textmodusbeispiele beim Erstellen eines Filters finden Sie auch im Abschnitt [Beispiele für benutzerdefinierte Filter](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters) im Artikel [Benutzerdefinierte Ansicht, Filter und Gruppierungsbeispiele: Artikelindex](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten</p> <p>Bearbeiten des Zugriffs auf Berichte, Dashboards und Kalender, um Berichtselemente in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berichtsberechtigungen zum Bearbeiten von Filtern in einem Bericht</p> <p>Verwalten von Berechtigungen für einen Filter, um ihn zu bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie mit der Verwendung des Textmodus in einem Bericht oder einer Liste beginnen, stellen Sie immer sicher, dass Sie mit der Workfront-Textmodussyntax vertraut sind.

Weitere Informationen finden Sie unter:

* [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [Übersicht über die Textmodus-Syntax](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [Beispiele für benutzerdefinierte Ansichten, Filter und Gruppierungen: Artikelindex](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## Textmodus in einem Filter bearbeiten

Die Bearbeitung eines Filters im Textmodus ist für Berichte und Listen identisch. Der Zugriff auf den Filter über einen Bericht oder eine Liste unterscheidet sich.

>[!TIP]
>
>Es wird empfohlen, so viel Filter wie möglich im Standardmodus zu erstellen und den Filter dann in den Textmodus zu konvertieren, um ihn zu bearbeiten.

Weitere Informationen zum Erstellen von Filtern finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Führen Sie einen der folgenden Schritte aus:

   Um auf den Filter aus einer Liste zuzugreifen, wechseln Sie zur Liste, klicken Sie auf das Symbol **Filter**, bewegen Sie dann den Mauszeiger über den Filter im seitlichen Bedienfeld **Filter**, das Sie ändern möchten, und klicken Sie auf das Symbol **Bearbeiten** ![Bearbeiten](assets/edit-icon.png). Entweder wird im **Filter** Seitenbereich Ihr ausgewählter Filter angezeigt oder der Legacy-Filter-Builder wird geöffnet.

   ODER

   Um auf den Filter aus einem Bericht zuzugreifen, gehen Sie zum Bericht und klicken Sie dann auf **Berichtsaktionen** > **Bearbeiten** > **Filter** Registerkarte.

1. Führen Sie einen der folgenden Schritte aus:

   Wenn Sie den Seitenbereich **Filter** in einer Liste verwenden, klicken Sie auf **Textmodus**.

   ODER

   Wenn Sie den alten Filter-Builder oder einen Bericht verwenden, klicken Sie auf **Filterregel hinzufügen**, um die Bedingungen Ihres Filters hinzuzufügen. Klicken Sie dann auf **Zum Textmodus wechseln** und dann **Textmodus bearbeiten** auf der rechten Seite des Builders.

1. Fügen Sie Filteranweisungen im Textmodus hinzu. Jede Filteranweisung kann die folgenden Zeilen und zusätzliche Informationen enthalten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>Zeile/Informationen filtern</b></td> 
      <td><b>Beispiel</b></td> 
     </tr> 
     <tr> 
      <td> <p>Feldname und der Wert, dem er entspricht, wie sie in der Workfront-Datenbank angezeigt werden.</p> <p>Diese Zeile ist obligatorisch.</p> <p> Weitere Informationen zur Darstellung von Objekten und Feldern in der Datenbank finden Sie unter <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API-Explorer</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>Um nach Aufgaben mit dem Status In Bearbeitung zu filtern, verwenden Sie die folgende Zeile:</p> <p><code>status=INP</code> </p> <p><b>TIPP</b>

   Beim Filtern nach Status müssen Sie den aus drei Buchstaben bestehenden Code des Status und nicht den Namen verwenden.</p> </td>
   </tr> 
     <tr> 
      <td> <p>Was der Modifikator „Feldname“ ist und was der Modifikator ist. Dies gibt an, welche Bedingungen das Feld, nach dem Sie filtern, erfüllen muss.</p> <p>Diese Zeile ist obligatorisch.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>Um anzugeben, dass der Status der Aufgaben, nach denen Sie filtern, gleich „In Bearbeitung“ sein muss, verwenden Sie die folgende Zeile zusätzlich zu der obigen:</p> <p><code>status_Mod=in</code> </p> <p>Wenn der Modifikator ein Bereich ist, gibt es zwei Zeilen, die den Modifikator angeben.</p> 
       <div> <span class="autonumber"><span><b>BEISPIEL </b></span></span> 
        <p>Dies ist ein Textmodusfilter, der nach Aufgaben sucht, die noch in Bearbeitung sind, für die ein geplantes Abschlussdatum innerhalb des aktuellen Monats vorliegt und die einem Benutzer mit einer bestimmten GUID zugewiesen sind:</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>Eine vollständige Liste der Filtermodifikatoren im Textmodus finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter- und Bedingungsmodifikatoren</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Anweisungsoperator. Standardmäßig ist jede Filteranweisung durch den Operator „AND“ verbunden. Dies wird nicht in der Textmodus-Benutzeroberfläche angezeigt. Sie können auch einen OR-Operator zwischen zwei Anweisungen hinzufügen, um anzugeben, dass Sie nach Objekten filtern möchten, die die eine oder die andere der beiden Bedingungen erfüllen.</p> <p>Filteroperatoren sind nur für Filter erforderlich, die mehr als eine Anweisung haben.</p> <p>Tipp:   
        <ul> 
         <li> <p>Bei „ODER“ wird zwischen Groß- und Kleinschreibung unterschieden und diese Angabe muss immer in Großbuchstaben geschrieben werden.</p> </li> 
         <li> <p>Wenn Sie den Operator von UND in ODER ändern, kann sich die Anzahl der Listenelemente erhöhen.</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>BEISPIEL </b></span></span> 
        <p>Um nach Aufgaben mit dem Status In Bearbeitung oder mit dem geplanten Abschlussdatum Heute zu filtern, verwenden Sie Folgendes: </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>Ein Platzhalter, mit dem Sie die Informationen in einem Filter generalisieren und auf die aktuelle Zeit des angemeldeten Benutzers verweisen können.</p> <p>Platzhalter sind optional.</p> <p>Tipp:   <p>Es wird empfohlen, nach Möglichkeit Platzhalter zu verwenden, um Ihre Filter dynamischer zu gestalten, und nicht dieselben Filter für jeden Benutzer oder ähnliche Zeitrahmen zu duplizieren.</p> <p>Informationen zu Filter-Platzhaltern finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Übersicht über Platzhalterfiltervariablen</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>BEISPIEL</b></span></span> 
        <p>Um nach Aufgaben zu filtern, die dem aktuell angemeldeten Benutzer zugewiesen sind, verwenden Sie Folgendes:</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. Gehen Sie wie folgt vor, um eine Filteranweisung hinzuzufügen, die durch den Operator „OR“ verbunden ist:

   1. Fügen Sie eine neue Codezeile hinzu und geben Sie ODER ein:1: gefolgt von dem Objekt oder Attribut, nach dem Sie filtern möchten, und dem Wert, mit dem Sie ihn vergleichen möchten. Um auf Aufgaben zu verweisen, die einen beliebigen Status außer Neu aufweisen, verwenden Sie die folgende Zeile:

      `OR:1:status=NEW`

   1. Fügen Sie eine zweite Zeile hinzu und geben Sie :1: ein, gefolgt vom -Objekt, dem Modifikator und dem Modifikatorcode. Um den Modifikator für die Codezeile zu definieren, die auf alle Aufgabenstatus mit Ausnahme von Neu verweist, verwenden Sie die folgende Modifikatorzeile:

      `OR:1:status_Mod=notin`

      Jeder Zeile der neuen Anweisung muss „OR:`<number>`:“ vorangestellt werden.

      Informationen zum Erstellen von „OR“-Anweisungen in einem Filter finden Sie unter [Erstellen von „OR“-Anweisungen in Textmodusfiltern](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

      >[!NOTE]
      >
      >Sie können mehrere „OR“-Anweisungen im selben Filter haben. Jedes Mal, wenn Sie eine neue „OR“-Anweisung haben, erhöht sich die Zahl nach „OR:“.
      >
      >Um nach Aufgaben zu filtern, die sich im Status In Bearbeitung befinden oder der angemeldeten Person zugewiesen sind oder die das geplante Abschlussdatum heute aufweisen, verwenden Sie Folgendes:
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. Klicken Sie auf **Anwenden** oder **Fertig**, um Ihre Textmodusänderungen zu speichern und mit der Bearbeitung des Berichts oder Filters fortzufahren.
1. Klicken Sie auf **Speichern + Schließen**, um Ihren Bericht zu speichern, oder **Filter speichern**, um den Filter in der Liste zu speichern.


