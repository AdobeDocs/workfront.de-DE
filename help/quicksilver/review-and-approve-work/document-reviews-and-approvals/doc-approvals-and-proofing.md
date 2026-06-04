---
product-area: documents
navigation-topic: approvals
title: Gemeinsames Verwenden von einheitlichen Genehmigungen und Proofing
description: Sie können einheitliche Genehmigungen mit Proofing verwenden.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: be484629-6e70-4809-ad4c-a489d5814da6
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UBrLQv-1DRwZ-TO3c1SAUn8OF0yOAYnKPGrf-lSS0xM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 955
ht-degree: 2%

---

# Gemeinsames Verwenden von einheitlichen Genehmigungen und Proofing

Einheitliche Genehmigungen in Workfront beinhalten jetzt eine Reihe neuer Funktionen, mit denen Sie Dokumente überprüfen und genehmigen können. Sie können einen einheitlichen Genehmigungs-Workflow mit dem vorhandenen Proofing Viewer verwenden, um Kommentare und Markups zu überprüfenden Dokumenten hinzuzufügen.

Es gibt einige wichtige Unterschiede im Workflow bei der gemeinsamen Verwendung von einheitlichen Genehmigungen und Proofing:

* Die Teilnehmer werden in der Dokumentzusammenfassung und nicht im Proofing-Workflow angezeigt.

* Die Details „Gesendet“, „Geöffnet“, „Kommentar“, „Entscheidung (SOCD)“ in der Dokumentliste sind mit Proofing verbunden und spiegeln den Entscheidungsstatus des Dokuments nicht wider.

## Dokument hochladen und Korrekturabzug erstellen

1. Navigieren Sie zum Projekt, zur Aufgabe oder zum Problem, dem bzw. dem Sie ein neues Dokument hinzufügen möchten.
1. Klicken Sie auf **Registerkarte** Dokumente“ und dann auf das **Neu hinzufügen** Dropdown-Menü.
oder
Ziehen Sie das Dokument per Drag-and-Drop in die Dokumentliste.

   >[!NOTE]
   >
   >Wenn Sie in **Benutzerprofil „Korrekturabzüge beim Hochladen von Dokumenten automatisch generieren** aktiviert haben, erstellt das System automatisch einen einfachen Korrekturabzug.

1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf den **Korrekturabzug erstellen** Link, der unter dem Dokumentnamen angezeigt wird, und wählen Sie **Einfacher Korrekturabzug** aus. Sie müssen einen einfachen Korrekturabzug erstellen, da Sie den Proofing-Workflow nicht für Genehmigungen verwenden werden.

Benutzende, die als Teilnehmer zugewiesen sind, können die Proofing Viewer verwenden, um Kommentare und Markups zu dem Dokument hinzuzufügen. Fahren Sie mit dem nächsten Abschnitt fort, um zu erfahren, wie Sie Reviewer hinzufügen.

## Öffnen Sie die Dokumentzusammenfassung und weisen Sie Teilnehmer zu

Sie haben die Möglichkeit, Prüfer, genehmigende Personen oder eine Mischung aus beidem zuzuweisen:

* **Reviewer** können Kommentare hinzufügen und Assets markieren. Nach Abschluss können sie ihre Überprüfung als abgeschlossen markieren. Die Überprüfung als abgeschlossen zu markieren ist nicht erforderlich, damit das Dokument im Genehmigungsprozess fortgesetzt werden kann.
* **Genehmigende Personen** können Kommentare hinzufügen und Assets markieren. Sie müssen eine Entscheidung treffen, um den Genehmigungsprozess voranzubringen.

So weisen Sie Teilnehmer zu:

1. Wählen Sie das hochgeladene Dokument aus und öffnen Sie die Dokumentzusammenfassung.
   ![Dokumentzusammenfassung öffnen](assets/open-doc-summary.png)

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow erstellen**.


1. Füllen Sie die folgenden Details aus:

   <table>
   <tr>
   <td><strong>Name der Phase</strong></td>
   <td>Einen Namen für das Stadium hinzufügen. Sie können den Namen in einen aussagekräftigeren Namen ändern, z. B<em> „Erstprüfung</em> oder "<em> Genehmigung</em>.</td>
   </tr>
   <tr>
   <td><strong>Namen oder E-Mails hinzufügen</strong></td>
   <td>Beginnen Sie mit der Eingabe eines Benutzer- oder Team-Namens, der als genehmigende Person oder Prüfende Person hinzugefügt werden soll. Wenn Sie nur über Validierungsverantwortliche verfügen, werden diese benachrichtigt und haben die Möglichkeit, die Überprüfung abzuschließen. Es ist jedoch keine Entscheidung erforderlich oder getroffen.</td>
   </tr>
   <tr>
   <td><strong>Eine Entscheidung erforderlich (optional)</strong></td>
   <td>Die erste Person, die eine Entscheidung trifft, schließt die Phase ab.</td>
   </tr>
   <tr>
   <td><strong>Fälligkeitsdatum (optional)</strong></td>
   <td>Legen Sie ein Fälligkeitsdatum für die Genehmigung fest. Benutzer und Teams werden 72 Stunden und dann 24 Stunden vor dem angegebenen Fälligkeitsdatum per E-Mail benachrichtigt.</td>
   </tr>
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Schritte nach Bedarf hinzuzufügen.

   >[!NOTE]
   >
   >Wenn Sie mehrere Phasen hinzufügen, wird der Genehmigungs-Workflow in der Reihenfolge fortgesetzt, in der die Phasen aufgelistet sind. Wenn alle erforderlichen Entscheidungen getroffen werden, beginnt die nächste Phase und die vorherige Phase wird gesperrt.

   ![Neues Stadium](assets/new-stage.png)

