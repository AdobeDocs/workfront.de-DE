---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Häufig gestellte Fragen zu Adobe Unified Experience
description: Einige Funktionen unterscheiden sich zwischen [!DNL Workfront] und Adobe Experience Cloud, und Sie haben möglicherweise einige Fragen als Ihre [!DNL Workfront] -Instanz zum einheitlichen Erlebnis migriert wird.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: 019a1b61cd97d5d61f9a4fbf3f98eccab50809a8
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] FAQs

Die [!DNL Adobe Unified Experience] für [!DNL Workfront] ermöglicht es Ihnen, alle [!DNL Adobe] Anwendungen an einem Ort mit einer einzigen Anmeldung. Die [!DNL Adobe] der Navigationsbereich nahtlos in [!DNL Workfront]. Einige Funktionen unterscheiden sich, und Sie haben möglicherweise einige Fragen zu Ihrer [!DNL Workfront] -Instanz zum einheitlichen Erlebnis migriert wird.

Informationen zum Anmelden bei der [!DNL Adobe Unified Experience], siehe [[!DNL Adobe Unified Experience] für [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Vergleich [!DNL Adobe Unified Experience] und [!DNL Workfront only] Erlebnis

Nur Kunden, die [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] kann auf die [!DNL Adobe Unified Experience]. Kunden, die noch nicht migriert wurden, sehen die [!DNL Workfront only] Erlebnis ohne die Möglichkeit, zwischen [!DNL Adobe] Anwendungen.

In dieser Tabelle werden einige Funktionen beschrieben, die sich zwischen den beiden Erlebnissen unterscheiden.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] Nur Erlebnis |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Hauptmenü] links ![Hauptmenü](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Hauptmenü] rechts ![Hauptmenü](assets/main-menu-icon.png) |
| Eine einzelne Anmelde-URL ist für alle [!DNL Adobe Experience Cloud] Anwendungen | Anmelden bei [!DNL Workfront] mit benutzerdefiniertem [!DNL Workfront] URL |
| Mit einem &quot;Organisationswechsel&quot;können Sie zwischen [!DNL Workfront] Organisationen und Umgebungen | Der &quot;Organisationswechsel&quot;ist nicht verfügbar. |
| Die Navigation enthält einen Navigationsbereich auf oberster Ebene für [!DNL Adobe] Produkte, [!DNL Adobe] Benachrichtigungen, Hilfe und Ihr Benutzerprofil, zusätzlich zum [!DNL Workfront] Navigationsleiste | Die Navigation umfasst die [!DNL Workfront] nur Navigationsleiste |
| Auf die Hilfe kann über das [!UICONTROL Hauptmenü] und oberer Navigationsbereich | Auf die Hilfe kann über das [!UICONTROL Hauptmenü] und [!DNL Workfront] Navigationsleiste |

{style="table-layout:auto"}

## Häufig gestellte Fragen

### Wie kann ich feststellen, ob ich Adobe Unified Experience oder Adobe Workfront verwende?

Um festzustellen, ob Ihr Unternehmen das Adobe Unified Experience verwendet, überprüfen Sie die URL, die Sie für den Zugriff auf Workfront verwenden.

| URL | Adobe-Erlebnis |
|------------|------------|
| (CompanyName).my.workfront.com | Workfront-Erfahrung |
| experience.adobe.com | Adobe Unified Experience |

### Wie kann ich mehr über die [!DNL Adobe Admin Console]?

Informationen zum [!DNL Admin Console], lesen Sie diese Artikel:

* [Vorbereiten auf die [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Plattformbasierte Verwaltungsunterschiede ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] Übersicht](https://helpx.adobe.com/de/enterprise/using/admin-console.html)

### Was muss ich als Kunde tun, um die Migration zu erleichtern?

Bestehende Kunden werden kontaktiert, um Migrationen zu planen. Die Mitarbeiter des Migrationsteams führen die Kunden durch den Prozess und beraten Sie bei [!DNL Admin Console] und Links zur Dokumentation bereitstellen, die erforderlich sind, um den Umstieg so einfach und einfach wie möglich zu gestalten.

* [[!DNL Adobe Workfront] Support-Übersicht](https://experienceleague.adobe.com/docs/customer-one/using/workfront/overview.html)
* [[!DNL Workfront Admin Console] Informationen](https://experienceleague.adobe.com/docs/customer-one/using/workfront/landing.html)
* [[!DNL Adobe Business Platform] und [!DNL Admin Console] FAQs](https://experienceleague.adobe.com/docs/customer-one/using/workfront/faq.html)

### Handhabung [!DNL Adobe Admin Console] für Unternehmen, bei denen dies bereits für Federated IDs anders aktiviert ist als [!DNL Workfront] SSO ist eingerichtet?

[!DNL Adobe Admin Console] verfügt über die Möglichkeit, [!DNL Workfront], wobei SSO durch IMS ersetzt wird. Die gesamte Benutzerbereitstellung erfolgt im [!DNL Admin Console], und die Benutzer sehen die [!DNL Adobe] Anmeldebildschirm zum Aufrufen [!DNL Experience Cloud] wo sie sehen werden [!DNL Workfront] als Option (wenn ihnen Zugriff gewährt wird).

### Wie wirkt sich dies auf Kunden aus, die bereits über das AEM Admin-Bedienfeld verfügen für [!DNL Adobe Assets] - aber die SSO ist anders konfiguriert als [!DNL Workfront?]

Einmal [!DNL Workfront] wird als [!DNL Admin Console] -Anwendung verwenden, sollten Sie nichts anderes tun müssen für [!DNL Workfront] zur Nutzung der vorhandenen SSO-Einrichtung, für die Sie [!DNL Adobe Assets].

### Wie wirkt sich dies auf diejenigen aus, die mit SSO eingerichtet sind?

Die einmalige Anmeldung wird im [!DNL Admin Console] und von der [!DNL Workfront] Anwendung.

### Ist SSO mit unserem internen [!DNL Active Directory] wird IMS noch eine Option sein?

IMS ist ein Ersatz für SSO und funktioniert größtenteils gleich. Alle Benutzerberechtigungen werden in [!DNL Adobe Admin Console]und der Benutzer die [!DNL Adobe] Anmeldebildschirm, auf dem sie &quot;[!UICONTROL Persönliches Konto]&quot; oder &quot;[!UICONTROL Firmenkonto]&quot;, um sich anzumelden (falls Sie [!DNL Active Directory], melden sich die meisten mit einem Unternehmenskonto an).

### Für diejenigen, die keine einmalige Anmeldung verwenden, führt die Funktion [!DNL Workfront] Änderung der Anmelde-URL?

Die Anmelde-URL ändert sich. Die alte URL leitet jedoch zur neuen Anmelde-URL um, sodass Sie Ihre Benutzer neu trainieren sollten, wohin sie gehen sollen.

### Werden Alias, die wir eingerichtet haben, weiterhin funktionieren oder sind die [!DNL Workfront] Links, die sich mit dieser Migration ändern?

[!DNL Workfront] Umleitungen/Aliase sind verfügbar, um zur Startseite zu gelangen.

### Gibt es eine Zeit, in der die Umleitungen deaktiviert sind? Oder können wir immer in my.company.workfront.com eingeben?

Sie können immer beliebige benutzerdefinierte URLs verwenden. Nachdem Sie auf einen dieser Links geklickt haben, werden Sie zu [!DNL Workfront] und eine andere URL anzeigen. Es ist jedoch besser [!DNL experience] , um sich bei experience.adobe.com anzumelden und Links mit Lesezeichen von [!DNL Experience Cloud]. Weniger Umleitung entspricht weniger Verzögerung/Ladezeit.

### Werden direkte Links zu Anforderungswarteschlangen beschädigt?

Alle direkten Links sollten zu den neuen URL-Mustern umgeleitet werden. Wenn Sie jedoch verteilte Links zu Personen haben, sollten Sie eine Aktualisierung senden, um den direkten Link zu nutzen und Verzögerungen beim Aufrufen der erwarteten Seite zu vermeiden.

### Werden wir zu [!DNL Experience Cloud] global oder können wir für bestimmte Nutzer auswählen (nicht alle Nutzer verwenden auch andere Adobe-Produkte)?

Das gesamte [!DNL Workfront] Kundenkonto wird migriert. Dies kann nicht von Benutzer zu Benutzer erfolgen.

### Alle [!DNL Workfront] -Benutzer müssen sich über anmelden [!DNL Experience Cloud]? Oder nur Administratoren?

Ja, alle Benutzer melden sich über an. [!DNL Experience Cloud]. Die IMS-Anmeldung ersetzt SSO. Es ist ein sehr ähnliches Erlebnis, nur ein anderer Anmeldebildschirm.

### Müssen Benutzer ihre [!DNL Adobe] der [!DNL Workfront] Konten, wenn sie bereits über beide verfügen?

Ja, dafür gibt es einen Prozess, und weitere Details werden bereitgestellt, wenn es Zeit für Ihr Unternehmen ist, zu IMS zu wechseln.

### Was geschieht mit dem [!DNL Workfront] Benutzer ohne [!DNL Adobe] Konto?

Benutzer, denen kein Zugriff gewährt wurde in [!DNL Adobe Admin Console] in [!DNL Workfront] muss ein &quot;&quot;[!UICONTROL persönliches Konto]&quot; oder [!DNL Adobe] ID-Konto für die Anmeldung. Dadurch wird eine E-Mail an den Administrator gesendet, um seine Anfrage zu genehmigen oder abzulehnen. Außerdem kann der Administrator konfigurieren, welche Zugriffsart dieser Benutzer hat. Wenn sie sich anmelden, gehen sie zu experience.adobe.com, geben ihre E-Mail-Adresse ein und wählen [!UICONTROL Persönliches Konto]. Dort können sie auf [!DNL Workfront].

### Was passiert, wenn wir keine [!DNL Adobe] andere Erzeugnisse als [!DNL Workfront?]

Es wird weiterhin empfohlen, dass Ihre Organisation zur [!DNL Adobe Unified Experience]. Sie erhalten eine [!DNL Adobe] ID sowie die oben aufgeführten Vorteile.

### Externe Benutzer sind in unserer [!DNL Workfront] -Instanz. Wir möchten nicht, dass sie Zugriff auf andere Produkte haben, die in [!DNL Adobe]. Wie würden wir ihren Zugriff innerhalb der Konsole einschränken?

[!DNL Admin Console] gibt Administratoren viel Kontrolle darüber, was Benutzer aufrufen können und was nicht. Wenn ein externer Benutzer Zugriff benötigt, muss er eine [!DNL Adobe] Kennung, die eine E-Mail an den Administrator sendet. Der Administrator kann dann den Zugriff auf ein Produkt akzeptieren oder ablehnen und definieren, was er für Produkte dieser Organisation verwenden kann bzw. nicht. Anschließend wird die [!DNL Workfront] Der Systemadministrator kann die [!UICONTROL Benutzer] Gebiet von [!DNL Workfront] um detaillierte Berechtigungen für den externen Benutzer zu erteilen.

### Gruppenadministratoren werden verwendet, um Personen in [!DNL Workfront]. Mit der Umstellung auf [!DNL Experience Cloud]werden Gruppenadministratoren weiterhin in der Lage sein, Personen zu erstellen?

Ja, die Benutzererstellung ist weiterhin möglich durch [!DNL Workfront]. Diese Benutzer können zu [!DNL Experience Cloud] automatisch. Sie können Ihre Gruppenadministratoren auch als Produkteigentümer im [!DNL Admin Console] , damit sie [!DNL Workfront] für Benutzer.

### Wie lange dauert die Umstellung auf [!DNL Experience Cloud]?

Es gibt derzeit keine Frist für die Umstellung auf [!DNL Adobe Experience Cloud]. Wir arbeiten mit den Kunden zusammen, um sie entscheiden zu lassen, wann sie bereit sind, den Umzug vorzunehmen.

### Wird unser Support-Team etwas für diese Änderung tun müssen?

Wenn das Supportteam für die Erstellung neuer Benutzer zuständig ist, müssen diese mit dem [!DNL Admin Console] Benutzeroberflächen zum Erstellen von Benutzern und zum Zuweisen einer Berechtigung zu Workfront. Andernfalls wird sich Ihr internes Supportteam wahrscheinlich nicht wesentlich ändern.

### Wie wirkt sich dies auf Integrationen aus, die wir über die API-Funktion haben?

Der vorhandene URL-Pfad ist weiterhin für den API-Traffic verfügbar. Sie sollten nichts tun müssen, um die Endpunkte in Ihren Integrationen zu aktualisieren. Die direkte Anmeldung über den Benutzernamen und das Kennwort wird jedoch nicht unterstützt - Sie müssen einen API-Schlüssel verwenden, mit Ausnahme von [!DNL Workfront Fusion] Connectoren.

### Was ist [!DNL Creative Cloud] Benutzer? Wie wirkt sich die Migration auf sie aus? Gibt es irgendwelche Vorteile für sie?

Es gibt keine Auswirkungen auf [!DNL Creative Cloud] Benutzer mit der Migration zu [!DNL Adobe Unified Experience].

### Ändert sich die Anmeldedaten für [!DNL Workfront] Mobilanwender?

[!DNL Workfront] mobile Benutzer sollten von der Migration zu [!DNL Adobe Unified Experience].
