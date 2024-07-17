---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Einrichten eines Testversands mit einem automatisierten Workflow in [!DNL Workfront Proof]
description: Dadurch werden die Informationen unter Testsendungen in Workfront konfigurieren wiederholt. Konsolidieren Sie hier oder dort. Vielleicht besser hier.
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
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Der automatisierte Workflow erleichtert die Verwaltung von Inhaltsüberprüfungen und -genehmigungen, wenn komplexe Überprüfungsprozesse vorliegen oder wenn Sie regelmäßig Inhalte zur Überprüfung an dieselben Personengruppen senden.

Sie erstellen den Testversand und wechseln dann von der Phase zur Phase bis zur endgültigen Validierung. Die betroffenen Benutzer werden jedes Mal benachrichtigt, wenn sie eine Genehmigung vornehmen müssen.

![stage_diagramm.png](assets/stages-diagram-350x81.png)

Sie können einem Testversand beim Hochladen des Dokuments oder nach dem Hochladen des Dokuments einen automatisierten Workflow hinzufügen.

## Erstellen eines Testversands mit automatisiertem Workflow

1. Erstellen Sie den Testversand.
1. Klicken Sie im Abschnitt **[!UICONTROL Freigabe]** auf **[!UICONTROL Automatisierten Workflow verwenden]**.

   Sie können diese Option deaktivieren, um zu einem standardmäßigen Workflow zurückzukehren.

1. (Optional) Wenn Sie eine Vorlage für einen automatisierten Workflow verwenden möchten, die Ihr [!DNL Workfront] -Administrator für Sie konfiguriert und freigegeben hat, wählen Sie sie im Dropdownmenü **[!UICONTROL Workflow-Vorlage auswählen]** aus.

   >[!NOTE]
   >
   >Ihre Fähigkeit, die Vorlage zu ändern, hängt von den Vorlageneinstellungen ab, die vom [!DNL Workfront] -Administrator konfiguriert wurden. Wenn die Möglichkeit zur Änderung der Vorlage deaktiviert ist, kann sie nur vom Inhaber der Vorlage geändert werden.

1. Geben Sie die folgenden Informationen an, um den ersten Schritt des automatisierten Workflows zu konfigurieren:

   * **[!UICONTROL Name]:** Der Staging-Name wird im Workflow-Diagramm angezeigt und ist in den an die Validierer gesendeten E-Mail-Benachrichtigungen enthalten.
   * **[!UICONTROL Deadline]:** Die Funktionalität dieses Felds hängt davon ab, welche Option Sie in der Dropdownliste **[!UICONTROL Aus der Dropdownliste]** berechnete Frist auswählen.

   * **[!UICONTROL Aus der Testversand-Erstellung]:** Wählen Sie das Stichtag für den Testversand aus.
   * **[!UICONTROL Von der Staging-Aktivierung]:** Wählen Sie die Anzahl der Geschäftstage aus, die zum Staging-Aktivierungsdatum hinzugefügt werden, um automatisch einen Termin für den Testversand festzulegen.
   * **[!UICONTROL Phase aktivieren]:** Sie können für jede Phase Ihres Workflows entscheiden, wann sie aktiviert werden soll. Für den ersten Schritt stehen die folgenden Optionen zur Verfügung.

      * Erstellen eines Testversands
      * Zu einem bestimmten Zeitpunkt und Datum
      * Manuell\

        Für nachfolgende Phasen stehen zusätzliche Optionen zur Verfügung. Diese Optionen erfordern eine übergeordnete Phase. Sie sind:
      * Nach Ablauf der vorherigen Frist
      * Alle Entscheidungen werden mit Änderungen genehmigt oder genehmigt
      * Alle Entscheidungen werden genehmigt
      * Alle Entscheidungen werden getroffen
   * **[!UICONTROL Aus ] berechnete Frist:** Die Option, die Sie in dieser Dropdownliste auswählen, wirkt sich darauf aus, welche Optionen im Feld **[!UICONTROL Frist]** verfügbar sind.

   * **[!UICONTROL Erstellung des Testversands]:** Wählen Sie im Feld **[!UICONTROL Frist]** das Datum für den Testversand aus.

   * **[!UICONTROL Staging-Aktivierung]:** Wählen Sie im Feld **[!UICONTROL Deadline]** die Anzahl der Geschäftstage aus, die zum Staging-Aktivierungsdatum hinzugefügt werden, um automatisch einen Termin für den Testversand festzulegen.

   * **[!UICONTROL Bühne sperren]:** Wählen Sie aus, wann die Bühne gesperrt werden kann.
   * **[!UICONTROL Primärer Entscheidungsträger]:** Wählen Sie den Primären Entscheidungsträger auf der Bühne aus. Entscheidungsträger sind erst dann in der Dropdown-Liste verfügbar, wenn Sie Überprüfer zur Bühne hinzufügen.
   * **[!UICONTROL Nur eine Entscheidung erforderlich]:** Wählen Sie diese Option, damit die Überprüfung abgeschlossen wird, nachdem ein Entscheidungsträger seine Entscheidung getroffen hat.\

     Diese Option ist nicht verfügbar, wenn Sie einen Benutzer im Dropdownmenü **[!UICONTROL Primärer Entscheidungsträger]** ausgewählt haben.

   * **[!UICONTROL Private Bühne]:** Wenn diese Option ausgewählt ist, sind Kommentare und Entscheidungen nicht für Personen sichtbar, die nicht zu dieser Phase hinzugefügt wurden oder keine Supervisoren, Administratoren oder Rechnungsadministratoren im Konto sind


