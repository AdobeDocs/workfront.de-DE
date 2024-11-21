---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Arbeiten über Zeitzonen hinweg
description: Es kann hilfreich sein, zu verstehen, wie [!DNL Adobe Workfront] Zeitzonen verwendet, um Zeitfelder für Objekte und Uhrzeiten in anderen Bereichen wie E-Mails zu berechnen.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: ef7f5d00bd74feee5e06b935c4bb8a18ee8b08a8
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# Arbeiten über Zeitzonen hinweg

<!-- Audited: 2/2024 -->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

Es kann hilfreich sein, zu verstehen, wie [!DNL Adobe Workfront] Zeitzonen verwendet, um Folgendes zu berechnen:

* Zeitfelder für Objekte
* Zeiten in anderen [!DNL Workfront] Bereichen, z. B. automatisierten Workfront-E-Mails

>[!WARNING]
>
>Wenn Sie Ihre genaue Zeitzone nicht in der von uns bereitgestellten Liste finden, suchen Sie die Zeitzone, die Ihrer am nächsten ist, und aktualisieren Sie sie für Ihre Instanz.
>
>Beachten Sie außerdem, dass eine ähnliche Zeitzone möglicherweise nicht genau mit Ihrer übereinstimmt.
>
>Zum Beispiel können einige Länder oder Gebiete die Sommerzeit beobachten, Ihr Land jedoch möglicherweise nicht. Möglicherweise müssen Sie bei Bedarf die Zeitzonen Ihres Systems entsprechend diesen Änderungen anpassen.


## Zeitzonen in [!DNL Workfront]

Die Zeiten, die Sie in [!DNL Workfront] sehen, basieren auf Zeitzonenkonfigurationen für die [!DNL Workfront] -Instanz Ihres Unternehmens und für Ihr Benutzerprofil. Wenn diese beiden Zeitzonen unterschiedlich sind, treten möglicherweise Zeitdiskrepanzen in verschiedenen Bereichen und Funktionen auf, die Sie in [!DNL Workfront] verwenden.

>[!NOTE]
>
>In einem benutzerdefinierten Formular, das an ein Objekt angehängt ist, werden Datums- und Uhrzeitanweisungen in berechneten benutzerdefinierten Feldern von der koordinierten UTC (Universal Time) berechnet und gespeichert, nicht von den Zeitzonenkonfigurationen, die für die Instanz Ihres Unternehmens und Ihr Benutzerprofil festgelegt sind. Berechnungen in einem benutzerdefinierten Formular werden basierend auf den individuellen Zeitzonen der einzelnen Benutzer generiert und angezeigt.

