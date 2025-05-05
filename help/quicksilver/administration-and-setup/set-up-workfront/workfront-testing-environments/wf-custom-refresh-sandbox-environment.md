---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Die  [!DNL Adobe Workfront] -benutzerdefinierte Sandbox-Umgebung aktualisieren
description: Die benutzerdefinierte Aktualisierungs-Sandbox ist eine Umgebung, in der Sie mit Daten aus Ihrer Produktionsumgebung testen und arbeiten können. Es ist auch ideal für Schulungen und die Bestimmung der Einrichtungsfunktionalität.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e18c005b-e6ff-4a1e-a589-63132f3a8ad2
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '1745'
ht-degree: 0%

---

# Die [!DNL Adobe Workfront] benutzerdefinierte Sandbox-Aktualisierungsumgebung

Die benutzerdefinierte Aktualisierungs-Sandbox ist eine Umgebung, in der Sie mit Daten aus Ihrer Produktionsumgebung testen und arbeiten können. Es ist auch ideal für Schulungen und die Bestimmung der Einrichtungsfunktionalität.

>[!NOTE]
>
>Dies unterscheidet sich von der Vorschau-Sandbox, die auch eine Testumgebung ist, die Ihre [!DNL Workfront] Produktionsumgebung repliziert.
>
>* Neue Funktionen werden in der Vorschau-Sandbox eingeführt, bevor sie in der Produktion verfügbar werden.
>* Neue Funktionen werden nicht in die benutzerdefinierte Aktualisierungs-Sandbox eingeführt, bevor sie in der Produktion verfügbar werden.
>
>  Außerdem fallen zusätzliche Kosten für den Erhalt der benutzerdefinierten Sandbox-Aktualisierung an, die für die Sandbox-Vorschau nicht erforderlich ist.
>
>  Weitere Informationen zur Sandbox-Vorschau finden Sie unter [Die  [!DNL Adobe Workfront] -Sandbox-Umgebung](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td> <p>[!UICONTROL -Plan] </p> <p>Sie müssen [!DNL Workfront] sein. Informationen zu [!DNL Workfront] finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Support-Paket</td> 
   <td> <p>[!UICONTROL Plus], [!UICONTROL Preferred] oder [!UICONTROL Enterprise]</p> <p>Das standardmäßige Support-Paket hat keinen Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox, jedoch Zugriff auf die Vorschau-Sandbox.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktualisieren der benutzerdefinierten Sandbox

Die benutzerdefinierte Aktualisierungs-Sandbox enthält Ihre tatsächlichen Produktionsdaten und wird erst aktualisiert, wenn Sie einen Zeitplan dafür festlegen. Sie können eine Aktualisierung zu jedem Zeitpunkt planen, der für Sie bequem ist, und zwar so oft wie einmal pro Woche.

>[!NOTE]
>
>* Für den aktuellen Tag kann keine Aktualisierung geplant werden. Wenn heute beispielsweise der 1. Juni ist, ist der früheste Tag, an dem Sie eine Aktualisierung planen können, der 2. Juni.
>* Die geplante Aktualisierung erfolgt zu einem bestimmten Zeitpunkt während der Nacht, basierend auf dem Cluster des Benutzers (US-Cluster werden nachts in den USA aktualisiert). Die spezifische Zeit ist aufgrund anderer Kunden in der Warteschlange und der Anzahl der aktualisierten Daten unvorhersehbar. Wenn die Warteschlange viele große Kunden hat, wird die Aktualisierung möglicherweise erst später an diesem Tag oder am nächsten Tag ausgeführt.
>* Ihre benutzerdefinierte Aktualisierungs-Sandbox hat immer dieselben Produktfunktionen wie Ihre Produktionsumgebung. Wenn Sie Ihre benutzerdefinierte Aktualisierungs-Sandbox aktualisieren, wird das Branding jedoch nur für die Hintergrundfarbe des Anmeldebildschirms beibehalten. Der Anmeldebildschirm und die Logos der Navigationsleiste werden auf [!DNL Workfront] Standardwerte zurückgesetzt, und Branding-Bilder, die Sie vor der Aktualisierung geändert haben, werden nicht angezeigt.
>



<!--
<note type="important">
If you are a Workfront Goals customer, Workfront Goals data does not transfer to the Custom Refresh Sandbox when you schedule a refresh. The ability to sync this data from your production environment to your Custom Refresh Sandbox will be available after September 2020.
</note>
-->

## Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox über Ihre Produktionsumgebung {#access-the-custom-refresh-sandbox-from-your-production-environment}

Als [!DNL Workfront] können Sie über Ihre Produktionsumgebung auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zugreifen.

>[!NOTE]
>
>Wenn sich Ihr Konto auf Cluster 4 (EMEA-Cluster) befindet, können Sie über die Produktionsumgebung nicht auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zugreifen. Weitere Informationen dazu, wie Sie auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zugreifen können, wenn Sie ein Konto auf Cluster 4 haben, finden Sie unter [Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox für Konten auf Cluster 4 (EMEA-Konten)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts) [Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox für Konten auf Cluster 4 (EMEA-Konten)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts).

So greifen Sie auf Ihre benutzerdefinierte Sandbox zu:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Setup]** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).

