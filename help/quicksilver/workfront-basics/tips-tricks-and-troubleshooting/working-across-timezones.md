---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Arbeiten über Zeitzonen hinweg
description: Es kann hilfreich sein zu verstehen, wie  [!DNL Adobe Workfront]  Zeitzonen verwendet, um Zeitfelder für Objekte und Zeiten in anderen Bereichen wie E-Mails zu berechnen.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# Arbeiten über Zeitzonen hinweg

<!-- Audited: 2/2024 -->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Es kann hilfreich sein zu verstehen, wie [!DNL Adobe Workfront] Zeitzonen verwendet, um Folgendes zu berechnen:

* Zeitfelder für Objekte
* Zeiten in anderen [!DNL Workfront] Bereichen, z. B. automatisierte Workfront-E-Mails

>[!WARNING]
>
>Wenn Sie Ihre genaue Zeitzone nicht in der von uns bereitgestellten Liste finden können, suchen Sie die Zeitzone, die Ihrer am nächsten liegt, und aktualisieren Sie sie für Ihre Instanz.
>
>Beachten Sie außerdem, dass eine ähnliche Zeitzone möglicherweise nicht perfekt mit Ihrer übereinstimmt.
>
>Beispielsweise können einige Länder oder Gebiete die Sommerzeit einhalten, Ihr Land jedoch nicht. Gegebenenfalls müssen Sie die Zeitzonen Ihres Systems entsprechend diesen Änderungen anpassen.


## Zeitzonen in [!DNL Workfront]

Die Zeiten, die Sie in [!DNL Workfront] sehen, basieren auf Zeitzonenkonfigurationen für die [!DNL Workfront] Ihres Unternehmens und für Ihr Benutzerprofil. Wenn diese beiden Zeitzonen unterschiedlich sind, kann es zu Zeitabweichungen in verschiedenen Bereichen und Funktionen kommen, die Sie in [!DNL Workfront] verwenden.

>[!NOTE]
>
>In einem benutzerdefinierten Formular, das an ein Objekt angehängt ist, werden Datums- und Zeitangaben in berechneten benutzerdefinierten Feldern durch die koordinierte Weltzeit (UTC) berechnet und gespeichert, nicht durch die Zeitzonenkonfigurationen, die für die Instanz Ihres Unternehmens und Ihr Benutzerprofil festgelegt sind. Berechnungen in einem benutzerdefinierten Formular werden basierend auf den individuellen Zeitzonen der einzelnen Benutzenden generiert und angezeigt.

