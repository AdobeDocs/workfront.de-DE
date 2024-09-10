---
user-type: administrator
content-type: overview;how-to-procedural
product-area: system-administration
navigation-topic: workfront-testing-environments
title: Vorschau der Sandbox-Umgebung [!DNL Adobe Workfront]
description: Die Vorschau-Sandbox ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient. Es wird jedes Wochenende von Workfront aktualisiert. Daten, die am Freitag zu Ihrer Live-Umgebung hinzugefügt wurden, werden am folgenden Montag in Ihrer Vorschau-Sandbox angezeigt. Alle Support-Pakete haben Zugriff auf diese Sandbox.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: e5c02b8c-854e-4c42-a599-f680443f425d
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 0%

---

# Die Vorschau-Sandbox-Umgebung [!DNL Adobe Workfront]

<!-- Audited: 12/2023 -->

Es gibt zwei Testumgebungen für [!DNL Workfront] , die Repliken Ihrer [!DNL Workfront] -Produktionsumgebung sind:

* Vorschau-Sandbox

  Die Vorschau-Sandbox ist eine Testumgebung, die als Replikation Ihrer Live-Umgebung dient und an jedem Wochenende von [!DNL Workfront] aktualisiert wird. Daten, die am Freitag zu Ihrer Live-Umgebung hinzugefügt wurden, werden am folgenden Montag in Ihrer Vorschau-Sandbox angezeigt.

  Alle Support-Pakete haben Zugriff auf die Vorschau-Sandbox.

* Die benutzerdefinierte Aktualisierungs-Sandbox

  Die Sandbox für benutzerdefinierte Aktualisierungen ist eine separate Testumgebung, die von Ihnen manuell aktualisiert wird. Es fallen zusätzliche Kosten an, um die Sandbox &quot;Benutzerdefinierte Aktualisierung&quot;zu erhalten. Weitere Informationen zu dieser Umgebung finden Sie unter [Die  [!DNL Adobe Workfront] Sandbox-Umgebung für benutzerdefinierte Aktualisierung](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p> </p> </th> 
   <th> <p><strong>[!UICONTROL Standard] Support-Paket</strong> </p> </th> 
   <th> <p><strong>[!UICONTROL Plus], [!UICONTROL Preferred] und [!UICONTROL Enterprise] Support Packs</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p>Vorschau-Sandbox</p> </td> 
   <td scope="col"> <p>ms</p> </td> 
   <td scope="col"> <p>ms</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p>Benutzerdefinierte Aktualisierungs-Sandbox</p> </td> 
   <td scope="col"> <p> </p> </td> 
   <td scope="col"> <p>ms</p> </td> 
  </tr> 
 </tbody> 
</table>

## Vorschau-Sandbox

Die Vorschau-Sandbox dient als Umgebung, in der Benutzer in Ihrer Organisation Daten aus der Produktionsumgebung sicher testen und verwenden können, ohne die Produktionsumgebung zu beeinträchtigen.

Die Vorschau-Sandbox enthält Ihre tatsächlichen Produktionsdaten. Sie wird jedoch jedes Wochenende aktualisiert, sodass die Daten bis zu einer Woche hinter der Produktionsumgebung liegen können. Elemente, die seit der letzten Aktualisierungszeit erstellt wurden, befinden sich bis zur folgenden Aktualisierung in der Umgebung &quot;Sandbox-Vorschau&quot;.

Daten fließen unidirektional, von der Produktion zur Vorschau und nicht umgekehrt. Eine Aktualisierung der Vorschauumgebung wird immer von [!DNL Workfront] an jedem Wochenende geplant.

Vorschau-Sandbox ermöglicht es [!DNL Workfront] auch, neue Funktionen in einer sicheren Umgebung bereitzustellen, bevor sie für die Bereitstellung in der Produktion bereit sind. Sie können die neuen Funktionen testen und [!DNL Workfront] Feedback zu ihrer Funktionalität geben, indem Sie auf die Vorschau-Sandbox zugreifen. Aus diesem Grund liegt der Code der Vorschau-Sandbox immer vor dem Produktions-Code, obwohl Ihre Daten wöchentlich aktualisiert werden.

Die Vorschau-Umgebung eignet sich ideal für Trainings, das Testen neuer Funktionen und die Bestimmung der Einrichtungsfunktionalität.

>[!NOTE]
>
>Beachten Sie beim Zugriff auf die Vorschau-Sandbox das blaue Banner oben im Bildschirm. Das Banner kann während der Arbeit in dieser Umgebung nicht entfernt werden.
>
>Der Name der Umgebung, auf die Sie zugreifen (Vorschau), und die Release-Version des Codes werden im Banner angezeigt. Klicken Sie auf **[!UICONTROL Siehe Neue Funktionen]** , um Informationen zu dieser Version zu erhalten.
>
>![](assets/preview-banner-nwe-350x161.png)

## Zugriff auf die Vorschau-Sandbox

Standardmäßig haben Sie als [!DNL Workfront] -Administrator Zugriff auf die Sandbox-Umgebung [!UICONTROL Vorschau] . Wenn Sie nicht auf die Sandbox-Umgebung [!UICONTROL Vorschau] zugreifen können, wie in diesem Abschnitt beschrieben, wenden Sie sich an Ihren [!DNL Workfront] -Administrator oder unser Support-Team.


### Zugriff auf die Vorschau-Sandbox über die [!DNL Workfront]-Oberfläche {#accessing-the-preview-sandbox-from-the-workfront-interface}

Als [!DNL Workfront] -Administrator können Sie über die Benutzeroberfläche von [!DNL Workfront] auf die Vorschau-Sandbox zugreifen.

So greifen Sie auf die Vorschau-Sandbox zu:

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL System]** > **[!UICONTROL Voreinstellungen]**.

