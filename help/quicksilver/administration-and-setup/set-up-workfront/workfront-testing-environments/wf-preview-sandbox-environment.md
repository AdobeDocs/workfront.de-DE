---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Die  [!DNL Adobe Workfront] -Vorschau-Sandbox-Umgebung
description: Die Vorschau-Sandbox ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient. Es wird jedes Wochenende von Workfront aktualisiert. Daten, die am Freitag zu Ihrer Live-Umgebung hinzugefügt wurden, werden bis zum folgenden Montag in Ihrer Vorschau-Sandbox angezeigt. Alle Support-Pakete haben Zugriff auf diese Sandbox.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: d585b698b6c7900d861a30dc6b5e0bff6bd6d13a
workflow-type: tm+mt
source-wordcount: '1302'
ht-degree: 0%

---

# Die Sandbox-[!DNL Adobe Workfront]

<!-- Audited: 12/2023 -->

Es gibt zwei Testumgebungen für [!DNL Workfront], bei denen es sich um Replikate Ihrer [!DNL Workfront] Produktionsumgebung handelt:

* Die Sandbox-Vorschau

  Die Vorschau-Sandbox ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient und jedes Wochenende [!DNL Workfront] aktualisiert wird. Daten, die am Freitag zu Ihrer Live-Umgebung hinzugefügt wurden, werden bis zum folgenden Montag in Ihrer Vorschau-Sandbox angezeigt.

  Alle Support-Pakete haben Zugriff auf die Sandbox-Vorschau.

* Die benutzerdefinierte Aktualisierungs-Sandbox

  Die benutzerdefinierte Aktualisierungs-Sandbox ist eine separate Testumgebung, die von Ihnen manuell aktualisiert wird. Es fallen zusätzliche Kosten an, um die benutzerdefinierte Aktualisierungs-Sandbox zu erhalten. Weitere Informationen zu dieser Umgebung finden Sie unter [Die [!DNL Adobe Workfront] Benutzerdefinierte Sandbox-Umgebung aktualisieren](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard]-Support-Paket</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus]-, [!UICONTROL Preferred]- und [!UICONTROL Enterprise]-Support-Pakete</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Sandbox-Vorschau</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Benutzerdefinierte Sandbox aktualisieren</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Sandbox-Vorschau

Die Sandbox-Vorschau dient als Umgebung, in der Benutzer in Ihrer Organisation Daten aus der Produktionsumgebung sicher testen und damit arbeiten können, ohne die Produktionsumgebung zu beeinträchtigen.

Die Vorschau-Sandbox enthält Ihre tatsächlichen Produktionsdaten. Sie wird jedoch jedes Wochenende aktualisiert, sodass die Daten bis zu eine Woche hinter der Produktionsumgebung liegen können. Elemente, die seit der letzten Aktualisierung erstellt wurden, befinden sich bis zur nächsten Aktualisierung in der Sandbox-Vorschau-Umgebung.

Die Daten fließen unidirektional von der Produktion zur Vorschau und nicht umgekehrt. An jedem Wochenende wird stets eine Aktualisierung der Vorschau-Umgebung [!DNL Workfront].

Die Sandbox-Vorschau ermöglicht es [!DNL Workfront] auch, neue Funktionen in einer sicheren Umgebung bereitzustellen, bevor sie für die Produktion bereitgestellt werden können. Sie können die neuen Funktionen testen und [!DNL Workfront] Feedback zu ihrer Funktionalität geben, indem Sie auf die Sandbox „Vorschau“ zugreifen. Aus diesem Grund ist der Code der Sandbox-Vorschau immer vor dem Produktions-Code, obwohl Ihre Daten wöchentlich aktualisiert werden.

Die Vorschauumgebung ist ideal für Schulungen, das Testen neuer Funktionen und das Bestimmen der Einrichtungsfunktionalität.

>[!NOTE]
>
>Beachten Sie beim Zugriff auf die Sandbox-Vorschau das blaue Banner oben auf dem Bildschirm. Das Banner kann nicht entfernt werden, während Sie in dieser Umgebung arbeiten.
>
>Der Name der Umgebung, auf die Sie zugreifen (Vorschau), und die Release-Version des Codes werden im Banner angezeigt. Klicken Sie **[!UICONTROL siehe Neue Funktionen]**, um Informationen über diese Version zu erhalten.
>
>![Vorschau des Banners](assets/preview-banner-nwe-350x161.png)

## Zugriff auf die Vorschau-Sandbox

