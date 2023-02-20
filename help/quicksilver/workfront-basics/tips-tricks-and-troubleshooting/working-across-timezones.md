---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Arbeiten über Zeitzonen hinweg
description: Es kann hilfreich sein zu verstehen, wie [!DNL Adobe Workfront] verwendet Zeitzonen, um Folgendes zu berechnen - BEARBEITEN SIE ME.
feature: Get Started with Workfront
exl-id: b6574165-a6dc-4694-a367-d98927abf1e3
source-git-commit: fb538c6511514eedf81f4b9be452d5f87e3f7577
workflow-type: tm+mt
source-wordcount: '1072'
ht-degree: 0%

---

# Arbeiten über Zeitzonen hinweg

Es kann hilfreich sein zu verstehen, wie [!DNL Adobe Workfront] verwendet Zeitzonen, um Folgendes zu berechnen:

* Zeitfelder für Objekte
* Zeiten in anderen [!DNL Workfront] Bereiche wie automatisierte Workfront-E-Mails

## Zeitzonen in [!DNL Workfront]

Die Zeiten, in denen [!DNL Workfront] basieren auf Zeitzonenkonfigurationen für die [!DNL Workfront] und für Ihr Benutzerprofil. Wenn diese beiden Zeitzonen unterschiedlich sind, treten möglicherweise Zeitdiskrepanzen in verschiedenen Bereichen und Funktionen auf, die Sie in [!DNL Workfront].

>[!NOTE]
>
><div class="preview">In einem benutzerdefinierten Formular, das an ein Objekt angehängt ist, werden Datums- und Uhrzeitanweisungen in berechneten benutzerdefinierten Feldern von der koordinierten UTC (Universal Time) berechnet und gespeichert, nicht von den Zeitzonenkonfigurationen, die für die Instanz Ihres Unternehmens und Ihr Benutzerprofil festgelegt sind. Berechnungen in einem benutzerdefinierten Formular werden basierend auf den individuellen Zeitzonen der einzelnen Benutzer generiert und angezeigt.</div>




