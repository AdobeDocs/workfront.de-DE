---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: connections-annd-webhooks
title: Verbinden von [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mit aktualisierten Sicherheitsmaßnahmen
description: Google hat kürzlich Einschränkungen für die Verwendung der API durch Benutzer eingeführt. In diesem Artikel wird beschrieben, wie Sie eine Verbindung mit Google herstellen, wobei diese aktualisierten Sicherheitsmaßnahmen berücksichtigt werden. [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mit aktualisierten Sicherheitsmaßnahmen verbinden

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] Beschränkungen

[!DNL Google] führte ab dem 1. Juni 2020 Einschränkungen dafür ein, wie Benutzer ihre API verwenden können. Diese Sicherheitsmaßnahmen schützen [!DNL Google] Benutzer vor dem Verlust oder Missbrauch ihrer personenbezogenen Daten auf [!DNL Google]. Die Einschränkungen beziehen sich auf die Anwendungen [!DNL Gmail] und [!DNL Google Drive]. Weitere Informationen zu diesen Einschränkungen finden Sie unter &quot;Zusätzliche Anforderungen für bestimmte API-Bereiche&quot;in der [[!DNL Google] Benutzerdatenrichtlinie für API-Dienste](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes) .

Um auf eingeschränkte Bereiche zugreifen zu können, muss der verbundene Dienst ([!DNL Adobe Workfront Fusion]) oder jeder andere Dienst, der über die API auf die Daten des Benutzers zugreifen möchte, überprüft werden und über ein Überprüfungsschreiben verfügen, das nachweist, dass der Dienst sicher und transparent in Bezug auf die Verwendung der Daten ist. [!DNL Workfront Fusion] erfüllt alle Anforderungen von [!DNL Google] für den Zugriff auf eingeschränkte Bereiche. Die meisten Dienste mit Drittanbieteranschluss in [!DNL Workfront Fusion] verfügen jedoch nicht über das Bewertungsschreiben und erfüllen daher nicht die [!DNL Google]-Bedingungen. Daher ist [!DNL Workfront Fusion] nicht berechtigt, Daten an diese Dienste zu senden.

## Ausnahmen von [!DNL Google Services] -Einschränkungen

Es gibt einige Ausnahmen, die es ermöglichen, Daten an einen nicht zugelassenen Drittanbieterdienst zu senden, der nicht über die Bewertungsbescheinigung verfügt, ohne gegen eine der neuen Beschränkungen zu verstoßen. Sie unterscheiden sich je nach [!DNL Google Workspace] und dem [!DNL Workfront Fusion] OAuth-Client, [!DNL Google Workspace] mit einem anderen OAuth-Client oder [!DNL @gmail.com] und [!DNL @google.mail.com].

* [[!DNL Google Workspace] mit  [!DNL Workfront Fusion] OAuth-Client](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] mit einem anderen OAuth-Client](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] und  [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] mit [!DNL Workfront Fusion] OAuth-Client

[!DNL Workfront Fusion] verwendet die Ausnahme [!UICONTROL Domänenweite Installation] . Die domänenweite Installation ist für [!DNL Google Workspace] -Benutzer geeignet und ermöglicht es Benutzern, nicht genehmigte Dienste ohne Einschränkungen zu integrieren. Wenn Sie Google Workspace-Benutzer sind, müssen Sie keine zusätzlichen Schritte ausführen und können direkt eine Verbindung zu nicht genehmigten Diensten herstellen.

### [!DNL Google Workspace] mit einem anderen OAuth-Client

[!DNL Google Workspace] Benutzer, die lieber ihren eigenen OAuth-Client anstelle des [!DNL Workfront Fusion] OAuth-Clients verwenden, können über den Einsatz von [!UICONTROL Internal] eine Verbindung zu [!DNL Google Services] herstellen. Diese Option ist für fortgeschrittene Benutzer gedacht. Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] und [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Benutzer, die über [!DNL @gmail.com] oder [!DNL @googlemail.com] auf [!DNL Google Services] zugreifen, können sich über den Ansatz für die persönliche Verwendung mit [!DNL Google Services] verbinden. Diese Option ist für fortgeschrittene Benutzer gedacht. Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQs

* [Welche Anwendungen in [!DNL Adobe Workfront Fusion] sind betroffen?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Verfüge ich über ein [!DNL Google Workspace] Konto?](#do-i-have-a-g-suite-account)
* [Was sollte ich tun, wenn ich  [!DNL @gmail.com] oder [!DNL @googlemail.com] Benutzer bin?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Was sollte ich tun, wenn ich ein [!DNL Google Workspace] Benutzer bin?](#what-should-i-do-if-im-a-g-suite-user)

### Welche Apps in [!DNL Adobe Workfront Fusion] sind betroffen? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] und E-Mail (mit dem [!DNL Gmail] -Konto verbunden).

### Verfüge ich über ein [!DNL Google Workspace]-Konto? {#do-i-have-a-g-suite-account}

Wenn Ihre E-Mail-Adresse mit [!DNL @gmail.com] oder [!DNL @googlemail.com] endet, ist Ihr Konto kein [!DNL Google Workspace] -Konto. Wenn Ihr [!DNL Google] -Konto mit einer benutzerdefinierten Domäne wie @my-company.com endet, ist es ein [!DNL Google Workspace] -Konto.

### Was soll ich tun, wenn ich [!DNL @gmail.com]- oder [!DNL @googlemail.com]-Benutzer bin? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Diese neuen Einschränkungen gelten nur, wenn Sie [!DNL Google Drive] oder [!DNL Gmail] integrieren. Wenn Sie eine Verbindung zu [!DNL Google Drive] oder [!DNL Gmail] herstellen möchten, können Sie

* Zu [!DNL Google Workspace] wechseln

  oder

* Erstellen Sie einen benutzerdefinierten OAuth-Client. Diese Option ist für fortgeschrittene Benutzer gedacht.

  Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mithilfe eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Wenn Sie einen anderen Dienst als [!DNL Google Drive] oder [!DNL Gmail] integrieren möchten, gelten diese Einschränkungen nicht.

Anweisungen zum Verbinden anderer [!DNL Google Services] mit [!DNL Workfront Fusion] finden Sie unter [Verbinden der App oder des Webdiensts des Moduls mit  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) im Artikel [Erstellen eines Szenarios in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Was sollte ich tun, wenn ich ein [!DNL Google Workspace] -Benutzer bin? {#what-should-i-do-if-im-a-g-suite-user}

Es sind keine Maßnahmen erforderlich.
