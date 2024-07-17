---
product-previous: workfront-goals
navigation-topic: goal-management
title: Informationen in Adobe Workfront-Zielen filtern
description: Sie können Ziele anzeigen, die Sie oder andere, die zu Adobe Workfront-Zielen hinzugefügt wurden. Informationen zum Erstellen von Zielen finden Sie unter Ziele in Adobe Workfront erstellen . Beim Anzeigen von Zielen können Sie Informationen in Workfront-Zielen filtern, um nur für Sie wichtige Ziele anzuzeigen.
author: Alina
feature: Workfront Goals
exl-id: ec9b6789-fffe-425c-8316-eefe670ad0d6
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '1382'
ht-degree: 2%

---

# Informationen in Adobe Workfront-Zielen filtern

Sie können Ziele anzeigen, die Sie oder andere, die zu Adobe Workfront-Zielen hinzugefügt wurden. Weitere Informationen zum Erstellen von Zielen finden Sie unter [Ziele in Adobe Workfront erstellen](../../workfront-goals/goal-management/create-goals.md). Beim Anzeigen von Zielen können Sie Informationen in Workfront-Zielen filtern, um nur für Sie wichtige Ziele anzuzeigen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

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
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
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

## Übersicht über Filter in Workfront-Zielen

>[!NOTE]
>
>Um die richtigen Ziele effizient zu finden und sich auf diese zu konzentrieren, empfehlen wir die Verwendung von Filtern in Workfront-Zielen. Auf diese Weise können Sie die richtigen Informationen anzeigen, bevor Sie mit der Verwaltung von für Sie wichtigen Zielen beginnen. Standardmäßig zeigt Workfront Goals alle Ziele im System an.

Sie können Ziele in den folgenden Abschnitten des Zielbereichs in Workfront suchen und filtern:

* Liste der Ziele
* Diagramme
* Ziel-Ausrichtung

Weitere Informationen zu den Abschnitten des Zielbereichs finden Sie unter [Überblick über die Adobe Workfront-Ziele](../../workfront-goals/goal-review-and-workfront-goals-sections/overview-of-wf-goals-sections.md).

>[!IMPORTANT]
>
>Sie können Filter für einen Bereich konfigurieren, die beim Wechsel zu einem anderen Bereich von Workfront-Zielen persistent bleiben.

Beachten Sie beim Arbeiten mit Filtern in Workfront-Zielen Folgendes:

* Sie können einen Filter erstellen und anwenden, ohne ihn zu speichern, oder Sie können einen Filter speichern, um ihn später wiederzuverwenden.

  Die folgenden Szenarien existieren:

   * Wenn Sie einen Filter speichern, wird er bei jeder Anmeldung bei Workfront Goals zum Standardfilter für Sie.
   * Wenn Sie einen Filter anwenden, ohne ihn zu speichern, können Sie zu den ursprünglichen Listen zurückkehren, indem Sie Ihre Seite aktualisieren.

* Sie können nur von Ihnen erstellte Filter anzeigen und anwenden. Von anderen Benutzern erstellte Filter werden nur für diese Benutzer angezeigt.
* Sie können von Ihnen erstellte Filter nicht für andere Benutzer freigeben.

## Schnellfilter in Workfront-Zielen anwenden

Sie können einen Schnellfilter in einer Liste von Zielen verwenden, um nur Elemente zu finden, die für Sie wichtig sind. Schnellfilter können nicht gespeichert werden und sind nicht persistent. Workfront löscht die Ergebnisse eines Schnellfilters beim Aktualisieren der Seite.