* [Die [!DNL Workfront] instance](#your-organization-s-workfront-instance)
* [Ihr Benutzerprofil](#your-user-profile)

### Die [!DNL Workfront] instance {#your-organization-s-workfront-instance}

Die Zeitzone für die [!DNL Workfront] -Instanz wird normalerweise für den Speicherort des Hauptbüros festgelegt. Dies bestimmt Folgendes:

* Die in E-Mails angezeigte Zeit, die von [!DNL Workfront]
* Die Zeitzone für neu hinzugefügte Benutzer (vor dem [!DNL Workfront] Administrator konfiguriert für sie je nach Arbeitsort eine andere Zeitzone.

   Weitere Informationen zu diesen beiden Beispielen finden Sie unter [Grundlegende Informationen für Ihr System konfigurieren](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* Der Beginn oder das Ende einer überschriebenen Abrechnungsrate für ein Projekt. Weitere Informationen finden Sie unter [Außerkraftsetzen der Abrechnungsraten für Auftragsrollen auf Projektebene](../../manage-work/projects/project-finances/override-job-role-billing-rates-at-the-project-level.md).

### Ihr Benutzerprofil {#your-user-profile}

Die Zeitzone in Ihrem Benutzerprofil sollte für den Ort konfiguriert werden, an dem Sie arbeiten. Dies bestimmt Folgendes:

* Die in Ihrem Ausgang angezeigte Zeit [!DNL Workfront] E-Mail-Nachrichten
* Zeiten für ein Objekt, an dem Sie arbeiten, z. B. Start- und Endzeiten

   Wenn Benutzer in mehreren Zeitzonen einem Objekt zugewiesen sind, [!DNL Workfront] konvertiert die Objektzeiten für alle involvierten Benutzer mithilfe der in den einzelnen Benutzerprofilen konfigurierten Zeitzone.

   **Beispiel:** In der Zeitzone Eastern Standard Time (EST), in der Sie arbeiten, legen Sie eine Aufgabe so fest, dass sie um 16:00 Uhr beginnt, und weisen sie Benutzern zu, die im Bereich Pacific Standard Time (PST) arbeiten. Für diese Benutzer wird die Startzeit als 13 Uhr angezeigt. Wenn es als 16:00 Uhr angezeigt würde, würden sie drei Stunden zu spät daran arbeiten.

   Wenn der Objektersteller den Unterschied zwischen den Zeitzonen der Bevollmächtigten nicht feststellt und beim Festlegen der Objektzeiten die erforderlichen Anpassungen vornimmt oder die Bevollmächtigten diesen Unterschied nicht feststellen, kann es schwierig sein, den richtigen Zeitpunkt zu finden, während alle am Objekt zusammenarbeiten.

   **Beispiel:** Sie konfigurieren eine eintägige Aufgabe, um 9:00 Uhr EST zu beginnen, und vergessen dabei, dass einige Benutzer der Aufgabe in der PST-Zone arbeiten. Die Startzeit beträgt 6:00 Uhr. Da sie erst um 9:00 Uhr (Mittag Ihrer Zeit) daran arbeiten werden, beginnt die Aufgabe und endet drei Stunden zu spät.

Informationen zum Konfigurieren der Zeitzone in Ihrem Benutzerprofil finden Sie unter [Meine Einstellungen konfigurieren](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md).

Informationen zum [!DNL Workfront] Administrator (oder eine Person mit [!UICONTROL Bearbeiten] Zugriff auf Benutzer) die Zeitzone in einem Benutzerprofil konfigurieren können, siehe [Benutzerprofil bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## So können Sie die Arbeit von Benutzern über Zeitzonen hinweg erleichtern

Sie können Benutzern auf verschiedene Weise dabei helfen, einfacher über mehrere Zeitzonen hinweg zu arbeiten:

* [Verwenden von Zeitplänen](#use-schedules)
* [Berechnete Zeitfelder in einem benutzerdefinierten Formular verwenden](#use-calculated-time-fields-in-a-custom-form)
* [Verwenden Sie in einem benutzerdefinierten Formular Textfelder anstelle von Datumsfeldern.](#use-text-fields-instead-of-date-fields-in-a-custom-form)

### Verwenden von Zeitplänen {#use-schedules}

[!DNL Workfront] -Administratoren erstellen für jede Zeitzone in Ihrer Organisation separate Zeitpläne, um sicherzustellen, dass die Arbeit für alle, unabhängig davon, wo sie sich befinden, angemessen geplant wird. Nachdem der Administrator die Zeitpläne erstellt hat, können sie bestimmten Projekten und Benutzern zugeordnet werden:

* **[!UICONTROL Projekte]**: Ein Projektersteller kann einen Zeitplan für ein einzelnes Projekt auswählen. Dies bestimmt die Planung der Aufgaben im Projekt basierend auf den für die Zeitzonen der Bevollmächtigten festgelegten Arbeitszeiten.
* **[!UICONTROL Benutzer]**: A [!DNL Workfront] Administrator (oder eine Person mit [!UICONTROL Bearbeiten] -Zugriff auf Benutzer) können einen Zeitplan für einzelne Benutzer im Profil des Benutzers auswählen.

   Dieser Zeitplan unterscheidet sich möglicherweise von einem Projektplan. Wenn beispielsweise jemand eine Aufgabe im Projekt erstellt und ihr noch niemand zugewiesen hat, verwendet die Aufgabe den Projektplan. Wenn ein Benutzer der Aufgabe zugewiesen ist, verwendet die Aufgabe den Zeitplan dieses Benutzers.

   Wenn einer Aufgabe mehrere Benutzer zugewiesen sind, verwendet das System eine der folgenden Optionen, wie in den systemweiten Projektvoreinstellungen konfiguriert:

   * Die Zeitzone für den Zeitplan des primären Eigentümers der Aufgabe
   * Die Zeitzone für den Zeitplan des Projekts.

   Dies kann dazu führen, dass sich die Aufgabendaten ändern.

   **Beispiel:** Ein EST-Benutzer wird einer eintägigen Aufgabe zugewiesen, die für den Start um 9:00 Uhr PST geplant ist, also um 12:00 Uhr EST. Da dem EST-Benutzer für den Tag nur noch zwei Arbeitsstunden verbleiben, erstreckt sich das Abschlussdatum der Aufgabe um etwa 6 Stunden bis zum nächsten Arbeitstag.

   Informationen zum [!UICONTROL Projektvoreinstellungen] Gebiet von [!UICONTROL Einrichtung], siehe [Systemweite Projektvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   Anweisungen zum Zuweisen eines Zeitplans zu einem Projekt oder Benutzer finden Sie unter [Zeitplan erstellen](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

   Informationen dazu, wie sich die in Ihrem Zeitplan konfigurierte Zeitzone auf die Verteilung der [!UICONTROL Geplante Stunden] im [!DNL Workload Balancer], siehe [Verwalten Sie die Benutzerzuordnungen im [!DNL Workload Balancer]](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).


### Berechnete Zeitfelder in einem benutzerdefinierten Formular verwenden {#use-calculated-time-fields-in-a-custom-form}

Sie können eine Reihe berechneter benutzerdefinierter Felder in einem benutzerdefinierten Formular verwenden, um die aktuelle Zeit für Benutzer in Ihrer Organisation anzuzeigen, z. B. eine Reihe von Flughafenuhren, die die Zeit in mehreren Städten anzeigen. Sie können für jede Zeitzone, in der Ihre Benutzer arbeiten, ein Feld erstellen, in dem die Zeit für die Zeitzone berechnet wird.

Weitere Informationen finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)sowie den Abschnitt [Berechnete benutzerdefinierte Felder für Datum und Uhrzeit](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md#date) im Artikel [Berechnete Datenausdrücke](../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

### Verwenden Sie in einem benutzerdefinierten Formular Textfelder anstelle von Datumsfeldern. {#use-text-fields-instead-of-date-fields-in-a-custom-form}

Wenn du nicht willst [!DNL Workfront] Um Zeiten zu konvertieren, für die Sie in einem Objekt für Benutzer in verschiedenen Zeitzonen konfigurieren, können Sie ein Textfeld in einem benutzerdefinierten Formular verwenden, das Sie an ein Objekt anhängen, anstatt ein Datumsfeld zu verwenden. Auf diese Weise zeigt die Zeit die Zeit an, die Sie für jeden im Projekt eingeben.

Wenn Sie dies tun, sollten Sie die Benutzer des Formulars daran erinnern, den Unterschied zwischen ihrer Zeitzone und Ihrer zu berechnen, damit sie bestimmen können, wann die Arbeit beginnen und enden soll. Sie können dies in die Anweisungen aufnehmen, die Sie für das benutzerdefinierte Formular eingeben, oder in eine QuickInfo für dieses Feld. Weitere Informationen finden Sie unter [Benutzerdefiniertes Feld zu einem benutzerdefinierten Formular hinzufügen](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md).
