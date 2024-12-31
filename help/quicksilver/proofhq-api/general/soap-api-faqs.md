---
title: Häufig gestellte Fragen zur SOAP-API
description: Häufig gestellte Fragen zur SOAP-API
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
role: Developer
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 79b6370ec3283922a16435e8eb8069f7f9560c55
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Häufig gestellte Fragen zur SOAP-API

## Wie erstelle ich meinen ersten Korrekturabzug?

Dazu sind drei einfache Schritte erforderlich:

**Schritt 1**: Laden Sie die Datei in Workfront Proof hoch, indem Sie sie über eine POST-Anfrage an senden.  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Wir geben Ihnen den Datei-Hash zurück - das ist sehr wichtig! Beachten Sie, dass Sie in diesem Stadium nichts in Ihrem Konto sehen werden, alles was Sie bisher getan haben, ist uns die Datei zu senden, aber nicht gesagt, was wir damit tun sollen.

**Schritt 2**: Wenn Sie noch keine Sitzungs-ID haben, erhalten Sie eine mit den Methoden doLogin() oder getSessionID(). Verwenden Sie die erste Methode, um sich mit der E-Mail-Adresse und dem Kennwort eines Benutzers anzumelden, oder die zweite Methode, wenn Sie die E-Mail-Adresse und das Authentifizierungs-Token des Benutzers haben.

**Schritt 3:** Jetzt ist es an der Zeit, den Testversand zu erstellen. Verwenden Sie die Methode createProof() und senden Sie uns mindestens die erforderlichen Felder (derzeit gibt es nur 5 davon). Stellen Sie sicher, dass Sie den Hash-Parameter auf den Datei-Hash setzen, der während „Schritt 1“ zurückgegeben wurde, da dies uns ermöglicht, zu bestimmen, welche Datei beim Erstellen Ihres Korrekturabzugs verwendet werden soll.

Wenn Sie sich jetzt bei Ihrem Konto anmelden, sehen Sie den Testversand.

## Wie erstelle ich meinen ersten Web-Schnappschuss-Korrekturabzug?

Dazu sind zwei einfache Schritte erforderlich:

**Schritt 1**: Wenn Sie noch keine Sitzungs-ID haben, erhalten Sie eine mit der doLogin()- oder getSessionID()-Methode. Verwenden Sie die erste Methode, um sich mit der E-Mail-Adresse und dem Kennwort eines Benutzers anzumelden, oder die zweite Methode, wenn Sie die E-Mail-Adresse und das Authentifizierungs-Token des Benutzers haben.

**Schritt 2:**Jetzt ist es an der Zeit, den Korrekturabzug zu erstellen. Verwenden Sie die Methode createProof() und senden Sie uns mindestens die erforderlichen Felder (derzeit gibt es nur 5 davon). Stellen Sie sicher, dass Sie den Hash-Parameter auf „web“ und den SourceName-Parameter als URL der Web-Seite festlegen, die Sie erfassen möchten.

Wenn Sie sich jetzt bei Ihrem Konto anmelden, sehen Sie den Testversand.

## Was ist der Unterschied zwischen einem Korrekturabzug und einer Version?

In Workfront Proof werden Versionen als einzelner Korrekturabzug angezeigt. Durch Klicken auf eine bestimmte Version in der Web-Benutzeroberfläche werden die Details dieser Version angezeigt. In Wirklichkeit ist jede Version ein separater Korrekturabzug, und die Web-Benutzeroberfläche zeigt diese zusammen an.

Aus Sicht der API ist jede Version ein separater Korrekturabzug, und die Korrekturabzüge werden durch ihre IDs miteinander verknüpft.

**createProof()** erstellt immer **Version 1** des Korrekturabzugs. Nehmen wir für unser Beispiel die ID an, die für diesen Korrekturabzug „100“ zurückgegeben wurde.

Bei Verwendung von **createProofVersion()** immer die ID der vorherigen Version gesendet. Wenn wir Version 2 **Korrekturabzug** „100“ erstellen möchten, **wir „100“ für den Parameter ParentFileID** übergeben. Dadurch wird dem System mitgeteilt, dass dieser Korrekturabzug Version 2 des Sets sein sollte. Die Methode gibt eine eindeutige Korrekturabzugs-ID zurück. In unserem Beispiel lautet diese „101“.

Wenn eine dritte Version, d. h. **Version 3**, erforderlich ist, rufen Sie **createProofVersion()** erneut auf und geben Sie diesmal **101“ für die ParentFileID ein** um sicherzustellen, dass die verknüpfte Liste der Versionen ordnungsgemäß erstellt wird.

## Muss ich vor jedem Aufruf eine neue Sitzungs-ID abrufen?

Es ist wichtig darauf hinzuweisen, dass jede Sitzungs-ID im Wesentlichen ein Benutzer ist, der die Aktionen ausführt. 

Sie müssen nicht vor jedem Aufruf der API eine neue Sitzungs-ID abrufen und diese bleibt 24 Stunden lang gültig. Die Ablaufzeit wird jedes Mal zurückgesetzt, wenn Sie die -API aufrufen.

## Was ist eine Korrekturabzugs-/persönliche URL?

**Team/Öffentlich**: Jede Korrekturabzugsversion verfügt über eine eindeutige Team (Öffentlich)-URL. Wenn aktiviert, wird der Korrekturabzug im schreibgeschützten Modus geöffnet. Sie können die Team-URL mit der Methode [getProofURL()](https://api.proofhq.com/home/proofs/getproofurl.html) abrufen.

**Persönlich**: Eine persönliche URL ist für jede Reviewer- und Korrekturabzugsversion eindeutig. Wenn ein Korrekturabzugssatz drei Versionen enthält und bei allen Versionen ein Prüfer vorhanden ist, verfügt der Prüfer über drei eindeutige persönliche URLs. Eine persönliche URL öffnet die Korrekturabzugsversion mit dem bereits identifizierten Prüfer und sollte daher sicher aufbewahrt und nicht freigegeben werden. Persönliche URLs können durch Aufruf der Methode [getProofReviewers()](https://api.proofhq.com/home/proofs/getproofreviewers.html) und anschließende Iteration über jede URL abgerufen werden  [SOAPRecepientObject](https://api.proofhq.com/home/objects/soaprecipientobject.html) und den Parameter „proof_url“ abrufen.

## >Wie lassen sich beim Öffnen des Mini-Korrekturabzugs benutzerdefinierte Parameter einbeziehen?

Mit dem Miniproof können Sie das Proofing-Tool in Ihre eigene Seite einbetten. Ein Parameter „referer“ kann als Teil des Mini-Korrekturabzugs eingeschlossen werden, um eine Umleitungs-URL bereitzustellen, wenn ein Benutzer im Mini-Korrekturabzug auf die Schaltfläche „Schließen“ klickt. Sie können beliebig viele benutzerdefinierte Parameter als Teil dieser Umleitungs-URL einbeziehen, indem Sie sie mit dem Escape-Zeichen &quot;&amp;&quot; anhängen, z. B. %26.

Beispiel: die miniproof URL
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` muss wie folgt codiert sein 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=`, damit die benutzerdefinierten Parameter weitergeleitet werden.


