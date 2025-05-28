---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: Platzhalterfiltervariablen
description: Durch die Verwendung von Platzhaltern in Filtern können Sie auf einen allgemeinen Benutzer oder ein Datum anstelle eines bestimmten Benutzers oder Datums verweisen. Auf diese Weise sind die von Ihnen erstellten Elemente dynamisch und die Ergebnisse ändern sich je nach dem Kontext, in dem sie verwendet werden.
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 577761ff5d1fb59db104df5995af953a0b5e6c0c
workflow-type: tm+mt
source-wordcount: '1439'
ht-degree: 1%

---

# Übersicht über Platzhalterfiltervariablen

<!-- Audited: 11/2024 -->

<!--(NOTE: This article is linked to the training self-serve promoted articles for user-based and date-based wildcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.)
(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.
This was included but it is not supported???:
The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.
For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:
AssignedToID Equals $$USER.roleIDs.)-->

Mithilfe von Platzhaltern können Sie auf einen allgemeinen Benutzer oder ein Datum anstelle eines bestimmten Benutzers oder Datums verweisen. Auf diese Weise sind die von Ihnen erstellten Elemente dynamisch. Die Ergebnisse ändern sich je nach dem Kontext, in dem sie verwendet werden.

Durch Filtern nach $$USER.homeGroupID in einem Projektbericht werden beispielsweise nur Projekte abgerufen, die der Hauptgruppe des angemeldeten Benutzers zugeordnet sind.

Beim Erstellen der folgenden Elemente können Sie Filtervariablen (auch als Platzhalter bezeichnet) verwenden:

<table>
    <tr>
        <td>Filter in Listen, Berichten und im Ressourcenplaner</td>
        <td>Informationen zu Workfront-Filtern finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">Filter - Übersicht</a>.
</td>
    </tr>
    <tr>
        <td>Erweiterte Suche</td>
        <td>Weitere Informationen zu erweiterten Suchen finden Sie im Abschnitt <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">Verwenden der erweiterten Suche</a> im Artikel <a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Adobe Workfront durchsuchen</a>.
    </tr>
    <tr>
        <td>Berechnete Spalten in Ansichten</td>
        <td></td>
    </tr>
    <tr>
        <td>Bedingte Formatierung in Ansichten</td>
        <td>Informationen zur bedingten Formatierung finden Sie im Artikel <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">Verwenden der bedingten Formatierung in Ansichten</a>.
    </tr>
    <tr>
        <td>Berechnete benutzerdefinierte Felder</td>
        <td>Platzhalterfiltervariablen werden beim Referenzieren verschachtelter Sammlungen in einer berechneten Spalte nicht unterstützt.

Informationen zu berechneten benutzerdefinierten Feldern und Spalten finden Sie im Artikel <a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">Berechnete benutzerdefinierte Felder im Vergleich zu berechneten Spalten</a>.
</td>
    </tr>
</table>

## Datumsbasierte Platzhalterfilter-Variablen

