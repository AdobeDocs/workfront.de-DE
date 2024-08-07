---
product-area: projects
navigation-topic: manage-issues
title: Probleme anzeigen
description: Sie können Probleme anzeigen, die mit einem Projekt, einer Aufgabe oder einer Iteration verbunden sind.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1035'
ht-degree: 0%

---

# Probleme anzeigen

Sie können Probleme anzeigen, die mit einem Projekt, einer Aufgabe oder einer Iteration verbunden sind.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> <p>Überprüfen Sie oder eine höhere Lizenz, um Probleme im Abschnitt Probleme eines Projekts anzuzeigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme anzeigen</p> <p>Anzeigen oder höherer Zugriff auf Projekte und Aufgaben</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Probleme in Ihrer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Probleme gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Problem anzeigen</p> <p> Informationen zum Gewähren von Berechtigungen für Probleme finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a></p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anzeigen von Problemen basierend auf dem Status

So zeigen Sie Probleme in einem Projekt, einer Aufgabe oder einer Iteration an:

1. Öffnen Sie ein Projekt, eine Aufgabe oder eine Iteration, die Probleme enthält, und klicken Sie dann im linken Bereich auf **Probleme** .

1. Um alle, geöffneten oder geschlossenen Probleme anzuzeigen, klicken Sie auf einen der unten aufgeführten Filter aus dem Dropdown-Menü **Filter** .

>[!TIP]
>
>Die Liste der Filter hängt davon ab, welches System- oder Gruppenadministrator ausgewählt hat, um sie anzuzeigen.