1. Klicken Sie auf **[!UICONTROL System]** > **[!UICONTROL Voreinstellungen]**.

1. Klicken Sie **[!UICONTROL Abschnitt &quot;]**&quot; auf **[!UICONTROL Sandbox 1]** oder **[!UICONTROL Sandbox 2]**.

   Ihr Support-Paket gibt an, ob Sie Zugriff auf eine oder zwei benutzerdefinierte Aktualisierungs-Sandboxes haben.

1. Melden Sie sich mit Ihren benutzerdefinierten Sandbox-Aktualisierungs-Anmeldeinformationen an.

   Ihre benutzerdefinierten Sandbox-Aktualisierungs-Anmeldeinformationen sind mit Ihren Produktions-Anmeldeinformationen identisch, es sei denn, Sie haben Ihre Produktions-Anmeldeinformationen seit der letzten Aktualisierung Ihrer benutzerdefinierten Sandbox-Aktualisierung geändert. Die Anmeldungen werden nur synchronisiert, wenn eine Aktualisierung erfolgt. Sie werden nicht automatisch synchronisiert.

   Die benutzerdefinierte Aktualisierungs-Sandbox zeigt im Banner oben im Bildschirm die Version sowie das Datum der letzten Aktualisierung an. Alle Informationen aus der Produktion sind verfügbar und können nach Abschluss einer Aktualisierung verwendet werden.

## Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox über eine URL {#access-the-custom-refresh-sandbox-using-a-url}

Jeder Benutzer kann über eine URL auf die benutzerdefinierte Aktualisierungs-Sandbox zugreifen.

