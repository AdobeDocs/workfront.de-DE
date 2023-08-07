---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Die [!DNL Adobe Workfront] Benutzerdefinierte Sandbox-Umgebung aktualisieren
description: Die Sandbox für benutzerdefinierte Aktualisierungen ist eine Umgebung, in der Sie Daten aus Ihrer Produktionsumgebung testen und verwenden können. Es ist auch ideal für Trainings und die Bestimmung der Einrichtungsfunktionalität.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 0e2c529e61ed1c9c85dbd826029cf64346f865ff
workflow-type: tm+mt
source-wordcount: '1555'
ht-degree: 0%

---

# Die [!DNL Adobe Workfront] Benutzerdefinierte Sandbox-Umgebung aktualisieren

Die Sandbox für benutzerdefinierte Aktualisierungen ist eine Umgebung, in der Sie Daten aus Ihrer Produktionsumgebung testen und verwenden können. Es ist auch ideal für Trainings und die Bestimmung der Einrichtungsfunktionalität.

>[!NOTE]
>
>Dies unterscheidet sich von der Vorschau-Sandbox, bei der es sich auch um eine Testumgebung handelt, die Ihre [!DNL Workfront] Produktionsumgebung.
>
>* Neue Funktionen werden in die Vorschau-Sandbox eingeführt, bevor sie in der Produktion verfügbar werden.
>* Neue Funktionen werden nicht in die Sandbox für benutzerdefinierte Aktualisierung eingeführt, bevor sie in der Produktion verfügbar werden.
>
>  Darüber hinaus fallen zusätzliche Kosten an, um die Sandbox für benutzerdefinierte Aktualisierung zu erhalten, die nicht für die Sandbox &quot;Vorschau&quot;erforderlich ist.
>
>  Weitere Informationen zur Vorschau-Sandbox finden Sie unter [Die [!DNL Adobe Workfront] Vorschau der Sandbox-Umgebung](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

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
   <td> <p>[!UICONTROL Plan] </p> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Support-Paket</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] oder [!UICONTROL Enterprise]</p> <p>Das standardmäßige Support-Paket hat keinen Zugriff auf die Sandbox Benutzerdefinierte Aktualisierung, aber es hat Zugriff auf die Vorschau-Sandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Aktualisieren der benutzerdefinierten Aktualisierungs-Sandbox

Die Sandbox Benutzerdefinierte Aktualisierung enthält Ihre tatsächlichen Produktionsdaten und wird erst aktualisiert, wenn Sie dies planen. Sie können eine Aktualisierung jederzeit planen, und zwar so oft wie nur einmal pro Woche.

