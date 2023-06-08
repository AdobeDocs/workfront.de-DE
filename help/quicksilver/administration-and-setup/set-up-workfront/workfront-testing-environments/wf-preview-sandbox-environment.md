---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Die [!DNL Adobe Workfront] Vorschau der Sandbox-Umgebung
description: Die Vorschau-Sandbox ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient. Es wird jedes Wochenende von Workfront aktualisiert. Daten, die am Freitag zu Ihrer Live-Umgebung hinzugefügt wurden, werden am folgenden Montag in Ihrer Vorschau-Sandbox angezeigt. Alle Support-Pakete haben Zugriff auf diese Sandbox.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '1212'
ht-degree: 0%

---

# Die [!DNL Adobe Workfront] Vorschau der Sandbox-Umgebung

Es gibt zwei Testumgebungen für [!DNL Workfront] , die Repliken Ihrer [!DNL Workfront] Produktionsumgebung:

* Vorschau-Sandbox

   Die Vorschau-Sandbox ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient und an jedem Wochenende aktualisiert wird [!DNL Workfront]. Daten, die am Freitag zu Ihrer Live-Umgebung hinzugefügt wurden, werden am folgenden Montag in Ihrer Vorschau-Sandbox angezeigt.

   Alle Support-Pakete haben Zugriff auf die Vorschau-Sandbox.

* Die benutzerdefinierte Aktualisierungs-Sandbox

   Die Sandbox für benutzerdefinierte Aktualisierungen ist eine separate Testumgebung, die von Ihnen manuell aktualisiert wird. Es fallen zusätzliche Kosten an, um die Sandbox für benutzerdefinierte Aktualisierung zu erhalten. Weitere Informationen zu dieser Umgebung finden Sie unter [Die [!DNL Adobe Workfront] Benutzerdefinierte Sandbox-Umgebung aktualisieren](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard] Support-Paket</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus], [!UICONTROL Preferred] und [!UICONTROL Enterprise] Support Packages</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Vorschau-Sandbox</p> </td> 
   <td scope="col"> <p>ms</p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Benutzerdefinierte Aktualisierungs-Sandbox</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>✔</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vorschau-Sandbox

Die Vorschau-Sandbox dient als Umgebung, in der Benutzer in Ihrer Organisation Daten aus der Produktionsumgebung sicher testen und verwenden können, ohne die Produktionsumgebung zu beeinträchtigen.

Die Vorschau-Sandbox enthält Ihre tatsächlichen Produktionsdaten. Er wird jedoch jedes Wochenende aktualisiert, sodass die Daten bis zu einer Woche hinter der Produktionsumgebung liegen können. Elemente, die seit der letzten Aktualisierungszeit erstellt wurden, befinden sich bis zur folgenden Aktualisierung in der Umgebung &quot;Sandbox-Vorschau&quot;.

Daten fließen unidirektional, von der Produktion zur Vorschau und nicht umgekehrt. Eine Aktualisierung der Vorschauumgebung wird immer von [!DNL Workfront] jedes Wochenende.

Vorschau-Sandbox ermöglicht auch [!DNL Workfront] , um neue Funktionen in einer sicheren Umgebung bereitzustellen, bevor sie für die Bereitstellung in der Produktion bereit sind. Sie können die neuen Funktionen testen und [!DNL Workfront] Feedback zu ihrer Funktionalität durch Zugriff auf die Vorschau-Sandbox. Aus diesem Grund liegt der Code der Vorschau-Sandbox immer vor dem Produktions-Code, obwohl Ihre Daten wöchentlich aktualisiert werden.

Die Vorschau-Umgebung eignet sich ideal für Trainings, das Testen neuer Funktionen und die Bestimmung der Einrichtungsfunktionalität.