Weitere Informationen finden Sie unter [Anwenden des Schnellfilters auf eine Liste](../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

## Erstellen und Anwenden eines Filters in Workfront-Zielen

Die Erstellung von Filtern erfolgt für alle Bereiche von Workfront-Zielen auf die gleiche Weise.

Sie können einen Filter von Grund auf neu erstellen oder einen der integrierten Filter bearbeiten.

1. Gehen Sie zu den Workfront-Zielen.

   Informationen zum Zugriff auf Workfront-Ziele finden Sie unter [Zugreifen auf und Öffnen von Zielen in Adobe Workfront-Zielen](../../workfront-goals/goal-management/access-goals-in-wf-goals.md)

   Standardmäßig wird der Abschnitt &quot;Zielliste&quot;angezeigt.

1. Klicken Sie oben rechts in der Liste auf **Filter** .

   ![](assets/filter-icon-and-label.png)

   Standardmäßig wendet Workfront den Filter **Alle** an, der alle Ziele in Ihrem System anzeigt.

   >[!TIP]
   >
   >Der Filter Alle kann nicht bearbeitet oder gelöscht werden.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf einen der folgenden vordefinierten Filter, um Ziele nur für die folgenden Inhaber anzuzeigen:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td>Alle</td> 
        <td> <p>Alle Ziele in Ihrem System, unabhängig davon, wer sie erstellt hat, welchen Zeitraum sie haben oder wer der Eigentümer ist. Dies ist der Standardfilter und kann nicht bearbeitet werden. </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: what the ALL filter displays might change; right now, it displays all, regardless of status, period, owner, etc)</p>
         --> </td> 
       </tr> 
       <tr> 
        <td>Persönlich</td> 
        <td>Die Ziele, für die Sie der Eigentümer sind.</td> 
       </tr> 
       <tr> 
        <td>Meine Teams</td> 
        <td> <p>Die Ziele, für die eines Ihrer Teams als Eigentümer ausgewählt ist. </p> <p><b>TIPP</b>

     Es werden keine Ziele angezeigt, wenn Sie keinem Team zugewiesen sind. </p> </td>
     </tr> 
       <tr> 
        <td>Meine Gruppen</td> 
        <td>Die Ziele, für die eine Ihrer Gruppen als Inhaber ausgewählt wird. </td> 
       </tr> 
       <tr> 
        <td>Firma</td> 
        <td> <p>Die mit Ihrer Organisation verknüpften Ziele. </p> <p><b>TIP</b>
        <p>Unter Adobe Workfront-Ziele zeigt der Filter Unternehmen die Ziele an, für die Ihr Unternehmen als Inhaber ausgewählt wurde. </p> <p>Sie können nicht nach Unternehmen suchen, die dieses Feld verwenden. Standardmäßig wird nur Ihr Unternehmen ausgewählt, das Eigentümer Ihrer Workfront-Instanz ist. </p> </p> </td> 
       </tr> 
      </tbody> 
     </table>

   * Bewegen Sie den Mauszeiger über den Namen eines Filters und klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) neben seinem Namen, um ihn anzupassen und spezifische Namen von Benutzern, Teams, Gruppen oder dem Namen Ihrer Organisation hinzuzufügen. Wählen Sie dann den Filter aus, wenn er in der Liste angezeigt wird.

   * Klicken Sie auf **Neuer Filter** , um einen neuen Filter zu erstellen, und wählen Sie dann aus den folgenden Optionen aus, um den neuen Filter anzupassen:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Zeitraum</td> 
        <td>Wählen Sie im Dropdown-Menü einen Zeitraum aus. Sie können mehrere Zeiträume auswählen. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Status</td> 
        <td> <p>Wählen Sie aus den folgenden Optionen einen Status im Dropdown-Menü aus:</p> 
         <ul> 
          <li> <p>Aktiv</p> </li> 
          <li> <p>Entwurf</p> </li> 
          <li> <p>Inaktiv</p> </li> 
          <li> <p>Geschlossen</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Fortschritt</td> 
        <td> <p>Wählen Sie aus den folgenden Optionen einen Fortschritt im Dropdown-Menü aus: </p> 
         <ul> 
          <li> <p>In Schwierigkeiten</p> </li> 
          <li> <p>Gefährdet</p> </li> 
          <li> <p>Im Zielbereich</p> </li> 
         </ul> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Besitzerin bzw. Besitzer</td> 
        <td> <p>Geben Sie den Namen des Eigentümers ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird. </p> <p>Sie können die Namen von Benutzern, Teams, Gruppen oder den Namen Ihrer Organisation eingeben oder aus vordefinierten Optionen auswählen. </p> <p>Die folgenden vordefinierten Filteroptionen beziehen sich immer auf den Benutzer, der derzeit angemeldet ist: </p> 
         <ul> 
          <li> <p><strong>Me</strong>: Zeigt Ziele an, deren Inhaber Sie sind.</p> </li> 
          <li> <p><strong>My Home Team</strong> und <strong>All My Teams</strong>: Zeigt Ziele an, bei denen entweder Ihr Home Team oder eines Ihrer Teams als Eigentümer benannt sind. </p> <p>Tipp: Es werden keine Ziele angezeigt, wenn Sie keinem Team zugewiesen sind. </p> </li> 
          <li> <p><strong>Meine Heimatgruppe</strong> und <strong>Alle meine Gruppen</strong>: Zeigt Ziele an, bei denen entweder Ihre Home-Gruppe oder eine Ihrer Gruppen als Inhaber ausgewiesen ist.</p> </li> 
         </ul> </td> 
       </tr> 
      </tbody> 
     </table>