Standardmäßig haben Sie als [!DNL Workfront] Zugriff auf die [!UICONTROL Vorschau] Sandbox-Umgebung. Wenn Sie nicht wie in diesem Abschnitt beschrieben auf [!UICONTROL Vorschau]-Sandbox-Umgebung zugreifen können, wenden Sie sich an Ihren [!DNL Workfront] oder an unser Support-Team.


### Zugriff auf die Sandbox-Vorschau über die [!DNL Workfront] {#accessing-the-preview-sandbox-from-the-workfront-interface}

Als [!DNL Workfront] können Sie über die [!DNL Workfront] auf die Sandbox-Vorschau zugreifen.

So greifen Sie auf die Sandbox-Vorschau zu:

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL System]** > **[!UICONTROL Voreinstellungen]**.

1. Klicken Sie **[!UICONTROL Abschnitt]** Testumgebungen“ auf **[!UICONTROL Sandbox-Vorschau]**.

1. Melden Sie sich mit Ihren Vorschau-Anmeldedaten an.

   Diese sollten mit Ihren Produktionsanmeldeinformationen übereinstimmen, es sei denn, Sie haben sie in der Produktion nach der Aktualisierung der Vorschau geändert. Die Anmeldungen werden nur synchronisiert, wenn eine Aktualisierung erfolgt. Sie werden nicht automatisch synchronisiert.

### Zugriff auf die Sandbox-Vorschau über eine URL {#accessing-the-preview-sandbox-using-a-url}

Sie können über eine URL auf die Sandbox-Vorschau zugreifen.

#### Zugriff auf die Vorschau-Sandbox für Konten auf Cluster 1, 2, 3 und 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Die URL für die Sandbox-Vorschau lautet: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Wenn Sie Lesezeichen haben, die auf die alte URL für die Vorschau-Sandbox verlinken, notieren Sie sich diese Änderung und aktualisieren Sie die URL in Ihren Lesezeichen.

So melden Sie sich mit einer URL bei der Sandbox-Vorschau an:

1. Navigieren Sie zu dieser URL: `https://companyname.preview.workfront.com/`.

   Wenn Sie EMEA-Kunde sind und sich Ihr Konto auf Cluster 4 befindet, lesen Sie den Abschnitt Zugriff auf die Vorschau-Sandbox für Konten auf Cluster 4 (EMEA-Konten) weiter unten.

1. Melden Sie sich mit Ihren Vorschau-Anmeldedaten an.

   >[!TIP]
   >
   >Die Vorschau-Anmeldedaten sollten den Produktions-Anmeldedaten entsprechen, es sei denn, Sie haben sie in der Produktionsumgebung nach der Aktualisierung der Vorschau geändert. Die Anmeldungen werden nur synchronisiert, wenn eine Aktualisierung erfolgt. Sie werden nicht automatisch synchronisiert.


#### Zugriff auf die Vorschau-Sandbox für Konten auf Cluster 4 (EMEA-Konten) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

So melden Sie sich mit einer URL bei der Sandbox-Vorschau an:

