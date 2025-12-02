---
title: Datensatztypen löschen
description: Sie können Datensatztypen löschen, wenn sie nicht mehr relevant sind. Durch das Löschen von Datensatztypen werden auch alle mit den Datensatztypen verknüpften Informationen gelöscht, z. B. ihre Datensätze, Felder und Ansichten.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 476e10f2962f19fd17705cb5f20619d3b636aaa4
workflow-type: tm+mt
source-wordcount: '1062'
ht-degree: 1%

---


<!--keep the global record type reference in yellow till January 2026-->

# Datensatztypen löschen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können Datensatztypen löschen, wenn sie nicht mehr relevant sind.

Beim Löschen von Datensatztypen werden jedoch auch alle mit den Datensatztypen verknüpften Informationen gelöscht. Weitere Informationen finden Sie im Abschnitt [Überlegungen beim Löschen von Datensatztypen](#considerations-when-deleting-record-types) in diesem Artikel.

Weitere Informationen zu Datensatztypen finden Sie unter [Datensatztypen - Übersicht](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
Oder
<li><p>Beliebiger Workflow und beliebiges Planungspaket</p></li></ul>
<div class="preview">
<p>So löschen Sie globale Datensatztypen:</p>
<ul><li><p>Beliebiges Workfront-Paket und Planning Plus-Paket</p></li>
Oder
<li><p>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li></ul>
</div>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
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

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## Überlegungen beim Löschen von Datensatztypen

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Sie können nur Datensatztypen aus Arbeitsbereichen löschen, für die Sie über Verwaltungsberechtigungen verfügen.
* Durch das Löschen von Datensatztypen werden die folgenden mit ihnen verknüpften Informationen entfernt:

   * Alle Datensätze dieses Typs.
   * Alle mit dem Datensatztyp verknüpften Felder.
   * Alle Ansichten (einschließlich Filtern, Gruppierungen und Sortierkriterien) des Datensatztyps.
* Der Datensatztyp wird aus allen Benutzern entfernt, die auf den Arbeitsbereich zugreifen.
* Gelöschte Datensatztypen oder deren Informationen können nicht wiederhergestellt werden.
* Es wird empfohlen, die Felder und die mit dem Datensatztyp verknüpften Datensätze, die Sie löschen möchten, in einem anderen Datensatztyp neu zu erstellen, bevor Sie sie löschen.

<div class="preview">

* Ein globaler Datensatztyp, der anderen Arbeitsbereichen hinzugefügt wurde, kann nicht gelöscht werden.

  Weitere Informationen finden Sie im Abschnitt [Löschen globaler ](#delete-global-record-types)) in diesem Artikel.

</div>

## Datensatztypen löschen

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie löschen möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Zeigen Sie mit der Maus auf die Karte für den Datensatztyp und klicken Sie auf das Menü **Mehr** und dann auf **Löschen**.
   * Klicken Sie auf die Karte für den Datensatztyp, den Sie löschen möchten, und klicken Sie auf der Seite Datensatztyp auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Löschen**.

   ![Datensatztyp-Bestätigung dauerhaft löschen](assets/permanently-delete-record-type-confirmation.png)


1. Geben Sie **Bestätigungsfeld** Löschen“ ein und klicken Sie dann auf **Dauerhaft löschen**. Hierbei wird nicht zwischen Groß- und Kleinschreibung unterschieden.

   Der ausgewählte Datensatztyp wird zusammen mit den zugehörigen Feldern, zugehörigen Datensätzen und Ansichten gelöscht und kann nicht wiederhergestellt werden.

<div class="preview">

## Globale Datensatztypen löschen

Beim Löschen globaler Datensatztypen gibt es die folgenden Szenarien:

* Wenn ein als „global“ konfigurierter Datensatztyp noch nicht zu einem anderen Arbeitsbereich hinzugefügt wurde, können Sie ihn aus dem ursprünglichen Arbeitsbereich löschen.

* Wenn ein als globaler Datensatztyp konfigurierter Datensatztyp zu mindestens einem anderen Arbeitsbereich hinzugefügt wurde, können Sie ihn nicht aus dem ursprünglichen Arbeitsbereich löschen. Zunächst müssen Sie globale Datensatztypen aus den sekundären Arbeitsbereichen, in denen sie hinzugefügt wurden, entfernen (indem Sie sie löschen). Anschließend können Sie den globalen Datensatztyp dauerhaft aus dem ursprünglichen Arbeitsbereich löschen.

### Löschen eines globalen Datensatztyps aus dem ursprünglichen Arbeitsbereich

Sie können einen Datensatztyp aus seinem ursprünglichen Arbeitsbereich löschen, wenn er nicht mehr relevant ist.

1. Zum globalen Datensatztyp in seinem ursprünglichen Arbeitsbereich gehen.

1. (Bedingt) Führen Sie einen der folgenden Schritte aus, je nachdem, ob der globale Datensatztyp zu sekundären Arbeitsbereichen hinzugefügt wurde:

   * Wenn der Datensatztyp nicht zu einem sekundären Arbeitsbereich hinzugefügt wurde, klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) auf der Karte des Datensatztyps oder rechts neben dem Namen des Datensatztyps auf seiner Seite und klicken Sie dann auf **Löschen**.
   * Wenn der Datensatztyp mindestens einem anderen sekundären Arbeitsbereich hinzugefügt wurde, wechseln Sie zunächst zum sekundären Arbeitsbereich und löschen Sie den globalen Datensatz aus diesem Bereich.

     Weitere Informationen finden Sie im Abschnitt [Löschen eines globalen Datensatztyps aus einem sekundären ](#delete-a-global-record-type-from-a-secondary-workspace)) in diesem Artikel.

1. (Bedingt) Löschen Sie den Datensatztyp weiter, wie im Abschnitt [Löschen von Datensatztypen](#delete-record-types-1) in diesem Artikel beschrieben.

   Folgendes geschieht:

   * Der globale Datensatztyp wird aus dem ursprünglichen Arbeitsbereich entfernt, und der Datensatztyp, seine Datensätze und Felder können nicht wiederhergestellt werden.
   * Alle globalen Datensatztypen aus den sekundären Arbeitsbereichen und deren Datensätze werden ebenfalls entfernt.

### Löschen eines globalen Datensatztyps aus einem sekundären Arbeitsbereich

Sie können einen Datensatztyp löschen, den Sie aus einem anderen Arbeitsbereich hinzugefügt haben, falls er nicht mehr benötigt wird.

Beachten Sie Folgendes:

* Wenn Sie einen globalen Datensatztyp aus einem sekundären Arbeitsbereich löschen, wird er nur aus dem sekundären Arbeitsbereich entfernt. Der Datensatztyp verbleibt im ursprünglichen Arbeitsbereich.

* Wenn Sie einen globalen Datensatztyp aus einem sekundären Arbeitsbereich löschen, werden auch die folgenden gelöscht:

   * Die vom sekundären Arbeitsbereich hinzugefügten Datensätze.

  <!--Coming later: * The fields added from the secondary workspace.-->

* Globale Datensatztypen, die aus ihren sekundären Arbeitsbereichen gelöscht wurden, können nicht wiederhergestellt werden.

* Der ursprüngliche Datensatztyp verbleibt sowohl im ursprünglichen Arbeitsbereich als auch in anderen Arbeitsbereichen, in denen er hinzugefügt wurde.

So löschen Sie einen globalen Datensatztyp aus einem sekundären Arbeitsbereich:

1. Wechseln Sie zum Typ Globaler Datensatz im sekundären Arbeitsbereich.

1. (Optional) Klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) auf der Karte des Datensatztyps oder rechts neben dem Namen des Datensatztyps auf seiner Seite und klicken Sie dann auf **Löschen**.
1. (Bedingt) Geben Sie **Löschen** in das bereitgestellte Feld ein und klicken Sie dann auf **Dauerhaft löschen**.

   ![Bestätigungsfeld Sekundärer globaler Datensatztyp löschen](assets/delete-secondary-global-record-type.png)

   Folgendes geschieht:

   * Der aus einem globalen Datensatztyp erstellte Datensatztyp wird aus dem ausgewählten Arbeitsbereich entfernt.
   * Der ursprüngliche Datensatztyp mit den Feldern verbleibt im ursprünglichen Arbeitsbereich.
   * Der Datensatztyp verbleibt in allen anderen Arbeitsbereichen, in denen er hinzugefügt wurde.
   * Die Datensätze, die dem Datensatztyp aus dem aktuellen Arbeitsbereich hinzugefügt <!--and fields-->, werden gelöscht. Alle anderen Datensätze, die von zusätzlichen Arbeitsbereichen hinzugefügt wurden, in denen der globale Datensatztyp hinzugefügt wurde, bleiben in ihren jeweiligen Arbeitsbereichen und im ursprünglichen Arbeitsbereich erhalten. &lt;!- Felder bleiben in den Arbeitsbereichen erhalten, in denen sie hinzugefügt wurden.

</div>