1. (Optional) Klicken Sie in der rechten unteren Ecke des Filterfelds auf **Zurücksetzen** , um alle ausgewählten Felder zu löschen und mit der Erstellung des Filters zu beginnen.
1. (Optional) Klicken Sie auf **Anwenden** , um den Filter ohne Speichern anzuwenden.

   Der Filter wird im Bereich **Nicht gespeichert** des Filter-Builders als **Neuer Filter** angezeigt.

   Sie können einen nicht gespeicherten Filter nicht umbenennen.

   Nicht gespeicherte Filter werden beim nächsten Abmelden von Workfront und erneuten Anmelden aus dem Zielbereich entfernt.

   >[!TIP]
   >
   >Sie können immer nur einen nicht gespeicherten neuen Filter gleichzeitig haben.

1. Klicken Sie auf **Speichern** , um den Filter zu speichern und später zu verwenden. Fügen Sie dann einen Namen für den Filter in das Feld **Filtername hinzufügen** ein und klicken Sie auf **Fertig**.

   Dadurch wird der Filter im Abschnitt **gespeichert** des Filter-Builders gespeichert. Sie können diesen Filter in Zukunft verwenden.

   Der zuletzt gespeicherte und angewendete Filter wird standardmäßig beim nächsten erneuten Anmelden bei Workfront angezeigt.

1. (Optional) Klicken Sie auf den Pfeil **links neben** **Neuer Filter** , um den Filter-Builder zu verlassen und zur Liste der Filter zurückzukehren.
1. (Optional) Bewegen Sie den Mauszeiger über den Namen eines benutzerdefinierten Filters, klicken Sie auf das Menü **Mehr** und dann auf **Löschen** und dann auf **Löschen**. Dadurch wird der Filter gelöscht und kann nicht wiederhergestellt werden.

   >[!TIP]
   >
   >Die vordefinierten Filter können nicht gelöscht werden.

1. Klicken Sie oben rechts im Filtergenerator auf das Symbol **X** , um den Filtergenerator zu schließen.

   Der Name des aktuell angewendeten Filters wird rechts neben dem Symbol Filter in der oberen rechten Ecke der Zielliste angezeigt.

   Die Liste der Ziele wird nach Ihren Filterkriterien gefiltert.

1. (Optional und bedingt) Klicken Sie beim Anzeigen von Zielen im Abschnitt &quot;Zielausrichtung&quot;auf **Anzeigen** , wenn Sie die gefilterten Ziele anzeigen möchten.

   ![](assets/show-them-link-on-filtered-items-goal-list-350x109.png)

   Der Filtername ist gelb umrandet, um anzugeben, dass er ignoriert wird.

   ![](assets/filter-yellow-outline-next-to-reapply-filter-link-350x118.png)


1. (Optional und bedingt) Klicken Sie auf **Filter erneut anwenden** , um den Filter anzuwenden und die im vorherigen Schritt angezeigten Elemente wegzulassen.


