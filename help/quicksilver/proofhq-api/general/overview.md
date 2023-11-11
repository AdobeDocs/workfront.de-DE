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
source-wordcount: '266'
ht-degree: 1%

---

# Übersicht

**Willkommen bei der Workfront Testversand-API**

Die Workfront Proof-API ist ein einfacher HTTP-Dienst, der mit SSL gesichert wird. Die API soll Ihnen alle Funktionen zur Verfügung stellen, die in unserer eigenen Anwendung verwendet werden.

## Unterstützte Formate

Die öffentliche Benutzeroberfläche ist SOAP 1.1-kompatibel mit WSDL-Unterstützung. Alle Anfragen werden daher mithilfe von XML über HTTPS ausgeführt.

## API-Versionierung

Um die Kompatibilität mit der vorhandenen Client-Integration zu gewährleisten, haben wir die API-Versionierung ab unserer Version 12.1 eingeführt. Lesen Sie hierzu die  [API-Aktualisierungen](https://api.proofhq.com/new-updates.html) für weitere Informationen. Wenn eine Methode oder ein Parameter keine Versionsinformationen enthält, bedeutet dies, dass Sie dies als Teil unserer Standard-API finden, finden Sie im Abschnitt &quot;Erste Schritte mit der API&quot;unten.

## Erste Schritte mit der API

Der API-Einstiegspunkt:

`https://soap.proofhq.com/soap` (bitte beachten Sie die Verwendung von HTTPS)

Die WSDL finden Sie hier:

`https://soap.proofhq.com/soap?wsdl`

>[!NOTE]
>
>**Diese WSDL enthält alle Änderungen bis zur Version 12.1, nach der wir die API-Versionierung eingeführt haben. Weitere Informationen zu den verschiedenen WSDL-Versionen und bevorstehenden Änderungen finden Sie auf der Seite API-Aktualisierungen .**

Für jede API-Anfrage ist ein Sitzungsschlüssel erforderlich. Dieser Sitzungsschlüssel identifiziert den Workfront-Testbenutzer, der die Aktion(en) ausführt. Er wird abgerufen, indem die Methode doLogin() aufgerufen und die E-Mail-Adresse und das Kennwort des Benutzers übergeben werden. Die Methode doLogin() muss nur einmal vor einer Sequenz von API-Anfragen aufgerufen werden. Der Sitzungsschlüssel bleibt für einen kurzen Zeitraum aktiv und wird bei jedem Methodenaufruf erneuert. *Wir werden in Kürze Unterstützung für Token-basierte Authentifizierung hinzufügen.*

Alle Anforderungen verwenden das folgende Umschlag-, Header- und Textformat:

```
<soapenv:Envelope xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/" xmlns:urn="urn:proofhqapi">`
   <soapenv:Header/>
   <soapenv:Body>
       ... API function and data inserted here ...
    </soapenv:Body>
    </soapenv:Envelope>
```

