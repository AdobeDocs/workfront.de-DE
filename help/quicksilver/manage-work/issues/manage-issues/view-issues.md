---
product-area: projects
navigation-topic: manage-issues
title: Anfragen anzeigen
description: Sie können Probleme anzeigen, die mit einem Projekt, einer Aufgabe oder einer Iteration verbunden sind.
author: Alina
feature: Work Management
exl-id: b6791c8f-b356-4235-8b0e-952e29a88952
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1035'
ht-degree: 0%

---

# Anfragen anzeigen

Sie können Probleme anzeigen, die mit einem Projekt, einer Aufgabe oder einer Iteration verbunden sind.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anfrage oder höher</p> <p>Überprüfen Sie die Lizenz oder eine höhere Lizenz, um Probleme im Abschnitt Probleme eines Projekts anzuzeigen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Anfragen anzeigen</p> <p>Anzeigen oder Hochladen des Zugriffs auf Projekte und Aufgaben</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen zum Zugriff auf Probleme in Ihrer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Probleme gewähren</a>. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen der Berechtigungen für das Problem</p> <p> Informationen zum Gewähren von Berechtigungen für Probleme finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Freigeben eines Problems </a></p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriff auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Anfragen basierend auf Status anzeigen

So zeigen Sie Probleme in einem Projekt, einer Aufgabe oder einer Iteration an:

1. Öffnen Sie ein Projekt, eine Aufgabe oder eine Iteration, das/die Probleme enthält, und klicken Sie **linken Bereich** Probleme“.

1. Um alle offenen oder geschlossenen Probleme anzuzeigen, klicken Sie im Dropdown-Menü **Filter** auf einen der unten aufgeführten Filter.

>[!TIP]
>
>Die Liste der Filter hängt davon ab, was Ihr System- oder Gruppenadministrator ausgewählt hat, um sie anzuzeigen.

