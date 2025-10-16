---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Erstellen eines benutzerdefinierten Berichts
description: Sie können durch die Erstellung von Berichten Zugriff auf die Informationen gewähren, die Ihr Unternehmen in Adobe Workfront benötigt. Sie können jeden der in Workfront verfügbaren integrierten Berichte verwenden oder Ihre benutzerdefinierten Berichte von Grund auf neu erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 10c4df37-f09f-4b91-9cfd-3d0c3835bc7b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1816'
ht-degree: 1%

---


# Erstellen eines benutzerdefinierten Berichts

<!--Audited: 10/2024-->

Sie können durch die Erstellung von Berichten Zugriff auf die Informationen gewähren, die Ihr Unternehmen in Adobe Workfront benötigt. Sie können jeden der in Workfront verfügbaren integrierten Berichte verwenden oder Ihre benutzerdefinierten Berichte von Grund auf neu erstellen.

Weitere Informationen zu integrierten Berichten finden Sie unter [Verwenden von integrierten Adobe Workfront-Berichten](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md).

Informationen zum Erstellen eines Berichts durch Kopieren finden Sie unter [Erstellen einer Berichtskopie](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

Weitere Informationen zum Erstellen und Verwalten von Berichten, einschließlich Klassen, Videos und Tutorials, finden Sie im Abschnitt „Lernen“ auf der Adobe Experience League-Website.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Sie erhalten Verwaltungsberechtigungen für die von Ihnen erstellten Berichte</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Berichts {#create-a-report}

{{step1-to-reports}}

1. Klicken Sie **Neuer Bericht** und wählen Sie dann den Objekttyp aus, den Sie für den Bericht benötigen.

   Report Builder wird geladen.

   Spezifische Informationen zu verfügbaren Objektberichten finden Sie im Abschnitt [Berichte zu Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) im Artikel &quot;[&#x200B; von Objekten in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

   ![Neuen Bericht auswählen](assets/nwe-select-new-report-350x666.png)

   >[!TIP]
   >
   >Sie können auch einen Bericht erstellen, indem Sie eine Kopie eines vorhandenen Berichts erstellen. Weitere Informationen finden Sie unter [Erstellen einer Berichtskopie](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. (Optional) Um den Titel Ihres neuen Berichts zu bearbeiten, geben Sie den gewünschten Berichtstitel in das Textfeld oben links im Report Builder ein. Es wird empfohlen, nur UTF-8-Zeichen zu verwenden, um Kompatibilitätsprobleme zu vermeiden.

1. Fügen Sie in Report Builder Folgendes zu Ihrem Bericht hinzu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Funktion</th> 
      <th>Beschreibung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>Spalten (Ansicht)</td> 
      <td> <p>Durch das Hinzufügen von Spalten zu Ihrem Bericht wird bestimmt, welche Informationen Ihr Bericht enthält.</p> <p>Informationen zum Hinzufügen einer Spalte finden Sie unter <a href="#add-columns-view-to-a-report" class="MCXref xref">Hinzufügen von Spalten (Ansicht) zu einem Bericht</a>.<br></p> </td> 
     </tr> 
     <tr> 
      <td>Gruppierungen</td> 
      <td> <p>Durch das Hinzufügen von Gruppierungen zu Ihrem Bericht wird festgelegt, wie Ihr Bericht organisiert ist.</p> <p>Informationen zum Hinzufügen einer Gruppierung finden Sie unter <a href="#add-groupings-to-a-report" class="MCXref xref">Hinzufügen von Gruppierungen zu einem Bericht</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Filter</td> 
      <td> <p>Durch das Hinzufügen von Filterregeln zu Ihrem Bericht werden die Informationen bestimmt, die Sie in Ihrem Bericht sehen.</p> <p>Informationen zum Hinzufügen eines Filters finden Sie unter <a href="#add-filters-to-a-report" class="MCXref xref">Hinzufügen von Filtern zu einem Bericht</a>.</p> </td> 
     </tr> 
     <tr> 
      <td>Diagramm</td> 
      <td> <p>Durch das Hinzufügen eines Diagramms zu Ihrem Bericht wird festgelegt, wie die Informationen in Ihrem Bericht visuell dargestellt werden.</p> <p>Informationen zum Hinzufügen eines Diagramms finden Sie unter <a href="#add-a-chart-to-a-report" class="MCXref xref">Hinzufügen eines Diagramms zu einem Bericht</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie während der Berichterstellung jederzeit auf &quot;**&quot;,** Ihre Änderungen zu speichern.
1. Wenn Sie fertig sind, klicken Sie auf **Speichern + Schließen**.

### Spalten (Ansicht) zu einem Bericht hinzufügen {#add-columns-view-to-a-report}

1. Beginnen Sie mit der Erstellung eines Berichts, wie [&#x200B; Abschnitt „Erstellen eines &#x200B;](#create-a-report)&quot; in diesem Artikel beschrieben.
1. Wählen Sie in Report Builder die Registerkarte **Spalten (Ansicht)**, um die Spalten zu identifizieren, die im Bericht angezeigt werden sollen.
1. (Optional) Klicken Sie **Vorhandene Ansicht anwenden** und klicken Sie im Dropdown-Menü auf den Namen einer Ansicht, um eine vorhandene Ansicht zu verwenden.

   Weitere Informationen zum Erstellen einer Ansicht finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Optional) Um eine vorhandene Spalte zu entfernen, klicken Sie auf die Spalte, die Sie entfernen möchten, und klicken Sie dann auf **x** neben dem aktuellen Namen in der Spaltenüberschrift.

1. Um eine neue Spalte hinzuzufügen, klicken Sie auf **Spalte hinzufügen**.

   Oder

   Um eine vorhandene Spalte zu ändern, klicken Sie auf die Spalte, klicken Sie auf das **Entfernen**-Symbol ![Entfernen-Symbol](assets/remove-column-icon.png) rechts neben dem aktuellen Feld im Bereich **In diesem Spaltenfeld** anzeigen) in der linken oberen Ecke von Report Builder, und beginnen Sie mit der Eingabe eines neuen Felds. Klicken Sie dann auf das Feld, wenn es in der Liste angezeigt wird.

   Weitere Informationen zu den Feldern, die Sie in den Spalten sehen, finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

   ![Spaltentypvervollständigung hinzufügen](assets/nwe-add-column-typeahead-350x459.png)

1. (Optional) Klicken Sie im Bereich **Spalteneinstellungen** auf **Sortieren nach dieser Spalte**, um die Werte in der Spalte entweder in aufsteigender oder in absteigender alphabetischer Reihenfolge zu sortieren. Geben Sie dann an, ob die Liste diese Spalte als erste Sortierung verwenden soll.

   Sie können in einer Berichtsansicht mehrere Sortierebenen haben, wenn Sie nach dem Wert in einer ersten Spalte, dem Wert in einer zweiten Spalte usw. sortieren möchten.

   Wenn mehrere Ergebnisse nach den ersten Sortierkriterien identisch sind, werden sie in der Reihenfolge der zweiten Sortierkriterien sortiert. Wenn mehrere Ergebnisse nach dem ersten und zweiten Sortierkriterium identisch sind, werden sie nach dem dritten Sortierkriterium sortiert usw.

   >[!NOTE]
   >
   >Wenn Sie ein Feld hinzufügen, das auf ein Objekt verweist, das zu weit von dem Objekt entfernt ist, über das Sie Bericht erstatten, können Sie möglicherweise nicht nach diesem Feld sortieren.\
   >Beispielsweise kann ein Problembericht nicht nach dem Feld „Projektbesitzer“ sortiert werden, da er auf drei zusätzliche Objekte verweist: „Projekt“, „Eigentümer“ und „Name“. Sie können dieses Feld jedoch weiterhin zu einem Problembericht hinzufügen und die entsprechenden Informationen anzeigen.

   <!--outdated: To learn more about cross-object references in reports, see the section "Advanced Reporting Part 1 of 3" in the [Reports and Dashboards Learning Path](https://one.workfront.com/s/learningpath2/workfront-reporting-MC7MZT2BOL2ZC2LMJ4MA3EMHOCNY?tabset-dc70e=2).-->

1. (Optional) Wenn Sie Gruppierungen verwenden und die Informationen in einer Spalte zusammenfassen (aggregieren) möchten, klicken Sie auf die Dropdown-Liste **Diese Spalte zusammenfassen nach** im Bereich **Spalteneinstellungen** und wählen Sie dann die Option aus, die Sie zum Aggregieren der Informationen in der Spalte verwenden möchten.

   Die aggregierten Informationen werden in der Spalte in den Gruppierungszeilen angezeigt.

   ![Aggregierte Zusammenfassung zu Gruppierungen](assets/aggregate-summary-displays-on-groupings-2022-350x195.png)

   Weitere Informationen zum Zusammenfassen von Daten in einer Spalte finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

   >[!NOTE]
   >
   >Die folgenden Ausnahmen gelten für übergeordnete Objekte (z. B. übergeordnete Aufgaben), wenn Sie Werte für die folgenden Felder in Gruppierungen aggregieren:
   >
   >* Alle Zahlen- und Währungsfelder mit Ausnahme der tatsächlichen Stunden (z. B. geplante oder Ist-Lohnkosten, geplante oder Ist-Ausgaben-Kosten, geplante oder Ist-Kosten, geplante Stunden) aggregieren nur die Werte für untergeordnete Aufgaben und eigenständige Aufgaben. Sie aggregieren nicht die Werte für die übergeordneten Aufgaben oder die übergeordneten Aufgaben.
   >* Tatsächliche Stunden aggregieren die Werte für die übergeordnete Hauptaufgabe und die eigenständigen Aufgaben. Sie aggregieren nicht die Zahlen für die übergeordneten Aufgaben oder die untergeordneten Aufgaben.
   >* Benutzerdefinierte Datenfelder für Zahlen- und Währungswerte aggregieren alle Aufgaben: Eltern, Kinder, Eltern von Eltern und eigenständige Aufgaben.

   Weitere Informationen zur Verwendung von Gruppierungen in einem Bericht finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Optional) Klicken Sie auf **Erweiterte Optionen**, um die folgenden Informationen für die Spalte anzugeben:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Benutzerdefiniertes Spalten-Label</td> 
      <td> <p>Geben Sie eine benutzerdefinierte Beschriftung für die Spalte an. Diese Beschriftung ersetzt die Standardbeschriftung.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Feldformat</td> 
      <td> <p>Wählen Sie das Format aus, in dem die Werte für Felder in der Spalte angezeigt werden sollen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diese Spalte im Dashboard anzeigen</td> 
      <td> <p>Wählen Sie diese Option aus, um diese Spalte auf einem Dashboard anzuzeigen, wenn der Bericht Seite an Seite mit einem anderen Bericht angezeigt wird. Wenn diese Option deaktiviert ist, wird diese Spalte nicht angezeigt, wenn der Bericht in einem Dashboard angezeigt wird, in dem Berichte nebeneinander angezeigt werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Spaltenregeln</td> 
      <td> <p>Klicken Sie <strong>Regel für diese Spalte hinzufügen</strong>, um der Spalte eine bedingte Formatierung hinzuzufügen. Nachdem Sie eine Regel hinzugefügt haben, können Sie Feld- und Textstile dafür definieren, wie Felder, die dieser Regel entsprechen, angezeigt werden. Klicken Sie <strong>Regel hinzufügen</strong> nachdem Sie die Definition der Regel abgeschlossen haben. Weitere Informationen zur bedingten Formatierung in einer Ansicht finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md" class="MCXref xref">Verwenden der bedingten Formatierung in Ansichten</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Übernehmen**, um Ihre bisherigen Änderungen anzuwenden und den Bericht mit den folgenden Optionen weiter zu bearbeiten.

   Klicken Sie **Speichern + Schließen** wenn Sie mit der Bearbeitung der Spalten im Bericht fertig sind und den Bericht speichern möchten.

### Gruppierungen zu einem Bericht hinzufügen {#add-groupings-to-a-report}

1. Beginnen Sie mit der Erstellung eines Berichts, wie [&#x200B; Abschnitt „Erstellen eines &#x200B;](#create-a-report)&quot; in diesem Artikel beschrieben.
1. Wählen Sie in Report Builder die Registerkarte **Gruppierungen**, um festzulegen, wie Sie Elemente im Bericht gruppieren möchten.
1. Klicken Sie **Gruppierung hinzufügen**, um eine neue Gruppierung hinzuzufügen.

   Oder

   Wählen Sie **Vorhandene Gruppierung anwenden**, um eine vorhandene Gruppierung auszuwählen, wenn sie in der Liste angezeigt wird.

   ![Gruppierung hinzufügen](assets/nwe-add-grouping-350x230.png)

1. Beginnen Sie, das Feld einzugeben, das Sie als Gruppierung hinzufügen möchten. Wenn das Feld verfügbar ist, wird es für jedes Objekt ausgefüllt, mit dem es verknüpft werden kann. Klicken Sie auf den Namen des Felds, um es dieser Gruppierung hinzuzufügen.
1. (Optional) Sie können eine Gruppierung im Textmodus erstellen, indem Sie auf **In Textmodus wechseln** klicken. Weitere Informationen zum Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Weitere Informationen zum Erstellen neuer Gruppierungen finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. (Optional) Wählen Sie **Diese Gruppierung standardmäßig reduzieren** aus, wenn die Ergebnisse in dieser Gruppierung reduziert anstatt erweitert angezeigt werden sollen.

   Diese Einstellung ist standardmäßig deaktiviert und die Gruppierungsergebnisse werden immer in einer erweiterten Liste angezeigt.

   >[!TIP]
   >
   >* Wenn Sie beim Anzeigen einer Liste Gruppierungen manuell anpassen, speichert Workfront Ihre manuellen Einstellungen, bis Sie sich abmelden. Beim erneuten Anmelden wird die Liste entsprechend dieser Einstellung angezeigt.
   >* Die Ergebnisse einer Gruppierung werden immer erweitert angezeigt, nachdem über ein Diagrammelement darauf zugegriffen wurde.

1. (Optional) Klicken Sie auf **Zu Matrix-Gruppierung wechseln**, um eine Matrix-Gruppierung zu erstellen und Ihre Ergebnisse in einem Rasterformat anzuzeigen.

   Weitere Informationen zum Erstellen eines Matrixberichts finden Sie unter [Erstellen eines Matrixberichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

1. Klicken Sie **Übernehmen**, um Ihre bisherigen Änderungen anzuwenden und den Bericht mit den folgenden Optionen weiter zu bearbeiten.

   Klicken Sie **Speichern + Schließen** wenn Sie mit dem Bearbeiten der Gruppierungen im Bericht fertig sind und den Bericht speichern möchten.

### Hinzufügen von Filtern zu einem Bericht {#add-filters-to-a-report}

1. Beginnen Sie mit der Erstellung eines Berichts, wie [&#x200B; Abschnitt „Erstellen eines &#x200B;](#create-a-report)&quot; in diesem Artikel beschrieben.
1. Wählen Sie in Report Builder die Registerkarte **Filter**, um die Menge an Informationen anzugeben, die der Bericht enthalten soll.
1. Klicken Sie **Filterregel hinzufügen**, um einen benutzerdefinierten Filter hinzuzufügen.\
   Oder\
   Wählen **Vorhandenen Filter anwenden**, um einen vorhandenen Filter zu verwenden.

   ![Filter hinzufügen](assets/nwe-add-a-filter-350x93.png)

1. Wenn Sie auf **Filterregel hinzufügen** geklickt haben, geben Sie das Feld ein, das Sie als Filter hinzufügen möchten. Wenn das Feld verfügbar ist, wird es für jedes Objekt ausgefüllt, mit dem es verknüpft werden kann. Klicken Sie auf den Namen des Felds, um es diesem Filter hinzuzufügen.\
   Verwenden Sie Filtermodifikatoren, um Ihren Filter zu erstellen. Weitere Informationen zu Filtermodifikatoren finden Sie unter [Filter- und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   Weitere Informationen zum Erstellen neuer Filter finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. (Optional) Sie können einen Filter im Textmodus erstellen, indem Sie auf **In Textmodus wechseln** klicken.

   Weitere Informationen zum Textmodus finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

1. Klicken Sie **Anwenden** wenn Sie mit der Bearbeitung der Filter im Bericht fertig sind, um Ihre bisherigen Änderungen anzuwenden und mit der Bearbeitung des Berichts mit den folgenden Optionen fortzufahren.

   Klicken Sie **Speichern + Schließen** wenn der Bericht gespeichert werden soll und Sie den Bericht speichern möchten.

### Diagramm zu einem Bericht hinzufügen {#add-a-chart-to-a-report}

1. Beginnen Sie mit der Erstellung eines Berichts, wie [&#x200B; Abschnitt „Erstellen eines &#x200B;](#create-a-report)&quot; in diesem Artikel beschrieben.
1. Wählen Sie in Report Builder die Registerkarte **Diagramm** und wählen Sie dann den Diagrammtyp aus, den Sie hinzufügen möchten.

   ![Diagramm hinzufügen](assets/nwe-add-a-chart-350x247.png)

   Weitere Informationen zum Erstellen eines Diagramms in einem Bericht finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

1. Klicken Sie **Übernehmen**, um Ihre bisherigen Änderungen anzuwenden und den Bericht mit den folgenden Optionen weiter zu bearbeiten.

   Klicken Sie **Speichern + Schließen** wenn Sie mit der Bearbeitung des Berichts fertig sind und den Bericht speichern möchten.