* [Die Instanz  [!DNL Workfront]  Organisation](#your-organization-s-workfront-instance)
* [Ihr Benutzerprofil](#your-user-profile)

### Die [!DNL Workfront] Instanz Ihres Unternehmens {#your-organization-s-workfront-instance}

Die Zeitzone für die [!DNL Workfront]-Instanz Ihres Unternehmens ist in der Regel am Standort des Hauptbüros festgelegt. Damit wird Folgendes festgelegt:

* Die Zeit, die in von [!DNL Workfront] generierten E-Mails angezeigt wird
* Die Zeitzone für neu hinzugefügte Benutzer (bevor der [!DNL Workfront]-Administrator eine andere Zeitzone für sie konfiguriert, je nachdem, wo sie arbeiten)

  Weitere Informationen zu diesen beiden Beispielen finden Sie unter [Konfigurieren grundlegender Informationen für Ihr System](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Beginn oder Ende eines überschriebenen Abrechnungssatzes für ein Projekt. Weitere Informationen finden Sie unter [Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Projektebene](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Ihr Benutzerprofil {#your-user-profile}

Die Zeitzone in Ihrem Benutzerprofil sollte für den Ort konfiguriert werden, an dem Sie arbeiten. Damit wird Folgendes festgelegt:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Zeiten für ein Objekt, an dem Sie arbeiten, z. B. Start- und Endzeiten

  Wenn einem Objekt Benutzende in mehreren Zeitzonen zugewiesen sind, konvertiert [!DNL Workfront] die Objektzeiten für alle Beteiligten mithilfe der in den einzelnen Benutzerprofilen konfigurierten Zeitzone.

  **Beispiel:** In der Eastern Standard Time (EST)-Zone, in der Sie arbeiten, legen Sie eine Aufgabe so fest, dass sie um 16:00 Uhr beginnt, und weisen Sie sie Benutzern zu, die in der Pacific Standard Time (PST)-Zone arbeiten. Für diese Benutzer wird die Startzeit als 13:00 Uhr angezeigt. Wenn es um 16:00 Uhr angezeigt würde, würden sie drei Stunden später anfangen, daran zu arbeiten.

  Wenn der Ersteller des Objekts den Unterschied zwischen den Zeitzonen der Verantwortlichen nicht bemerkt und die erforderlichen Anpassungen beim Festlegen der Objektzeiten vornimmt, oder die Verantwortlichen diesen Unterschied nicht bemerken, kann es schwierig sein, den richtigen Zeitpunkt zu finden, während alle am Objekt zusammenarbeiten.

  **Beispiel:** Sie konfigurieren eine eintägige Aufgabe so, dass sie um 9:00 Uhr EST beginnt, wobei Sie vergessen, dass einige Benutzer an der Aufgabe in der PST-Zone arbeiten. Für sie die Startzeit 6:00 Uhr. Da sie die Arbeit erst um 9:00 Uhr (Ihre Mittagszeit) beginnen, beginnt die Aufgabe und endet mit drei Stunden Verspätung.

Informationen zum Konfigurieren Ihrer Zeitzone in Ihrem Benutzerprofil finden Sie unter [Konfigurieren meiner Einstellungen](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Informationen dazu, wie [!DNL Workfront] (oder eine Person mit [!UICONTROL Bearbeiten]-Zugriff auf Benutzer) die Zeitzone in einem Benutzerprofil konfigurieren können, finden Sie unter [Bearbeiten des Benutzerprofils](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Wie Sie es Benutzern erleichtern können, über Zeitzonen hinweg zu arbeiten

Sie können Benutzenden auf verschiedene Weise dabei helfen, einfacher über mehrere Zeitzonen hinweg zu arbeiten:

* [Zeitpläne verwenden](#use-schedules)
* [Verwenden von berechneten Zeitfeldern in einem benutzerdefinierten Formular](#use-calculated-time-fields-in-a-custom-form)
* [Verwenden von Textfeldern anstelle von Datumsfeldern in einem benutzerdefinierten Formular](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Zeitpläne verwenden {#use-schedules}

[!DNL Workfront]-Administratoren erstellen separate Zeitpläne für jede Zeitzone in Ihrer Organisation, um sicherzustellen, dass Arbeit für alle angemessen geplant wird, unabhängig davon, wo sie sich befinden. Nachdem der Administrator die Zeitpläne erstellt hat, können sie mit bestimmten Projekten und Benutzern verknüpft werden:

* **[!UICONTROL Projekte]**: Ein Projektersteller kann einen Zeitplan für ein einzelnes Projekt auswählen. Diese bestimmt die Planung der Aufgaben im Projekt basierend auf den Arbeitsstunden, die für die Zeitzonen der Beauftragten festgelegt wurden.
* **[!UICONTROL Benutzer]**: Ein [!DNL Workfront]-Administrator (oder jemand mit [!UICONTROL Bearbeiten]-Zugriff auf Benutzer) kann einen Zeitplan für einzelne Benutzer im Benutzerprofil auswählen.

  Dieser Zeitplan kann sich von einem Projektzeitplan unterscheiden. Wenn beispielsweise jemand eine Aufgabe im Projekt erstellt und ihr noch niemand zugewiesen hat, verwendet die Aufgabe den Projektplan. Wenn ein(e) Benutzende(r) der Aufgabe zugewiesen wird, verwendet die Aufgabe den Zeitplan dieses Benutzenden.

  Wenn einer Aufgabe mehrere Benutzer zugewiesen sind, verwendet das System eine der folgenden Vorgehensweisen, wie in den systemweiten oder gruppenweiten Projektvoreinstellungen konfiguriert:

   * Die Zeitzone für den Zeitplan des primären Besitzers der Aufgabe
   * Die Zeitzone für den Zeitplan des Projekts.

  <div class="preview">

  Wenn ein(e) Benutzende(r) einer Aufgabe zugewiesen wird, verwendet das System eine der folgenden Optionen, wie in den System- oder gruppenweiten Projektvoreinstellungen konfiguriert:

   * Die Zeitzone für den Zeitplan des Verantwortlichen für die Aufgabe
   * Die Zeitzone für den Zeitplan des Projekts.

  </div>

  Dies kann dazu führen, dass sich die Aufgabendaten ändern.

>[!BEGINSHADEBOX]

**BEISPIEL:**
Ein EST-Benutzer wird einer eintägigen Aufgabe zugewiesen, die um 9:00 Uhr PST beginnen soll, d. h. um 12:00 Uhr EST. Da dem EST-Benutzer nur noch 2 Arbeitsstunden für den Tag verbleiben, verlängert sich das Abschlussdatum der Aufgabe um etwa 6 Stunden auf den nächsten Arbeitstag.


>[!ENDSHADEBOX]

Weitere Informationen zum Bereich [!UICONTROL Projektvoreinstellungen] von [!UICONTROL Setup] finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Anweisungen zum Zuweisen eines Zeitplans zu einem Projekt oder einem Benutzer finden Sie unter [Erstellen eines Zeitplans](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Weitere Informationen dazu, wie sich die in Ihrem Zeitplan konfigurierte Zeitzone auf die Verteilung der [!UICONTROL geplanten Stunden] im [!UICONTROL Workload Balancer] auswirkt, finden Sie unter [Verwalten von Benutzerzuweisungen im [!UICONTROL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Verwenden von berechneten Zeitfeldern in einem benutzerdefinierten Formular {#use-calculated-time-fields-in-a-custom-form}

Sie können eine Reihe berechneter benutzerdefinierter Felder in einem benutzerdefinierten Formular verwenden, um die aktuelle Zeit für Benutzende in Ihrer Organisation anzuzeigen, z. B. eine Reihe von Flughafenuhren, die die Zeit in mehreren Städten anzeigt. Sie können für jede der Zeitzonen, in denen Ihre Benutzer arbeiten, ein Feld erstellen, wobei jede Zeitzone berechnet wird.

Weitere Informationen finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) sowie im Abschnitt [Berechnete benutzerdefinierte Felder mit Datum und Uhrzeit](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) im Artikel [Übersicht über berechnete Datenausdrücke](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Verwenden von Textfeldern anstelle von Datumsfeldern in einem benutzerdefinierten Formular {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Wenn Sie nicht möchten, dass [!DNL Workfront] Zeiten konvertieren, die Sie für in einem -Objekt konfigurieren, für Benutzer in verschiedenen Zeitzonen, können Sie ein Textfeld in einem benutzerdefinierten Formular verwenden, das Sie an ein -Objekt anhängen, anstatt ein Datumsfeld zu verwenden. Auf diese Weise wird die Zeit, die Sie eingeben, für alle am Projekt beteiligten Personen angezeigt.

In diesem Fall empfehlen wir, die Benutzer des Formulars daran zu erinnern, den Unterschied zwischen ihrer Zeitzone und Ihrer zu berechnen, damit sie bestimmen können, wann die Arbeit beginnen und enden soll. Sie können dies in die Anweisungen aufnehmen, die Sie für das benutzerdefinierte Formular eingeben, oder in eine QuickInfo für dieses Feld einfügen. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
