---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Häufig gestellte Fragen zu Adobe Unified Experience
description: Einige Funktionen unterscheiden sich zwischen [!DNL Workfront] und Adobe Experience Cloud. Möglicherweise haben Sie einige Fragen, da Ihre [!DNL Workfront] Instanz zum einheitlichen Erlebnis migriert wird.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 019a1b61cd97d5d61f9a4fbf3f98eccab50809a8
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] FAQ

Mit dem [!DNL Adobe Unified Experience] für [!DNL Workfront] können Sie alle Ihre [!DNL Adobe] Anwendungen an einem Ort mit einer einzigen Anmeldung verwalten. Der Navigationsbereich [!DNL Adobe] ist nahtlos in [!DNL Workfront] integriert. Einige Funktionen unterscheiden sich. Möglicherweise haben Sie einige Fragen, da Ihre [!DNL Workfront] -Instanz zum einheitlichen Erlebnis migriert wird.

Informationen zum Anmelden bei [!DNL Adobe Unified Experience] finden Sie unter [[!DNL Adobe Unified Experience] für  [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Vergleich des Erlebnisses [!DNL Adobe Unified Experience] und [!DNL Workfront only]

Nur Kunden, die die [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] verwenden, können auf die [!DNL Adobe Unified Experience] zugreifen. Kunden, die noch nicht migriert wurden, sehen das Erlebnis [!DNL Workfront only], ohne dass sie zwischen [!DNL Adobe] -Anwendungen wechseln können.

In dieser Tabelle werden einige Funktionen beschrieben, die sich zwischen den beiden Erlebnissen unterscheiden.

| [!DNL Adobe Unified Experience] | Erlebnis nur [!DNL Workfront] |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Hauptmenü] befindet sich auf der linken Seite ![Hauptmenü](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Hauptmenü] befindet sich auf der rechten Seite ![Hauptmenü](assets/main-menu-icon.png) |
| Eine einzelne Anmelde-URL ist für alle [!DNL Adobe Experience Cloud] -Anwendungen verfügbar | Bei [!DNL Workfront] mit einer benutzerdefinierten [!DNL Workfront] URL anmelden |
| Mit einem &quot;Organisationswechsel&quot;können Sie zwischen [!DNL Workfront] Organisationen und Umgebungen wechseln | Der &quot;Organisationswechsel&quot;ist nicht verfügbar. |
| Die Navigation enthält einen Navigationsbereich auf oberster Ebene für [!DNL Adobe] Produkte, [!DNL Adobe] Benachrichtigungen, Hilfe und Ihr Benutzerprofil sowie die Navigationsleiste von [!DNL Workfront]. | Die Navigation enthält nur die Navigationsleiste [!DNL Workfront] . |
| Auf die Hilfe kann über das Hauptmenü [!UICONTROL  und den oberen Navigationsbereich zugegriffen werden.] | Auf die Hilfe kann über das [!UICONTROL Hauptmenü] und die Navigationsleiste [!DNL Workfront] zugegriffen werden. |

{style="table-layout:auto"}

## Häufig gestellte Fragen

### Wie kann ich feststellen, ob ich Adobe Unified Experience oder Adobe Workfront verwende?

Um festzustellen, ob Ihr Unternehmen das Adobe Unified Experience verwendet, überprüfen Sie die URL, die Sie für den Zugriff auf Workfront verwenden.

| URL | Adobe-Erlebnis |
|------------|------------|
| (CompanyName).my.workfront.com | Workfront-Erfahrung |
| experience.adobe.com | Adobe Unified Experience |

### Wie kann ich mehr über die [!DNL Adobe Admin Console] erfahren?

Weitere Informationen zum [!DNL Admin Console] finden Sie in diesen Artikeln:

* [Vorbereiten auf den  [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Plattformbasierte Verwaltungsunterschiede ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] overview](https://helpx.adobe.com/de/enterprise/using/admin-console.html)

### Was muss ich als Kunde tun, um die Migration zu erleichtern?

Bestehende Kunden werden kontaktiert, um Migrationen zu planen. Die Mitarbeiter des Migrationsteams unterstützen Kunden durch den Prozess, beraten bei der Einrichtung von [!DNL Admin Console] und stellen Links zur Dokumentation bereit, die erforderlich sind, um den Umstieg so einfach und unkompliziert wie möglich zu gestalten.

* [[!DNL Adobe Workfront] Support - Übersicht](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] information](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] und [!DNL Admin Console] FAQ](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### Wie verarbeiten Sie [!DNL Adobe Admin Console] für Unternehmen, für die diese Funktion bereits für Federated IDs aktiviert ist, anders als die einmalige Anmeldung von [!DNL Workfront]?

[!DNL Adobe Admin Console] hat die Option, [!DNL Workfront] einzuschließen und SSO durch IMS zu ersetzen. Die gesamte Benutzerbereitstellung erfolgt in [!DNL Admin Console] und Benutzer sehen den Anmeldebildschirm [!DNL Adobe], um zu [!DNL Experience Cloud] zu gelangen, wo sie [!DNL Workfront] als Option sehen (sofern ihnen Zugriff gewährt wird).

### Wie wirkt sich dies auf Kunden aus, die bereits über das AEM Admin-Bedienfeld für [!DNL Adobe Assets] verfügen - die SSO jedoch anders konfiguriert ist als [!DNL Workfront?]?

Sobald [!DNL Workfront] als [!DNL Admin Console] -Anwendung hinzugefügt wurde, sollten Sie nichts anderes tun müssen, damit [!DNL Workfront] die vorhandene SSO-Einrichtung für [!DNL Adobe Assets] nutzt.

### Wie wirkt sich dies auf diejenigen aus, die mit SSO eingerichtet sind?

Die einmalige Anmeldung wird in der [!DNL Admin Console] eingerichtet und von der [!DNL Workfront] -Anwendung übernommen.

### Wird SSO mit unserem internen [!DNL Active Directory] noch eine Option mit IMS sein?

IMS ist ein Ersatz für SSO und funktioniert größtenteils gleich. Alle Benutzerberechtigungen werden in [!DNL Adobe Admin Console] gewährt und bereitgestellt. Der Benutzer sieht den Anmeldebildschirm [!DNL Adobe], auf dem er sich mit &quot;[!UICONTROL Persönliches Konto]&quot;oder &quot;[!UICONTROL Unternehmenskonto]&quot;anmelden kann (wenn Sie über [!DNL Active Directory] verfügen, melden sich die meisten mit einem Unternehmenskonto an).

### Ändert sich für diejenigen, die keine einmalige Anmeldung verwenden, die [!DNL Workfront] Anmelde-URL?

Die Anmelde-URL ändert sich. Die alte URL leitet jedoch zur neuen Anmelde-URL um, sodass Sie Ihre Benutzer neu trainieren sollten, wohin sie gehen sollen.

### Funktionieren Aliase, die wir eingerichtet haben, weiterhin oder ändern sich die [!DNL Workfront]-Links mit dieser Migration?

[!DNL Workfront] Umleitungen/Aliase sind verfügbar, um zur Homepage zu gelangen.

### Gibt es eine Zeit, in der die Umleitungen deaktiviert sind? Oder können wir immer in my.company.workfront.com eingeben?

Sie können immer beliebige benutzerdefinierte URLs verwenden. Nachdem Sie auf einen dieser Links geklickt haben, werden Sie zu [!DNL Workfront] weitergeleitet und eine andere URL angezeigt. Es ist jedoch besser [!DNL experience], sich bei experience.adobe.com anzumelden und Links mit Lesezeichen aus [!DNL Experience Cloud] heraus zu markieren. Weniger Umleitung entspricht weniger Verzögerung/Ladezeit.

### Werden direkte Links zu Anforderungswarteschlangen beschädigt?

Alle direkten Links sollten zu den neuen URL-Mustern umgeleitet werden. Wenn Sie jedoch verteilte Links zu Personen haben, sollten Sie eine Aktualisierung senden, um den direkten Link zu nutzen und Verzögerungen beim Aufrufen der erwarteten Seite zu vermeiden.

### Werden wir global zu [!DNL Experience Cloud] migrieren oder können wir für bestimmte Benutzer wählen (nicht alle unsere Benutzer verwenden auch andere Adobe-Produkte)?

Das gesamte [!DNL Workfront] -Kundenkonto wird migriert. Dies kann nicht von Benutzer zu Benutzer erfolgen.

### Müssen sich alle [!DNL Workfront] -Benutzer über [!DNL Experience Cloud] anmelden? Oder nur Administratoren?

Ja, alle Benutzer melden sich über [!DNL Experience Cloud] an. Die IMS-Anmeldung ersetzt SSO. Es ist ein sehr ähnliches Erlebnis, nur ein anderer Anmeldebildschirm.

### Müssen Benutzer ihre [!DNL Adobe]-Konten mit ihren [!DNL Workfront]-Konten verknüpfen, wenn sie bereits über beide verfügen?

Ja, dafür gibt es einen Prozess, und weitere Details werden bereitgestellt, wenn es Zeit für Ihr Unternehmen ist, zu IMS zu wechseln.

### Was passiert mit den [!DNL Workfront] -Benutzern, die kein [!DNL Adobe] -Konto haben?

Benutzer, denen in [!DNL Adobe Admin Console] kein Zugriff auf [!DNL Workfront] gewährt wurde, müssen ein &quot;[!UICONTROL persönliches Konto]&quot; oder ein [!DNL Adobe] ID-Konto erstellen, um sich anmelden zu können. Dadurch wird eine E-Mail an den Administrator gesendet, um seine Anfrage zu genehmigen oder abzulehnen. Außerdem kann der Administrator konfigurieren, welche Zugriffsart dieser Benutzer hat. Wenn sie sich anmelden, gehen sie zu experience.adobe.com, geben ihre E-Mail-Adresse ein und wählen [!UICONTROL Persönliches Konto]. Von dort aus können sie auf [!DNL Workfront] zugreifen.

### Was passiert, wenn wir keine anderen [!DNL Adobe]-Produkte als [!DNL Workfront?] haben?

Es wird weiterhin empfohlen, dass Ihr Unternehmen zum [!DNL Adobe Unified Experience] migriert. Sie erhalten eine [!DNL Adobe] ID mit den oben aufgeführten Vorteilen.

### Externe Benutzer sind in unserer [!DNL Workfront] -Instanz enthalten. Wir möchten nicht, dass sie Zugriff auf andere Produkte haben, die in [!DNL Adobe] enthalten sind. Wie würden wir ihren Zugriff innerhalb der Konsole einschränken?

[!DNL Admin Console] gibt Administratoren viel Kontrolle darüber, welche Benutzer darauf zugreifen können und welche nicht. Wenn ein externer Benutzer Zugriff wünschen, muss er eine [!DNL Adobe] -ID erstellen, die eine E-Mail an den Administrator sendet. Der Administrator kann dann den Zugriff auf ein Produkt akzeptieren oder ablehnen und definieren, was er für Produkte dieser Organisation verwenden kann bzw. nicht. Anschließend kann der [!DNL Workfront] Systemadministrator in den Bereich [!UICONTROL Benutzer] von [!DNL Workfront] wechseln, um detaillierte Berechtigungen für den externen Benutzer zu erteilen.

### Gruppenadministratoren werden verwendet, um Personen in [!DNL Workfront] zu erstellen. Können Gruppenadministratoren nach dem Wechsel zu [!DNL Experience Cloud] noch Personen erstellen?

Ja, die Benutzererstellung ist weiterhin über [!DNL Workfront] möglich. Diese Benutzer können automatisch zu [!DNL Experience Cloud] hinzugefügt werden. Sie können Ihre Gruppenadministratoren auch als Produkteigentümer in der [!DNL Admin Console] einrichten, damit sie Benutzern [!DNL Workfront] zuweisen können.

### Wie lange dauert der Wechsel auf [!DNL Experience Cloud]?

Es gibt derzeit keinen Termin für den Wechsel zu [!DNL Adobe Experience Cloud]. Wir arbeiten mit den Kunden zusammen, um sie entscheiden zu lassen, wann sie bereit sind, den Umzug vorzunehmen.

### Wird unser Support-Team etwas für diese Änderung tun müssen?

Wenn das Supportteam für die Erstellung neuer Benutzer zuständig ist, müssen diese mit den [!DNL Admin Console] -Schnittstellen vertraut sein, die zum Erstellen von Benutzern und zum Zuweisen einer Berechtigung zu Workfront verwendet werden. Andernfalls wird sich Ihr internes Supportteam wahrscheinlich nicht wesentlich ändern.

### Wie wirkt sich dies auf Integrationen aus, die wir über die API-Funktion haben?

Der vorhandene URL-Pfad ist weiterhin für den API-Traffic verfügbar. Sie sollten nichts tun müssen, um die Endpunkte in Ihren Integrationen zu aktualisieren. Die direkte Anmeldung über Benutzername und Kennwort wird jedoch nicht unterstützt - Sie müssen einen API-Schlüssel verwenden, mit Ausnahme von [!DNL Workfront Fusion] -Connectoren.

### Was ist mit [!DNL Creative Cloud] Benutzern? Wie wirkt sich die Migration auf sie aus? Gibt es irgendwelche Vorteile für sie?

Die Migration zu [!DNL Adobe Unified Experience] wirkt sich nicht auf [!DNL Creative Cloud] Benutzer aus.

### Wird sich die Anmeldung für [!DNL Workfront] Mobilbenutzer ändern?

[!DNL Workfront] Benutzer mit Mobilgeräten sollten von der Migration auf [!DNL Adobe Unified Experience] nicht betroffen sein.
