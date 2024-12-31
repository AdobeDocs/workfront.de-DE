---
title: Übersicht
description: Übersicht
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: 882b657a-1bde-4efd-93e8-1de80c065b2d
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 1%

---

# Übersicht

**Willkommen bei der Workfront Proof-API**

Die Workfront Proof-API ist ein einfacher HTTP-Service, der mit SSL gesichert wird. Die API zielt darauf ab, Ihnen alle Funktionen bereitzustellen, die in unserer eigenen Anwendung verwendet werden.

## Unterstützte Formate

Die öffentliche Schnittstelle ist SOAP 1.1-kompatibel mit WSDL-Unterstützung. Alle Anfragen werden daher mit XML über HTTPS ausgeführt.

## API-Versionierung

Um die Kompatibilität mit den vorhandenen Client-Integrationen zu wahren, haben wir die API-Versionierung ab unserer Version 12.1 eingeführt. Siehe  [API-](https://api.proofhq.com/new-updates.html)) für weitere Informationen. Wenn eine Methode oder ein Parameter keine Versionsinformationen enthält, bedeutet dies, dass Sie dies als Teil unserer Standard-API finden, siehe den Abschnitt „Erste Schritte mit der API“ unten.

## Erste Schritte mit der API

Der API-Einstiegspunkt:

`https://soap.proofhq.com/soap` (bitte beachten Sie die Verwendung von HTTPS)

Die WSDL finden Sie hier:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Diese WSDL enthält alle Änderungen bis zur Version 12.1, nach der wir die API-Versionierung eingeführt haben. Weitere Informationen zu den verschiedenen WSDL-Versionen und bevorstehenden Änderungen finden Sie auf der Seite zu API-Aktualisierungen**

Jede API-Anfrage erfordert einen Sitzungsschlüssel. Dieser Sitzungsschlüssel identifiziert den Workfront Proof-Benutzer, der die Aktion(en) ausführt, und wird durch Aufruf der doLogin()-Methode und Übergabe der E-Mail-Adresse und des Passworts des Benutzers abgerufen. Die Methode doLogin() muss nur einmal vor einer Sequenz von API-Anfragen aufgerufen werden. Der Sitzungsschlüssel bleibt kurze Zeit aktiv und wird bei jedem Methodenaufruf erneuert. *Wir werden sehr bald Unterstützung für Token-basierte Authentifizierung hinzufügen.*

Alle Anfragen verwenden das folgende Umschlag-, Kopfzeilen- und Textkörperformat:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

