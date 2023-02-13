---
product-previous: workfront-proof
product-area: documents
navigation-topic: automated-workflow-workfront-proof
title: Einen Testversand mit einem automatisierten Workflow einrichten in [!DNL Workfront Proof]
description: Dadurch werden die Informationen unter Testsendungen in Workfront konfigurieren wiederholt. Konsolidieren Sie hier oder dort. Vielleicht besser hier.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 605569df-8e63-476d-a0cd-e73802042011
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1637'
ht-degree: 0%

---

# Einen Testversand mit einem automatisierten Workflow einrichten in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Der automatisierte Workflow erleichtert die Verwaltung von Inhaltsüberprüfungen und -genehmigungen, wenn komplexe Überprüfungsprozesse vorliegen oder wenn Sie regelmäßig Inhalte zur Überprüfung an dieselben Personengruppen senden.

Sie erstellen den Testversand und wechseln dann von der Phase zur Phase bis zur endgültigen Validierung. Die betroffenen Benutzer werden jedes Mal benachrichtigt, wenn sie eine Genehmigung vornehmen müssen.

![states_chart.png](assets/stages-diagram-350x81.png)

Sie können einem Testversand beim Hochladen des Dokuments oder nach dem Hochladen des Dokuments einen automatisierten Workflow hinzufügen.

## Erstellen eines Testversands mit automatisiertem Workflow

1. Beginnen Sie mit der Erstellung des Testversands.
1. Im **[!UICONTROL Freigeben]** Abschnitt, klicken Sie auf **[!UICONTROL Automatisierte Workflows verwenden]**.

   Sie können diese Option deaktivieren, um zu einem standardmäßigen Workflow zurückzukehren.

1. (Optional) Wenn Sie eine Automated Workflow-Vorlage verwenden möchten, die Ihre [!DNL Workfront] Administrator konfiguriert und für Sie freigegeben haben, wählen Sie ihn im **[!UICONTROL Auswählen einer Workflow-Vorlage]** Dropdown-Menü.

   >[!NOTE]
   >
   >Ihre Fähigkeit, die Vorlage zu ändern, hängt von den Vorlageneinstellungen ab, die von der [!DNL Workfront] Administrator. Wenn die Möglichkeit zur Änderung der Vorlage deaktiviert ist, kann sie nur vom Inhaber der Vorlage geändert werden.

1. Geben Sie die folgenden Informationen an, um den ersten Schritt des automatisierten Workflows zu konfigurieren:

   * **[!UICONTROL Name]:** Der Staging-Name erscheint im Workflow-Diagramm und ist in den E-Mail-Benachrichtigungen enthalten, die an die Validierer gesendet werden.
   * **[!UICONTROL Termin]:** Die Funktionalität dieses Felds variiert je nach ausgewählter Option im **[!UICONTROL Errechneter Termin]** Dropdown-Liste.

   * **[!UICONTROL Erstellen von Testsendungen]:** Wählen Sie das Stichtag für den Testversand aus.
   * **[!UICONTROL Von der Staging-Aktivierung]:** Wählen Sie die Anzahl der Geschäftstage aus, die zum Aktivierungsdatum der Bühne hinzugefügt werden, um automatisch einen Termin für den Testversand festzulegen.
   * **[!UICONTROL Phase aktivieren]:** Sie können für jede Workflow-Phase entscheiden, wann der Workflow aktiviert werden soll. Für den ersten Schritt stehen die folgenden Optionen zur Verfügung.

      * Erstellen eines Testversands
      * Zu einem bestimmten Zeitpunkt und Datum
      * Manuell\

         Für nachfolgende Phasen stehen zusätzliche Optionen zur Verfügung. Diese Optionen erfordern eine übergeordnete Phase. Sie sind:
      * Nach Ablauf der vorherigen Frist
      * Alle Entscheidungen werden mit Änderungen genehmigt oder genehmigt
      * Alle Entscheidungen werden genehmigt
      * Alle Entscheidungen werden getroffen
   * **[!UICONTROL Errechneter Termin]:** Die Option, die Sie in dieser Dropdown-Liste auswählen, wirkt sich darauf aus, welche Optionen in der **[!UICONTROL Termin]** -Feld.

   * **[!UICONTROL Erstellung von Testsendungen]:** Im **[!UICONTROL Termin]** das Datum des Testversands festlegen.

   * **[!UICONTROL Staging-Aktivierung]:** Im **[!UICONTROL Termin]** Geben Sie die Anzahl der Geschäftstage an, die zum Aktivierungsdatum der Bühne hinzugefügt werden, um automatisch einen Termin für den Testversand festzulegen.

   * **[!UICONTROL Bühne sperren]:** Wählen Sie aus, wann die Bühne gesperrt werden kann.
   * **[!UICONTROL Primärer Entscheidungsträger]:** Wählen Sie den Primären Entscheidungsträger auf der Bühne aus. Entscheidungsträger sind erst dann in der Dropdownliste verfügbar, wenn Sie Überprüfer zur Bühne hinzufügen.
   * **[!UICONTROL Nur eine Entscheidung erforderlich]:** Wählen Sie diese Option, damit die Überprüfung abgeschlossen wird, nachdem einer der Entscheidungsträger seine Entscheidung getroffen hat.\

      Diese Option ist nicht verfügbar, wenn Sie einen Benutzer in der **[!UICONTROL Primärer Entscheidungsträger]** Dropdown-Menü.

   * **[!UICONTROL Private Bühne]:** Wenn diese Option aktiviert ist, sind Kommentare und Entscheidungen für Personen nicht sichtbar, die nicht zu dieser Phase hinzugefügt wurden oder keine Supervisoren, Administratoren oder Rechnungsadministratoren im Konto sind