>[!NOTE]
>
>Beachten Sie beim Zugriff auf die Vorschau-Sandbox das blaue Banner oben im Bildschirm. Das Banner kann während der Arbeit in dieser Umgebung nicht entfernt werden.
>
>Der Name der Umgebung, auf die Sie zugreifen (Vorschau), und die Release-Version des Codes werden im Banner angezeigt. Klicken **[!UICONTROL Neue Funktionen]** für Informationen zu dieser Version.
>
>![](assets/preview-banner-nwe-350x161.png)

## Zugriff auf die Vorschau-Sandbox

Standardmäßig wird als [!DNL Workfront] Administrator haben Sie Zugriff auf die [!UICONTROL Vorschau] Sandbox-Umgebung. Wenn Sie nicht auf die [!UICONTROL Vorschau] Sandbox-Umgebung, wie in diesem Abschnitt beschrieben, kontaktieren Sie Ihre [!DNL Workfront] Administrator oder unserem Support-Team.

* [Zugriff auf die Vorschau-Sandbox über [!DNL Workfront] Schnittstelle](#accessing-the-preview-sandbox-from-the-workfront-interface)
* [Zugriff auf die Vorschau-Sandbox mithilfe einer URL](#accessing-the-preview-sandbox-using-a-url)

### Zugriff auf die Vorschau-Sandbox über [!DNL Workfront] Schnittstelle {#accessing-the-preview-sandbox-from-the-workfront-interface}

Als [!DNL Workfront] Administrator können Sie über die [!DNL Workfront] -Schnittstelle.

So greifen Sie auf die Vorschau-Sandbox zu:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL System]** > **[!UICONTROL Voreinstellungen]**.

1. Im **[!UICONTROL Testumgebungen]** Abschnitt, klicken Sie auf **[!UICONTROL Sandbox-Vorschau]**.

1. Melden Sie sich mit Ihren Vorschauanmeldeinformationen an.

   Diese sollten mit Ihren Produktionsberechtigungen übereinstimmen, es sei denn, Sie haben sie in der Produktion geändert, nachdem die Vorschau aktualisiert wurde. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.

### Zugriff auf die Vorschau-Sandbox mithilfe einer URL {#accessing-the-preview-sandbox-using-a-url}

* [Zugreifen auf die Vorschau-Sandbox für Konten auf Cluster 1,2,3 und 5](#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5)
* [Zugreifen auf die Vorschau-Sandbox für Konten auf Cluster 4 (EMEA-Konten)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts)

#### Zugreifen auf die Vorschau-Sandbox für Konten auf Cluster 1,2,3 und 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Die URL für die Vorschau-Sandbox lautet: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Wenn Sie Lesezeichen mit der alten URL für die Vorschau-Sandbox verknüpft haben, notieren Sie sich diese Änderung und aktualisieren Sie die URL in Ihren Lesezeichen.

So melden Sie sich mit einer URL bei der Vorschau-Sandbox an:

1. Navigieren Sie zu dieser URL: `https://companyname.preview.workfront.com/`.

   Wenn Sie EMEA-Kunde sind und Ihr Konto auf Cluster 4 ist, lesen Sie den Abschnitt . [Zugreifen auf die Vorschau-Sandbox für Konten auf Cluster 4 (EMEA-Konten)](#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts) in diesem Artikel.

1. Melden Sie sich mit Ihren Anmeldedaten für die Vorschau an.

   Ihre Vorschauberechtigungen sollten mit Ihren Produktionsberechtigungen übereinstimmen, es sei denn, Sie haben sie in der Produktion geändert, nachdem die Vorschauaktualisierung stattgefunden hat. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.

#### Zugreifen auf die Vorschau-Sandbox für Konten auf Cluster 4 (EMEA-Konten) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

So melden Sie sich mit einer URL bei der Vorschau-Sandbox an:

1. Navigieren Sie zu dieser URL: `https://companyname.preview.workfront.com/`.

   Sie können auch auf die Vorschau-Sandbox zugreifen, indem Sie [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login).

1. Melden Sie sich mit Ihren Anmeldedaten für die Vorschau an.

   Ihre Vorschauberechtigungen sollten mit Ihren Produktionsberechtigungen übereinstimmen, es sei denn, Sie haben sie in der Produktion geändert, nachdem die Vorschauaktualisierung stattgefunden hat. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.

## Empfangen von E-Mails über die Vorschau-Sandbox

Workfront deaktiviert die gesamte E-Mail-Kommunikation in der Vorschau-Sandbox-Umgebung. Wenn Sie E-Mail-Benachrichtigungen von der Vorschau-Sandbox-Umgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren. Weitere Informationen zum Aktivieren von E-Mail-Benachrichtigungen in der Vorschau-Sandbox-Umgebung finden Sie unter [Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Berichtversand und Push-Benachrichtigungen in der Mobile App sind in der Sandbox-Umgebung &quot;Vorschau&quot;immer deaktiviert. Weder du noch der [!DNL Workfront] -Administrator kann die Berichtbereitstellung oder Push-Benachrichtigungen für die mobile App aktivieren, wenn Sie auf die Sandbox-Vorschau-Umgebung zugreifen.
>
>Weitere Informationen zu Berichtbereitstellungen für die Produktionsumgebung finden Sie unter [Berichtversand - Übersicht](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Einmaliges Anmelden (SSO)

Wenn Sie SSO verwenden, wenden Sie sich an unser Support-Team, um sicherzustellen, dass es ordnungsgemäß konfiguriert ist, damit Sie sich mit Ihren SSO-Anmeldeinformationen bei der anmelden können. [!UICONTROL Vorschau] Sandbox. Wenn Ihre anfängliche Anmeldung fehlschlägt, wenden Sie sich an Ihren regulären Support-Ansprechpartner oder [!DNL Workfront] Administrator um Hilfe.

Weitere Informationen zu Single Sign-On finden Sie unter [Überblick über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Konfigurieren von Single Sign-On in der Vorschau-Sandbox

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die [!DNL Adobe Admin Console]. Wenn Ihr Unternehmen bei der [!DNL Adobe Admin Console]keine Maßnahmen erforderlich sind.
>
>Für eine Liste von Verfahren, die je nachdem, ob Ihr Unternehmen in die [!DNL Adobe Admin Console], siehe [Plattformbasierte Verwaltungsunterschiede ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Wenn Sie Ihre Vorschau-Sandbox so konfigurieren möchten, dass sie mit einer Single-Sign-On-Lösung funktioniert, können Sie dies tun, indem Sie sie getrennt von Ihrer Produktionsumgebung konfigurieren. Die SSO-Konfiguration in der Vorschau-Sandbox ist unabhängig von Ihrer SSO-Konfiguration in der Produktionsumgebung.

Wenn Ihre Vorschau-Sandbox aktualisiert wird (an jedem Wochenende), werden die SSO-Informationen nicht aus Ihrer Produktionsumgebung kopiert, um die Vorschau-Sandbox-Konfiguration zu überschreiben.

Die Schritte zum Konfigurieren von Single Sign-on in der Vorschau-Sandbox ähneln denen zum Konfigurieren in der Produktionsumgebung.

Weitere Informationen zur Konfiguration [!DNL Workfront] mit SSO, siehe [Überblick über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Vorschau der Umgebungsleistung und -verfügbarkeit

[!DNL Workfront] Vorschau-Umgebungen sind nicht für Leistungs- oder Belastungstests vorgesehen. Verwenden Sie stattdessen diese Umgebungen, um die Funktionsfunktionalität mit den vorhandenen Workflows Ihres Unternehmens zu validieren.

[!DNL Workfront] Vorschauumgebungen sollten immer verfügbar sein.

Jeder Ausfall zu einem [!DNL Workfront] Die Vorschau der Umgebung während der regulären Geschäftszeiten hat unmittelbar nach der Lösung von etwaigen Produktionsproblemen Priorität.

Jeder Ausfall zu einem [!DNL Workfront] Die Vorschau der Umgebung am Wochenende (Samstag und Sonntag) wird angesprochen, damit die Umgebung am Montag für Geschäftszeiten läuft.