1. (Optional) Fügen Sie Überprüfer zur Bühne hinzu.
1. Beachten Sie beim Hinzufügen von Validierungsverantwortlichen Folgendes:

   * Ein Validierer kann einem Testversand nur einmal hinzugefügt werden. (Sie können dieselbe Person nicht zu mehr als einer Testphase hinzufügen.)
   * Überprüfer, die einer privaten Bühne hinzugefügt werden, können nur die Bühne sehen, der sie auf dem Testversand und den Kommentaren in dieser Phase hinzugefügt wurden.
   * Wenn ein Benutzer zu einer Phase hinzugefügt wird, erhält dieser Benutzer standardmäßig Zugriff auf den Testversand ab der Erstellung des Testversands.\

     Der Systemadministrator kann das Testsystem so konfigurieren, dass Benutzer nur dann auf den Testversand zugreifen können, wenn der Workflow in die Phase gelangt, in der der Benutzer hinzugefügt wurde. Weitere Informationen finden Sie unter

1. (Optional) Klicken Sie auf **[!UICONTROL Neue Phase]** und wiederholen Sie dann Schritt 4 und Schritt 5, um dem automatisierten Workflow mehrere Phasen hinzuzufügen.
1. Fahren Sie mit der Erstellung des Testversands fort, indem Sie die erforderlichen Informationen in den Abschnitten [!UICONTROL Organisieren] und [!UICONTROL Weitere Einstellungen] auf der Seite [!UICONTROL Neuer Testversand] angeben, wie unter

## Automatisierte Workflow-Diagramme

Beim Einrichten des Workflows für Ihren Testversand wird Ihnen ein Diagramm angezeigt, das erstellt wird. Jede Etappe, die Sie Ihrem Testversand hinzufügen, wird im Diagramm angezeigt, was die Abhängigkeiten zwischen den Phasen deutlich angibt. Private Bühnen sind mit einem Schlüsselsymbol gekennzeichnet.

Das Diagramm schwebt, was bedeutet, dass es auch dann sichtbar bleibt, wenn Sie nach unten scrollen.

Wenn Sie das Diagramm nicht sehen müssen, können Sie es verbergen (1).

![diagram.png](assets/diagram-350x93.png)

## Hinzufügen einer Bühne

Sie können einem Workflow, den Sie erstellen oder ändern, eine zusätzliche Phase hinzufügen.

