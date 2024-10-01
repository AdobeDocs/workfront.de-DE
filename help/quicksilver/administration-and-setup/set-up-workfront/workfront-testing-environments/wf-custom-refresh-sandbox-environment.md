---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Die [!DNL Adobe Workfront] benutzerdefinierte Sandbox-Umgebung für die Aktualisierung
description: Die Sandbox für benutzerdefinierte Aktualisierungen ist eine Umgebung, in der Sie Daten aus Ihrer Produktionsumgebung testen und verwenden können. Es ist auch ideal für Trainings und die Bestimmung der Einrichtungsfunktionalität.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 7c2d6d1960752a109c02039c1af8d1d1850bcb8c
workflow-type: tm+mt
source-wordcount: '1749'
ht-degree: 0%

---

# Die [!DNL Adobe Workfront] benutzerdefinierte Aktualisierungs-Sandbox-Umgebung

Die Sandbox für benutzerdefinierte Aktualisierungen ist eine Umgebung, in der Sie Daten aus Ihrer Produktionsumgebung testen und verwenden können. Es ist auch ideal für Trainings und die Bestimmung der Einrichtungsfunktionalität.

>[!NOTE]
>
>Dies unterscheidet sich von der Vorschau-Sandbox, bei der es sich auch um eine Testumgebung handelt, die Ihre [!DNL Workfront] -Produktionsumgebung repliziert.
>
>* Neue Funktionen werden in die Vorschau-Sandbox eingeführt, bevor sie in der Produktion verfügbar werden.
>* Neue Funktionen werden nicht in die Sandbox für benutzerdefinierte Aktualisierung eingeführt, bevor sie in der Produktion verfügbar werden.
>
>  Darüber hinaus fallen zusätzliche Kosten an, um die Sandbox für benutzerdefinierte Aktualisierung zu erhalten, die nicht für die Sandbox &quot;Vorschau&quot;erforderlich ist.
>
>  Weitere Informationen zur Vorschau-Sandbox finden Sie unter [Die  [!DNL Adobe Workfront] Sandbox-Umgebung in der Vorschau anzeigen](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Workfront] Plan</td> 
   <td> <p>[!UICONTROL Business] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!DNL Workfront] Lizenz</p> </td> 
   <td> <p>[!UICONTROL Plan] </p> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen zu [!DNL Workfront] -Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Support-Paket</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] oder [!UICONTROL Enterprise]</p> <p>Das standardmäßige Support-Paket hat keinen Zugriff auf die Sandbox Benutzerdefinierte Aktualisierung, aber es hat Zugriff auf die Vorschau-Sandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktualisieren der benutzerdefinierten Aktualisierungs-Sandbox

Die Sandbox Benutzerdefinierte Aktualisierung enthält Ihre tatsächlichen Produktionsdaten und wird erst aktualisiert, wenn Sie dies planen. Sie können eine Aktualisierung jederzeit planen, und zwar so oft wie nur einmal pro Woche.

