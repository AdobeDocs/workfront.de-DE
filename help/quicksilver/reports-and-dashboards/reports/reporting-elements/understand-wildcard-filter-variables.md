---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Platzhalterfiltervariablen
description: Durch die Verwendung von Platzhaltern in Filtern können Sie auf einen generischen Benutzer oder ein generisches Datum statt auf einen bestimmten Benutzer oder ein bestimmtes Datum verweisen. Auf diese Weise sind die von Ihnen erstellten Elemente dynamisch und die Ergebnisse ändern sich je nach Kontext, in dem sie verwendet werden.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: d6094d944b7955db8a97b5e1ce0af8cb85f82a9e
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 1%

---

# Übersicht über Wildcard-Filtervariablen

<!-- Audited: 12/2023 -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

Mithilfe von Platzhaltern können Sie auf einen generischen Benutzer oder ein generisches Datum statt auf einen bestimmten Benutzer oder ein bestimmtes Datum verweisen. Auf diese Weise sind die von Ihnen erstellten Elemente dynamisch. Die Ergebnisse ändern sich je nach Kontext, in dem sie verwendet werden.

Wenn Sie beispielsweise in einem Projektbericht nach $$USER.homeGroupID filtern, werden nur Projekte abgerufen, die mit der Home Group des angemeldeten Benutzers verknüpft sind.

Sie können beim Erstellen der folgenden Elemente Filtervariablen verwenden, die auch als Platzhalter bezeichnet werden:

<table>
    <tr>
        <td>Filter in Listen, Berichten und im Ressourcenplaner</td>
        <td>Weitere Informationen zu Workfront-Filtern finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">Filterübersicht</a>.
</td>
    </tr>
    <tr>
        <td>Erweiterte Suchvorgänge</td>
        <td>Informationen zu erweiterten Suchen finden Sie im Abschnitt <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">Erweiterte Suche verwenden</a> im Artikel <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Adobe Workfront durchsuchen</a>.
    </tr>
    <tr>
        <td>Berechnete Spalten in Ansichten</td>
        <td></td>
    </tr>
    <tr>
        <td>Bedingte Formatierung in Ansichten</td>
        <td>Weitere Informationen zur bedingten Formatierung finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">Bedingte Formatierung in Ansichten verwenden</a>.
    </tr>
    <tr>
        <td>Berechnete benutzerdefinierte Felder</td>
        <td>Platzhalterfiltervariablen werden nicht unterstützt, wenn in einer berechneten Spalte auf verschachtelte Sammlungen verwiesen wird.

Informationen zu berechneten benutzerdefinierten Feldern und Spalten finden Sie im Artikel <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">Berechnete benutzerdefinierte Felder vs. berechnete Spalten</a>.
</td>
    </tr>
</table>

## Datumsbasierte Platzhalterfiltervariablen