1. Navigieren Sie zu dieser URL: `https://companyname.preview.workfront.com/`.

   Sie können auch auf die Sandbox-Vorschau zugreifen, indem Sie [https://cl04.preview.workfront.com/login} ](https://cl04.preview.workfront.com/login).

1. Melden Sie sich mit Ihren Vorschau-Anmeldedaten an.

   Die Vorschau-Anmeldedaten sollten den Produktions-Anmeldedaten entsprechen, es sei denn, Sie haben sie in der Produktionsumgebung nach der Aktualisierung der Vorschau geändert. Die Anmeldungen werden nur synchronisiert, wenn eine Aktualisierung erfolgt. Sie werden nicht automatisch synchronisiert.

## E-Mails von der Vorschau-Sandbox empfangen

Workfront deaktiviert die gesamte E-Mail-Kommunikation über die Sandbox-Vorschau-Umgebung. Wenn Sie E-Mail-Benachrichtigungen von der Sandbox-Vorschau-Umgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren. Weitere Informationen zur Aktivierung von E-Mail-Benachrichtigungen in der Sandbox-Vorschau-Umgebung finden Sie unter [E-Mail-Versand über die Sandbox-Vorschau-Umgebung aktivieren](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Berichtsversand und Push-Benachrichtigungen in der Mobile App sind für die Sandbox-Vorschau-Umgebung immer deaktiviert. Weder Sie noch der [!DNL Workfront]-Administrator können die Berichtsbereitstellung oder Push-Benachrichtigungen für die Mobile App aktivieren, wenn Sie auf die Sandbox-Vorschau-Umgebung zugreifen.
>
>Weitere Informationen zu Berichtssendungen für die Produktionsumgebung finden Sie unter [Übersicht über die Berichtsbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Einmaliges Anmelden (SSO)

Wenn Sie SSO verwenden, wenden Sie sich an unser Support-Team, um sicherzustellen, dass es ordnungsgemäß konfiguriert ist, sodass Sie Ihre SSO-Anmeldeinformationen verwenden können, um sich bei der Sandbox [!UICONTROL Vorschau] anzumelden. Wenn Ihre erste Anmeldung fehlschlägt, wenden Sie sich an Ihren regulären Support-Kontakt oder [!DNL Workfront] Administrator, um Hilfe zu erhalten.

Weitere Informationen zum einmaligen Anmelden finden Sie unter [Übersicht über das einmalige Anmelden in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Konfigurieren von Single Sign-On in der Sandbox für die Vorschau

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in das [!DNL Adobe Admin Console] integriert wurden. Wenn Ihre Organisation in die [!DNL Adobe Admin Console] integriert wurde, ist keine Aktion erforderlich.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die [!DNL Adobe Admin Console] integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Wenn Sie Ihre Vorschau-Sandbox für die Verwendung mit einer Single Sign-On-Lösung konfigurieren möchten, können Sie sie separat von Ihrer Produktionsumgebung konfigurieren. Die SSO-Konfiguration in der Sandbox-Vorschau ist unabhängig von Ihrer SSO-Konfiguration in der Produktionsumgebung.

Wenn Ihre Sandbox-Vorschau (jedes Wochenende) aktualisiert wird, werden die SSO-Informationen nicht aus Ihrer Produktionsumgebung kopiert, um die Sandbox-Vorschau-Konfiguration zu überschreiben.

Die Schritte zum Konfigurieren von Single Sign-on in der Vorschau-Sandbox ähneln denen zum Konfigurieren in der Produktionsumgebung.

Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit SSO finden Sie unter [Übersicht über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Automatische Neuberechnung der Projektzeitleisten

Durch die Neuberechnung der Zeitleisten können Manager sehen, wie sich Kräfte außerhalb des Projekts auf die Zeitleiste des Projekts auswirken. Der Zeitplan eines Projekts bezieht sich auf die geplanten und geplanten Termine für das Projekt.

Als Workfront-Administrator können Sie konfigurieren, wenn Workfront die Projektzeitleisten automatisch neu berechnet. Workfront kann Projektzeitleisten entweder jede Nacht oder bei einer Änderung des Projektumfangs oder beides neu berechnen.

Weitere Informationen finden Sie unter [Konfigurieren von Zeitleisten-Neuberechnungen für Projekte](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-timeline-recalculations-projects.md).

In der Vorschau-Umgebung ist die nächtliche Neuberechnung deaktiviert und die Projektzeitleisten werden nicht automatisch neu berechnet. Sie müssen die Zeitleiste des Projekts für die Vorschau-Umgebung manuell neu berechnen. Weitere Informationen finden Sie unter [Neuberechnen von Projektzeitleisten](/help/quicksilver/manage-work/projects/manage-projects/recalculate-project-timeline.md).


## Vorschau der Umgebungsleistung und -verfügbarkeit

* [!DNL Workfront] Vorschau-Umgebungen sind nicht für Leistungs- oder Belastungstests vorgesehen. Verwenden Sie diese Umgebungen vielmehr, um die Funktionsfunktionen mit den vorhandenen Workflows Ihres Unternehmens zu validieren.

* Workflows mit Dokumenten sollten sich auf Prozesse und nicht auf Belastungstests konzentrieren. Große Dateien werden in Sandbox-Umgebungen nicht unterstützt.

* [!DNL Workfront] Vorschau-Umgebungen sind so konzipiert, dass sie immer verfügbar sind.

* Jeder Ausfall einer [!DNL Workfront]-Vorschau-Umgebung während der regulären Geschäftszeiten hat unmittelbar nach der Behebung von Produktionsproblemen (sofern vorhanden) oberste Priorität.

* Jeder Ausfall einer [!DNL Workfront] Vorschau-Umgebung am Wochenende (samstags und sonntags) wird behoben, sodass die Umgebung montags zu den Geschäftszeiten geöffnet ist.