Datumsbasierte Platzhalteroptionen können in Kombination mit einem beliebigen Datumsfilterattribut verwendet werden. Informationen zum Hinzufügen eines datumsbasierten Platzhalters zu einem Bericht finden Sie im Artikel [Verwenden von datumsbasierten Platzhaltern zum Verallgemeinern von Berichten](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Wenn Sie eine Datums- und Uhrzeitberechnung erstellen, die keinen Zeitanteil enthält oder die Datums-Platzhalter $$TODAY oder $$NOW verwendet, verwendet das System das Datum in der UTC-Zone (Coordinated Universal Time) und nicht in der Zeitzone Ihrer lokalen Zeitzone. Dies kann zu einem unerwarteten Datumsergebnis führen.

Sie können aus den folgenden datumsbasierten Platzhaltern auswählen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>Es wird empfohlen, datumsabhängige Filter mit diesem Platzhalter zu erstellen, damit der Filter nicht morgen, in der nächsten Woche oder im nächsten Monat erneut erstellt wird.</p> <p>Wenn Sie beispielsweise alle vor dem heutigen Tag fälligen Aufgaben anzeigen möchten, können Sie die folgende Regel in einem Aufgabenfilter verwenden: <em>Geplantes Startdatum weniger als $$TODAY</em>.</p> <p>$$TODAY ist immer gleich Mitternacht für den aktuellen Tag.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Dies ähnelt dem $$TODAY-Platzhalter, enthält jedoch das aktuelle Datum und die aktuelle Uhrzeit. $$NOW ist gleich dem aktuellen Datum und der aktuellen Uhrzeit.</p> <p>Wenn Sie beispielsweise alle Stundeneinträge anzeigen möchten, die bis zur aktuellen Zeit bereitgestellt wurden, können Sie dies tun, indem Sie die folgende Regel in einem Stundenfilter verwenden: <em>Geplantes Startdatum weniger als $$NOW</em>.</p> <p>Hinweis: Dieser Platzhalter wird im Ressourcenplaner nicht unterstützt.</p> </td> 
  </tr> 
 </tbody> 
</table>

Um verschiedene Zeiträume und verschiedene Zeitpunkte (zukünftig oder vergangen) anzugeben, können Sie die oben genannten Platzhalter mit folgenden Elementen kombinieren:

| Attribute |   |
|---|---|
| **q** | Kalenderquartal |
| **h** | Stunde |
| **d** | Tag |
| **W** | Woche |
| **m** | Monat |
| **J** | Jahr |

{style="table-layout:auto"}

| **Kennungen** | |
|---|---|
| **b** | Beginn des Zeitraums (ohne angegebenes Attribut, standardmäßig der Beginn der Woche: Sonntag) |
| **E** | Ende des Zeitraums (ohne angegebenes Attribut, standardmäßig am Ende der Woche: Samstag) |

{style="table-layout:auto"}

| **Benutzer** | |
|---|---|
| **+** | Wert zum Platzhalterwert hinzufügen |
| **-** | Wert vom Platzhalterwert subtrahieren |

{style="table-layout:auto"}

Beispiel: Der Platzhalter `$$TODAYb+2w` bezieht sich auf „2 Wochen ab Beginn dieser Woche“. Der Platzhalter *`$$NOW+2h` bezieht sich auf „in 2 Stunden“.

## Benutzerbasierte Platzhalterfilter-Variablen

>[!IMPORTANT]
>
>Wenn ein Filter oder Bericht eine benutzerbasierte Platzhalterfiltervariable enthält, zeigen die Ergebnisse immer die Informationen an, die von dem aktuell angemeldeten Benutzer gefiltert wurden. Wenn Sie einen solchen Filter oder Bericht für einen anderen Benutzer freigeben, ruft der Platzhalter Informationen für den Benutzer ab, der den Bericht betrachtet. Die beiden Benutzer sehen unterschiedliche Ergebnisse.
>
>Informationen zum Hinzufügen eines benutzerbasierten Platzhalters zu einem Bericht finden Sie im Artikel [Verwenden von benutzerbasierten Platzhaltern zum Verallgemeinern von Berichten](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Sie können aus den folgenden benutzerbasierten Variablen auswählen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>Die häufigste benutzerbasierte Variable ist $$USER.ID. Dadurch wird immer die ID des angemeldeten Benutzers zurückgegeben. Dies ist die ID, die verwendet wird, um zu identifizieren, welcher Benutzer die einzelnen Objekte und deren Arbeitszuweisungen erstellt hat.</p> <p>Bei Verwendung in Berichten verringert dieser Platzhalter die Anzahl der Berichte, die Sie in Ihrem System erstellen müssen. Sie können einen Bericht erstellen und ihn für mehrere Benutzer freigeben. Die Ergebnisse ändern sich je nach dem Benutzer, der angemeldet ist, und sehen sich den Bericht an.</p> <p>Um beispielsweise einen Bericht für alle Probleme zu erstellen, die dem angemeldeten Benutzer zugewiesen sind, können Sie die folgende Regel in einem Problemfilter verwenden: <em>Der ID zugewiesen ist gleich $$USER.ID</em>.</p> <p>Workfront verwendet diese Variable in den folgenden integrierten Filtern:</p> 
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
   <td> <p>Die Variable $$USER.categoryID bezieht sich auf ein bestimmtes benutzerdefiniertes Formular, das mit dem angemeldeten Benutzer verknüpft ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.accessLevelID bezieht sich auf die ID der Zugriffsebene, die dem angemeldeten Benutzer zugeordnet ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>Die Variable $$USER.accessLevelRank bezieht sich auf den Zugriffsebenen-Rang, der dem angemeldeten Benutzer zugeordnet ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.companyID bezieht sich auf das Unternehmen, das dem angemeldeten Benutzer zugeordnet ist.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.customerID bezieht sich auf die ID des Kundenkontos, das mit Ihrer Umgebung verknüpft ist. In Ihrer Umgebung gibt es nur einen möglichen Wert für diese Variable und sie wird normalerweise nur beim Erstellen von Integrationen über die API verwendet.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>Die Variable $$USER.firstName verweist auf den Vornamen des angemeldeten Benutzers.</p> </td> 
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
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.homeGroupID bezieht sich auf die ID der Hauptgruppe des angemeldeten Benutzers. Als Gruppenadministrator können Sie diese Variable verwenden, um nur nach Elementen zu filtern, die zu den Benutzern in Ihrer Hauptgruppe gehören.</p> <p>Um beispielsweise alle unvollständigen Aufgaben für Projekte in der Finanzgruppe anzuzeigen, verwenden Sie die folgenden Filterregeln in einem Aufgabenfilter:<br><em>Projekt: Gruppen-ID ist gleich $$USER.homeGroupID </em><br><em>Prozent abgeschlossen weniger als 100</em></p> <p>Verwenden Sie die folgenden Filterregeln in einem Aufgabenfilter, um alle nicht abgeschlossenen Aufgaben anzuzeigen, die Einzelpersonen in einer bestimmten Gruppe zugewiesen sind, die der Hauptgruppe des angemeldeten Benutzers entspricht:</p> <p><em>Zugewiesen an: Gruppen-ID ist gleich $$USER.homeGroupID<br>Percent complete Weniger als 100</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>Die Variable $$USER.otherGroupIDs bezieht sich auf alle Gruppen (einschließlich der Hauptgruppe), die mit dem Profil des angemeldeten Benutzers verknüpft sind.</p> <p>Die Funktionalität dieser Variablen ist ähnlich wie die der Variablen $$USER.homeGroupID, mit der Ausnahme, dass in den Ergebnissen Informationen über die Benutzer angezeigt werden, die zu einer der Gruppen gehören, die mit dem angemeldeten Benutzer verknüpft sind.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.homeTeamID bezieht sich auf die ID des Home-Teams des angemeldeten Benutzers. Als Team-Manager können Sie diese Variable verwenden, um nur nach Elementen zu filtern, die zu den Benutzern in Ihrem Home-Team gehören.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>Die Variable $$USER.teamIDs gibt eine Liste aller Teams zurück, die mit dem angemeldeten Benutzer verknüpft sind.</p> <p>Die Funktionalität dieser Variablen ist ähnlich wie die der Variablen $$USER.homeTeamID, mit der Ausnahme, dass in den Ergebnissen Informationen über den Benutzer angezeigt werden, der zu einem der im Filter identifizierten Teams gehört.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>Die Variable $$USER.roleID bezieht sich auf die Primäre Rolle des angemeldeten Benutzers. Mit dieser Variablen können Sie Berichte zu Aufgaben oder Problemen erstellen, die einem bestimmten Aufgabengebiet zugewiesen sind.</p> <p>Um beispielsweise alle Aufgaben anzuzeigen, die der Primären Rolle des angemeldeten Benutzers zugewiesen sind, können Sie die folgende Filterregel in einem Aufgabenfilter verwenden:</p> <p><em>Aufgabe: Rollen-ID ist gleich $$USER.roleID.</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>Die Variable $$USER.roleIDs bezieht sich auf alle Aufgabengebiete, die mit dem angemeldeten Benutzer verknüpft sind. Mit dieser Variablen können Sie Berichte zu Aufgaben oder Problemen erstellen, die einem der Aufgabengebiete zugewiesen sind, die mit dem angemeldeten Benutzer verknüpft sind. </p> <p>Um beispielsweise alle Aufgaben anzuzeigen, die einer der Rollen zugewiesen sind, die dem angemeldeten Benutzer zugeordnet sind, können Sie die folgende Filterregel in einem Aufgabenfilter verwenden:</p> <p><i>Aufgabe: Rollen-ID ist gleich $$USERID.roleIDs<br></i> </p> <p>Tipp: <i> Filterregel (Aufgabe: Rollen-ID ist gleich $$USERID.roleIDs</i> ist in den integrierten Filtern Nicht zugewiesene Aufgaben in meiner Rolle und Nicht zugewiesene Probleme in meiner Rolle vorhanden. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Objektbasierte Platzhalterfilter-Variablen

Sie können aus den folgenden objektbasierten Platzhaltern auswählen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>Die Variable $$OBJCODE bezieht sich auf den Typ eines Objekts. </p> 
     <p>Wenn in einem benutzerdefinierten Formular die ausgewählten Objekttypen des Formulars mit einem Feld inkompatibel sind, auf das in einem berechneten benutzerdefinierten Feld verwiesen wird, können Sie diesen Platzhalter verwenden, um die Problemumgehung der Erstellung doppelter Formulare für diese Objekttypen zu vermeiden.</p> 
     <p>Im berechneten benutzerdefinierten Feld schließen Sie dazu den Platzhalter in einen IF-Ausdruck ein, damit die Berechnung für jeden Objekttyp Ihres Formulars unterschiedliche Werte ausgeben kann. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
