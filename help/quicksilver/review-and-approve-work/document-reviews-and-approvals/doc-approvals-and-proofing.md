---
product-area: documents
navigation-topic: approvals
title: Verwenden neuer Dokumentgenehmigungen und Testsendungen gemeinsam
description: Sie können neue Dokumentgenehmigungen mit Testversand verwenden.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 8dc9df69bbce86f141ac451381fcc41a112ca0bc
workflow-type: tm+mt
source-wordcount: '924'
ht-degree: 0%

---


# Verwenden neuer Dokumentgenehmigungen und Testsendungen gemeinsam

Die neuen Dokumentgenehmigungen in Workfront enthalten eine Reihe neuer Funktionen, mit denen Sie Dokumente überprüfen und genehmigen können. Sie können den neuen Workflow für Dokumentgenehmigungen mit dem vorhandenen Testversand-Viewer verwenden, um in der Prüfung befindliche Dokumente mit Kommentaren und Markierungen zu versehen.

Es gibt einige wesentliche Unterschiede im Workflow bei der gemeinsamen Verwendung neuer Dokumentgenehmigungen und Testsendungen:

* Entscheidungsschaltflächen werden im Testversand-Viewer nicht angezeigt

* Die Teilnehmer werden in der Dokumentzusammenfassung und nicht im Testversand-Workflow angezeigt.

* Die in der Dokumentenliste enthaltenen Informationen zu Gesendet, Geöffnet, Kommentar, Entscheidung (SOCD) beziehen sich auf die Prüfung und spiegeln nicht den Entscheidungsstatus des Dokuments wider.

## Hochladen eines Dokuments und Erstellen eines Testversands

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, dem Sie ein neues Dokument hinzufügen möchten.
1. Klicken Sie auf die Registerkarte **Dokumente** und dann auf das Dropdown-Menü **Neu hinzufügen** .
Oder
Ziehen Sie das Dokument in die Dokumentliste.

   >[!NOTE]
   >
   >Wenn Sie in Ihrem Benutzerprofil **Testsendungen beim Hochladen von Dokumenten automatisch generieren** aktiviert haben, erstellt das System automatisch einen einfachen Testversand.

1. Bewegen Sie den Mauszeiger über das Dokument, klicken Sie auf den Link **Testversand erstellen** , der unter dem Dokumentnamen angezeigt wird, und wählen Sie **Einfacher Testversand** aus. Sie müssen einen einfachen Testversand erstellen, da Sie den Testversand-Workflow nicht für Validierungen verwenden.

Als Teilnehmer zugewiesene Benutzer können den Testversand-Viewer verwenden, um dem Dokument Kommentare und Markierungen hinzuzufügen. Fahren Sie mit dem nächsten Abschnitt fort, um zu erfahren, wie Sie Überprüfungsteilnehmer hinzufügen.

## Öffnen Sie die Dokumentzusammenfassung und weisen Sie Teilnehmer zu.

Sie haben die Möglichkeit, Überprüfer, Genehmiger oder eine Mischung aus beiden zuzuweisen:

* **Überprüfer** können Kommentare hinzufügen und Assets markieren. Nach Abschluss können sie ihre Überprüfung als abgeschlossen markieren. Die Kennzeichnung der Überprüfung als abgeschlossen ist nicht erforderlich, damit das Dokument im Genehmigungsprozess vorankommt.
* **Genehmiger** können Kommentare hinzufügen und Assets markieren. Sie müssen eine Entscheidung treffen, um den Genehmigungsprozess voranzubringen.

Zuweisen von Teilnehmern:

1. Wählen Sie das hochgeladene Dokument aus und öffnen Sie die Dokumentzusammenfassung.
   ![](assets/open-doc-summary.png)

1. Scrollen Sie nach unten zum Abschnitt Genehmigungen und klicken Sie dann auf **Hinzufügen**.

1. (Optional) Wählen Sie eine vorhandene Validierungsvorlage aus. Benutzer mit einer Standardlizenz können im Bereich &quot;Setup&quot;wiederaufgenommene Genehmigungsvorlagen erstellen. Weitere Informationen finden Sie unter [Erstellen einer Genehmigungsvorlage für Assets und Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Optional) Legen Sie einen Termin für die Genehmigung fest. Benutzer und Teams werden per E-Mail 72 Stunden und 24 Stunden vor Ablauf der angegebenen Frist benachrichtigt.

1. Um einen Genehmiger hinzuzufügen, klicken Sie auf die Schaltfläche Genehmiger und beginnen Sie mit der Eingabe eines Benutzers oder Teams.

1. Um einen Validierer hinzuzufügen, klicken Sie auf die Schaltfläche Validierer und geben Sie den Namen des Benutzers oder Teams ein.

   ![](assets/add-approvers.png)

1. Nachdem Sie alle Prüfer und Genehmiger hinzugefügt haben, klicken Sie auf **Anfrage senden**. Teilnehmer werden per E-Mail benachrichtigt.

