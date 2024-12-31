---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Einrichten eines Korrekturabzugs mit einem automatisierten Workflow in [!DNL Workfront Proof]
description: Dies wiederholt Informationen, die unter Konfigurieren von Testsendungen in Workfront zu finden sind. Hier oder dort konsolidieren. Vielleicht besser hier.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 0%

---

# Einrichten eines Testversands mit einem automatisierten Workflow in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Automatisierter Workflow erleichtert Ihnen die Verwaltung der Inhaltsüberprüfung und -validierung, wenn Sie komplexe Prüfprozesse haben oder wenn Sie Inhalte regelmäßig zur Überprüfung an dieselben Personengruppen senden.

Der Korrekturabzug wird erstellt und dann von Schritt zu Schritt bis zur endgültigen Genehmigung verschoben. Die relevanten Benutzer werden jedes Mal benachrichtigt, wenn sie eine Genehmigung erteilen müssen.

![stages_diagram.png](assets/stages-diagram-350x81.png)

Sie können einen automatisierten Workflow zu einem Korrekturabzug hinzufügen, wenn Sie das Dokument hochladen oder nachdem es hochgeladen wurde.

## Erstellen eines Korrekturabzugs mit einem automatisierten Workflow

1. Erstellen Sie den Korrekturabzug.
1. Klicken Sie im Abschnitt **[!UICONTROL Freigeben]** auf **[!UICONTROL Automatisierten Workflow verwenden]**.

   Sie können diese Option deaktivieren, um zu einem Standard-Workflow zurückzukehren.

1. (Optional) Wenn Sie eine automatisierte Workflow-Vorlage verwenden möchten, die Ihr [!DNL Workfront] konfiguriert und für Sie freigegeben hat, wählen Sie sie im Dropdown-Menü **[!UICONTROL Workflow-Vorlage]**.

   >[!NOTE]
   >
   >Welche Möglichkeiten Sie haben, die Vorlage zu ändern, hängt von den Vorlageneinstellungen ab, die vom [!DNL Workfront] konfiguriert wurden. Wenn die Möglichkeit, die Vorlage zu ändern, deaktiviert ist, kann nur der Besitzer der Vorlage sie ändern.

1. Geben Sie die folgenden Informationen an, um die erste Phase des automatisierten Workflows zu konfigurieren:

   * **[!UICONTROL Name]:** Der Name des Stadiums wird im Workflow-Diagramm angezeigt und ist in den E-Mail-Benachrichtigungen enthalten, die an Validierungsverantwortliche gesendet werden.
   * **[!UICONTROL Frist]:** Die Funktionalität dieses Felds unterscheidet sich je nachdem, welche Option Sie in der Dropdown-Liste **[!UICONTROL Frist berechnet]** auswählen.

   * **[!UICONTROL Von der Erstellung des Korrekturabzugs]:** Wählen Sie das Stichtag für den Korrekturabzug aus.
   * **[!UICONTROL Von Staging-Aktivierung]:** Wählen Sie die Anzahl der Werktage aus, die zum Staging-Aktivierungsdatum hinzugefügt werden sollen, um automatisch eine Frist für den Korrekturabzug festzulegen.
   * **[!UICONTROL Phase aktivieren]:** Sie können für jede Phase Ihres Workflows festlegen, wann sie aktiviert werden soll. Für das erste Stadium stehen die folgenden Optionen zur Verfügung.

      * Bei der Erstellung eines Korrekturabzugs
      * An einem bestimmten Datum und zu einer bestimmten Uhrzeit
      * Manuell\

        Für nachfolgende Phasen stehen zusätzliche Optionen zur Verfügung. Diese Optionen erfordern ein übergeordnetes Stadium. Sie sind:
      * Nach Ablauf der vorherigen Frist
      * Alle Entscheidungen werden genehmigt oder mit Änderungen genehmigt
      * Alle Entscheidungen werden genehmigt
      * Alle Entscheidungen werden getroffen
   * **[!UICONTROL Frist berechnet ab]:** Die Option, die Sie in dieser Dropdown-Liste auswählen, wirkt sich darauf aus, welche Optionen im Feld **[!UICONTROL Frist]** verfügbar sind.

   * **[!UICONTROL Testversand-Erstellung]:** Wählen Sie im Feld **[!UICONTROL Frist]** das Ablaufdatum für den Testversand aus.

   * **[!UICONTROL Staging-Aktivierung]:** Wählen Sie im Feld **[!UICONTROL Deadline]** die Anzahl der Werktage aus, die zum Staging-Aktivierungsdatum hinzugefügt werden, um automatisch eine Frist für den Korrekturabzug festzulegen.

   * **[!UICONTROL Phase sperren]:** Wählen Sie aus, wann die Phase gesperrt werden kann.
   * **[!UICONTROL Primärer Entscheidungsträger]:** Wählen Sie den Primären Entscheidungsträger auf der Bühne aus. Entscheidungsträger sind in der Dropdown-Liste erst verfügbar, nachdem Sie Reviewer zum Stadium hinzugefügt haben.
   * **[!UICONTROL Nur eine Entscheidung erforderlich]:** Wählen Sie diese Option, damit die Überprüfung abgeschlossen wird, nachdem einer der Entscheidungsträger seine Entscheidung getroffen hat.\

     Diese Option ist nicht verfügbar, wenn Sie im Dropdown-Menü **[!UICONTROL Primärer Entscheidungsträger]** einen Benutzer angegeben haben.

   * **[!UICONTROL Privater Schritt]:** Wenn diese Option aktiviert ist, sind Kommentare und Entscheidungen für Personen, die diesem Schritt nicht hinzugefügt wurden oder keine Supervisoren, Administratoren oder Abrechnungsadministratoren im Konto sind, nicht sichtbar


