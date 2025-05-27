---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Häufig gestellte Fragen zu Berichten
description: Häufig gestellte Fragen zu Berichten
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 66fc75ed9a7fca4b44ac776c314a6e08a6fbd450
workflow-type: tm+mt
source-wordcount: '1494'
ht-degree: 0%

---

# Häufig gestellte Fragen zu Berichten

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Im Folgenden finden Sie häufig gestellte Fragen zu Berichten.

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
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p> 
   <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Warum zeigt meine benutzerdefinierte Berechnung für eine Stundendifferenz nicht das richtige Ergebnis in einer Spalte an?

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

In einem Projektbericht habe ich eine Berechnung, die die tatsächlichen Stunden von den geplanten Stunden abzieht. Das Ergebnis, das ich erhalte, ist falsch.

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->


Meine Berechnung lautet:

`valueexpression=SUB(workRequired,actualWorkRequiredDouble)`

### Antwort

Die meisten Felder, die in Workfront Stunden verwenden, werden in Minuten gespeichert. Wenn Sie diese Felder in einer Berechnung verwenden, liegt das Ergebnis meistens in Minuten. Um das Ergebnis in Stunden zu erhalten, müssen Sie das Ergebnis der Berechnung oder des Feldes, auf das Sie verweisen, durch 60 teilen.

Beispielsweise werden „Geplante Stunden“ in Minuten gespeichert, während „Tatsächliche Stunden“ in Stunden gespeichert werden. Daher müssen Sie „Geplante Stunden“ von Minuten in Stunden konvertieren.

Die korrekte Berechnung lautet:

`valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`

## Warum wird der Wert der einzelnen Diagrammelemente in einem Bericht nicht im Diagramm angezeigt?

### Antwort

Wenn ein Berichtsdiagramm mehr als 50 Diagrammelemente enthält, wird der Wert der einzelnen Elemente nicht im Diagramm angezeigt.

Wenn ein Diagramm weniger als 50 Elemente enthält, wird der Wert der einzelnen Elemente im Diagramm angezeigt. Erwägen Sie, einen Filter hinzuzufügen oder die Gruppierungen im Bericht zu ändern, um die Anzahl der Elemente zu begrenzen, die Sie in jedem Element des Diagramms anzeigen.

## Warum gibt mein Bericht zu viele Ergebnisse zurück, um das Diagramm anzuzeigen?

Wenn ich einen Bericht mit einem Diagramm ausführe, sehe ich die Fehlermeldung „Hoppla… Dieser Bericht hat viele Daten zurückgegeben, die das Diagramm unlesbar machen. Es empfiehlt sich, die Ergebnisse durch Hinzufügen eines Filters oder Ändern der Gruppierungen in Ihrem Diagramm einzugrenzen.“

### Antwort

Dieser Fehler bedeutet, dass Ihr Diagramm bis zu 618 verschiedene Ergebnisse enthält - z. B. mehr als 618 Balken in einem Balkendiagramm. Um das Anzeigeproblem zu beheben, müssen Sie die Ergebnisse verfeinern, indem Sie Ihre aktuelle Filter- und Gruppierungsauswahl ändern.

