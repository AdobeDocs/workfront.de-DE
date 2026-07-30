---
title: Abhängige Verbindungen verwalten
description: Als Workspace-Manager können Sie beim Erstellen von Verbindungsfeldern zwischen Datensatztypen in Adobe Workfront Planning abhängige Verbindungen definieren. Beim Hinzufügen von verbundenen Feldern können Sie eine Einstellung aktivieren, die anzeigt, dass die Werte des verbundenen Datensatztyps von den Werten des Quelldatensatztyps (des Datensatztyps, zu dem Sie die Verbindung hinzufügen) abhängen, wenn beide Felder gemeinsam auf einem dritten Datensatztyp angezeigt werden.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 36e7e482a46a4991e9fae2d895e586e3ca08c476
workflow-type: tm+mt
source-wordcount: '1283'
ht-degree: 2%

---


# Abhängige Verbindungen verwalten

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach der Veröffentlichung in der Vorschau sind dieselben Funktionen auch monatlich in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Als Workspace-Manager können Sie beim Erstellen von Verbindungsfeldern zwischen Datensatztypen in Adobe Workfront Planning abhängige Verbindungen definieren.

Beim Hinzufügen von verbundenen Feldern können Sie eine Einstellung aktivieren, die anzeigt, dass die Werte des verbundenen Datensatztyps von den Werten des Quelldatensatztyps (des Datensatztyps, zu dem Sie die Verbindung hinzufügen) abhängen, wenn beide Felder gemeinsam auf einem dritten Datensatztyp angezeigt werden.

Beispielsweise können Sie sicherstellen, dass ein Feld Region nur Werte anzeigt, die mit der ausgewählten Geografie verknüpft sind. Dies wird direkt im Setup des Verbindungsfelds konfiguriert: Beim Hinzufügen einer Verbindung von einem Geodatensatztyp zu einem abhängigen Datensatztyp (wie Region) ermöglicht eine neue Einstellung es Workspace-Managern, sie als abhängig vom Geodatensatztyp zu markieren, wobei die bereits zwischen diesen Datensatztypen eingerichteten Beziehungen verwendet werden.

Nach der Konfiguration hat jeder Datensatztyp, der auf beide Felder verweist (z. B. eine Kampagne), sofort Auswirkungen: Wenn Sie einen Geo-Wert auswählen, wird die Regionsauswahl auf die tatsächlich mit dieser Geo-Region verknüpften Regionen beschränkt. Dadurch wird Ihre Datensatzstruktur automatisch erzwungen, sodass nicht übereinstimmende Kombinationen vermieden und die manuelle Bereinigung reduziert wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>So verbinden Sie Datensatztypen aus demselben Arbeitsbereich: </p>
<ul> 
<li><p>Jedes Workfront- oder Workflow-Paket mit einem beliebigen Planungspaket</p></li>
<p>ODER</p>
<li><p>Jedes Planungspaket, wenn es als eigenständiges Produkt gekauft wird</p></li>
</ul>

<p>So verbinden Sie Datensatztypen aus verschiedenen Arbeitsbereichen:</p>

<ul>

<li><p>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li>
<p>ODER</p>
<li><p>Jedes Planning Prime- oder Ultimate-Paket, wenn es als eigenständiges Produkt gekauft wird</p></li>
</ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
<tr> 
<td> 
   <p> Zusätzliche Produkte</p> </td> 
   <td> 
   <p> Zusätzlich zu Adobe Workfront müssen Sie über Folgendes verfügen, wenn Sie Datensatztypen mit Objekten aus den folgenden Programmen verbinden möchten:</p>
   <ul><li><p>Eine Adobe Experience Manager Assets-Lizenz und eine Integration zwischen AEM Assets und Workfront, um AEM-Assets mit Planungs-Datensatztypen zu verbinden.</p>
   <p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront für Experience Manager Assets und Assets Essentials: Artikelindex</a>. </p></li>
   <li><p> Eine Adobe GenStudio for Performance Marketing-Lizenz zum Verbinden von Datensatztypen mit GenStudio-Objekten und -Marken</p>
   <p>Weitere Informationen finden Sie <a href="https://experienceleague.adobe.com/de/docs/genstudio-for-performance-marketing/user-guide/get-started">Erste Schritte mit Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Sent a slack message to Norayr, Predator, Snowstorm, Armine for info for this section: 
-->

## Überlegungen zu abhängigen verbundenen Feldern


* Abhängige verbundene Felder können nur zwischen Datensatztypen eingerichtet werden, die über eine etablierte Beziehung zu Verbindungsfeldern verfügen. Sie können keine Abhängigkeitslogik zwischen nicht verwandten Datensatztypen definieren.

* Sie können ein abhängiges Feld zwischen Datensatztypen in separaten Arbeitsbereichen haben.

* Es kann kein abhängiges verknüpftes Feld zwischen Planning-Datensatztypen und Workfront- oder AEM-Objekttypen vorhanden sein.

* Die Abhängigkeitseinstellung wird einzeln im Verbindungsfeld selbst und nicht als globale Regel konfiguriert.

* Das Filterverhalten zwischen den beiden verbundenen Datensätzen wird nur aktiviert, wenn sowohl die Quell- als auch die abhängigen Felder in einem dritten Datensatztyp gemeinsam vorhanden sind. Die Abhängigkeit hat keine Auswirkungen, wenn nur eines der beiden Felder auf einem Datensatztyp angezeigt wird.

* Die Auswahl des abhängigen Felds ist auf Werte beschränkt, die bereits auf Datensatzebene mit dem ausgewählten Quellwert verknüpft sind. Es können keine unverknüpften Werte angezeigt oder vorgeschlagen werden.

