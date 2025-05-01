---
title: Freigeben von Datensätzen
description: Sie können Datensätze für andere freigeben, um die Zusammenarbeit zu verbessern.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Freigeben von Datensätzen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Um mit anderen Benutzern zusammenzuarbeiten, können Sie Datensätze für andere freigeben.

Sie können einen Adobe Workfront Planning-Datensatz wie folgt freigeben:

* Kopieren Sie den Link der Datensatzseite aus Ihrem Browser, wenn die Seite geöffnet ist.

* Kopieren Sie bei der Anzeige von Datensätzen in der Tabellenansicht des Datensatztyps einen Link auf die Seite des Datensatzes.

* Sie können alle Datensätze in einem Arbeitsbereich für andere Benutzer freigeben, indem Sie den Arbeitsbereich (<span class="preview"> den Datensatztyp) freigeben</span>

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [Datensatztyp freigeben](/help/quicksilver/planning/access/share-record-types.md)

  </div>

In diesem Artikel wird beschrieben, wie Sie einen Link zur Datensatzseite aus der Tabellenansicht eines Datensatztyps kopieren können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Mitwirkende oder höhere Lizenz </p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  <p>Anzeigen oder Erweitern von Berechtigungen für einen Arbeitsbereich (<span class="preview"> Datensatztyp) </span> Freigabe   Einen Datensatz unter Verwendung eines Links </p>
   <p>Verwalten von Berechtigungen für einen Arbeitsbereich <span class="preview">und Datensatztyp</span> um die Datensätze im Arbeitsbereich freizugeben </p>
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>In der Produktionsumgebung müssen alle Benutzer, einschließlich der Systemadministratoren, einer Layoutvorlage zugewiesen werden, die die Planungsbereiche enthält.</p>
   <div class="preview">
<p> In der Vorschau-Umgebung müssen Benutzenden mit einer Light- oder Contributor-Lizenz eine Layout-Vorlage zugewiesen werden, die Planning enthält.</p>

<p>Für Standardbenutzer und Systemadministratoren ist die Planung standardmäßig aktiviert.</p></div>

<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Erstellen und Verwalten von Layout-Vorlagen</a>.</p></td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Freigeben von Datensatz-Links aus der Tabellenansicht vom Typ Datensatz

{{step1-to-planning}}

Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Wählen Sie **Dropdownmenü** Ansicht“ oben rechts in der Tabelle eine Tabellenansicht aus. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Zeitleisten -Ansicht zum Zeitpunkt des letzten Zugriffs angezeigt.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Rechtsklick auf eine Datensatzzeile

   Oder

   Bewegen Sie den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und dann auf **Link kopieren**.

   ![Kontextmenü für Datensatzzeile](assets/contextual-menu-for-record-row.png)

   Der Link wird in die Zwischenablage kopiert.

1. Fügen Sie den Link in ein E-Mail- oder Chat-Fenster ein, um ihn für andere Benutzer freizugeben. Wenn Benutzende den Link erhalten, wird die Datensatzseite geöffnet.

   >[!TIP]
   >
   >Die Felder auf der Datensatzseite sind dieselben Felder, die auch in der Tabellenansicht des Datensatzes verfügbar sind.


   <!--add there when it will be available: if they have access to this record-->

## Freigeben aller Datensätze in einem Arbeitsbereich durch Freigeben des Arbeitsbereichs

Sie können alle Datensätze in einem Arbeitsbereich freigeben, wenn Sie den Arbeitsbereich für andere freigeben.

Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können ihn für andere freigeben.

Weitere Informationen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md).


<div class="preview">

## Freigabe aller Datensätze in einem Datensatztyp durch Freigabe des Datensatztyps

In der Produktionsumgebung erben Datensätze Berechtigungen vom Arbeitsbereich.

In der Vorschau-Umgebung erben Datensätze Berechtigungen vom Datensatztyp.

Standardmäßig erben Datensatztypen Berechtigungen vom Arbeitsbereich.

Sie können jedoch einen der folgenden Schritte ausführen:

* Deaktivieren Sie geerbte Berechtigungen aus dem Arbeitsbereich für einen Datensatztyp. Dadurch werden höhere Berechtigungen für die Datensätze entfernt, aber die Anzeigeberechtigungen für den Arbeitsbereich, den Datensatztyp und die Datensätze werden beibehalten.
* Benutzern manuell Berechtigungen für einen Datensatztyp erteilen, selbst wenn sie keine Berechtigungen für den Arbeitsbereich haben. Dadurch erhalten sie automatisch Ansichtsberechtigungen für den Arbeitsbereich. Dadurch erhalten Benutzende Berechtigungen für die Datensätze.

Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können seine Datensatztypen und Datensätze für andere freigeben.

Weitere Informationen finden Sie unter [Freigeben von Datensatztypen](/help/quicksilver/planning/access/share-record-types.md).

</div>