1. Wenn Sie eine Phase zu einem vorhandenen Testversand hinzufügen, gehen Sie zur Seite mit den Testversanddetails, wie unter [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md) beschrieben.
1. Klicken Sie im Abschnitt **[!UICONTROL Workflow]** auf **[!UICONTROL Neue Phase]**.

1. Geben Sie Informationen für die Phase wie in Schritt 4 unter dem Abschnitt [!UICONTROL Erstellen eines Testversands mit einem automatisierten Workflow] in diesem Artikel an.
1. Klicken Sie auf **[!UICONTROL Phase hinzufügen]** und dann auf **[!UICONTROL Fertig]**.

## Löschen einer Phase

1. Klicken Sie auf das Papierkorbsymbol oben rechts auf der Bühne (1).\
   Das Symbol wird angezeigt, wenn Sie den Mauszeiger über die Bühne bewegen.\
   ![Löschen_a_stage.png](assets/deleting-a-stage-350x250.png)

## Staging-Einstellungen

* **[!UICONTROL Staging-Name]**: Wird im Workflow-Diagramm angezeigt und ist in den an die Validierer gesendeten E-Mail-Benachrichtigungen enthalten.
* **[!UICONTROL Phase aktivieren]**: Sie können für jede Phase Ihres Workflows entscheiden, wann sie aktiviert werden soll. Für den ersten Schritt stehen folgende Optionen zur Verfügung:

   * Erstellen eines Testversands
   * Zu einem bestimmten Zeitpunkt und Datum
   * Manuell
   * Für den ersten Schritt stehen nur diese drei Optionen zur Verfügung. Die anderen Optionen werden verfügbar, wenn Sie eine zweite Phase hinzufügen. Sie müssen eine übergeordnete Phase auswählen.
   * Nach Ablauf der vorherigen Frist (Auswahl einer übergeordneten Phase erforderlich)
   * Alle Entscheidungen werden genehmigt oder [!UICONTROL mit Änderungen genehmigt] (erfordert die Auswahl einer übergeordneten Phase)
   * Alle Entscheidungen werden genehmigt (Auswahl einer übergeordneten Phase erforderlich)
   * Alle Entscheidungen werden getroffen (es muss eine übergeordnete Phase ausgewählt werden)

* **[!UICONTROL Deadline]:** Sie können festlegen, wie der Termin in jeder Workflow-Phase berechnet werden soll. Die Optionen sind:

   * Von der Erstellung des Testversands: Im Feld [!UICONTROL Deadline] (9) können Sie das Deadline-Datum für den Testversand auswählen.
   * Von der Staging-Aktivierung: Wählen Sie in der Dropdown-Liste [!UICONTROL Deadline] die Anzahl der Geschäftstage aus, die zum Staging-Aktivierungsdatum hinzugefügt werden, um automatisch einen Termin für den Testversand festzulegen.

* **[!UICONTROL Sperren]:** Es gibt eine Reihe von Optionen, die bestimmen, wann eine Bühne gesperrt werden kann. Zu den Optionen gehören:

   * Manuelle Sperre
   * Nie
   * Wenn die nächste Phase beginnt
   * Wann alle Entscheidungen getroffen werden

**[!UICONTROL Primärer Entscheidungsträger]**: Sie legen den Primären Entscheidungsträger auf der Bühne fest. Die verfügbaren Entscheidungsträger werden erst in der Liste angezeigt, nachdem Sie die Prüfer zur Bühne hinzugefügt haben.

>[!NOTE]
>
>Wenn Sie einen Primären Entscheidungsträger auswählen, ist in dieser Phase nicht mehr nur eine Entscheidungsoption verfügbar.

