---
title: Löschen von Datensätzen
description: Sie können Datensätze löschen, die Sie oder ein anderer Benutzer erstellt haben.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 2%

---


# Löschen von Datensätzen

<!--take Preview and Production references out at release-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können Datensätze löschen, die in Adobe Workfront Planning nicht mehr relevant sind. Gelöschte Datensätze können nach dem Löschen 30 Tage lang wiederhergestellt werden. Informationen zum Wiederherstellen gelöschter Datensätze finden Sie unter [Wiederherstellen gelöschter Datensätze](/help/quicksilver/planning/records/restore-deleted-records.md).

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
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard</p>
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
   <td>   <p>Mitwirken an oder höhere Berechtigungen für einen Arbeitsbereich <span class="preview">und einen Datensatztyp</span> </a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>In der Produktionsumgebung müssen alle Benutzer, einschließlich der Systemadministratoren, einer Layoutvorlage zugewiesen werden, die Planning enthält.</p>
<p><span class="preview">In der Vorschau-Umgebung ist für Standardbenutzer und Systemadministratoren „Planung“ standardmäßig aktiviert.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Löschen von Datensätzen

* Sie können Datensätze löschen, die Sie oder ein anderer Benutzer erstellt haben.
* Gelöschte Datensätze können nicht in der Produktionsumgebung wiederhergestellt werden. Sie können gelöschte Datensätze in der Vorschau-Umgebung wiederherstellen.
* Wenn die gelöschten Datensätze mit anderen Datensätzen verknüpft sind, werden die verknüpften Datensätze nicht gelöscht, aber die Informationen aus dem gelöschten Datensatz werden ebenfalls gelöscht.
* Sie können keine Datensätze aus der Zeitleiste oder den Kalenderansichten löschen.

## Löschen von Datensätzen

Sie können einen Datensatz aus den folgenden Bereichen löschen:

* [Von der Datensatzseite](#delete-a-record-from-the-records-page)
* [Aus der Tabellenansicht eines Datensatztyps](#delete-a-record-from-the-record-type-table-view)

### Löschen eines Datensatzes auf der Datensatzseite

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie löschen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in einer Tabellenansicht auf den Namen eines Datensatzes.
   * Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen eines Datensatzes und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und anschließend auf **Anzeigen**

     ![Kontextmenü für Datensatzzeile](assets/contextual-menu-for-record-row.png)
   * Klicken Sie in einer Zeitleisten -Ansicht auf eine Datensatzleiste.

   Die Datensatzseite wird geöffnet.

1. Klicken Sie auf das **Mehr**-Menü ![Mehr](assets/more-menu.png) rechts neben dem Datensatznamen und klicken Sie dann zur Bestätigung **Löschen** und dann erneut auf **Löschen**.

   ![Weitere Menüoptionen auf der Seite „Datensatzdetails“](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
Der Datensatz wird gelöscht.
1. (Optional und bedingt) Wenn Sie den Datensatz in der Vorschau-Umgebung löschen, wechseln Sie zur Tabellenansicht der Datensatzseite und klicken Sie auf das **Rückgängig**-Symbol ![Rückgängig-Symbol](assets/undo-icon.png) in der oberen rechten Ecke der Ansicht und klicken Sie dann auf **Kürzlich gelöscht**, um die gelöschten Datensätze wiederherzustellen.

Informationen zum Wiederherstellen gelöschter Datensätze finden Sie unter [Wiederherstellen gelöschter Datensätze](/help/quicksilver/planning/records/restore-deleted-records.md).

### Löschen eines Datensatzes aus der Tabellenansicht vom Typ Datensatz

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie löschen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Wählen Sie **Dropdownmenü** Ansicht“ in der linken oberen Ecke der Tabelle eine Tabellenansicht aus. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Zeitleisten -Ansicht zum Zeitpunkt des letzten Zugriffs angezeigt.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie mit der rechten Maustaste auf eine Datensatzzeile und dann auf **Löschen**.
   * Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Datensatznamen und dann auf **Löschen**.

     ![Kontextmenü für Datensatzzeile](assets/contextual-menu-for-record-row.png)

   * Klicken Sie auf **Symbol** Details öffnen![ (Symbol „Details öffnen“ im Feld &quot;](assets/open-details-icon-in-table-name-field.png)„), um das Feld mit den detaillierten Informationen zum Datensatz zu öffnen, und klicken Sie auf **Mehr** ![Mehr Menü](assets/more-menu.png) rechts neben dem Datensatznamen und dann auf **Löschen**.

   Der Datensatz wird gelöscht.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um das Löschen eines Datensatzes rückgängig zu machen oder wiederherzustellen:

   * Klicken Sie auf das **Rückgängig**-Symbol ![Rückgängig-Symbol](assets/undo-icon.png) und dann auf **Kürzlich gelöscht**, um die gelöschten Datensätze wiederherzustellen. Informationen zum Wiederherstellen gelöschter Datensätze finden Sie unter [Wiederherstellen gelöschter Datensätze](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Mit den folgenden Tastaturbefehlen können Sie das Löschen eines Datensatzes rückgängig machen oder wiederholen:

      * Strg+Z (⌘+Z für Mac), um das Löschen eines Eintrags rückgängig zu machen
      * Strg+Umsch+Z (⌘+Umschalt+Z für Mac), um das Löschen eines Eintrags wiederherzustellen




