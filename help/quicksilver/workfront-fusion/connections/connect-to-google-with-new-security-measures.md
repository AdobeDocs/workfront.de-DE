---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: connections-annd-webhooks
title: Verbindung  [!DNL Adobe Workfront Fusion] / [!DNL Google Services]  mit aktualisierten Sicherheitsmaßnahmen
description: Google hat kürzlich Einschränkungen für die Verwendung seiner API eingeführt. In diesem Artikel wird beschrieben, wie Sie  [!DNL Adobe Workfront Fusion]  Google verbinden, wobei diese Sicherheitsmaßnahmen für die Aktualisierung berücksichtigt werden.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Verbinden von [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] mit aktualisierten Sicherheitsmaßnahmen

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services]

[!DNL Google] hat ab dem 1. Juni 2020 Einschränkungen für die Verwendung der API durch -Benutzer eingeführt. Diese Sicherheitsmaßnahmen schützen [!DNL Google] Nutzer vor Datenlecks oder Missbrauch ihrer personenbezogenen Daten auf [!DNL Google]. Die Einschränkungen beziehen sich auf die [!DNL Gmail] und [!DNL Google Drive] Apps. Weitere Informationen zu diesen Einschränkungen finden Sie unter „Zusätzliche Anforderungen für bestimmte API-Bereiche“ in der [[!DNL Google] API-Services-Benutzerdatenrichtlinie](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Um auf eingeschränkte Bereiche zugreifen zu können, muss der verbundene Dienst ([!DNL Adobe Workfront Fusion] oder jeder andere Dienst, der über die API auf die Daten des Benutzers zugreifen möchte) überprüft werden und über ein Bewertungsschreiben verfügen, um nachzuweisen, dass der Dienst sicher und transparent in Bezug auf die Verwendung der Daten ist. [!DNL Workfront Fusion] erfüllt alle Anforderungen von [!DNL Google] für den Zugang zu beschränkten Bereichen. Allerdings verfügen die meisten der von Drittanbietern verbundenen Dienste in [!DNL Workfront Fusion] nicht über das Begutachtungsschreiben und erfüllen daher nicht [!DNL Google] Bedingungen. Aus diesem Grund ist es [!DNL Workfront Fusion] nicht erlaubt, Daten an diese Services zu senden.

## Ausnahmen von [!DNL Google Services] Einschränkungen

Es gibt einige Ausnahmen, die es ermöglichen, Daten an einen nicht genehmigten Drittanbieterdienst zu senden, der nicht über das Begutachtungsschreiben verfügt, ohne die neuen Einschränkungen zu verletzen. Sie unterscheiden sich je nach [!DNL Google Workspace] mit dem [!DNL Workfront Fusion] OAuth-Client, [!DNL Google Workspace] mit einem anderen OAuth-Client oder [!DNL @gmail.com] und [!DNL @google.mail.com].

* [[!DNL Google Workspace] mit  [!DNL Workfront Fusion] -OAuth-Client](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL Google Workspace] mit einem anderen OAuth-Client](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] und [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL Google Workspace] mit [!DNL Workfront Fusion] OAuth-Client

[!DNL Workfront Fusion] verwendet die [!UICONTROL Domain-wide Installation] Exception. Die Domain-weite Installation ist für [!DNL Google Workspace] Benutzer geeignet und ermöglicht es Benutzern, nicht genehmigte Services ohne Einschränkungen zu integrieren. Wenn Sie ein Google Workspace-Benutzer sind, müssen Sie keine zusätzlichen Schritte ausführen und können direkt eine Verbindung zu nicht genehmigten Services herstellen.

### [!DNL Google Workspace] mit einem anderen OAuth-Client

[!DNL Google Workspace] Benutzer, die lieber ihren eigenen OAuth-Client anstelle des [!DNL Workfront Fusion] OAuth-Clients verwenden, können über den Ansatz der [!UICONTROL internen]-Verwendung eine Verbindung zu [!DNL Google Services] herstellen. Diese Option ist für fortgeschrittene Benutzer gedacht. Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] und [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Benutzer, die über [!DNL @gmail.com] oder [!DNL @googlemail.com] auf [!DNL Google Services] zugreifen, können über den Ansatz der persönlichen Nutzung eine Verbindung zu [!DNL Google Services] herstellen. Diese Option ist für fortgeschrittene Benutzer gedacht. Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQs

* [Welche Apps in [!DNL Adobe Workfront Fusion] sind betroffen?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Habe ich ein - [!DNL Google Workspace] ?](#do-i-have-a-g-suite-account)
* [Was sollte ich tun, wenn ich  [!DNL @gmail.com]  oder  [!DNL @googlemail.com]  verwende?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Was sollte ich als Benutzer  [!DNL Google Workspace] ?](#what-should-i-do-if-im-a-g-suite-user)

### Welche Apps in [!DNL Adobe Workfront Fusion] sind betroffen? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail] und E-Mail (mit [!DNL Gmail] Konto verbunden).

### Habe ich ein [!DNL Google Workspace]? {#do-i-have-a-g-suite-account}

Wenn Ihre E-Mail-Adresse mit [!DNL @gmail.com] oder [!DNL @googlemail.com] endet, ist Ihr Konto kein [!DNL Google Workspace]. Wenn Ihr [!DNL Google]-Konto mit einer benutzerdefinierten Domain wie @my-company.com endet, ist es ein [!DNL Google Workspace].

### Was sollte ich tun, wenn ich [!DNL @gmail.com] oder [!DNL @googlemail.com] Benutzer bin? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Diese neuen Einschränkungen gelten nur, wenn Sie [!DNL Google Drive] oder [!DNL Gmail] integrieren. Wenn Sie eine Verbindung zu [!DNL Google Drive] oder [!DNL Gmail] herstellen möchten, können Sie

* Zu [!DNL Google Workspace] wechseln

  oder

* Erstellen Sie einen benutzerdefinierten OAuth-Client. Diese Option ist für fortgeschrittene Benutzer gedacht.

  Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] mit [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Wenn Sie einen anderen Service als [!DNL Google Drive] oder [!DNL Gmail] integrieren möchten, gelten diese Einschränkungen nicht.

Anweisungen zum Verbinden anderer [!DNL Google Services] mit [!DNL Workfront Fusion] finden Sie unter [Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) im Artikel [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Was sollte ich tun, wenn ich [!DNL Google Workspace] verwende? {#what-should-i-do-if-im-a-g-suite-user}

Es ist keine Aktion erforderlich.