* [Die [!DNL Workfront] Instanz Ihres Unternehmens](#your-organization-s-workfront-instance)
* [Ihr Benutzerprofil](#your-user-profile)

### Die [!DNL Workfront] -Instanz Ihres Unternehmens {#your-organization-s-workfront-instance}

Die Zeitzone für die [!DNL Workfront] -Instanz Ihres Unternehmens wird normalerweise für den Speicherort des Hauptbüros festgelegt. Dies bestimmt Folgendes:

* Die in E-Mails angezeigte Zeit, die von [!DNL Workfront] generiert wurden
* Die Zeitzone für neu hinzugefügte Benutzer (bevor der [!DNL Workfront] -Administrator eine andere Zeitzone für sie konfiguriert, je nachdem wo sie funktionieren)

  Weitere Informationen zu diesen beiden Beispielen finden Sie unter [Grundlegende Informationen für Ihr System konfigurieren](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Beginn oder Ende einer überschriebenen Abrechnungsrate für ein Projekt. Weitere Informationen finden Sie unter [Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Ihr Benutzerprofil {#your-user-profile}

Die Zeitzone in Ihrem Benutzerprofil sollte für den Ort konfiguriert werden, an dem Sie arbeiten. Dies bestimmt Folgendes:

<!--
* The time shown in your outgoing [!DNL Workfront] email messages
[NOTE FROM LISA: Saeid that dates/times shown in emails are more complicated than how it is described in the article so we decided to comment out this line.]
-->
* Zeiten für ein Objekt, an dem Sie arbeiten, z. B. Start- und Endzeiten

  Wenn einem Objekt Benutzer in mehreren Zeitzonen zugewiesen sind, wandelt [!DNL Workfront] die Objektzeiten für alle beteiligten Benutzer mithilfe der in den einzelnen Benutzerprofilen konfigurierten Zeitzone um.

  **Beispiel:** In der Zeitzone Eastern Standard Time (EST), in der Sie arbeiten, legen Sie eine Aufgabe so fest, dass sie um 16:00 Uhr beginnt, und weisen sie Benutzern zu, die im Bereich Pacific Standard Time (PST) arbeiten. Für diese Benutzer wird die Startzeit als 13 Uhr angezeigt. Wenn es als 16:00 Uhr angezeigt würde, würden sie drei Stunden zu spät daran arbeiten.

  Wenn der Objektersteller den Unterschied zwischen den Zeitzonen der Bevollmächtigten nicht feststellt und beim Festlegen der Objektzeiten die erforderlichen Anpassungen vornimmt oder die Bevollmächtigten diesen Unterschied nicht feststellen, kann es schwierig sein, den richtigen Zeitpunkt zu finden, während alle am Objekt zusammenarbeiten.

  **Beispiel:** Sie konfigurieren eine eintägige Aufgabe, um 9:00 Uhr EST zu beginnen, und vergessen dabei, dass einige Benutzer der Aufgabe in der PST-Zone arbeiten. Die Startzeit beträgt 6:00 Uhr. Da sie erst um 9:00 Uhr (Mittag Ihrer Zeit) daran arbeiten werden, beginnt die Aufgabe und endet drei Stunden zu spät.

Informationen zum Konfigurieren der Zeitzone in Ihrem Benutzerprofil finden Sie unter [Meine Einstellungen konfigurieren](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Informationen dazu, wie ein [!DNL Workfront] -Administrator (oder jemand mit [!UICONTROL Bearbeiten] -Zugriff für Benutzer) die Zeitzone in einem Benutzerprofil konfigurieren kann, finden Sie unter [Profil eines Benutzers bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## So können Sie die Arbeit von Benutzern über Zeitzonen hinweg vereinfachen

Sie können Benutzern auf verschiedene Weise dabei helfen, einfacher über mehrere Zeitzonen hinweg zu arbeiten:

* [Verwenden von Zeitplänen](#use-schedules)
* [Berechnete Zeitfelder in einem benutzerdefinierten Formular verwenden](#use-calculated-time-fields-in-a-custom-form)
* [Verwenden Sie in einem benutzerdefinierten Formular Textfelder anstelle von Datumsfeldern.](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Verwenden von Zeitplänen {#use-schedules}

[!DNL Workfront] -Administratoren erstellen für jede Zeitzone in Ihrer Organisation separate Zeitpläne, um sicherzustellen, dass die Arbeit für alle, unabhängig davon, wo sie sich befinden, angemessen geplant wird. Nachdem der Administrator die Zeitpläne erstellt hat, können sie bestimmten Projekten und Benutzern zugeordnet werden:

* **[!UICONTROL Projekte]**: Ein Projektersteller kann einen Zeitplan für ein einzelnes Projekt auswählen. Dies bestimmt die Planung der Aufgaben im Projekt basierend auf den für die Zeitzonen der Bevollmächtigten festgelegten Arbeitszeiten.
* **[!UICONTROL Benutzer]**: Ein [!DNL Workfront] -Administrator (oder eine Person mit [!UICONTROL Bearbeitungszugriff] auf Benutzer) kann einen Zeitplan für einzelne Benutzer im Profil des Benutzers auswählen.

  Dieser Zeitplan unterscheidet sich möglicherweise von einem Projektplan. Wenn beispielsweise jemand eine Aufgabe im Projekt erstellt und ihr noch niemand zugewiesen hat, verwendet die Aufgabe den Projektplan. Wenn ein Benutzer der Aufgabe zugewiesen ist, verwendet die Aufgabe den Zeitplan dieses Benutzers.

  Wenn einer Aufgabe mehrere Benutzer zugewiesen sind, verwendet das System eine der folgenden Optionen, wie in den systemweiten oder gruppenweiten Projektvoreinstellungen konfiguriert:

   * Die Zeitzone für den Zeitplan des primären Eigentümers der Aufgabe
   * Die Zeitzone für den Zeitplan des Projekts.

  <div class="preview">

  Wenn ein Benutzer einer Aufgabe zugewiesen ist, verwendet das System eine der folgenden Optionen, wie in den systemweiten oder gruppenweiten Projekteigenschaften konfiguriert:

   * Die Zeitzone für den Zeitplan des Verantwortlichen der Aufgabe
   * Die Zeitzone für den Zeitplan des Projekts.

  </div>

  Dies kann dazu führen, dass sich die Aufgabendaten ändern.

>[!BEGINSHADEBOX]

**BEISPIEL:**
Ein EST-Benutzer wird einer eintägigen Aufgabe zugewiesen, die für den Start um 9:00 Uhr PST geplant ist, also um 12:00 Uhr EST. Da dem EST-Benutzer für den Tag nur noch zwei Arbeitsstunden verbleiben, erstreckt sich das Abschlussdatum der Aufgabe um etwa 6 Stunden bis zum nächsten Arbeitstag.


>[!ENDSHADEBOX]

Weitere Informationen zum Bereich [!UICONTROL Projektvoreinstellungen] von [!UICONTROL Einrichtung] finden Sie unter [Systemweite Projektanvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Anweisungen zum Zuweisen eines Zeitplans zu einem Projekt oder Benutzer finden Sie unter [Erstellen eines Zeitplans](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Informationen dazu, wie sich die in Ihrem Zeitplan konfigurierte Zeitzone auf die Verteilung von [!UICONTROL geplanten Stunden] im [!UICONTROL Lastenausgleich] auswirkt, finden Sie unter [Verwalten von Benutzerzuordnungen im [!UICONTROL Lastenausgleich]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Berechnete Zeitfelder in einem benutzerdefinierten Formular verwenden {#use-calculated-time-fields-in-a-custom-form}

Sie können eine Reihe berechneter benutzerdefinierter Felder in einem benutzerdefinierten Formular verwenden, um die aktuelle Zeit für Benutzer in Ihrer Organisation anzuzeigen, z. B. eine Reihe von Flughafenuhren, die die Zeit in mehreren Städten anzeigen. Sie können für jede Zeitzone, in der Ihre Benutzer arbeiten, ein Feld erstellen, in dem die Zeit für die Zeitzone berechnet wird.

Weitere Informationen finden Sie unter [Berechnete Felder zu einem Formular hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md) sowie im Abschnitt [Berechnete benutzerdefinierte Felder für Datum und Uhrzeit](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) im Artikel [Übersicht über berechnete Datenausdrücke](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Verwenden Sie in einem benutzerdefinierten Formular Textfelder anstelle von Datumsfeldern. {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Wenn Sie nicht möchten, dass [!DNL Workfront] die Zeiten, für die Sie in einem Objekt konfigurieren, für Benutzer in verschiedenen Zeitzonen konvertiert, können Sie ein Textfeld in einem benutzerdefinierten Formular verwenden, das Sie an ein Objekt anhängen, und nicht ein Datumsfeld. Auf diese Weise zeigt die Zeit die Zeit an, die Sie für jeden im Projekt eingeben.

Wenn Sie dies tun, empfehlen wir, die Benutzer des Formulars daran zu erinnern, den Unterschied zwischen ihrer Zeitzone und Ihrer zu berechnen, damit sie bestimmen können, wann die Arbeit beginnen und enden soll. Sie können dies in die Anweisungen aufnehmen, die Sie für das benutzerdefinierte Formular eingeben, oder in eine QuickInfo für dieses Feld. Weitere Informationen finden Sie unter [Benutzerdefiniertes Formular erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
