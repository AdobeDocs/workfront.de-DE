---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: connections-annd-webhooks
title: Verbinden [!DNL Adobe Workfront Fusion] nach [!DNL Google Services] mit aktualisierten Sicherheitsmaßnahmen
description: Google hat kürzlich Einschränkungen für die Verwendung der API durch Benutzer eingeführt. In diesem Artikel wird beschrieben, wie Sie eine Verbindung herstellen [!DNL Adobe Workfront Fusion] an Google, unter Berücksichtigung dieser aktualisierten Sicherheitsmaßnahmen.
author: Becky
feature: Workfront Fusion
exl-id: 32dfef7a-7942-4025-8cb9-055d4e28090b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Verbinden [!DNL Adobe Workfront Fusion] nach [!DNL Google Services] mit aktualisierten Sicherheitsmaßnahmen

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Google Services] Einschränkungen

[!DNL Google] hat Einschränkungen dafür eingeführt, wie Benutzer ihre API ab dem 1. Juni 2020 verwenden können. Diese Sicherheitsmaßnahmen schützen [!DNL Google] Benutzer aus dem Verlust oder Missbrauch ihrer personenbezogenen Daten [!DNL Google]. Die Beschränkungen betreffen die [!DNL Gmail] und [!DNL Google Drive] Apps. Weitere Informationen zu diesen Einschränkungen finden Sie unter &quot;Zusätzliche Anforderungen für bestimmte API-Bereiche&quot;in der [[!DNL Google] Benutzerdatenrichtlinie für API Services](https://developers.google.com/terms/api-services-user-data-policy#additional_requirements_for_specific_api_scopes)

Um auf eingeschränkte Bereiche zuzugreifen, muss der verbundene Dienst ([!DNL Adobe Workfront Fusion] oder andere Dienste, die über die API auf die Daten des Benutzers zugreifen möchten, müssen überprüft werden und über ein Überprüfungsschreiben verfügen, das nachweist, dass der Dienst sicher und transparent in Bezug auf die Verwendung der Daten ist. [!DNL Workfront Fusion] erfüllt alle [!DNL Google]Anforderungen für den Zugang zu eingeschränkten Bereichen. Der größte Teil der Dienste, die von Drittanbietern angeboten werden, ist jedoch [!DNL Workfront Fusion] Sie verfügen nicht über das Überprüfungsschreiben und erfüllen daher nicht die [!DNL Google] Begriffe. Aus diesem Grund [!DNL Workfront Fusion] darf keine Daten an diese Dienste senden.

## Ausnahmen von [!DNL Google Services] Einschränkungen

Es gibt einige Ausnahmen, die es ermöglichen, Daten an einen nicht zugelassenen Drittanbieterdienst zu senden, der nicht über die Bewertungsbescheinigung verfügt, ohne gegen eine der neuen Beschränkungen zu verstoßen. Sie unterscheiden sich je nach [!DNL G Suite] mit dem [!DNL Workfront Fusion] OAuth-Client, [!DNL G Suite] mit einem anderen OAuth-Client oder [!DNL @gmail.com] und [!DNL @google.mail.com].

* [[!DNL G Suite] mit [!DNL Workfront Fusion] OAuth-Client](#g-suite-with-workfront-fusion-oauth-client)
* [[!DNL G Suite] mit einem anderen OAuth-Client](#g-suite-with-another-oauth-client)
* [[!DNL @gmail.com] und [!DNL @googlemail.com]](#gmailcom-and-googlemailcom)

### [!DNL G suite] mit [!DNL Workfront Fusion] OAuth-Client

[!DNL Workfront Fusion] verwendet die [!UICONTROL Domänenweite Installation] Ausnahme. Die domänenweite Installation eignet sich für [!DNL G Suite] Benutzer und ermöglicht Benutzern, nicht genehmigte Dienste ohne Einschränkungen zu integrieren. Wenn Sie G Suite-Benutzer sind, müssen Sie keine zusätzlichen Schritte ausführen und können direkt eine Verbindung zu nicht genehmigten Diensten herstellen.

### [!DNL G suite] mit einem anderen OAuth-Client

[!DNL G Suite] -Benutzer, die lieber ihren eigenen OAuth-Client verwenden, anstatt die [!DNL Workfront Fusion] OAuth-Client kann eine Verbindung zu [!DNL Google Services] durch [!UICONTROL intern] Verwenden Sie den Ansatz. Diese Option ist für fortgeschrittene Benutzer gedacht. Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] nach [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

### [!DNL @gmail.com] und [!DNL @googlemail.com] {#gmailcom-and-googlemailcom}

Benutzer, auf die zugegriffen wird [!DNL Google Services] bis [!DNL @gmail.com] oder [!DNL @googlemail.com] kann eine Verbindung zu [!DNL Google Services] durch den Ansatz der persönlichen Nutzung. Diese Option ist für fortgeschrittene Benutzer gedacht. Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] nach [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## FAQs

* [Funktionen in [!DNL Adobe Workfront Fusion] sind betroffen?](#what-apps-in-adobe-workfront-fusion-are-affected)
* [Verfüge ich über ein [!DNL G Suite]-Konto?](#do-i-have-a-g-suite-account)
* [Was soll ich tun, wenn ich [!DNL @gmail.com] oder [!DNL @googlemail.com] Benutzer?](#what-should-i-do-if-im-gmailcom-or-googlemailcom-user)
* [Was sollte ich tun, wenn ich [!DNL G Suite]-Benutzer bin?](#what-should-i-do-if-im-a-g-suite-user)

### Funktionen in [!DNL Adobe Workfront Fusion] sind betroffen? {#what-apps-in-adobe-workfront-fusion-are-affected}

[!DNL Google Drive], [!DNL Gmail]und E-Mail (verbunden mit [!DNL Gmail] -Konto).

### Habe ich eine [!DNL G Suite] Konto? {#do-i-have-a-g-suite-account}

Wenn Ihre E-Mail-Adresse [!DNL @gmail.com] oder [!DNL @googlemail.com] Ihr Konto ist nicht [!DNL G Suite] -Konto. Wenn [!DNL Google] -Konto mit einer benutzerdefinierten Domäne endet, z. B. @my-company.com . Dann handelt es sich um eine [!DNL G Suite] -Konto.

### Was soll ich tun, wenn ich [!DNL @gmail.com] oder [!DNL @googlemail.com] Benutzer? {#what-should-i-do-if-im-gmailcom-or-googlemailcom-user}

Diese neuen Einschränkungen gelten nur bei der Integration von [!DNL Google Drive] oder [!DNL Gmail]. Wenn Sie eine Verbindung zu [!DNL Google Drive] oder [!DNL Gmail]können Sie

* Wechseln zu [!DNL G Suite]

   oder

* Erstellen Sie einen benutzerdefinierten OAuth-Client. Diese Option ist für fortgeschrittene Benutzer gedacht.

   Anweisungen finden Sie unter [Verbinden [!DNL Adobe Workfront Fusion] nach [!DNL Google Services] Verwenden eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

Wenn Sie einen anderen Dienst als [!DNL Google Drive] oder [!DNL Gmail], gelten diese Beschränkungen nicht.

Anweisungen zum Verbinden anderer [!DNL Google Services] nach [!DNL Workfront Fusion], siehe [Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) im Artikel [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Was soll ich tun, wenn ich [!DNL G Suite] Benutzer? {#what-should-i-do-if-im-a-g-suite-user}

Es sind keine Maßnahmen erforderlich.