1. (Optional) Fügen Sie Überprüfer zur Bühne hinzu.
1. Beachten Sie beim Hinzufügen von Validierungsverantwortlichen Folgendes:

   * Ein Validierer kann einem Testversand nur einmal hinzugefügt werden. (Sie können dieselbe Person nicht zu mehr als einer Testphase hinzufügen.)
   * Überprüfer, die einer privaten Bühne hinzugefügt werden, können nur die Bühne sehen, der sie auf dem Testversand und den Kommentaren in dieser Phase hinzugefügt wurden.
   * Wenn ein Benutzer zu einer Phase hinzugefügt wird, erhält dieser Benutzer standardmäßig Zugriff auf den Testversand ab der Erstellung des Testversands.\

      Der Systemadministrator kann das Testsystem so konfigurieren, dass Benutzer nur dann auf den Testversand zugreifen können, wenn der Workflow in die Phase gelangt, in der der Benutzer hinzugefügt wurde. Weitere Informationen finden Sie unter

1. (Optional) Klicken Sie auf **[!UICONTROL Neue Phase]** und wiederholen Sie dann Schritt 4 und Schritt 5, um dem automatisierten Workflow mehrere Phasen hinzuzufügen.
1. Fahren Sie mit der Erstellung des Testversands fort, indem Sie die erforderlichen Informationen im Abschnitt [!UICONTROL Organisieren] und [!UICONTROL Weitere Einstellungen] in den [!UICONTROL Neuer Testversand] Seite, wie beschrieben in

## Automatisierte Workflow-Diagramme

Beim Einrichten des Workflows für Ihren Testversand wird Ihnen ein Diagramm angezeigt, das erstellt wird. Jede Etappe, die Sie Ihrem Testversand hinzufügen, wird im Diagramm angezeigt und zeigt die Abhängigkeiten zwischen den Phasen deutlich an. Private Bühnen sind mit einem Schlüsselsymbol gekennzeichnet.

Das Diagramm schwebt, was bedeutet, dass es auch dann sichtbar bleibt, wenn Sie nach unten scrollen.

Wenn Sie das Diagramm nicht sehen müssen, können Sie es verbergen (1).

![Diagramm.png](assets/diagram-350x93.png)

## Hinzufügen einer Bühne

Sie können einem Workflow, den Sie erstellen oder ändern, eine zusätzliche Phase hinzufügen.