* **[!UICONTROL Nur eine Entscheidung erforderlich]**: Sie können diese Option auf einer Bühne aktivieren. Dies bedeutet, dass die Überprüfung abgeschlossen wird, sobald einer der Entscheidungsträger seine Entscheidung trifft.
* **[!UICONTROL Datenschutz]:** Jede Phase kann privat gemacht werden. Wenn eine Bühne privat ist, sind die Kommentare und Entscheidungen nicht für Personen sichtbar, die nicht zu dieser Phase hinzugefügt wurden oder keine Supervisoren, Administratoren oder Rechnungsadministratoren in dem Konto sind. Weitere Informationen finden Sie unter [Überblick über den automatisierten Workflow](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Hinzufügen von Validierern zu einer Phase

1. Geben Sie unten in jeder Phase einen Kontaktnamen oder eine E-Mail-Adresse in das Feld ein.
1. Klicken Sie auf das grüne Pluszeichen, um sie hinzuzufügen.
1. Legen Sie die Rolle auf dem Testversand fest.
1. Setzen Sie den E-Mail-Warnhinweis.
1. Beim Einrichten der ersten Phase haben Sie auch die Möglichkeit, den Inhaber des Testversands zu ändern.

   >[!NOTE]
   >
   >* Ein Validierer kann einem Testversand nur einmal hinzugefügt werden. Dieselbe Person kann nicht zu mehr als einer Testphase hinzugefügt werden.
   >* Überprüfer, die nicht zu einer privaten Bühne hinzugefügt wurden, können die Bühne des Testversands oder der in dieser Phase abgegebenen Kommentare nicht sehen.


## Konvertieren eines Testversands in einen automatisierten Workflow

Sie können einen einfachen Testversand in den automatisierten Workflow konvertieren.

1. Klicken Sie auf der Seite [!UICONTROL Testversand-Details] auf **[!UICONTROL In automatisierten Workflow konvertieren]** .
Nachdem der Testversand in den automatisierten Workflow überarbeitet wurde, sind alle Phasen aktiv, öffentlich und ihre Option [!UICONTROL Phase sperren] ist standardmäßig auf Manuell eingestellt. Alle Phasen verbleiben bei den Benutzern und deren Einstellungen.

   * Die Phase &quot;Aktivieren&quot;ist in jeder Phase auf Die Erstellung eines Testversands eingestellt.
   * Die von der Option berechnete Frist ist in jeder Phase auf die Erstellung eines Testversands festgelegt.
   * Wenn nur eine Entscheidungsoption für den Basisnachweis ausgewählt wurde, wird sie in allen Phasen ausgewählt.
   * Wenn bei einem einfachen Testversand [!UICONTROL Primärer Entscheidungsträger] ausgewählt wurde, werden Bühnen mit diesem Empfänger auf ihn gesetzt und bei allen anderen auf Ohne gesetzt.
   * Der Staging-Name bleibt derselbe.

## Hinzufügen einer zusätzlichen Vorlage zu einem vorhandenen automatisierten Workflow

Nachdem ein grundlegender Testversand in den automatisierten Workflow konvertiert wurde, können Sie ihm zusätzliche Vorlage hinzufügen.

1. Klicken Sie auf der Seite mit den Testversanddetails im Abschnitt &quot;Workflow&quot;auf **[!UICONTROL Vorlage hinzufügen].**

   * Die Vorlageneinstellungen bestimmen, was mit einem Testversand durchgeführt werden kann, dem diese Vorlage hinzugefügt wurde. Wenn beispielsweise in der Vorlage die Optionen [!UICONTROL Phase hinzufügen und Personen zu Bühnen hinzufügen] deaktiviert sind, sind Schaltflächen zum Hinzufügen von [!UICONTROL Bühne hinzufügen] und zum Hinzufügen von [!UICONTROL Testsendungen freigeben] nicht sichtbar.
   * Wenn [!UICONTROL Hinzufügen einer Staging-Option] in der angegebenen Vorlage deaktiviert ist, ist die Schaltfläche [!UICONTROL Vorlage hinzufügen] nach dem Hinzufügen nicht sichtbar.
   * Wenn eine Person einer Bühne in einer Vorlage für automatisierte Workflows hinzugefügt, aber bereits im Testversand vorhanden ist, entfernt das System diese Person automatisch aus der Bühne, wenn diese Vorlage angewendet wird. Wenn zu dieser Phase niemand anderes hinzugefügt wurde, wird der folgende Fehler angezeigt, da das System keine leere Phase zum Workflow hinzufügen kann.

     ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