1. (Optional) Fügen Sie Reviewer zur Phase hinzu.
1. Beachten Sie beim Hinzufügen von Reviewern Folgendes:

   * Ein Prüfer kann einem Korrekturabzug nur einmal hinzugefügt werden. (Sie können dieselbe Person nicht zu mehr als einem Schritt im Korrekturabzug hinzufügen.)
   * Reviewer, die zu einer privaten Phase hinzugefügt werden, können nur die Phase sehen, zu der sie zum Korrekturabzug hinzugefügt werden, sowie Kommentare, die in dieser Phase eingegeben wurden.
   * Standardmäßig gewährt das Hinzufügen eines Benutzers zu einem Schritt diesem Benutzer Zugriff, um den Korrekturabzug ab dem Zeitpunkt anzuzeigen, zu dem der Korrekturabzug erstellt wird.\

     Der Systemadministrator kann das Proofing-System so konfigurieren, dass Benutzer erst dann auf den Korrekturabzug zugreifen können, wenn der Workflow in die Phase eintritt, in der der Benutzer hinzugefügt wurde. Weitere Informationen finden Sie unter

1. (Optional) Klicken Sie auf **[!UICONTROL Neue Phase]** und wiederholen Sie dann Schritt 4 und Schritt 5, um dem automatisierten Workflow mehrere Phasen hinzuzufügen.
1. Fahren Sie mit der Erstellung des Korrekturabzugs fort, indem Sie die erforderlichen Informationen in den Abschnitten  und [!UICONTROL Weitere Einstellungen] auf der Seite [!UICONTROL Neuer Korrekturabzug] angeben, wie in beschrieben

## Automatisierte Workflow-Diagramme

Beim Einrichten des Workflows für Ihren Korrekturabzug wird ein Diagramm erstellt. Jedes Stadium, das Sie Ihrem Korrekturabzug hinzufügen, wird im Diagramm angezeigt und zeigt die Abhängigkeiten zwischen den Stadien deutlich an. Private Stadien sind mit einem Schlüsselsymbol gekennzeichnet.

Das Diagramm ist unverankert, was bedeutet, dass es auch dann sichtbar bleibt, wenn Sie auf der Seite nach unten scrollen.

Wenn Sie das Diagramm nicht sehen müssen, können Sie es ausblenden (1).

![diagram.png](assets/diagram-350x93.png)

## Phase hinzufügen

Sie können einem Workflow, den Sie erstellen oder ändern, einen zusätzlichen Schritt hinzufügen.

