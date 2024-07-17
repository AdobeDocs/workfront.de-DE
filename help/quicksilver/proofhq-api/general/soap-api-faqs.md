---
title: Häufig gestellte Fragen zu SOAP API
description: Häufig gestellte Fragen zu SOAP API
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# Häufig gestellte Fragen zu SOAP API

## Wie erstelle ich meinen ersten Dateiversand?

Es werden drei einfache Schritte ausgeführt:

**Schritt 1**: Laden Sie die Datei in Workfront Proof hoch, indem Sie sie über eine Post-Anfrage an senden.  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Wir werden Ihnen den Datei-Hash zurückgeben - das ist sehr wichtig! Beachten Sie, dass Sie in dieser Phase nichts in Ihrem Konto sehen werden, alles was Sie bisher getan haben, ist uns die Datei zu schicken, aber nicht gesagt, was wir damit tun sollen.

**Schritt 2**: Wenn Sie noch keine Sitzungs-ID haben, können Sie eine mit den Methoden doLogin() oder getSessionID() abrufen. Verwenden Sie die erste Methode, um sich mit der E-Mail-Adresse und dem Passwort eines Benutzers anzumelden, oder die zweite Methode, wenn Sie über die E-Mail-Adresse und das Authentifizierungstoken des Benutzers verfügen.

**Schritt 3:** Jetzt ist es an der Zeit, Ihren Testversand zu erstellen. Verwenden Sie die Methode createProof() und senden Sie uns mindestens die erforderlichen Felder (derzeit gibt es nur 5 davon). Stellen Sie sicher, dass Sie den Hash-Parameter auf den Datei-Hash setzen, der während &quot;Schritt 1&quot;zurückgegeben wurde, da wir so feststellen können, welche Datei bei der Erstellung Ihres Testversands verwendet werden soll.

Wenn Sie sich jetzt bei Ihrem Konto anmelden, sehen Sie den Testversand.

## Wie erstelle ich meinen ersten Web-Schnappschuss-Testversand?

Es umfasst zwei einfache Schritte:

**Schritt 1**: Wenn Sie noch keine Sitzungs-ID haben, können Sie eine mit den Methoden doLogin() oder getSessionID() abrufen. Verwenden Sie die erste Methode, um sich mit der E-Mail-Adresse und dem Passwort eines Benutzers anzumelden, oder die zweite Methode, wenn Sie über die E-Mail-Adresse und das Authentifizierungstoken des Benutzers verfügen.

**Schritt 2:**Jetzt ist es an der Zeit, Ihren Testversand zu erstellen. Verwenden Sie die Methode createProof() und senden Sie uns mindestens die erforderlichen Felder (derzeit gibt es nur 5 davon). Stellen Sie sicher, dass der Hash-Parameter auf &quot;web&quot;und der SourceName-Parameter als URL der Webseite festgelegt ist, die Sie erfassen möchten.

Wenn Sie sich jetzt bei Ihrem Konto anmelden, sehen Sie den Testversand.

## Was ist der Unterschied zwischen einem Testversand und einer Version?

In Workfront Proof werden Versionen als ein Testversand angezeigt. Wenn Sie auf eine bestimmte Version in der Web-Benutzeroberfläche klicken, werden die Details dieser Version angezeigt. In Wirklichkeit ist jede Version ein separater Testversand, und die Web-Benutzeroberfläche zeigt diese zusammen an.

Aus Sicht der API ist jede Version ein separater Testversand und die Testsendungen werden anhand ihrer Kennungen verknüpft.

**createProof()** erstellt stets die Version 1 **des Testversands.** Nehmen wir als Beispiel die für diesen Testversand zurückgegebene ID &quot;100&quot;.

Bei Verwendung von **createProofVersion()** wird immer die ID der vorherigen Version gesendet. Wenn wir **Version 2** für den Testversand &quot;100&quot;erstellen möchten, übergeben wir **&quot;100&quot;für den Parameter ParentFileID** . Dadurch wird dem System mitgeteilt, dass dieser Testversand Version 2 des Sets sein sollte. Die -Methode gibt eine eindeutige Testversand-ID zurück. Nehmen wir in unserem Beispiel an, dass dies &quot;101&quot;ist.

Wenn eine dritte Version erforderlich ist, d. h. **Version 3**, rufen Sie **createProofVersion()** erneut auf und geben Sie dieses Mal **den Wert &quot;101&quot;für die ParentFileID** an, um sicherzustellen, dass die verknüpfte Liste der Versionen ordnungsgemäß erstellt wird.

## Muss ich vor jedem Aufruf eine neue Sitzungs-ID erhalten?

Es ist wichtig darauf hinzuweisen, dass jede Sitzungs-ID im Wesentlichen ein Benutzer ist, der die Aktionen durchführt. 

Sie müssen vor jedem Aufruf der API keine neue Sitzungs-ID abrufen, die 24 Stunden lang gültig bleibt. Die Ablaufzeit wird jedes Mal zurückgesetzt, wenn Sie die API aufrufen.

## Was ist ein Testversand/eine persönliche URL?

**Team/Public**: Jede Testversion verfügt über eine eindeutige Team-URL (Public). Wenn diese Option aktiviert ist, wird der Testversand im schreibgeschützten Modus geöffnet. Sie können die Team-URL mit der Methode [getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html) abrufen.

**Persönlich**: Eine persönliche URL ist für jede Reviewer- und Testversion eindeutig. Wenn ein Testversand 3 Versionen enthält und sich ein Validierer auf allen Versionen befindet, verfügt der Validierer über 3 eindeutige persönliche URLs. Eine persönliche URL öffnet die Testversand-Version, wobei der Validierer bereits identifiziert wurde und daher sicher und nicht freigegeben werden sollte. Persönliche URLs können abgerufen werden, indem die Methode [getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html) aufgerufen und dann für jede  [SOAPRecepientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html) und Abrufen des Parameters &quot;proof_url&quot;.

## >Wie werden benutzerdefinierte Parameter beim Öffnen des minimierten Fensters einbezogen?

Mit dem miniproof-Werkzeug können Sie das Testwerkzeug in Ihre eigene Seite einbetten. Ein &quot;referer&quot;-Parameter kann als Teil des miniproof-Parameters enthalten sein, um eine Umleitungs-URL bereitzustellen, wenn ein Benutzer auf die Schließen-Schaltfläche im miniproof klickt. Sie können eine beliebige Anzahl benutzerdefinierter Parameter als Teil dieser Umleitungs-URL angeben, indem Sie sie mit dem Escape-Zeichen &quot;&amp;&quot;anhängen, z. B. %26.

Beispielsweise die URL für die minimierte Suche
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` muss als 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=`, damit die benutzerdefinierten Parameter weitergegeben werden.

## Wie erstelle ich einen Java Web Service Client?

[In diesem Video](https://screencast.com/t/xsSNrqs5b) wird gezeigt, wie Sie einen Java-Webdienstclient mithilfe von Eclipse und der Workfront Proof-WSDL-Definition erstellen können.