1. Wenn Sie eine Stufe zu einem vorhandenen Testversand hinzufügen, gehen Sie zur Seite Testversand-Details , wie hier beschrieben: [Testversanddetails verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Im **[!UICONTROL Workflow]** Abschnitt, klicken Sie auf **[!UICONTROL Neue Phase]**.

1. Geben Sie Informationen für die Phase wie in Schritt 4 unter dem [!UICONTROL Erstellen eines Testversands mit einem automatisierten Workflow] in diesem Artikel.
1. Klicken **[!UICONTROL Phase hinzufügen]** Klicken Sie auf **[!UICONTROL Fertig]**.

## Löschen einer Phase

1. Klicken Sie auf das Papierkorbsymbol oben rechts auf der Bühne (1).\
   Das Symbol wird angezeigt, wenn Sie den Mauszeiger über die Bühne bewegen.\
   ![deleting_a_stage.png](assets/deleting-a-stage-350x250.png)

## Staging-Einstellungen

* **[!UICONTROL Staging-Name]**: Wird im Workflow-Diagramm angezeigt und ist in den an die Validierer gesendeten E-Mail-Benachrichtigungen enthalten.
* **[!UICONTROL Phase aktivieren]**: Sie können für jede Workflow-Phase entscheiden, wann der Workflow aktiviert werden soll. Für den ersten Schritt stehen folgende Optionen zur Verfügung:

   * Erstellen eines Testversands
   * Zu einem bestimmten Zeitpunkt und Datum
   * Manuell
   * Für den ersten Schritt stehen nur diese drei Optionen zur Verfügung. Die anderen Optionen werden verfügbar, wenn Sie eine zweite Phase hinzufügen. Sie müssen eine übergeordnete Phase auswählen.
   * Nach Ablauf der vorherigen Frist (Auswahl einer übergeordneten Phase erforderlich)
   * Alle Entscheidungen werden genehmigt oder [!UICONTROL Genehmigt mit Änderungen] (Auswahl einer übergeordneten Phase erforderlich)
   * Alle Entscheidungen werden genehmigt (Auswahl einer übergeordneten Phase erforderlich)
   * Alle Entscheidungen werden getroffen (es muss eine übergeordnete Phase ausgewählt werden)

* **[!UICONTROL Termin]:** Sie können festlegen, wie der Termin in jeder Workflow-Phase berechnet werden soll. Die Optionen sind:

   * Von der Erstellung des Testversands: Im [!UICONTROL deadline] Feld (9) können Sie das Datum für den Testversand auswählen.
   * Von der Staging-Aktivierung: Im [!UICONTROL deadline] in der Dropdown-Liste die Anzahl der Geschäftstage auswählen, die zum Aktivierungsdatum der Bühne hinzugefügt werden, um automatisch einen Termin für den Testversand festzulegen.

* **[!UICONTROL Sperren]:** Es gibt verschiedene Optionen, die bestimmen, wann eine Phase gesperrt werden kann. Zu den Optionen gehören:

   * Manuelle Sperre
   * Nie
   * Wenn die nächste Phase beginnt
   * Wann alle Entscheidungen getroffen werden

**[!UICONTROL Primärer Entscheidungsträger]**: Du stellst den Primären Entscheidungsträger auf die Bühne. Die verfügbaren Entscheidungsträger werden erst in der Liste angezeigt, nachdem Sie die Prüfer zur Bühne hinzugefügt haben.

>[!NOTE]
>
>Wenn Sie einen Primären Entscheidungsträger auswählen, ist in dieser Phase nicht mehr nur eine Entscheidungsoption verfügbar.

* **[!UICONTROL Nur eine Entscheidung erforderlich]**: Sie können diese Option auf einer Bühne aktivieren. Dies bedeutet, dass die Überprüfung abgeschlossen wird, sobald einer der Entscheidungsträger seine Entscheidung trifft.
* **[!UICONTROL Datenschutz]:** Jede Bühne kann privat gemacht werden. Wenn eine Bühne privat ist, sind die Kommentare und Entscheidungen nicht für Personen sichtbar, die nicht zu dieser Phase hinzugefügt wurden oder keine Supervisoren, Administratoren oder Rechnungsadministratoren in dem Konto sind. Weitere Informationen finden Sie unter [Übersicht über den automatisierten Workflow](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md) .

## Hinzufügen von Validierern zu einer Phase

1. Geben Sie unten in jeder Phase einen Kontaktnamen oder eine E-Mail-Adresse in das Feld ein.
1. Klicken Sie auf das grüne Pluszeichen, um sie hinzuzufügen.
1. Legen Sie die Rolle beim Testversand fest.
1. Setzen Sie den E-Mail-Warnhinweis.
1. Beim Einrichten der ersten Phase haben Sie auch die Möglichkeit, den Inhaber des Testversands zu ändern.

   >[!NOTE]
   >
   >* Ein Validierer kann einem Testversand nur einmal hinzugefügt werden. Dieselbe Person kann nicht zu mehr als einer Testphase hinzugefügt werden.
   >* Überprüfer, die nicht zu einer privaten Bühne hinzugefügt wurden, können die Bühne des Testversands oder der in dieser Phase abgegebenen Kommentare nicht sehen.



## Konvertieren eines Testversands in einen automatisierten Workflow

Sie können einen einfachen Testversand in den automatisierten Workflow konvertieren.

1. Klicken **[!UICONTROL In automatisierten Workflow konvertieren]** auf [!UICONTROL Testversanddetails] Seite.
Nachdem der Testversand in den automatisierten Workflow überarbeitet wurde, sind alle Phasen aktiv, öffentlich und ihre [!UICONTROL Bühne sperren] ist standardmäßig auf Manuell eingestellt. Alle Phasen verbleiben bei den Benutzern und deren Einstellungen.

   * Die Phase &quot;Aktivieren&quot;ist in jeder Phase auf Die Erstellung eines Testversands eingestellt.
   * Die von der Option berechnete Frist ist in jeder Phase auf die Erstellung eines Testversands festgelegt.
   * Wenn nur eine Entscheidungsoption für den Basisnachweis ausgewählt wurde, wird sie in allen Phasen ausgewählt.
   * Bei Basisnachweis [!UICONTROL Primärer Entscheidungsträger] ausgewählt wurde, werden die Bühnen mit diesem Empfänger auf sie gesetzt und bei allen anderen auf Ohne gesetzt.
   * Der Staging-Name bleibt derselbe.

## Hinzufügen einer zusätzlichen Vorlage zu einem vorhandenen automatisierten Workflow

Nachdem ein grundlegender Testversand in den automatisierten Workflow konvertiert wurde, können Sie ihm zusätzliche Vorlage hinzufügen.

1. Klicken Sie auf der Seite &quot;Testdetails&quot;im Abschnitt &quot;Workflow&quot;auf **[!UICONTROL Vorlage hinzufügen].**

   * Die Vorlageneinstellungen bestimmen, was mit einem Testversand durchgeführt werden kann, dem diese Vorlage hinzugefügt wurde. Wenn die Vorlage beispielsweise die Variable [!UICONTROL Hinzufügen einer Bühne und Hinzufügen von Personen zu Bühnen] Optionen deaktiviert, Schaltflächen zu [!UICONTROL Phase hinzufügen] und [!UICONTROL Freigeben-Testversand] wird nicht angezeigt.
   * Wenn [!UICONTROL Hinzufügen einer Staging-Option] ist in der angegebenen Vorlage deaktiviert, nachdem sie hinzugefügt wurde. [!UICONTROL Vorlage hinzufügen] -Schaltfläche nicht angezeigt.
   * Wenn eine Person einer Bühne in einer Vorlage für automatisierte Workflows hinzugefügt, aber bereits im Testversand vorhanden ist, entfernt das System diese Person automatisch aus der Bühne, wenn diese Vorlage angewendet wird. Wenn zu dieser Phase niemand anderes hinzugefügt wurde, wird der folgende Fehler angezeigt, da das System keine leere Phase zum Workflow hinzufügen kann.

      ![error_when_adding_template.png](assets/error-when-adding-template-350x66.png)