>[!NOTE]
>
>* Sie können keine Aktualisierung für den aktuellen Tag planen. Wenn heute beispielsweise der 1. Juni ist, ist der früheste Tag, an dem Sie eine Aktualisierung planen können, der 2. Juni.
>* Die geplante Aktualisierung erfolgt um 12:00 Uhr am angegebenen Datum, basierend auf der Zeitzone des Benutzers, der die Anforderung gesendet hat.
>* Ihre Sandbox für benutzerdefinierte Aktualisierungen verfügt immer über dieselben Produktfunktionen wie Ihre Produktionsumgebung. Wenn Sie jedoch Ihre Sandbox für benutzerdefinierte Aktualisierung aktualisieren, wird das Branding nur für die Hintergrundfarbe des Anmeldebildschirms beibehalten. Die Logos auf dem Anmeldebildschirm und der Navigationsleiste werden auf [!DNL Workfront] -Standardeinstellungen sowie alle Branding-Bilder, die Sie vor der Aktualisierung geändert haben, werden nicht angezeigt.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Zugriff auf die Sandbox für benutzerdefinierte Aktualisierungen über Ihre Produktionsumgebung {#access-the-custom-refresh-sandbox-from-your-production-environment}

Als [!DNL Workfront] Administrator können Sie über Ihre Produktionsumgebung auf Ihre Sandbox für benutzerdefinierte Aktualisierungen zugreifen.

>[!NOTE]
>
>Wenn Ihr Konto auf Cluster 4 (EMEA-Cluster) basiert, können Sie nicht über die Produktionsumgebung auf Ihre Sandbox für benutzerdefinierte Aktualisierung zugreifen. Weitere Informationen dazu, wie Sie auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zugreifen können, wenn Sie ein Konto auf Cluster 4 haben, finden Sie unter [Zugriff auf die Sandbox für benutzerdefinierte Aktualisierung für Konten auf Cluster 4 (EMEA-Konten)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Zugriff auf die Sandbox für benutzerdefinierte Aktualisierung für Konten auf Cluster 4 (EMEA-Konten)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

So greifen Sie auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zu:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicks **[!UICONTROL System]** >**[!UICONTROL Voreinstellungen]**.

1. Im **[!UICONTROL Testumgebung]** Abschnitt, klicken Sie auf **[!UICONTROL Sandbox 1]** oder **[!UICONTROL Sandbox 2]**.

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

Wenn [!DNL Workfront] -Konto auf Cluster 4 (EMEA-Cluster) befindet, können Sie nur über eine URL auf Ihre Sandbox für benutzerdefinierte Aktualisierungen zugreifen. Wenden Sie sich an unseren Kundensupport, um herauszufinden, auf welchem Cluster Ihr Konto sich befindet.

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

Nachdem Sie eine Aktualisierung Ihrer benutzerdefinierten Aktualisierungs-Sandbox geplant haben, können Sie sie abbrechen, indem Sie auf [!UICONTROL Abbrechen] oben auf der Seite. Sie können sie auch für einen späteren Zeitpunkt neu planen.

>[!NOTE]
>
>Sie können keine automatischen Sandbox-Aktualisierungen planen.

So planen Sie eine Aktualisierung Ihrer Sandbox zur Kundenaktualisierung:

1. Melden Sie sich bei Ihrer benutzerdefinierten Aktualisierungs-Sandbox an.
1. Klicks **[!UICONTROL Zeitplan]** im Banner am oberen Bildschirmrand ein Datum aus dem Kalender auswählen.
1. Wählen Sie ein Datum aus, an dem die Aktualisierung durchgeführt werden soll, und klicken Sie dann auf **[!UICONTROL Zeitplanaktualisierung]**.

## Von der Sandbox für benutzerdefinierte Aktualisierung zur Produktion wechseln

1. Melden Sie sich bei Ihrer benutzerdefinierten Aktualisierungs-Sandbox an.

   Weitere Informationen zum Zugriff auf Ihre benutzerdefinierte Aktualisierungs-Sandbox finden Sie unter [Zugriff auf die Sandbox für benutzerdefinierte Aktualisierungen über Ihre Produktionsumgebung](#access-the-custom-refresh-sandbox-from-your-production-environment) oder [Zugriff auf die Sandbox für benutzerdefinierte Aktualisierungen über eine URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Klicks **[!UICONTROL Zu Produktion wechseln]** im Banner am oberen Bildschirmrand angezeigt.

   Denken Sie daran, dass die in der Sandbox geleistete Arbeit nicht im [!UICONTROL production] -Umgebung, da die Übertragung von Daten unidirektional ist, von der Produktion zu Ihrer benutzerdefinierten Aktualisierungs-Sandbox und nicht umgekehrt.

## Empfangen von E-Mails aus der Sandbox &quot;Benutzerdefinierte Aktualisierung&quot;

[!DNL Workfront] Deaktiviert die gesamte E-Mail-Kommunikation in der Sandbox-Umgebung &quot;Benutzerdefinierte Aktualisierung&quot;. Wenn Sie E-Mail-Benachrichtigungen von der Sandbox-Umgebung für benutzerdefinierte Aktualisierungen erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren. Weitere Informationen zum Aktivieren von E-Mail-Benachrichtigungen in der Umgebung &quot;Custom Refresh Sandbox&quot;finden Sie unter [Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Berichtversand und Push-Benachrichtigungen in der Mobile App sind in der Umgebung der benutzerdefinierten Aktualisierungs-Sandbox immer deaktiviert. Weder du noch der [!DNL Workfront] -Administrator kann die Berichtbereitstellung oder Push-Benachrichtigungen für die mobile App aktivieren, wenn Sie auf die Sandbox-Umgebung für benutzerdefinierte Aktualisierungen zugreifen.\
>Weitere Informationen zu Berichtbereitstellungen für die Produktionsumgebung finden Sie unter [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).Weitere Informationen zu Push-Benachrichtigungen in der mobilen App für die Produktionsumgebung finden Sie im Abschnitt unter .

## Konfigurieren von Single Sign-On in der benutzerdefinierten Aktualisierungs-Sandbox

Wenn Sie Ihre benutzerdefinierte Aktualisierungs-Sandbox für die Verwendung mit einer Single Sign-On-Lösung konfigurieren möchten, können Sie dies tun, indem Sie sie getrennt von Ihrer Produktionsumgebung konfigurieren. Die SSO-Konfiguration in der Sandbox für benutzerdefinierte Aktualisierung ist unabhängig von Ihrer SSO-Konfiguration in der Produktionsumgebung.\
Wenn Sie Ihre benutzerdefinierte Aktualisierungs-Sandbox aktualisieren, werden die SSO-Informationen nicht aus Ihrer Produktionsumgebung kopiert, um die Konfiguration der benutzerdefinierten Aktualisierungs-Sandbox zu überschreiben.

Die Schritte zum Konfigurieren von Single Sign-on in der Sandbox für benutzerdefinierte Aktualisierung ähneln denen zum Konfigurieren in der Produktionsumgebung.\
Weitere Informationen zur Konfiguration [!DNL Workfront] mit SSO, siehe [Überblick über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die [!DNL Workfront] -Instanz mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

## Vorgesehene Nutzung und Verfügbarkeit

[!DNL Workfront] Benutzerdefinierte Update-Sandbox-Umgebungen sind nicht für Leistungs- oder Belastungstests vorgesehen. Verwenden Sie stattdessen diese Umgebungen, um die Funktionsfunktionalität mit den vorhandenen Workflows Ihres Unternehmens zu validieren.

[!DNL Workfront] Benutzerdefinierte Update-Sandbox-Umgebungen sollten immer verfügbar sein. Jeder Ausfall einer benutzerdefinierten Workfront-Aktualisierungs-Sandbox-Umgebung während der regulären Geschäftszeiten hat unmittelbar nach Behebung etwaiger Produktionsprobleme Priorität. Jeder Ausfall einer benutzerdefinierten Workfront-Aktualisierungs-Sandbox-Umgebung an Wochenenden (Samstags und Sonntagen) wird behoben, damit die Umgebung am Montag für Geschäftszeiten ausgeführt wird.