* **Offen:** Zeigt Probleme an, die offen sind.

  Dazu gehören diejenigen, die mit einem Lösungsobjekt verknüpft sind, und solche mit dem Status Geschlossen - Genehmigung steht aus.

  Informationen zum Auflösen von Objekten finden Sie unter [Übersicht über das Auflösen und das Auflösen von Objekten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

* **Abgeschlossen:** Zeigt alle Anfragen an, die ein tatsächliches Abschlussdatum haben.
* **Alle** Zeigt alle Probleme an.

## Informationen zu Problemen

Sie können Informationen zu einem Problem anzeigen, wenn Sie darauf zugreifen.

So greifen Sie auf ein Problem zu und zeigen Informationen dazu an:

1. Öffnen Sie ein Projekt, eine Aufgabe oder eine Iteration, das/die Probleme enthält, und klicken Sie **linken Bereich** Probleme“.
1. Wählen **im Dropdown** Menü „Filter“ den Filter aus, um die Probleme anzuzeigen, die angezeigt werden sollen.

   Wählen Sie aus den folgenden Optionen aus:

   * Öffnen
   * Abgeschlossen
   * Alle

1. Klicken Sie auf den Namen eines Problems.

   Wenn Sie Verwaltungsberechtigungen für das Problem haben, können Sie jedes bearbeitbare Feld im Problem bearbeiten und Genehmigungen, Stunden oder Dokumente zum Problem hinzufügen.

1. Klicken Sie im linken Bedienfeld auf eine der folgenden Optionen, um weitere Informationen zum Problem anzuzeigen:

* **Aktualisierungen**: Sie können die folgenden Aktionen ausführen:

   * Kommentieren Sie das Problem oder antworten Sie auf einen vorhandenen Kommentar.
   * Zeit erfassen.
   * Den Status des Problems ändern.

     Weitere Informationen zum Aktualisieren der Arbeit in Workfront finden Sie unter [Arbeit aktualisieren](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* **Dokumente**: Fügen Sie dem Problem Dokumente hinzu. Weitere Informationen zum Hinzufügen von Dokumenten zu Workfront finden Sie unter [Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem Dateisystem](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

* **Problemdetails**: Erweitern Sie diesen Link, um die Bereiche **Übersicht** und **Benutzerdefinierte Forms** anzuzeigen.

  Wenn Sie über Verwaltungsberechtigungen für das Problem und Bearbeitungsrechte für das benutzerdefinierte Formular verfügen, können Sie einige der Informationen hier bearbeiten.

  Sie können die folgenden Felder im Bereich **Übersicht** anzeigen oder bearbeiten:

   * **Name**
   * **Path**: Der Pfad, über den das Problem im Projekt protokolliert wurde.

     Wenn ein Problem als Anfrage in einer Anfrage-Warteschlange gesendet wurde, werden die Namen des Projekts, der Themengruppe und des Warteschlangenthemas hier aufgeführt. Dieses Feld kann nicht bearbeitet werden.

     Weitere Informationen zum Senden von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

   * **Beschreibung**
   * **URL**: Jede Web-Adresse im Zusammenhang mit dem Problem.
   * **Priorität**: Eine visuelle Markierung, mit der Sie Probleme priorisieren können.
   * **Schweregrad**: Eine visuelle Markierung, die anzeigt, wie schwerwiegend das in diesem Problem beschriebene Problem ist.
   * **Primärer Kontakt**: Der Primäre Standardkontakt ist der Benutzer, der das Problem erstellt hat. Dieses Feld kann bearbeitet werden.
   * **Geplante Stunden**: Zeigt die Zeit an, die jemand benötigt, um das Problem zu beheben. Der Standardwert ist 8 Stunden. Dieses Feld kann bearbeitet werden.
   * **Tatsächliche Stunden**: Zeigt die Zeit an, die zum Fertigstellen des Problems benötigt wurde. Dies ist die tatsächliche Zeit, zu der sich jemand für das Problem anmeldet.
   * **Geplantes Startdatum**: Das Datum, an dem das Problem beginnen soll. Der Standardwert ist das Datum und die Uhrzeit, zu der das Problem erstellt wurde.
   * **Tatsächliches Startdatum**: Datum und Uhrzeit, zu der der Problemstatus in „In Bearbeitung“ geändert wurde.
   * **Geplantes Abschlussdatum**: Das Datum, an dem die Anfrage voraussichtlich abgeschlossen wird.
   * **Tatsächliches Abschlussdatum**: Das Datum, an dem das Problem tatsächlich abgeschlossen ist. Dieses Feld wird automatisch ausgefüllt, wenn sich der Problemstatus in „Geschlossen“ oder „Gelöst“ ändert, oder es kann manuell bearbeitet werden.
   * **Istkosten**: Die Kosten basierend auf den für das Problem protokollierten tatsächlichen Stunden. Dieses Feld kann nicht bearbeitet werden. Die Istkosten eines Problems werden anhand der folgenden Formel berechnet, wobei der Benutzerkostensatz der Kostensatz ist, der dem Benutzer zugeordnet ist, der die Zeit bis zum Problem protokolliert:

     Anfrage-Istkosten = protokollierte Stunden * Benutzerkostensatz

   * **Eingegeben von**: Dies ist der Benutzer, der das Problem erstellt hat. Dieses Feld kann nicht bearbeitet werden.
   * **Zuletzt aktualisiert von**: Dies ist der Benutzer, der ein Feld zum Problem zuletzt aktualisiert hat. Dieses Feld kann nicht bearbeitet werden.

     Im Bereich **Benutzerdefinierte Forms** können Sie ein oder mehrere benutzerdefinierte Formulare anzeigen oder auswählen, die mit dem Problem verknüpft werden sollen.

* **Stunden**: Zeigt eine Liste der Stundeneinträge für das Problem an.
* **Genehmigungen:** Zeigt die mit dem Problem verbundenen Genehmigungspfade an.

  Weitere Informationen zum Verknüpfen von Genehmigungen mit einem Problem finden Sie [ Abschnitt „Verknüpfen eines Genehmigungsprozesses mit einem ](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md#associating-the-approval-process-with-an-object)&quot; in [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Anzeigen, welche Projekte und Aufgaben Probleme aufweisen

Sie können Symbole in der Ansicht eines Projekt- oder Aufgabenberichts oder einer Liste hinzufügen, um anzuzeigen, ob Probleme damit verbunden sind. Das Hinzufügen von Symbolen zur Ansicht eines Berichts oder einer Liste ist bei Projekten und Aufgaben ähnlich.

So fügen Sie Symbole hinzu, die anzeigen, ob ein Projekt in einem Projektbericht Probleme aufweist:

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.
1. Klicken Sie **Reporting** > **Neuer Bericht** > **Projektbericht**.
1. Beginnen Sie im Feld **In dieser Spalte anzeigen** mit der Eingabe **Statussymbole** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie **Speichern + Schließen** .

   Die Problemsymbole werden in den Projekten mit Problemen in der Spalte **Statussymbole** angezeigt.

   ![project_list_with_issue_icon.png](assets/project-list-with-issue-icon-350x132.png)