* Wenn sich der Wert des Quellfelds ändert, wird das abhängige Feld automatisch gelöscht, anstatt einen ungültigen Status zu erhalten, wodurch verhindert wird, dass nicht übereinstimmende Kombinationen bestehen bleiben.

  Sie erhalten eine Inline- oder Popup-Nachricht, in der erläutert wird, warum das abhängige Feld gelöscht wurde.

## Erstellen einer abhängigen Verbindung

1. Wechseln Sie als Workspace-Manager zu einem Datensatztyp in Workfront Planning und öffnen Sie ihn in der Tabellenansicht.
1. Klicken Sie auf das Symbol **+** in der oberen rechten Ecke der Tabellenansicht, um ein neues Feld hinzuzufügen.
1. Klicken Sie **Neue Verbindung** und beginnen Sie dann mit dem Hinzufügen einer neuen Verbindung für einen zweiten Datensatztyp.

   >[!TIP]
   >
   >Eine abhängige Verbindung kann nur zwischen zwei Planungs-Datensatztypen hergestellt werden. Sie können keine abhängigen Verbindungen zwischen Datensatztypen und Objekten aus Workfront oder AEM erstellen.
1. Aktivieren Sie **Abschnitt** Verbindungseinstellungen“ die Option **Diese Verbindung abhängig machen**.

   >[!TIP]
   >
   >Wenn Sie die Einstellung **Verbindung abhängig machen** aktivieren, wird automatisch die Einstellung **Entsprechendes Feld für verknüpften Datensatztyp erstellen**. Pro Datensatztyp sind maximal 500 Felder zulässig.

   ![Neue Registerkarte „Verbindung“ mit aktivierter abhängiger Verbindung](assets/dependent-connection-enabled-setting.png)

1. Fahren Sie mit dem Einrichten der Verbindung fort, wie im Artikel [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md) beschrieben.
1. Klicken Sie auf **Speichern**.

   Folgendes geschieht:

   * Die Verbindung zwischen den beiden Datensatztypen wird erstellt und ihre Werte hängen voneinander ab, wenn sie gemeinsam auf demselben Datensatztyp angezeigt werden.
   * Für den zweiten Datensatztyp wird ein entsprechendes Feld mit dem ersten Datensatztyp erstellt.
   * Wenn beide Datensatztypen mit einem dritten Datensatztyp verbunden sind, werden als Optionen für das zweite verbundene Datensatzfeld die Werte angezeigt, die mit dem ersten Datensatz verbunden sind. Die als Auswahl für den ersten Datensatztyp angezeigten Werte sind die Werte, die mit dem zweiten Datensatztyp verbunden sind.

     Weitere Informationen finden Sie im Abschnitt [Beispiel für abhängige verbundene Datensatztypen](#example-of-dependent-connected-record-types) in diesem Artikel.
   * In der Spaltenüberschrift der verbundenen Datensatzfelder gibt es einen Hinweis darauf, dass das Feld in einer abhängigen Verbindungsbeziehung steht.

     ![Tooltip des abhängigen Symbols in der Spaltenüberschrift](assets/dependent-icon-tooltip-in-column-header.png)

1. (Optional und empfohlen) Wechseln Sie zu einem dritten Datensatztyp und fügen Sie sowohl den ersten als auch den zweiten Datensatztyp als verbundene Datensatzfelder hinzu.

   ![Abhängige Anzeige für verbundene Felder eines dritten Datensatztyps](assets/dependent-connected-field-indicator-on-a-third-record-type.png)

## Beispiel für abhängige verbundene Datensatztypen

Dieser Abschnitt enthält ein einfaches Beispiel dafür, wie Sie abhängige Datensatztypen einrichten können und wie sie für einen dritten Datensatztyp funktionieren.

1. Erstellen Sie in einem Arbeitsbereich, den Sie verwalten können, die folgenden Datensatztypen:

   * Campaign
   * Länder
   * Kontinente

1. Fügen Sie **Datensatztyp** Länder“ die folgenden Datensätze hinzu:

   * Frankreich
   * Vereinigte Staaten
   * Japan
1. Fügen Sie **Datensatztyp** Kontinente“ die folgenden Datensätze hinzu:

   * Europa
   * Amerika
   * Asien

1. Erstellen Sie über **Datensatztyp** Länder“ ein verbundenes abhängiges Feld für **Kontinente**.

   Dadurch werden die folgenden verbundenen Datensatzfelder hinzugefügt:

   * Das **Länder** verbundene Datensatzfeld für den Datensatztyp **Kontinente**.
   * Das **Kontinente** verbundene Datensatzfeld für den Datensatztyp **Länder**.

1. Führen Sie einen der folgenden Schritte aus:

   * Fügen Sie in **Tabellenansicht** Länder“ die folgenden Werte für das Datensatzfeld Kontinente verbunden hinzu:

     * Europa für Frankreich
     * Amerika für die Vereinigten Staaten
     * Asien für Japan
   * Fügen Sie in **Tabellenansicht** Kontinente“ die folgenden Werte für das Feld **Länder“** verbundenen Datensatzes hinzu:

     * Frankreich für Europa
     * Vereinigte Staaten für Amerika
     * Japan für Asien
1. Fügen Sie die verbundenen Felder **Länder** und **Kontinente** zur Tabellenansicht **Kampagne** des Datensatztyps hinzu.
1. Wählen Sie **Japan** für das Feld **Länder** im Datensatztyp **Kampagne** aus. Beachten Sie, dass für das verbundene Feld **Kontinente** in der Kampagne nur der Wert **Asien** verfügbar ist.

   ODER

   Wählen Sie **Europa** für das Feld **Kontinente** im Datensatztyp der Kampagne aus.

   Beachten Sie, dass für das verbundene Feld **Länder** in der Kampagne nur der Wert **Frankreich** verfügbar ist.