## Erstellen Sie bei Bedarf eine neue Version

Wenn Sie eine weitere Überprüfungs- und Validierungsrunde benötigen, können Sie eine neue Testversion erstellen.  <!-- and add the previous participants, new participants, or a mix of both. --> Sie können Informationen zu früheren Versionen und Teilnehmern in der Dokumentzusammenfassung anzeigen.

So fügen Sie eine neue Version hinzu:

1. Ziehen Sie die neue Datei per Drag-and-Drop auf das vorherige Dokument in Workfront. Dadurch wird automatisch eine neue Version erstellt.

1. Nachdem das Hochladen des Dokuments abgeschlossen ist, wählen Sie das Dokument aus und klicken Sie auf **Testversand erstellen** > **Einfacher Testversand**.

1. Wählen Sie das Dokument erneut aus und öffnen Sie die Dokumentzusammenfassung.
   ![](assets/open-doc-summary.png)

1. Scrollen Sie nach unten zum Abschnitt Genehmigungen und klicken Sie dann auf **Hinzufügen**.

1. (Optional) Wählen Sie eine vorhandene Validierungsvorlage aus. Benutzer mit einer Standardlizenz können im Bereich &quot;Setup&quot;wiederaufgenommene Genehmigungsvorlagen erstellen. Weitere Informationen finden Sie unter [Erstellen einer Genehmigungsvorlage für Assets und Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

1. (Optional) Legen Sie einen Termin für die Genehmigung fest. Benutzer und Teams werden per E-Mail 72 Stunden und 24 Stunden vor Ablauf der angegebenen Frist benachrichtigt.

1. Um einen Genehmiger hinzuzufügen, klicken Sie auf die Schaltfläche Genehmiger und beginnen Sie mit der Eingabe eines Benutzers oder Teams.

1. Um einen Validierer hinzuzufügen, klicken Sie auf die Schaltfläche Validierer und geben Sie den Namen des Benutzers oder Teams ein.

   ![](assets/add-approvers.png)

1. Nachdem Sie alle Prüfer und Genehmiger hinzugefügt haben, klicken Sie auf **Anfrage senden**. Teilnehmer werden per E-Mail benachrichtigt.

<!-- add info about reusing previous participants once released -->


## Testversand überprüfen und Entscheidung treffen

Das Dokument wechselt erst dann in den Status &quot;Genehmigt&quot;, wenn alle zugewiesenen Genehmiger &quot;Genehmigt&quot; wählen.

Wenn ein Genehmiger &quot;Arbeit erforderlich&quot;auswählt, ändert sich der Status des Dokuments sofort in &quot;Arbeiten erforderlich&quot;. Das Dokument muss überarbeitet und als neue Version mit einem neuen Genehmigungs-Workflow hochgeladen werden.

>[!IMPORTANT]
>
>Die Schaltflächen für Dokumententscheidungen werden nicht im Testversand-Viewer angezeigt. Sie müssen zurück zur Seite &quot;Dokumentzusammenfassung&quot;oder &quot;Dokumentdetails&quot;navigieren, um Ihre Entscheidung zu treffen oder die Überprüfung als abgeschlossen zu kennzeichnen.

So überprüfen und genehmigen Sie ein Dokument:

1. Rufen Sie Ihre E-Mail-Benachrichtigung zur Überprüfung auf und klicken Sie auf **Zum Review wechseln**.

1. Sobald Sie sich in Workfront befinden, klicken Sie auf **Zum Testversand wechseln**.

1. Überprüfen Sie den Inhalt und fügen Sie Kommentare oder Markierungen hinzu. Weitere Informationen zur Verwendung des Testversand-Viewers finden Sie unter [Testsendungen in Adobe Workfront überprüfen: Artikelindex](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Wenn Sie mit der Überprüfung fertig sind, schließen Sie den Testversand-Viewer.

1. Wenn Sie sich auf der Seite &quot;Dokumentdetails&quot;befinden, befinden sich die Entscheidungsschaltflächen in der oberen rechten Ecke des Bildschirms.

1. Wählen Sie eine der folgenden Entscheidungen:

   * **Genehmigen**: Das Dokument muss nicht geändert werden und kann verwendet werden.
   * **Mit Änderungen genehmigen**: Das Dokument muss geändert werden und kann verwendet werden, sobald es erstellt wurde. Eine zusätzliche Genehmigung ist nicht erforderlich.
   * **Erfordert Arbeit**: Das Dokument muss geändert werden und kann nicht verwendet werden. Sobald die angegebenen Änderungen vorgenommen wurden, muss das Dokument als neue Version hochgeladen werden und eine weitere Genehmigungsrunde durchlaufen. Weitere Informationen zum Hochladen einer neuen Version finden Sie unter [Erstellen einer neuen Version nach Bedarf](#create-a-new-version-as-needed) in diesem Artikel.

Sobald Sie eine Entscheidung treffen, wird der Dokumenteigentümer per E-Mail benachrichtigt.