1. Klicken Sie im Abschnitt **[!UICONTROL Testumgebungen]** auf **[!UICONTROL Sandbox-Vorschau]**.

1. Melden Sie sich mit Ihren Vorschauanmeldeinformationen an.

   Diese sollten mit Ihren Produktionsberechtigungen übereinstimmen, es sei denn, Sie haben sie in der Produktion geändert, nachdem die Vorschau aktualisiert wurde. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.

### Zugriff auf die Vorschau-Sandbox mithilfe einer URL {#accessing-the-preview-sandbox-using-a-url}

Sie können über eine URL auf die Vorschau-Sandbox zugreifen.

#### Zugreifen auf die Vorschau-Sandbox für Konten auf Cluster 1,2,3 und 5 {#accessing-the-preview-sandbox-for-accounts-on-cluster-1-2-3-and-5}

Die URL für die Vorschau-Sandbox lautet: `https://companyname.preview.workfront.com/`.

>[!NOTE]
>
>Wenn Sie Lesezeichen mit der alten URL für die Vorschau-Sandbox verknüpft haben, notieren Sie sich diese Änderung und aktualisieren Sie die URL in Ihren Lesezeichen.

So melden Sie sich mit einer URL bei der Vorschau-Sandbox an:

1. Navigieren Sie zu dieser URL: `https://companyname.preview.workfront.com/`.

   Wenn Sie EMEA-Kunde sind und Ihr Konto auf Cluster 4 ist, lesen Sie den Abschnitt Zugriff auf die Vorschau-Sandbox für Konten auf Cluster 4 (EMEA-Konten) unten.

1. Melden Sie sich mit Ihren Anmeldedaten für die Vorschau an.

   >[!TIP]
   >
   >Ihre Vorschauberechtigungen sollten mit Ihren Produktionsberechtigungen übereinstimmen, es sei denn, Sie haben sie in der Produktion geändert, nachdem die Vorschauaktualisierung stattgefunden hat. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.


#### Zugreifen auf die Vorschau-Sandbox für Konten auf Cluster 4 (EMEA-Konten) {#accessing-the-preview-sandbox-for-accounts-on-cluster-4-emea-accounts}

So melden Sie sich mit einer URL bei der Vorschau-Sandbox an:

1. Navigieren Sie zu dieser URL: `https://companyname.preview.workfront.com/`.

   Sie können auch auf die Vorschau-Sandbox zugreifen, indem Sie zu [https://cl04.preview.workfront.com/login](https://cl04.preview.workfront.com/login) navigieren.

1. Melden Sie sich mit Ihren Anmeldedaten für die Vorschau an.

   Ihre Vorschauberechtigungen sollten mit Ihren Produktionsberechtigungen übereinstimmen, es sei denn, Sie haben sie in der Produktion geändert, nachdem die Vorschauaktualisierung stattgefunden hat. Die Anmeldungen werden nur bei einer Aktualisierung synchronisiert. Sie werden nicht automatisch synchronisiert.

## Empfangen von E-Mails über die Vorschau-Sandbox

Workfront deaktiviert die gesamte E-Mail-Kommunikation in der Vorschau-Sandbox-Umgebung. Wenn Sie E-Mail-Benachrichtigungen von der Vorschau-Sandbox-Umgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren. Weitere Informationen zum Aktivieren von E-Mail-Benachrichtigungen in der Vorschau-Sandbox-Umgebung finden Sie unter [Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

>[!NOTE]
>
>Berichtversand und Push-Benachrichtigungen in der Mobile App sind in der Sandbox-Umgebung &quot;Vorschau&quot;immer deaktiviert. Weder Sie noch der Administrator [!DNL Workfront] können die Berichtübermittlung oder Push-Benachrichtigungen für die mobile App aktivieren, wenn Sie auf die Umgebung &quot;Sandbox-Vorschau&quot;zugreifen.
>
>Weitere Informationen zu Berichtbereitstellungen für die Produktionsumgebung finden Sie unter [Übersicht über die Berichtbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).


## Einmaliges Anmelden (SSO)

Wenn Sie SSO verwenden, wenden Sie sich an unser Support-Team, um sicherzustellen, dass es ordnungsgemäß konfiguriert ist, damit Sie sich mit Ihren SSO-Anmeldeinformationen bei der Sandbox [!UICONTROL Vorschau] anmelden können. Wenn Ihre anfängliche Anmeldung fehlschlägt, wenden Sie sich an Ihren regulären Support-Ansprechpartner oder an den [!DNL Workfront] -Administrator, um Hilfe zu erhalten.

Weitere Informationen zu Single Sign-On finden Sie unter [Überblick über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Konfigurieren von Single Sign-On in der Vorschau-Sandbox

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in den [!DNL Adobe Admin Console] integriert wurden. Wenn Ihr Unternehmen in die [!DNL Adobe Admin Console] integriert wurde, ist keine Aktion erforderlich.
>
>Eine Liste der Vorgehensweisen, die sich je nachdem, ob Ihr Unternehmen in den [!DNL Adobe Admin Console] integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede ([!UICONTROL Adobe Workfront]/[!UICONTROL Adobe Business Platform])](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


Wenn Sie Ihre Vorschau-Sandbox so konfigurieren möchten, dass sie mit einer Single-Sign-On-Lösung funktioniert, können Sie dies tun, indem Sie sie getrennt von Ihrer Produktionsumgebung konfigurieren. Die SSO-Konfiguration in der Vorschau-Sandbox ist unabhängig von Ihrer SSO-Konfiguration in der Produktionsumgebung.

Wenn Ihre Vorschau-Sandbox aktualisiert wird (an jedem Wochenende), werden die SSO-Informationen nicht aus Ihrer Produktionsumgebung kopiert, um die Vorschau-Sandbox-Konfiguration zu überschreiben.

Die Schritte zum Konfigurieren von Single Sign-on in der Vorschau-Sandbox ähneln denen zum Konfigurieren in der Produktionsumgebung.

Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit SSO finden Sie unter [Überblick über die einmalige Anmeldung in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md).

## Vorschau der Umgebungsleistung und -verfügbarkeit

[!DNL Workfront] Vorschau-Umgebungen sind nicht für Leistungs- oder Belastungstests vorgesehen. Verwenden Sie stattdessen diese Umgebungen, um die Funktionsfunktionalität mit den vorhandenen Workflows Ihres Unternehmens zu validieren.

[!DNL Workfront] Die Vorschau-Umgebungen sollten immer verfügbar sein.

Jeder Ausfall der Vorschau-Umgebung während der regulären Geschäftszeiten wird unmittelbar nach Behebung etwaiger Produktionsprobleme eine erste Priorität haben.[!DNL Workfront]

Jeder Ausfall einer [!DNL Workfront] Vorschau-Umgebung an Wochenenden (Samstags und Sonntagen) wird behoben, damit die Umgebung am Montag für Geschäftszeiten ausgeführt wird.