* **Öffnen:** Zeigt offene Probleme an.

  Dazu gehören die mit einem auflösenden Objekt und denen mit dem Status Geschlossen - Ausstehende Genehmigung .

  Weitere Informationen zum Auflösen von Objekten finden Sie unter [Übersicht über das Auflösen und Auflösen von Objekten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Abgeschlossen:** Zeigt alle Probleme mit dem tatsächlichen Abschlussdatum an.
* **Alle** Zeigt alle Probleme an.

## Informationen zu Problemen

Sie können Informationen zu einem Problem anzeigen, wenn Sie darauf zugreifen.

So greifen Sie auf ein Problem zu und zeigen Informationen dazu an:

1. Öffnen Sie ein Projekt, eine Aufgabe oder eine Iteration, die Probleme enthält, und klicken Sie dann im linken Bereich auf **Probleme** .
1. Wählen Sie aus dem Dropdownmenü **Filter** den Filter aus, um die Probleme anzuzeigen, die Sie anzeigen möchten.

   Wählen Sie aus den folgenden Optionen aus:

   * Offen
   * Abgeschlossen
   * Alle

1. Klicken Sie auf den Namen eines Problems.

   Wenn Sie über Verwaltungsberechtigungen für das Problem verfügen, können Sie jedes bearbeitbare Feld im Problem bearbeiten und dem Problem Genehmigungen, Stunden oder Dokumente hinzufügen.

1. Klicken Sie im linken Bereich auf einen der folgenden Elemente, um weitere Informationen zum Problem anzuzeigen:

* **Aktualisierungen**: Sie können die folgenden Aktionen durchführen:

   * Kommentar zum Thema oder Antwort auf einen vorhandenen Kommentar.
   * Protokollzeit.
   * Ändern Sie den Status des Problems.

     Weitere Informationen zum Aktualisieren der Arbeit in Workfront finden Sie unter [Arbeit aktualisieren](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Dokumente**: Hängen Sie Dokumente an das Problem an. Weitere Informationen zum Hinzufügen von Dokumenten zu Workfront finden Sie unter [Dokumente aus Ihrem Dateisystem zu Adobe Workfront hinzufügen](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Problemdetails**: Erweitern Sie diesen Link, um die Bereiche **Überblick** und **Benutzerdefinierter Forms** anzuzeigen.

  Wenn Sie über Verwaltungsberechtigungen für das Problem verfügen und Berechtigungen für das benutzerdefinierte Formular bearbeiten, können Sie hier einige der Informationen bearbeiten.

  Zeigen Sie die folgenden Felder im Bereich **Überblick** an oder bearbeiten Sie sie:

   * **Name**
   * **Pfad**: der Pfad, über den das Problem beim Projekt protokolliert wurde.

     Wenn ein Problem als Anfrage in einer Anforderungswarteschlange gesendet wurde, werden hier die Namen des Projekts, der Themengruppe und das Warteschlangenthema aufgelistet. Dieses Feld kann nicht bearbeitet werden.

     Weitere Informationen zum Senden von Anforderungen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Beschreibung**
   * **URL**: jede Webadresse, die mit dem Problem in Verbindung steht.
   * **Priorität**: eine visuelle Markierung, mit der Sie Probleme priorisieren können.
   * **Schweregrad**: eine visuelle Markierung, die anzeigt, wie schwerwiegend das im Problem beschriebene Problem ist.
   * **Primärer Kontakt**: Der standardmäßige Primäre Kontakt ist der Benutzer, der das Problem erstellt hat. Dieses Feld kann bearbeitet werden.
   * **Geplante Stunden**: Zeigt den Zeitraum an, der benötigt wird, um das Problem abzuschließen. Der Standardwert ist 8 Stunden. Dieses Feld kann bearbeitet werden.
   * **Tatsächliche Stunden**: zeigt die Zeit an, die zum Abschließen des Problems benötigt wurde. Dies ist der tatsächliche Zeitpunkt, zu dem sich ein Benutzer für das Problem anmeldet.
   * **Geplantes Startdatum**: Das Datum, an dem das Problem beginnen soll. Die Standardeinstellung ist das Datum und die Uhrzeit der Erstellung des Problems.
   * **Tatsächliches Startdatum**: Datum und Uhrzeit der Änderung des Problemstatus in &quot;Wird ausgeführt&quot;.
   * **Geplantes Abschlussdatum**: Das Datum, an dem das Problem abgeschlossen werden soll.
   * **Tatsächliches Abschlussdatum**: Das Datum, an dem das Problem tatsächlich abgeschlossen ist. Dieses Feld wird automatisch ausgefüllt, wenn sich der Problemstatus in &quot;Geschlossen&quot;oder &quot;Gelöst&quot;ändert oder manuell bearbeitet werden kann.
   * **Tatsächliche Kosten**: die Kosten basierend auf den tatsächlich für das Problem angemeldeten Stunden. Dieses Feld kann nicht bearbeitet werden. Die tatsächlichen Kosten eines Problems werden anhand der folgenden Formel berechnet, wobei die Benutzerkostenrate der Kostensatz ist, der dem Benutzer zugeordnet ist, der die Zeit bis zum Problem protokolliert:

     Tatsächliche Kosten des Problems = Stunden protokolliert * Benutzerkostenrate

   * **Eingestiegen von**: Dies ist der Benutzer, der das Problem erstellt hat. Dieses Feld kann nicht bearbeitet werden.
   * **Zuletzt aktualisiert von**: Dies ist der Benutzer, der ein Feld zum Problem zuletzt aktualisiert hat. Dieses Feld kann nicht bearbeitet werden.

     Wählen Sie im Bereich **Benutzerdefinierter Forms** ein oder mehrere benutzerdefinierte Formulare aus, die mit dem Problem verknüpft werden sollen.

* **Stunden**: Zeigt eine Liste der Stundeneinträge zum Problem an.
* **Genehmigungen:** Zeigt die mit dem Problem verknüpften Genehmigungspfade an.

  Weitere Informationen zum Verknüpfen von Genehmigungen mit einem Problem finden Sie im Abschnitt [Verknüpfen eines Genehmigungsprozesses mit einem Arbeitselement](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object) in [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Anzeigen der Projekte und Aufgaben, die Probleme aufweisen

Sie können in der Ansicht eines Projekts, eines Aufgabenberichts oder einer Liste Symbole hinzufügen, um anzuzeigen, ob Probleme angehängt sind. Das Hinzufügen von Symbolen zur Ansicht eines Berichts oder einer Liste ist für Projekte und Aufgaben ähnlich.

So fügen Sie Symbole hinzu, die anzeigen, ob ein Projekt in einem Projektbericht Probleme hat:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).
1. Klicken Sie auf **Berichterstellung** > **Neuer Bericht** > **Projektbericht**.
1. Geben Sie im Feld **In dieser Spalte anzeigen** **Statussymbole** ein und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie auf **Speichern + Schließen** .

   Die Problemsymbole werden in den Projekten angezeigt, die Probleme in der Spalte **Statussymbole** haben.

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