1. Nachdem Sie alle validierungsverantwortlichen Personen und genehmigenden Personen hinzugefügt haben, klicken Sie auf **Genehmigungen anfordern**. Die Teilnehmer werden per E-Mail benachrichtigt.


## Erstellen Sie nach Bedarf eine neue Version

Wenn Sie eine weitere Runde der Überprüfung und Genehmigung benötigen, können Sie eine neue Korrekturabzugsversion erstellen und die vorherigen Teilnehmer, neue Teilnehmer oder eine Mischung aus beiden hinzufügen. In der Dokumentzusammenfassung können Sie Informationen zu früheren Versionen und Teilnehmern anzeigen.

Hinzufügen einer neuen Version:

1. Ziehen Sie die neue Datei per Drag-and-Drop auf das vorherige Dokument in Workfront. Dadurch wird automatisch eine neue Version erstellt.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus und klicken Sie auf **Korrekturabzug erstellen** > **Einfacher Korrekturabzug**.

1. Wählen Sie das Dokument erneut aus und öffnen Sie die Dokumentzusammenfassung.
   ![Dokumentzusammenfassung öffnen](assets/open-doc-summary.png)

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow erstellen**.


1. Füllen Sie die folgenden Details aus:

   <table>
   <tr>
   <td><strong>Name der Phase</strong></td>
   <td>Einen Namen für das Stadium hinzufügen. Sie können den Namen in einen aussagekräftigeren Namen ändern, z. B<em> „Erstprüfung</em> oder "<em> Genehmigung</em>.</td>
   </tr>
   <tr>
   <td><strong>Namen oder E-Mails hinzufügen</strong></td>
   <td>Beginnen Sie mit der Eingabe eines Benutzer- oder Team-Namens, der als genehmigende Person oder Prüfende Person hinzugefügt werden soll. Wenn Sie nur über Validierungsverantwortliche verfügen, werden diese benachrichtigt und haben die Möglichkeit, die Überprüfung abzuschließen. Es ist jedoch keine Entscheidung erforderlich oder getroffen.</td>
   </tr>
   <tr>
   <td><strong>Eine Entscheidung erforderlich (optional)</strong></td>
   <td>Die erste Person, die eine Entscheidung trifft, schließt die Phase ab.</td>
   </tr>
   <tr>
   <td><strong>Fälligkeitsdatum (optional)</strong></td>
   <td>Legen Sie ein Fälligkeitsdatum für die Genehmigung fest. Benutzer und Teams werden 72 Stunden und dann 24 Stunden vor dem angegebenen Fälligkeitsdatum per E-Mail benachrichtigt.</td>
   </tr>
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Schritte nach Bedarf hinzuzufügen.

   >[!NOTE]
   >
   >Wenn Sie mehrere Phasen hinzufügen, wird der Genehmigungs-Workflow in der Reihenfolge fortgesetzt, in der die Phasen aufgelistet sind. Wenn alle erforderlichen Entscheidungen getroffen werden, beginnt die nächste Phase und die vorherige Phase wird gesperrt.

   ![Neues Stadium](assets/new-stage.png)

1. Nachdem Sie alle validierungsverantwortlichen Personen und genehmigenden Personen hinzugefügt haben, klicken Sie auf **Genehmigungen anfordern**. Die Teilnehmer werden per E-Mail benachrichtigt.



## Korrekturabzug prüfen und eine Entscheidung treffen

Das Dokument wechselt erst dann in den Status Genehmigt , wenn alle zugewiesenen genehmigenden Personen „Genehmigt“ auswählen.

So überprüfen und genehmigen Sie ein Dokument:

1. Gehen Sie zu Ihrer E-Mail-Benachrichtigung und klicken Sie auf **Zum Überprüfen gehen**.

1. Wenn Sie sich in Workfront befinden, klicken Sie auf **Zum Korrekturabzug gehen**.

1. Überprüfen Sie den Inhalt und fügen Sie Kommentare oder Markup hinzu. Weitere Informationen zur Verwendung der Proofing-Anzeige finden Sie unter [Testsendungen in Adobe Workfront überprüfen: Artikelindex](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Wählen Sie eine der folgenden Entscheidungen:

   * **Genehmigen**: Das Dokument muss nicht geändert werden und ist einsatzbereit.
   * **Mit Änderungen genehmigen**: Das Dokument benötigt Änderungen und ist nach deren Vornahme zur Verwendung bereit. Eine zusätzliche Genehmigung ist nicht erforderlich.
   * **Muss überarbeitet werden**: Das Dokument muss geändert werden und ist nicht einsatzbereit. Sobald die angegebenen Änderungen vorgenommen wurden, muss das Dokument als neue Version hochgeladen werden und eine weitere Genehmigungsrunde durchlaufen. Weitere Informationen zum Hochladen einer neuen Version finden Sie unter [Erstellen einer neuen Version nach Bedarf](#create-a-new-version-as-needed) in diesem Artikel.

Sobald Sie eine Entscheidung treffen, wird der Dokumentverantwortliche per E-Mail benachrichtigt.