* [Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox für Konten auf den Clustern 1, 2, 3 und 5](#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5)
* [Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox für Konten im Cluster 4 (EMEA-Konten)](#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts)

### Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox für Konten auf den Clustern 1, 2, 3 und 5 {#access-the-custom-refresh-sandbox-for-accounts-on-clusters-1-2-3-and-5}

Abhängig von Ihrem Support-Paket sollten Sie Zugriff auf eine oder zwei benutzerdefinierte Aktualisierungs-Sandboxes haben.

So greifen Sie über eine URL auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zu:

1. Navigieren Sie zu dieser URL, wenn Sie nur eine benutzerdefinierte Aktualisierungs-Sandbox haben:

   `https://companyname.sb01.workfront.com` (alte URL:`https://cr1.attasksandbox.com/`.)

   Wenn Sie zusätzlich zu den oben genannten URLs über zwei benutzerdefinierte Aktualisierungs-Sandboxes verfügen, können Sie auch auf die folgende URL zugreifen:

   `https://companyname.sb02.workfront.com` (alte URL:`https://cr2.attasksandbox.com/`)

1. Melden Sie sich auf dem Anmeldebildschirm mit Ihren benutzerdefinierten Sandbox-Aktualisierungs-Anmeldeinformationen an.
1. Ihre benutzerdefinierten Sandbox-Aktualisierungs-Anmeldeinformationen sind mit Ihren Produktions-Anmeldeinformationen identisch, es sei denn, Sie haben Ihre Produktions-Anmeldeinformationen seit der letzten Aktualisierung Ihrer benutzerdefinierten Sandbox-Aktualisierung geändert. Die Anmeldungen werden nur synchronisiert, wenn eine Aktualisierung erfolgt. Sie werden nicht automatisch synchronisiert.

### Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox für Konten im Cluster 4 (EMEA-Konten) {#access-the-custom-refresh-sandbox-for-accounts-on-cluster-4-emea-accounts}

Wenn sich Ihr [!DNL Workfront]-Konto auf Cluster 4 (EMEA-Cluster) befindet, können Sie nur über eine URL auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zugreifen. Um herauszufinden, auf welchem Cluster sich Ihr Konto befindet, wenden Sie sich an unser Kundensupportteam.

Abhängig von Ihrem Support-Paket sollten Sie Zugriff auf eine oder zwei benutzerdefinierte Aktualisierungs-Sandboxes haben.

So greifen Sie über eine URL auf Ihre benutzerdefinierte Aktualisierungs-Sandbox zu:

1. Navigieren Sie zu dieser URL, wenn Sie nur eine benutzerdefinierte Aktualisierungs-Sandbox haben:

   `https://companyname.sb01.workfront.com` (alte URL:`https://cr3.attasksandbox.com`)

   Oder

   Wechseln Sie zu einer dieser URLs, wenn Sie zwei benutzerdefinierte Aktualisierungs-Sandboxes haben:

   `https://companyname.sb01.workfront.com` (alte URL:`https://cr3.attasksandbox.com`)

   `https://companyname.sb02.workfront.com` (alte URL:`https://cr4.attasksandbox.com`)

1. Melden Sie sich auf dem Anmeldebildschirm mit Ihren benutzerdefinierten Sandbox-Aktualisierungs-Anmeldeinformationen an.

   Ihre benutzerdefinierten Sandbox-Aktualisierungs-Anmeldeinformationen sind mit Ihren Produktions-Anmeldeinformationen identisch, es sei denn, Sie haben Ihre Produktions-Anmeldeinformationen seit der letzten Aktualisierung Ihrer benutzerdefinierten Sandbox-Aktualisierung geändert. Die Anmeldungen werden nur synchronisiert, wenn eine Aktualisierung erfolgt. Sie werden nicht automatisch synchronisiert.

## Planen einer Aktualisierung Ihrer benutzerdefinierten Aktualisierungs-Sandbox

>[!IMPORTANT]
>
>Die Dauer der Aktualisierung hängt von der Größe der zu aktualisierenden Daten ab. Während des Aktualisierungsprozesses ist es wichtig, dass Ihre benutzerdefinierte Sandbox-Aktualisierungsumgebung in keiner Weise verwendet wird (einschließlich API-Aufrufe und Integrationen), da dies verhindert, dass die Sandbox-Aktualisierung erfolgreich abgeschlossen wird. [!DNL Workfront] wird die benutzerdefinierte Sandbox-Aktualisierungsumgebung deaktiviert, bevor sie beginnt. Sie müssen jedoch alle aktiven Sitzungen beenden, um sicherzustellen, dass die Sandbox-Aktualisierung erfolgreich ist.

Nachdem Sie eine Aktualisierung Ihrer benutzerdefinierten Aktualisierungs-Sandbox geplant haben, können Sie sie abbrechen, indem [!UICONTROL Abbrechen] oben auf der Seite klicken. Sie können ihn auch für einen späteren Zeitpunkt neu planen.

>[!NOTE]
>
>Sie können keine automatischen Sandbox-Aktualisierungen planen.

So planen Sie eine Aktualisierung Ihrer Kunden-Aktualisierungs-Sandbox:

1. Melden Sie sich bei Ihrer benutzerdefinierten Sandbox an.
1. Klicken Sie **[!UICONTROL Zeitplan]** in das Banner oben im Bildschirm und wählen Sie ein Datum aus dem Kalender aus.
1. Wählen Sie ein Datum für die Aktualisierung aus und klicken Sie dann auf **[!UICONTROL Aktualisierung planen]**.

## Von der benutzerdefinierten Aktualisierungs-Sandbox zur Produktion wechseln

1. Melden Sie sich bei Ihrer benutzerdefinierten Sandbox an.

   Weitere Informationen zum Zugriff auf Ihre benutzerdefinierte Aktualisierungs-Sandbox finden Sie unter [Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox aus Ihrer Produktionsumgebung](#access-the-custom-refresh-sandbox-from-your-production-environment) oder [Zugriff auf die benutzerdefinierte Aktualisierungs-Sandbox über eine URL](#access-the-custom-refresh-sandbox-using-a-url).

1. Klicken Sie **[!UICONTROL Banner oben]** Bildschirm auf „Zur Produktion wechseln“.

   Denken Sie daran, dass in der Sandbox ausgeführte Arbeiten in der [!UICONTROL Produktions]-Umgebung nicht sichtbar sind, da die Datenübertragung unidirektional erfolgt, von der Produktion an Ihre benutzerdefinierte Aktualisierungs-Sandbox und nicht umgekehrt.

## E-Mails von der benutzerdefinierten Aktualisierungs-Sandbox empfangen

[!DNL Workfront] Deaktiviert die gesamte E-Mail-Kommunikation über die benutzerdefinierte Sandbox-Aktualisierungsumgebung. Wenn Sie E-Mail-Benachrichtigungen von der benutzerdefinierten Sandbox-Aktualisierungsumgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren. Weitere Informationen zum Aktivieren von E-Mail-Benachrichtigungen in der benutzerdefinierten Sandbox-Aktualisierungsumgebung finden Sie unter [E-Mail-Versand über die Sandbox-Vorschau-Umgebung aktivieren](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Die Berichtversand- und Push-Benachrichtigungen in der mobilen App sind für die benutzerdefinierte Sandbox-Aktualisierungsumgebung immer deaktiviert. Weder Sie noch der [!DNL Workfront]-Administrator können die Berichtsbereitstellung oder Push-Benachrichtigungen für die Mobile App aktivieren, wenn Sie auf die benutzerdefinierte Sandbox-Aktualisierungsumgebung zugreifen.\
>Weitere Informationen zu Berichtssendungen für die Produktionsumgebung finden Sie unter [Übersicht über die Berichtsbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md). Weitere Informationen zu Push-Benachrichtigungen in der Mobile App für die Produktionsumgebung finden Sie im Abschnitt in .

## Konfigurieren von Single Sign-on in der benutzerdefinierten Aktualisierungs-Sandbox

Wenn Sie Ihre benutzerdefinierte Aktualisierungs-Sandbox für die Verwendung mit einer Single Sign-On-Lösung konfigurieren möchten, können Sie sie separat von Ihrer Produktionsumgebung konfigurieren. Die SSO-Konfiguration in der benutzerdefinierten Aktualisierungs-Sandbox ist unabhängig von Ihrer SSO-Konfiguration in der Produktionsumgebung.\
Wenn Sie Ihre benutzerdefinierte Aktualisierungs-Sandbox aktualisieren, werden die SSO-Informationen nicht aus Ihrer Produktionsumgebung kopiert, um die benutzerdefinierte Aktualisierungs-Sandbox-Konfiguration zu überschreiben.

Die Schritte zum Konfigurieren von Single Sign-on in der benutzerdefinierten Aktualisierungs-Sandbox ähneln denen zum Konfigurieren der Sandbox in der Produktionsumgebung.\
Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit SSO finden Sie unter [Übersicht über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die [!DNL Workfront]-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

## Automatische Neuberechnung der Projektzeitleisten

Durch die Neuberechnung der Zeitleisten können Manager sehen, wie sich Kräfte außerhalb des Projekts auf die Zeitleiste des Projekts auswirken. Der Zeitplan eines Projekts bezieht sich auf die geplanten und geplanten Termine für das Projekt.

Als Workfront-Administrator können Sie konfigurieren, wenn Workfront die Projektzeitleisten automatisch neu berechnet. Workfront kann Projektzeitleisten entweder jede Nacht oder bei einer Änderung des Projektumfangs oder beides neu berechnen.

Weitere Informationen finden Sie unter [Konfigurieren von Zeitleisten-Neuberechnungen für Projekte](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

In der benutzerdefinierten Sandbox-Aktualisierungsumgebung ist die nächtliche Neuberechnung deaktiviert, und die Projektzeitleisten werden nicht automatisch neu berechnet. Sie müssen die Zeitleiste des Projekts für die benutzerdefinierte Sandbox-Aktualisierungsumgebung manuell neu berechnen. Weitere Informationen finden Sie unter [Neuberechnen von Projektzeitleisten](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Vorgesehene Verwendung und Verfügbarkeit

* [!DNL Workfront] benutzerdefinierte Sandbox-Aktualisierungsumgebungen sind nicht für Leistungs- oder Belastungstests vorgesehen. Verwenden Sie diese Umgebungen vielmehr, um die Funktionsfunktionen mit den vorhandenen Workflows Ihres Unternehmens zu validieren.

* [!DNL Workfront] benutzerdefinierte Sandbox-Aktualisierungsumgebungen sind so konzipiert, dass sie immer verfügbar sind. Jeder Ausfall einer benutzerdefinierten Workfront-Aktualisierungs-Sandbox-Umgebung während der regulären Geschäftszeiten hat unmittelbar nach der Behebung von Produktionsproblemen, falls vorhanden, erste Priorität. Alle Ausfälle einer benutzerdefinierten Workfront-Aktualisierungs-Sandbox-Umgebung an Wochenenden (samstags und sonntags) werden behoben, sodass die Umgebung montags für Geschäftszeiten ausgeführt wird.

* Das Proofing ist in den benutzerdefinierten Sandbox-Aktualisierungsumgebungen nicht verfügbar.