1. Wenn Sie einen Schritt zu einem vorhandenen Korrekturabzug hinzufügen, gehen Sie zur Seite mit den Korrekturabzugsdetails, wie unter [Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.
1. Klicken Sie **[!UICONTROL Abschnitt]** Workflow“ auf **[!UICONTROL Neues]**.

1. Geben Sie Informationen für die Phase an, wie in Schritt 4 [!UICONTROL  Abschnitt „Erstellen eines Korrekturabzugs mit einem automatisierten Workflow] in diesem Artikel beschrieben.
1. Klicken Sie **[!UICONTROL Phase hinzufügen]** und dann auf **[!UICONTROL Fertig]**.

## Löschen eines Stadiums

1. Klicken Sie auf das Papierkorbsymbol oben rechts auf der Bühne (1).\
   Das Symbol wird angezeigt, wenn Sie den Mauszeiger über die Bühne bewegen.\
   ![deleting_a_stage.png](assets/deleting-a-stage-350x250.png)

## Staging-Einstellungen

* **[!UICONTROL Stufenname]**: Wird im Workflow-Diagramm angezeigt und ist in den E-Mail-Benachrichtigungen enthalten, die an Prüfende gesendet werden.
* **[!UICONTROL Phase aktivieren]**: Sie können für jede Phase Ihres Workflows festlegen, wann sie aktiviert werden soll. Für das erste Stadium stehen die folgenden Optionen zur Verfügung:

   * Bei der Erstellung eines Korrekturabzugs
   * An einem bestimmten Datum und zu einer bestimmten Uhrzeit
   * Manuell
   * Für das erste Stadium stehen nur diese drei Optionen zur Verfügung. Die anderen Optionen werden verfügbar, wenn Sie ein zweites Stadium hinzufügen. Sie erfordern, dass Sie ein übergeordnetes Stadium auswählen.
   * Nach Erreichen der vorherigen Frist (erfordert die Auswahl eines übergeordneten Stadiums)
   * Alle Entscheidungen werden genehmigt oder [!UICONTROL Mit Änderungen genehmigt] (erfordert die Auswahl eines übergeordneten Schritts)
   * Alle Entscheidungen sind genehmigt (erfordert die Auswahl eines übergeordneten Schritts)
   * Alle Entscheidungen werden getroffen (erfordert die Auswahl eines übergeordneten Schritts)

* **[!UICONTROL Frist]:** Sie können festlegen, wie die Frist in jedem Schritt eines Workflows berechnet werden soll. Die Optionen sind:

   * Bei der Erstellung des Korrekturabzugs: Im Feld [!UICONTROL Frist] (9) können Sie das Fristdatum für den Korrekturabzug auswählen.
   * Aus der Staging-Aktivierung[!UICONTROL  Wählen Sie in der Dropdown]Liste „Frist“ die Anzahl der Werktage aus, die zum Staging-Aktivierungsdatum hinzugefügt werden sollen, um automatisch eine Frist für den Korrekturabzug festzulegen.

* **[!UICONTROL lock]:** Es gibt eine Reihe von Optionen, die bestimmen, wann ein Schritt gesperrt werden kann. Zu den Optionen gehören:

   * Manuelle Sperre
   * Nie
   * Wenn die nächste Phase beginnt
   * Wenn alle Entscheidungen getroffen werden

**[!UICONTROL Primärer Entscheidungsträger]**: Sie bestimmen den Primären Entscheidungsträger auf der Bühne. Die verfügbaren Entscheidungsträger werden erst in der Liste angezeigt, nachdem Sie die Reviewer zur Stage hinzugefügt haben.

>[!NOTE]
>
>Wenn Sie einen Primären Entscheidungsträger auswählen, ist auf dieser Phase nur eine Option für Entscheidungserfordernisse nicht mehr verfügbar.

* **[!UICONTROL Nur eine Entscheidung erforderlich]**: Sie können diese Option in einem Stadium aktivieren. Dies bedeutet, dass die Überprüfung abgeschlossen sein wird, sobald einer der Entscheidungsträger seine Entscheidung trifft.
* **[!UICONTROL Datenschutz]:** Jede Phase kann als privat festgelegt werden. Wenn ein Schritt privat ist, sind die Kommentare und Entscheidungen für Personen, die diesem Schritt nicht hinzugefügt wurden oder keine Supervisoren, Administratoren oder Abrechnungsadministratoren im Konto sind, nicht sichtbar. Weitere Informationen finden Sie unter [Automatisierter Workflow - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Hinzufügen von Reviewern zu einem Schritt

1. Geben Sie unten in jedem Schritt einen Kontaktnamen oder eine E-Mail-Adresse in das Feld ein.
1. Klicken Sie auf das grüne Pluszeichen, um sie hinzuzufügen.
1. Legen Sie die Rolle für den Korrekturabzug fest.
1. E-Mail-Warnhinweis einrichten
1. Beim Einrichten des ersten Schritts haben Sie auch die Möglichkeit, den Verantwortlichen für den Korrekturabzug zu ändern.

   >[!NOTE]
   >
   >* Ein Prüfer kann einem Korrekturabzug nur einmal hinzugefügt werden. Dieselbe Person kann nicht zu mehr als einem Schritt im Korrekturabzug hinzugefügt werden.
   >* Prüfer, die nicht zu einer privaten Phase hinzugefügt wurden, können die Phase auf dem Korrekturabzug oder den Kommentaren in dieser Phase nicht sehen.


## Konvertieren eines Korrekturabzugs in einen automatisierten Workflow

Sie können einen einfachen Korrekturabzug in einen automatisierten Workflow konvertieren.

1. Klicken Sie **[!UICONTROL der Seite [!UICONTROL Korrekturabzugsdetails] auf In automatisierten Workflow]**.
Nachdem der Korrekturabzug in einen automatisierten Workflow überarbeitet wurde, sind alle Phasen aktiv und öffentlich, und ihre Option [!UICONTROL Phase sperren] ist standardmäßig auf Manuell festgelegt. Alle Stadien bleiben bei den Benutzenden und ihren Einstellungen.

   * Die Phase „Aktivieren“ ist in jedem Schritt auf Bei der Erstellung eines Korrekturabzugs eingestellt.
   * Die von der Option berechnete Frist wird in jedem Schritt auf die Erstellung von Korrekturabzügen festgelegt.
   * Wenn für den grundlegenden Korrekturabzug nur eine Entscheidungsoption ausgewählt wurde, ist sie für alle Phasen ausgewählt.
   * Wenn ein einfacher Korrekturabzug [!UICONTROL Primärer Entscheidungsträger] ausgewählt wurde, werden Etappen mit diesem Empfänger auf ihn festgelegt und alle anderen auf „Keine“ gesetzt.
   * Der Name des Stadiums bleibt gleich.

## Hinzufügen einer zusätzlichen Vorlage zu einem vorhandenen automatisierten Workflow

Nachdem ein einfacher Korrekturabzug in einen automatisierten Workflow konvertiert wurde, können Sie ihm zusätzliche Vorlagen hinzufügen.

1. Klicken Sie auf der Seite mit den Korrekturabzugsdetails im Abschnitt Workflow auf **[!UICONTROL Vorlage hinzufügen].**

   * Vorlageneinstellungen bestimmen, was mit einem Korrekturabzug getan werden kann, dem diese Vorlage hinzugefügt wurde. Wenn in der Vorlage beispielsweise die Optionen [!UICONTROL Phase hinzufügen und Personen zu Phasen hinzufügen] deaktiviert sind, werden die Schaltflächen [!UICONTROL Phase hinzufügen] und [!UICONTROL Korrekturabzug ].
   * Wenn [!UICONTROL Option „Stadium hinzufügen] in der angegebenen Vorlage deaktiviert ist, ist nach dem Hinzufügen die Schaltfläche [!UICONTROL Vorlage hinzufügen] nicht sichtbar.
   * Wenn eine Person zu einem Schritt in einer automatisierten Workflow-Vorlage hinzugefügt wird, aber auch bereits im Korrekturabzug vorhanden ist, entfernt das System diese Person automatisch aus dem Schritt, wenn diese Vorlage angewendet wird. Wenn zu diesem Schritt keine weitere Person hinzugefügt wird, wird der folgende Fehler angezeigt, da das System das Hinzufügen einer leeren Phase zum Workflow nicht zulässt.

     ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