>[!NOTE]
>
>* Sie können keine Aktualisierung für den aktuellen Tag planen. Wenn heute beispielsweise der 1. Juni ist, ist der früheste Tag, an dem Sie eine Aktualisierung planen können, der 2. Juni.
>* Die geplante Aktualisierung erfolgt manchmal nachts, basierend auf dem Cluster des Benutzers (US-Cluster werden in den USA nachts aktualisiert). Die spezifische Zeit ist aufgrund anderer Kunden in der Warteschlange und der Aktualisierungsmenge der Daten unvorhersehbar. Wenn die Warteschlange viele große Kunden hat, wird die Aktualisierung möglicherweise erst zu einem späteren Zeitpunkt an diesem Tag oder am nächsten Tag ausgeführt.
>* Ihre Sandbox für benutzerdefinierte Aktualisierungen verfügt immer über dieselben Produktfunktionen wie Ihre Produktionsumgebung. Wenn Sie jedoch Ihre Sandbox für benutzerdefinierte Aktualisierung aktualisieren, wird das Branding nur für die Hintergrundfarbe des Anmeldebildschirms beibehalten. Die Logos für den Anmeldebildschirm und die Navigationsleiste werden auf die Standardwerte [!DNL Workfront] zurückgesetzt, und alle Branding-Bilder, die Sie vor der Aktualisierung geändert haben, werden nicht angezeigt.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Zugriff auf die Sandbox für benutzerdefinierte Aktualisierungen über Ihre Produktionsumgebung {#access-the-custom-refresh-sandbox-from-your-production-environment}

Als [!DNL Workfront] -Administrator können Sie über Ihre Produktionsumgebung auf Ihre Sandbox für benutzerdefinierte Aktualisierungen zugreifen.

>[!NOTE]
>
>Wenn Ihr Konto auf Cluster 4 (EMEA-Cluster) basiert, können Sie nicht über die Produktionsumgebung auf Ihre Sandbox für benutzerdefinierte Aktualisierung zugreifen. Weitere Informationen dazu, wie Sie auf Ihre Sandbox für benutzerdefinierte Aktualisierungen zugreifen können, wenn Sie ein Konto auf Cluster 4 haben, finden Sie unter [Zugreifen auf die Sandbox für benutzerdefinierte Aktualisierungen für Konten auf Cluster 4 (EMEA-Konten)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Zugreifen auf die Sandbox für benutzerdefinierte Aktualisierungen für Konten auf Cluster 4 (EMEA-Konten)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

So greifen Sie auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zu:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **[!UICONTROL System]** >**[!UICONTROL Voreinstellungen]**.

1. Klicken Sie im Abschnitt **[!UICONTROL Testumgebung]** auf **[!UICONTROL Sandbox 1]** oder **[!UICONTROL Sandbox 2]**.

   Ihr Support-Paket gibt an, ob Sie Zugriff auf eine oder zwei benutzerdefinierte Aktualisierungs-Sandboxes haben.

1. Melden Sie sich mit Ihren benutzerdefinierten Sandbox-Anmeldeinformationen für die Aktualisierung an.

   Ihre benutzerdefinierten Update-Sandbox-Anmeldeinformationen sind mit Ihren Produktionsberechtigungen identisch, es sei denn, Sie haben Ihre Produktionsberechtigungen seit der letzten Aktualisierung Ihrer benutzerdefinierten Update-Sandbox geändert. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.

   Die Sandbox Benutzerdefinierte Aktualisierung zeigt die Version sowie das letzte Aktualisierungsdatum im Banner am oberen Rand des Bildschirms an. Alle Informationen aus der Produktion sind verfügbar und können nach Abschluss der Aktualisierung verwendet werden.

## Zugriff auf die Sandbox für benutzerdefinierte Aktualisierungen über eine URL {#access-the-custom-refresh-sandbox-using-a-url}

Jeder Benutzer kann über eine URL auf die Sandbox Benutzerdefinierte Aktualisierung zugreifen.

* [Zugriff auf die Sandbox für benutzerdefinierte Aktualisierungen für Konten in Clustern 1,2,3 und 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Zugriff auf die Sandbox für benutzerdefinierte Aktualisierung für Konten auf Cluster 4 (EMEA-Konten)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Zugriff auf die Sandbox für benutzerdefinierte Aktualisierungen für Konten in Clustern 1,2,3 und 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Je nach Support-Paket sollten Sie Zugriff auf eine oder zwei benutzerdefinierte Aktualisierungs-Sandboxes haben.

So greifen Sie über eine URL auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zu:

1. Navigieren Sie zu dieser URL, wenn Sie nur eine benutzerdefinierte Aktualisierungs-Sandbox haben:

   https://companyname.sb01.workfront.com (alte URL:https://cr1.attasksandbox.com/.)

   Wenn Sie über zwei benutzerdefinierte Aktualisierungs-Sandboxes verfügen, können Sie zusätzlich zu den oben genannten URLs auch über die folgende URL auf Ihre zweite Sandbox für benutzerdefinierte Aktualisierung zugreifen:

   https://companyname.sb02.workfront.com (alte URL:https://cr2.attasksandbox.com/)

1. Melden Sie sich auf dem Anmeldebildschirm mit Ihren benutzerdefinierten Sandbox-Anmeldedaten für die Aktualisierung an.
1. Ihre benutzerdefinierten Update-Sandbox-Anmeldeinformationen sind mit Ihren Produktionsberechtigungen identisch, es sei denn, Sie haben Ihre Produktionsberechtigungen seit der letzten Aktualisierung Ihrer benutzerdefinierten Update-Sandbox geändert. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.

### Zugriff auf die Sandbox für benutzerdefinierte Aktualisierung für Konten auf Cluster 4 (EMEA-Konten) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Wenn Ihr [!DNL Workfront] -Konto auf Cluster 4 (EMEA-Cluster) ist, können Sie nur über eine URL auf Ihre Sandbox für benutzerdefinierte Aktualisierung zugreifen. Wenden Sie sich an unseren Kundensupport, um herauszufinden, auf welchem Cluster Ihr Konto sich befindet.

Je nach Support-Paket sollten Sie Zugriff auf eine oder zwei benutzerdefinierte Aktualisierungs-Sandboxes haben.

So greifen Sie über eine URL auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zu:

1. Navigieren Sie zu dieser URL, wenn Sie nur eine benutzerdefinierte Aktualisierungs-Sandbox haben:

   https://companyname.sb01.workfront.com (alte URL:https://cr3.attasksandbox.com)

   Oder

   Wechseln Sie zu einer dieser URLs, wenn Sie zwei benutzerdefinierte Aktualisierungs-Sandboxes haben:

   https://companyname.sb01.workfront.com (alte URL:https://cr3.attasksandbox.com)

   https://companyname.sb02.workfront.com (alte URL:https://cr4.attasksandbox.com)

1. Melden Sie sich auf dem Anmeldebildschirm mit Ihren benutzerdefinierten Sandbox-Anmeldedaten für die Aktualisierung an.

   Ihre benutzerdefinierten Update-Sandbox-Anmeldeinformationen sind mit Ihren Produktionsberechtigungen identisch, es sei denn, Sie haben Ihre Produktionsberechtigungen seit der letzten Aktualisierung Ihrer benutzerdefinierten Update-Sandbox geändert. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.

## Planen einer Aktualisierung Ihrer benutzerdefinierten Aktualisierungs-Sandbox

>[!IMPORTANT]
>
>Die Dauer der Aktualisierung hängt von der Größe der zu aktualisierenden Daten ab. Während des Aktualisierungsprozesses ist es wichtig, dass Ihre benutzerdefinierte Aktualisierungs-Sandbox-Umgebung in keiner Weise verwendet wird (einschließlich API-Aufrufen und Integrationen), da dies verhindert, dass die Sandbox-Aktualisierung erfolgreich abgeschlossen wird. [!DNL Workfront] deaktiviert die benutzerdefinierte Aktualisierungs-Sandbox-Umgebung, bevor sie gestartet wird. Sie müssen jedoch alle aktiven Sitzungen beenden, um sicherzustellen, dass die Sandbox-Aktualisierung erfolgreich ist.

Nachdem Sie eine Aktualisierung Ihrer benutzerdefinierten Aktualisierungs-Sandbox geplant haben, können Sie sie abbrechen, indem Sie oben auf der Seite auf [!UICONTROL Abbrechen] klicken. Sie können sie auch für einen späteren Zeitpunkt neu planen.

>[!NOTE]
>
>Sie können keine automatischen Sandbox-Aktualisierungen planen.

So planen Sie eine Aktualisierung Ihrer Sandbox zur Kundenaktualisierung:

1. Melden Sie sich bei Ihrer benutzerdefinierten Aktualisierungs-Sandbox an.
1. Klicken Sie oben im Bildschirm im Banner auf **[!UICONTROL Planen]** und wählen Sie ein Datum aus dem Kalender aus.
1. Wählen Sie ein Datum aus, an dem die Aktualisierung durchgeführt werden soll, und klicken Sie dann auf **[!UICONTROL Aktualisierung planen]**.

## Von der Sandbox für benutzerdefinierte Aktualisierung zur Produktion wechseln

1. Melden Sie sich bei Ihrer benutzerdefinierten Aktualisierungs-Sandbox an.

   Weitere Informationen zum Zugriff auf Ihre Sandbox für benutzerdefinierte Aktualisierungen finden Sie unter [Zugriff auf die Sandbox für benutzerdefinierte Aktualisierungen aus Ihrer Produktionsumgebung](#access-the-custom-refresh-sandbox-from-your-production-environment) oder [Zugreifen auf die Sandbox für benutzerdefinierte Aktualisierungen mithilfe einer URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Klicken Sie im Banner oben auf dem Bildschirm auf **[!UICONTROL Gehe zur Produktion]** .

   Beachten Sie, dass in der Sandbox durchgeführte Arbeiten nicht in der Umgebung [!UICONTROL Produktion] sichtbar sind, da die Datenübertragung unidirektional von der Produktion an Ihre Sandbox für benutzerdefinierte Aktualisierung erfolgt und nicht umgekehrt.

## Empfangen von E-Mails aus der Sandbox &quot;Benutzerdefinierte Aktualisierung&quot;

[!DNL Workfront] deaktiviert die gesamte E-Mail-Kommunikation aus der Sandbox-Umgebung für benutzerdefinierte Aktualisierung. Wenn Sie E-Mail-Benachrichtigungen von der Sandbox-Umgebung für benutzerdefinierte Aktualisierungen erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren. Weitere Informationen zum Aktivieren von E-Mail-Benachrichtigungen in der Sandbox-Umgebung für benutzerdefinierte Aktualisierungen finden Sie unter [Aktivieren des Versands von E-Mails aus der Umgebung &quot;Sandbox-Vorschau&quot;](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Berichtversand und Push-Benachrichtigungen in der Mobile App sind in der Umgebung der benutzerdefinierten Aktualisierungs-Sandbox immer deaktiviert. Weder Sie noch der Administrator [!DNL Workfront] können die Berichtübermittlung oder Push-Benachrichtigungen für die mobile App aktivieren, wenn Sie auf die Umgebung &quot;Sandbox für benutzerdefinierte Aktualisierung&quot;zugreifen.\
>Weitere Informationen zu Berichtbereitstellungen für die Produktionsumgebung finden Sie unter [Übersicht über die Berichtbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Weitere Informationen zu Push-Benachrichtigungen für die mobile App in der Produktionsumgebung finden Sie im Abschnitt unter .

## Konfigurieren von Single Sign-On in der benutzerdefinierten Aktualisierungs-Sandbox

Wenn Sie Ihre benutzerdefinierte Aktualisierungs-Sandbox für die Verwendung mit einer Single Sign-On-Lösung konfigurieren möchten, können Sie dies tun, indem Sie sie getrennt von Ihrer Produktionsumgebung konfigurieren. Die SSO-Konfiguration in der Sandbox für benutzerdefinierte Aktualisierung ist unabhängig von Ihrer SSO-Konfiguration in der Produktionsumgebung.\
Wenn Sie Ihre benutzerdefinierte Aktualisierungs-Sandbox aktualisieren, werden die SSO-Informationen nicht aus Ihrer Produktionsumgebung kopiert, um die Konfiguration der benutzerdefinierten Aktualisierungs-Sandbox zu überschreiben.

Die Schritte zum Konfigurieren von Single Sign-on in der Sandbox für benutzerdefinierte Aktualisierung ähneln denen zum Konfigurieren in der Produktionsumgebung.\
Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit SSO finden Sie unter [Überblick über die einmalige Anmeldung in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die [!DNL Workfront] -Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

## Automatische Neuberechnung der Projektzeitpläne

Durch die Neuberechnung der Zeitpläne können Manager sehen, wie Kräfte außerhalb des Projekts die Zeitleiste des Projekts beeinflussen. Der Zeitrahmen eines Projekts bezieht sich auf die geplanten und geplanten Daten für das Projekt.

Als Workfront-Administrator können Sie konfigurieren, wann Workfront die Projektzeitpläne automatisch neu berechnet. Workfront kann die Projektzeitpläne entweder jede Nacht neu berechnen, den Projektumfang ändern oder beides.

Weitere Informationen finden Sie unter [Konfigurieren von Timeline-Neuberechnungen für Projekte](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

In der Umgebung der benutzerdefinierten Aktualisierungs-Sandbox ist die nächtliche Neuberechnung deaktiviert und die Projekt-Timelines werden nicht automatisch neu berechnet. Sie müssen die Projekt-Timeline für die Umgebung &quot;Custom Refresh Sandbox&quot;manuell neu berechnen. Weitere Informationen finden Sie unter [Projekt-Timelines neu berechnen](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Vorgesehene Nutzung und Verfügbarkeit

* [!DNL Workfront] Benutzerdefinierte Aktualisierungs-Sandbox-Umgebungen sind nicht für Leistungs- oder Belastungstests vorgesehen. Verwenden Sie stattdessen diese Umgebungen, um die Funktionsfunktionalität mit den vorhandenen Workflows Ihres Unternehmens zu validieren.

* [!DNL Workfront] Benutzerdefinierte Aktualisierungs-Sandbox-Umgebungen sollten immer verfügbar sein. Jeder Ausfall einer benutzerdefinierten Workfront-Aktualisierungs-Sandbox-Umgebung während der regulären Geschäftszeiten hat unmittelbar nach Behebung etwaiger Produktionsprobleme Priorität. Jeder Ausfall einer benutzerdefinierten Workfront-Aktualisierungs-Sandbox-Umgebung an Wochenenden (Samstags und Sonntagen) wird behoben, damit die Umgebung am Montag für Geschäftszeiten ausgeführt wird.

* Die Prüfung ist nicht in den Sandbox-Umgebungen für benutzerdefinierte Aktualisierungen verfügbar.