Informationen zum Ändern von Filtern und Gruppierungen finden Sie in den Artikeln [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) und [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## Warum werden meine Aufgaben (oder Probleme) angezeigt, wenn ich auf denselben Bericht (oder Kalender) wie mein Kollege zugreife und stattdessen dessen Aufgaben angezeigt werden?

### Antwort

Der Bericht oder Kalender kann über eine Platzhalterfiltervariable verfügen, die auf den angemeldeten Benutzer verweist. In diesem Fall zeigt der Bericht Informationen basierend auf dem angemeldeten Benutzer an. Passen Sie den Filter an, um den Platzhalter zu entfernen, der auf den angemeldeten Benutzer verweist.\
![Benutzer-ID-Filtervariable](assets/qs--user.id-filter-variable-350x79.png)

Eine vollständige Liste der benutzerbasierten Platzhalterfiltervariablen finden Sie unter [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Warum erscheinen die Daten in meinem Bericht unvollständig?

### Antwort

Dies kann in den meisten Fällen vorkommen, wenn Sie über einen eingeschränkten Zugriff verfügen, der verhindert, dass Elemente im System angezeigt werden. Darüber hinaus werden die Elemente, die Sie sehen möchten, nicht für Sie freigegeben.

Der Ersteller des Berichts kann den Bericht bearbeiten, um ihn mit den Zugriffsrechten eines Systemadministrators auszuführen, oder jeder Planbenutzer, der Zugriff hat, um die Daten anzuzeigen.

Weitere Informationen finden Sie unter [Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen und bereitstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## Wie melde ich Aufgaben (oder Probleme), denen ich zugewiesen bin, unabhängig davon, ob ich der Verantwortliche für sie bin oder nicht?

### Antwort

Verwenden Sie den folgenden Filter in einem Aufgaben- oder Problembericht, um alle Ihnen zugewiesenen Aufgaben oder Probleme anzuzeigen, unabhängig davon, ob Sie der Eigentümer (oder der Primäre Bevollmächtigte) sind oder nicht:

1. Zugriff auf einen Aufgaben- oder Problembericht.
1. Klicken Sie auf **Registerkarte** Filter **auf „Filterregel hinzufügen**.

1. Beginnen Sie im Feld **Feldname eingeben…** mit der Eingabe **Name des Arbeitsauftrags** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Verwenden Sie nicht das Feld **Zugewiesen an Name**, da dies nur nach den Aufgaben und Problemen filtert, für die Sie der Primäre Verantwortliche oder Inhaber sind.

1. Wählen Sie den **Gleich**.
1. Beginnen Sie, *$$USER.ID* in das Textfeld einzugeben und wählen Sie es aus der angezeigten Dropdown-Liste aus.\
   Dadurch wird sichergestellt, dass alle Aufgaben und Probleme angezeigt werden, die dem angemeldeten Benutzer zugewiesen sind. Sie können den Platzhalter durch einen bestimmten Benutzernamen ersetzen.\
   ![Mir zugewiesene Aufgaben](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Klicken Sie auf **Speichern + schließen**.

## Warum werden die Links Probleme hinzufügen/Aufgaben hinzufügen nicht unten in den Listen „Meine Probleme und Aufgaben“ in einem Projekt angezeigt?

### Antwort

Stellen Sie zunächst sicher, dass Sie über die richtigen Zugriffsrechte und Berechtigungen verfügen, um einem Projekt Probleme und Aufgaben hinzuzufügen. In diesem Fall sollten die Links **Probleme hinzufügen** und **Aufgaben hinzufügen** unten in den Listen **Probleme** und **Aufgaben** angezeigt werden.

Es gibt jedoch einige Dinge, die verhindern können, dass diese Links angezeigt werden:

* Wenn Sie den Schnellfilter auf diese Listen angewendet haben, werden die Links nicht angezeigt. Entfernen Sie den Schnellfilter. Die Links sollten nun angezeigt werden, damit Sie Ihren Projekten Probleme und Aufgaben hinzufügen können.\
  Weitere Informationen zum Schnellfilter finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Wenn Sie eine **Gruppierung** auf diese Listen angewendet haben, werden die Links nicht angezeigt. Entfernen Sie die **Gruppierung** und die Links sollten angezeigt werden, damit Sie Ihren Projekten Probleme und Aufgaben hinzufügen können.\
  Informationen zum Erstellen von Gruppierungen finden Sie unter [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Wenn Sie eine **Ansicht** auf diese Listen angewendet haben, bei der eine andere Währung als die Standardwährung für das Projekt ausgewählt ist, werden die Links nicht angezeigt. Ändern Sie **Ansicht** in **Originalwährung des Projekts** und die Links sollten angezeigt werden, damit Sie Ihren Projekten Probleme und Aufgaben hinzufügen können.\
  Weitere Informationen zum Ändern der Währung in Ihrer Ansicht finden Sie unter [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![Projektwährung](assets/nwe-project-original-currency-350x229.png)

## Werden die Informationen in meinem Bericht oder Dashboard automatisch aktualisiert?

### Antwort

Informationen in Berichten oder Dashboards werden nicht automatisch aktualisiert.

Informationen können in einem zwischengespeicherten Bericht manuell aktualisiert werden.\
Weitere Informationen zum Aktualisieren eines zwischengespeicherten Berichts finden Sie unter [Bericht ausführen](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

Informationen können in einem zwischengespeicherten Dashboard manuell aktualisiert werden.\
Weitere Informationen zum Aktualisieren eines zwischengespeicherten Dashboards finden Sie im Abschnitt [Anzeigen von Dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) im Artikel [Erste Schritte mit Dashboards](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Kann ich den Besitzer eines Berichts wechseln?

### Antwort

Sie können den Besitzer eines Berichts nicht ändern. Der Benutzer, der den Bericht erstellt hat, kann jedoch anderen Benutzern erlauben, den Bericht zu bearbeiten. Wie Sie Benutzern die Bearbeitung eines Berichts ermöglichen können, hängt vom verwendeten Benutzertyp ab.

* Systemadministratoren können Benutzern mit einer Planlizenz das Bearbeiten von Berichten gestatten, indem sie die Option Bearbeiten in der Zeile Berichte so konfigurieren, dass sie den Zugriff zum Erstellen eines Berichts einschließt.\
  Weitere Informationen finden Sie unter [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Jeder Endbenutzer, der Zugriff auf das Erstellen und Freigeben von Berichten hat, kann anderen erlauben, einzelne Berichte zu bearbeiten, indem er sie freigibt und anderen Benutzern Verwaltungsberechtigungen für sie erteilt.\
  Weitere Informationen finden Sie unter [Freigeben eines Berichts in Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Wenn Sie berechtigt sind, einen Bericht anzuzeigen oder zu verwalten, können Sie auch eine Kopie des Berichts erstellen, für die Sie dann standardmäßig Besitzer sind. Weitere Informationen zum Kopieren eines Berichts finden Sie unter [Erstellen einer Berichtskopie](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## Warum kann ich nicht auf einen Bericht zugreifen, der einem deaktivierten Benutzer gehört?

### Antwort

Manchmal ist der Eigentümer des Berichts auch der im Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** im Bericht angegebene Benutzer. Wenn der **Diesen Bericht ausführen mit den Zugriffsrechten von:** Benutzer deaktiviert ist, wird der Bericht nicht mehr für Benutzer angezeigt, die den Bericht für sie freigegeben haben. In diesem Fall können Sie den Bericht erneut zugänglich machen, indem Sie die **Diesen Bericht ausführen mit den Zugriffsrechten von:** leer lassen oder einen aktiven Benutzer in das Feld eingeben.

Weitere Informationen zum Feld **Diesen Bericht mit Zugriffsrechten von:** ausführen“ finden Sie unter [Ausführen und Bereitstellen eines Berichts mit Zugriffsrechten eines anderen Benutzers](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Informationen zur Identifizierung aller Berichte, die von deaktivierten Benutzern erstellt werden, finden Sie unter [Erstellen eines Berichts zu Berichtsaktivitäten](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## Wie greife ich auf ein Dashboard zu, das einen Bericht enthält, der einem gelöschten Benutzer gehört?

### Antwort

Wenn Sie einen Benutzer löschen, können Sie weiterhin auf alle von ihm erstellten Berichte zugreifen. Dashboards, die den Bericht enthalten, werden jedoch auch gelöscht. Dies bedeutet, dass Sie nicht mehr auf Folgendes zugreifen können:

* Ein Dashboard, das den Bericht enthält
* Ein benutzerdefinierter Abschnitt, der ein Dashboard des Berichts enthält

Weitere Informationen zu den Auswirkungen des Löschens eines Benutzers finden Sie unter [Löschen von Benutzern](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Wenn Sie Ansichtszugriff auf den Bericht haben, haben Sie folgende Möglichkeiten:

1. Erstellen Sie eine Kopie des Berichts.\
   Informationen zum Erstellen einer Kopie eines Berichts finden Sie unter [Erstellen einer Kopie eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Aktualisieren Sie das Dashboard, um den kopierten Bericht aufzunehmen.\
   Informationen zum Bearbeiten eines Dashboards finden Sie unter [Dashboard bearbeiten](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