Datumsbasierte Platzhalteroptionen können in Kombination mit einem beliebigen Datumsfilterattribut verwendet werden. Informationen zum Hinzufügen eines datumsbasierten Platzhalters zu einem Bericht finden Sie im Artikel [Verwenden datumsbasierter Platzhalter zum Generalisieren von Berichten ](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Wenn Sie eine Datums- und Uhrzeitberechnung erstellen, die keinen Zeitabschnitt enthält oder die Datumsfelder $$TODAY oder $$NOW verwendet, verwendet das System das Datum gemäß der UTC-Zone (Coordinated Universal Time), nicht gemäß Ihrer lokalen Zeitzone. Dies kann zu einem unerwarteten Datumsergebnis führen.

Sie können aus den folgenden datumsbasierten Platzhaltern wählen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$HEUTE</strong> </p> </td> 
   <td> <p>Es wird empfohlen, mit diesem Platzhalter datumssensitive Filter zu erstellen, damit Sie den Filter nicht morgen, nächste Woche oder nächsten Monat erneut erstellen.</p> <p>Wenn Sie beispielsweise alle Aufgaben anzeigen möchten, die vor heute anstehen, können Sie die folgende Regel in einem Aufgabenfilter verwenden: <em>Vorgesehenes Startdatum unter $$TODAY</em>.</p> <p>$$TODAY ist für den aktuellen Tag immer gleich Mitternacht.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Dies ähnelt dem Platzhalter $$TODAY , enthält jedoch das aktuelle Datum und die aktuelle Uhrzeit. $$NOW entspricht dem aktuellen Datum und der aktuellen Uhrzeit.</p> <p>Wenn Sie beispielsweise alle bis zur aktuellen Zeit bereitgestellten Stundeneinträge anzeigen möchten, können Sie dies mithilfe der folgenden Regel in einem Stundenfilter tun: <em>Geplantes Startdatum unter $$NOW</em>.</p> <p>Hinweis: Dieser Platzhalter wird im Ressourcen-Planer nicht unterstützt.</p> </td> 
  </tr> 
 </tbody> 
</table>

Um verschiedene Zeiträume und verschiedene Zeitpunkte (zukünftig oder früher) anzugeben, können Sie die obigen Platzhalter mit den folgenden kombinieren:

| Attribute |   |
|---|---|
| **q** | Kalenderquartal |
| **h** | Stunde |
| **d** | Tag |
| **w** | Woche |
| **m** | Monat |
| **y** | Jahr |

{style="table-layout:auto"}

| **Qualifikatoren** | |
|---|---|
| **b** | Beginn des Zeitraums (ohne angegebenes Attribut, standardmäßig der Anfang der Woche: Sonntag) |
| **e** | Ende des Zeitraums (ohne angegebenes Attribut wird standardmäßig das Ende der Woche festgelegt: Samstag) |

{style="table-layout:auto"}

| **Operatoren** | |
|---|---|
| **+** | Wert zum Platzhalterwert hinzufügen |
| **-** | Wert vom Platzhalterwert subtrahieren |

{style="table-layout:auto"}

Der Platzhalter `$$TODAYb+2w` verweist beispielsweise auf &quot;2 Wochen ab Beginn dieser Woche&quot;. Der Platzhalter *`$$NOW+2h` bezieht sich auf &quot;In zwei Stunden.&quot;

## Benutzerbasierte Platzhalterfiltervariablen

>[!IMPORTANT]
>
>Wenn ein Filter oder Bericht eine benutzerbasierte Platzhalterfiltervariable enthält, werden in den Ergebnissen immer Informationen angezeigt, die von dem Benutzer gefiltert wurden, der aktuell angemeldet ist. Wenn Sie einen solchen Filter oder Bericht für einen anderen Benutzer freigeben, ruft der Platzhalter Informationen für den Benutzer ab, der den Bericht betrachtet. Die beiden Benutzer sehen unterschiedliche Ergebnisse.
>
>Informationen zum Hinzufügen eines benutzerbasierten Platzhalters zu einem Bericht finden Sie im Artikel [Verwenden benutzerbasierter Platzhalterzeichen zum Generalisieren von Berichten ](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Sie können aus den folgenden benutzerbasierten Variablen auswählen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>Die häufigste benutzerbasierte Variable ist $$USER.ID. Dadurch wird immer die ID des angemeldeten Benutzers zurückgegeben. Dies ist die ID, mit der festgestellt wird, welcher Benutzer die einzelnen Objekte und deren Arbeitszuweisungen erstellt hat.</p> <p>Bei Verwendung in Berichten verringert dieser Platzhalter die Anzahl der Berichte, die Sie in Ihrem System erstellen müssen. Sie können einen Bericht erstellen und ihn für mehrere Benutzer freigeben. Die Ergebnisse ändern sich je nach dem Benutzer, der angemeldet ist und sich den Bericht ansieht.</p> <p>Um beispielsweise einen Bericht für alle Probleme zu erstellen, die dem angemeldeten Benutzer zugewiesen sind, können Sie die folgende Regel in einem Problemfilter verwenden: <em>Zugeordneter an ID entspricht $$USER.ID</em>.</p> <p>Workfront verwendet diese Variable in den folgenden integrierten Filtern:</p> 
    <ul> 
     <li>Meine Berichte</li> 
     <li>Meine Projekte</li> 
     <li>Meine Aufgaben</li> 
     <li>Meine Probleme</li> 
     <li>Meine Stunden</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.categoryID bezieht sich auf ein bestimmtes benutzerdefiniertes Formular, das dem angemeldeten Benutzer zugeordnet ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.accessLevelID bezieht sich auf die ID der Zugriffsstufe, die dem angemeldeten Benutzer zugeordnet ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>Die Variable $$USER.accessLevelRank bezieht sich auf den Rang der Zugriffsstufe, der dem angemeldeten Benutzer zugeordnet ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.companyID bezieht sich auf das Unternehmen, das dem angemeldeten Benutzer zugeordnet ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.customerID bezieht sich auf die ID des Kundenkontos, das mit Ihrer Umgebung verknüpft ist. Für Ihre Umgebung gibt es nur einen möglichen Wert für diese Variable. Dieser Wert wird normalerweise nur beim Erstellen von Integrationen über die API verwendet.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>Die Variable $$USER.firstName bezieht sich auf den Vornamen des angemeldeten Benutzers.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>Die Variable $$USER.lastName bezieht sich auf den Nachnamen des angemeldeten Benutzers.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>Die Variable $$USER.name bezieht sich auf den vollständigen Namen des angemeldeten Benutzers.</p> <p>Hinweis:   <p>Diese Platzhaltervariable funktioniert nur, wenn ein Filter im Textmodus geändert wird. Sie können diesen Platzhalter nicht in Filtern verwenden, die den Textmodus nicht unterstützen. Sie können diesen Platzhalter beispielsweise nicht in den Filtern in den folgenden Bereichen verwenden:</p> 
     <ul> 
      <li> <p>Ressourcenplaner</p> </li> 
      <li> <p>Workload Balancer</p> </li> 
      <li> <p>Analytik</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.homeGroupID bezieht sich auf die Kennung der Home Group des angemeldeten Benutzers. Als Gruppenadministrator können Sie diese Variable verwenden, um nur Elemente zu filtern, die zu den Benutzern in Ihrer Startseite gehören.</p> <p>Um beispielsweise alle unvollständigen Aufgaben für Projekte in der Finanzgruppe anzuzeigen, verwenden Sie die folgenden Filterregeln in einem Aufgabenfilter:<br><em>Projekt: Gruppen-ID entspricht $$USER.homeGroupID </em><br><em>Prozent abgeschlossen Kleiner als 100</em></p> <p>Verwenden Sie die folgenden Filterregeln in einem Aufgabenfilter, um alle unvollständigen Aufgaben anzuzeigen, die Einzelanwendern in einer bestimmten Gruppe, der Home Group des angemeldeten Benutzers, zugewiesen sind:</p> <p><em>Zugeordnet zu: Gruppen-ID entspricht $$USER.homeGroupID<br>Prozent abgeschlossen unter 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>Die Variable $$USER.otherGroupIDs bezieht sich auf alle Gruppen (einschließlich der Home Group), die mit dem Profil des angemeldeten Benutzers verknüpft sind.</p> <p>Die Funktionalität dieser Variablen ähnelt der der Variablen $$USER.homeGroupID , allerdings zeigen die Ergebnisse Informationen zu den Benutzern an, die zu einer der Gruppen gehören, die mit dem angemeldeten Benutzer verknüpft sind.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.homeTeamID bezieht sich auf die Kennung des Home-Teams des angemeldeten Benutzers. Als Teammanager können Sie diese Variable verwenden, um nur Elemente zu filtern, die zu den Benutzern in Ihrem Home Team gehören.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>Die Variable $$USER.teamIDs gibt eine Liste aller Teams zurück, die mit dem angemeldeten Benutzer verknüpft sind.</p> <p>Die Funktionalität dieser Variablen ähnelt der der Variablen $$USER.homeTeamID, allerdings zeigen die Ergebnisse Informationen über den Benutzer an, der zu einem der im Filter identifizierten Teams gehört.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.roleID bezieht sich auf die Primäre Rolle des angemeldeten Benutzers. Mithilfe dieser Variablen können Sie Berichte zu Aufgaben oder Problemen erstellen, die einer bestimmten Auftragsrolle zugewiesen sind.</p> <p>Um beispielsweise alle Aufgaben anzuzeigen, die der Primären Rolle des angemeldeten Benutzers zugewiesen sind, können Sie die folgende Filterregel in einem Aufgabenfilter verwenden:</p> <p><em>Aufgabe: Rolle-ID entspricht $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>Die Variable $$USER.roleIDs bezieht sich auf alle mit dem angemeldeten Benutzer verknüpften Vorgangsrollen. Mithilfe dieser Variablen können Sie Berichte zu Aufgaben oder Problemen erstellen, die einer der mit dem angemeldeten Benutzer verknüpften Vorgangsrollen zugewiesen sind. </p> <p>Um beispielsweise alle Aufgaben anzuzeigen, die einer der Rollen zugewiesen sind, die dem angemeldeten Benutzer zugeordnet sind, können Sie die folgende Filterregel in einem Aufgabenfilter verwenden:</p> <p><i>Aufgabe: Rolle-ID entspricht $$USERID.roleIDs<br></i> </p> <p>Tipp: Die Filterregel <i>Aufgabe: Rolle-ID gleich $$USERID.roleIDs</i> ist in den integrierten Filtern Nicht zugewiesene Aufgaben in meiner Rolle und Nicht zugewiesene Probleme in meiner Rolle vorhanden. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Objektbasierte Platzhalterfiltervariablen

Sie können aus den folgenden objektbasierten Platzhaltern wählen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>Die Variable $$OBJCODE bezieht sich auf den Typ eines Objekts. </p> 
     <p>Wenn in einem benutzerdefinierten Formular die ausgewählten Objekttypen des Formulars nicht mit einem Feld kompatibel sind, auf das in einem berechneten benutzerdefinierten Feld verwiesen wird, können Sie diesen Platzhalter verwenden, um zu vermeiden, dass für diese Objekttypen doppelte Formulare erstellt werden.</p> 
     <p>Im berechneten benutzerdefinierten Feld schließen Sie dazu den Platzhalter in einen IF-Ausdruck ein, damit die Berechnung für die Objekttypen Ihres Formulars unterschiedliche Werte ausgeben kann. </p> 
     <p>Weitere Informationen und ein Beispiel finden Sie im Abschnitt <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">Berechnete benutzerdefinierte Felder in benutzerdefinierten Formularen mit mehreren Objekten</a> im Artikel <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Berechnete Daten zu einem benutzerdefinierten Formular hinzufügen</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
