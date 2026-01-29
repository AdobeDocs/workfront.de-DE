---
product-area: workfront-navigation
navigation-topic: workfront-navigation
title: Häufig gestellte Fragen zu Adobe Unified Experience
description: Einige Funktionen unterscheiden sich zwischen  [!DNL Workfront]  und Adobe Experience Cloud, und Sie haben möglicherweise einige Fragen, wenn  [!DNL Workfront]  Instanz zum einheitlichen Erlebnis migriert wird.
author: Nolan
feature: Get Started with Workfront
exl-id: b9076fe0-26d7-4f33-80a4-564875ea13ba
source-git-commit: ff8866b2b48ead3b7b2e035a394fa038036fbfc0
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 0%

---

# [!DNL Adobe Unified Experience] Häufig gestellte Fragen

Mit dem [!DNL Adobe Unified Experience] für [!DNL Workfront] können Sie alle Ihre [!DNL Adobe] Anwendungen an einem Ort mit einer einzigen Anmeldung verwalten. Der [!DNL Adobe] Navigationsbereich ist nahtlos mit [!DNL Workfront] integriert. Einige Funktionen sind unterschiedlich, und Sie haben möglicherweise einige Fragen, wenn Ihre [!DNL Workfront]-Instanz zum einheitlichen Erlebnis migriert wird.

Informationen zum Anmelden bei der [!DNL Adobe Unified Experience] finden Sie unter [[!DNL Adobe Unified Experience] für [!DNL Workfront]](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

## Vergleich von [!DNL Adobe Unified Experience]- und [!DNL Workfront only]

Nur Kunden, die die [!DNL Adobe Business Platform] / [!DNL Adobe Admin Console] verwenden, können auf die [!DNL Adobe Unified Experience] zugreifen. Kunden, die noch nicht migriert haben, sehen das [!DNL Workfront only] Erlebnis, ohne die Möglichkeit, zwischen [!DNL Adobe] Anwendungen zu wechseln.

In dieser Tabelle werden einige Funktionen beschrieben, die sich in den beiden Erlebnissen unterscheiden.

| [!DNL Adobe Unified Experience] | [!DNL Workfront] Erlebnis |
| ---- | ----|
| [!UICONTROL [!DNL Workfront] Hauptmenü] befindet sich links ![Hauptmenü](assets/main-menu-icon-left-nav.png) | [!UICONTROL [!DNL Workfront] Hauptmenü] befindet sich auf der rechten ![Hauptmenü](assets/main-menu-icon.png) |
| Für alle [!DNL Adobe Experience Cloud]-Programme ist eine einzige Anmelde-URL verfügbar | Melden Sie sich mit einer benutzerdefinierten [!DNL Workfront]-URL bei [!DNL Workfront] an |
| Mit einem „Organisationswechsel“ können Sie zwischen [!DNL Workfront] Organisationen und Umgebungen wechseln | Der „Organisationswechsel“ ist nicht verfügbar |
| Die Navigation enthält zusätzlich zur [!DNL Adobe] Navigationsleiste einen Navigationsbereich auf oberster Ebene für [!DNL Adobe] Produkte, [!DNL Workfront], Hilfe und Ihr Benutzerprofil | Die Navigation umfasst nur die [!DNL Workfront] Navigationsleiste |
| Die Hilfe ist über das [!UICONTROL Hauptmenü] und den oberen Navigationsbereich zugänglich | Die Hilfe ist über das [!UICONTROL Hauptmenü] und [!DNL Workfront] Navigationsleiste verfügbar |
| Die Proofing Viewer wird in einer neuen Registerkarte geöffnet | Die Proofing-Anzeige wird in Workfront geöffnet |
| Die für den Zugriff auf Workfront verwendete URL ist `experience.adobe.com` | Die für den Zugriff auf Workfront verwendete URL ist `(CompanyName).my.workfront.adobe.com` |
| Das Datumsformat (z. B. MM/TT/JJJJ) basiert auf den Spracheinstellungen von Unified Experience Platform. Wenn der/die Benutzende seine/ihre Spracheinstellungen nicht aktualisiert hat, werden `en-US` verwendet. | Das Datumsformat (z. B. MM/TT/JJJJ) basiert auf den Browser-Voreinstellungen |

{style="table-layout:auto"}

## Häufig gestellte Fragen

### Wie kann ich feststellen, ob ich Adobe Unified Experience oder Adobe Workfront verwende?

Um festzustellen, ob sich Ihr Unternehmen im einheitlichen Adobe-Erlebnis befindet, überprüfen Sie die URL, über die Sie auf Workfront zugreifen.

| URL | Adobe Experience |
|------------|------------|
| (CompanyName).my.workfront.com | Workfront Experience |
| experience.adobe.com | Einheitliches Adobe-Erlebnis |

### Wie kann ich mehr über die [!DNL Adobe Admin Console] erfahren?

Informationen zum [!DNL Admin Console] finden Sie in den folgenden Artikeln:

* [Vorbereiten für das [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/adobe-admin-console/prep-for-admin-console.md)
* [Unterschiede bei der plattformbasierten Administration ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)
* [[!DNL Adobe Admin Console] Übersicht](https://helpx.adobe.com/de/enterprise/using/admin-console.html)

### Was muss ich als Kunde tun, um die Migration zu erleichtern?

Bestehende Kunden werden kontaktiert, um Migrationen zu planen. Das Migrations-Team unterstützt seine Kollegen dabei, den Kunden durch den Prozess zu führen, bei [!DNL Admin Console] Einrichtung zu beraten und Links zur Dokumentation bereitzustellen, die erforderlich ist, um den Umzug so einfach und unkompliziert wie möglich zu gestalten. Weitere Informationen finden Sie in [[!DNL Adobe Business Platform] und [!DNL Admin Console] FAQ](https://experienceleague.adobe.com/en/docs/support-resources/adobe-support-tools-guide/workfront/faq).

### Wie handhabt ihr [!DNL Adobe Admin Console] für Unternehmen, die dies bereits für Federated IDs aktiviert haben, anders als [!DNL Workfront] SSO eingerichtet ist?

[!DNL Adobe Admin Console] bietet die Möglichkeit, [!DNL Workfront] einzubeziehen und SSO durch das Identity Management System (IMS) von Adobe zu ersetzen. Die gesamte Benutzerbereitstellung erfolgt im [!DNL Admin Console] und die Benutzer sehen den [!DNL Adobe] Anmeldebildschirm, um zu [!DNL Experience Cloud] zu gelangen, wo sie [!DNL Workfront] als Option sehen (wenn sie Zugriff darauf erhalten).

### Wie wirkt sich dies auf Kunden aus, die bereits das AEM Admin Panel für [!DNL Adobe Assets] haben, aber das SSO ist anders konfiguriert als [!DNL Workfront?]

Nachdem [!DNL Workfront] als [!DNL Admin Console]-Anwendung hinzugefügt wurde, sollten Sie nichts mehr tun müssen, damit [!DNL Workfront] die vorhandene SSO-Einrichtung nutzen können, die Sie für [!DNL Adobe Assets] haben.

### Wie wirkt sich dies auf diejenigen aus, die mit SSO eingerichtet wurden?

SSO wird in der [!DNL Admin Console] eingerichtet und von der [!DNL Workfront] übernommen.

### Wird SSO mit unserem internen [!DNL Active Directory] weiterhin eine Option im Identity Management System (IMS) von Adobe sein?

IMS ist ein Ersatz für SSO und funktioniert größtenteils gleich. Alle Benutzerberechtigungen werden in [!DNL Adobe Admin Console] erteilt und bereitgestellt, und der Benutzer sieht den [!DNL Adobe] Anmeldebildschirm, auf dem er &quot;[!UICONTROL Persönliches Konto]&quot; oder &quot;[!UICONTROL Firmenkonto]&quot; auswählen kann, um sich anzumelden (wenn Sie [!DNL Active Directory] haben, melden sich die meisten mit einem Unternehmenskonto an).

### Ändert sich die [!DNL Workfront] Anmelde-URL für diejenigen, die SSO nicht verwenden?

Die Anmelde-URL wird sich ändern. Die alte URL wird jedoch zur neuen Anmelde-URL umgeleitet. Daher sollten Sie Ihre Benutzer neu schulen, wohin Sie gehen sollten.

### Werden die von uns eingerichteten Aliase weiterhin funktionieren, oder ändern sich die [!DNL Workfront] Links mit dieser Migration?

[!DNL Workfront] Umleitungen/Aliase sind verfügbar, um zur Homepage zu gelangen.

### Gibt es einen Zeitpunkt, zu dem die Weiterleitungen deaktiviert sind? Oder können wir immer my.company.workfront.com eingeben?

Sie können immer beliebige benutzerdefinierte URLs verwenden. Nachdem Sie auf einen dieser Links geklickt haben, werden Sie zum [!DNL Workfront] weitergeleitet, wo eine andere URL angezeigt wird. Es ist jedoch besser, sich [!DNL experience] experience.adobe.com anzumelden und Links von [!DNL Experience Cloud] aus mit Lesezeichen zu versehen. Weniger Umleitungen entspricht weniger Verzögerungszeit/Ladezeit.

### Werden direkte Links zu Anfragewarteschlangen unterbrochen?

Alle direkten Links sollten zu den neuen URL-Mustern umgeleitet werden. Wenn Sie jedoch verteilte Links an Personen haben, sollten Sie eine Aktualisierung senden, um den direkten Link zu nutzen und Verzögerungen beim Zugriff auf die erwartete Seite zu vermeiden.

### Werden wir global zu [!DNL Experience Cloud] migrieren oder können wir für bestimmte Benutzende (nicht alle unsere Benutzenden verwenden auch andere Adobe-Produkte) eine Auswahl treffen?

Das gesamte [!DNL Workfront] Kundenkonto wird migriert. Dies kann nicht für jeden einzelnen Benutzer geschehen.

### Müssen sich alle [!DNL Workfront] Benutzer über [!DNL Experience Cloud] anmelden? Oder nur Administratoren?

Ja, alle Benutzer melden sich über [!DNL Experience Cloud] an. Die Anmeldung beim Adobe Identity Management System (IMS) ersetzt SSO. Es ist ein sehr ähnliches Erlebnis, nur ein anderer Anmeldebildschirm.

### Müssen Benutzer ihre [!DNL Adobe] Konten mit ihren [!DNL Workfront] Konten verknüpfen, wenn sie bereits über beide verfügen?

Ja, es gibt einen Prozess dafür. Weitere Details werden bereitgestellt, wenn es für Ihr Unternehmen an der Zeit ist, zu IMS zu wechseln.

### Was passiert mit den [!DNL Workfront] Benutzern, die kein [!DNL Adobe] Konto haben?

Benutzer, denen in [!DNL Adobe Admin Console] kein Zugriff auf [!DNL Workfront] gewährt wurde, müssen ein &quot;[!UICONTROL persönliches Konto“ ] ein [!DNL Adobe] ID-Konto erstellen, um sich anmelden zu können. Dadurch wird eine E-Mail an den Administrator gesendet, um die Anfrage zu genehmigen oder abzulehnen, und der Administrator kann damit zusätzlich konfigurieren, welche Art von Zugriff dieser Benutzer hat. Wenn sie sich anmelden, gehen sie zu experience.adobe.com, geben ihre E-Mail-Adresse ein und wählen [!UICONTROL Persönliches Konto]. Dort können sie auf [!DNL Workfront] zugreifen.

### Was ist, wenn wir außer [!DNL Adobe] keine [!DNL Workfront?] Produkte haben?

Es wird weiterhin empfohlen, dass Ihre Organisation zum [!DNL Adobe Unified Experience] migriert. Sie erhalten eine [!DNL Adobe] ID zusammen mit den oben aufgeführten Vorteilen.

### Externe Benutzer sind in unserer [!DNL Workfront]-Instanz enthalten. Wir möchten nicht, dass sie Zugriff auf andere Produkte haben, die in [!DNL Adobe] enthalten sind. Wie würden wir ihren Zugriff innerhalb der Konsole einschränken?

[!DNL Admin Console] gibt Administratoren eine große Kontrolle darüber, auf was Benutzer zugreifen können und was nicht. Wenn ein externer Benutzer Zugriff wünscht, muss er eine [!DNL Adobe] ID erstellen, die eine E-Mail an den Administrator sendet. Der Administrator kann dann den Zugriff auf ein Produkt akzeptieren oder ablehnen und festlegen, auf was er für Produkte im Besitz dieser Organisation zugreifen darf/kann. Anschließend kann der [!DNL Workfront]-Systemadministrator in den Bereich [!UICONTROL Benutzer] von [!DNL Workfront] wechseln, um für den externen Benutzer granularere Berechtigungen festzulegen.

### Gruppenadministratoren werden verwendet, um Personen in [!DNL Workfront] zu erstellen. Können Gruppenadministratoren nach der Umstellung auf [!DNL Experience Cloud] weiterhin Personen erstellen?

Ja, die Benutzererstellung ist weiterhin über [!DNL Workfront] möglich. Diese Benutzer können [!DNL Experience Cloud] automatisch hinzugefügt werden. Sie können Ihre Gruppenadministratoren auch als Produkteigentümer in der [!DNL Admin Console] einrichten, damit sie Benutzern [!DNL Workfront] zuweisen können.

### Bis wann muss auf [!DNL Experience Cloud] umgestellt werden?

Es gibt derzeit keine Frist für den Wechsel zu [!DNL Adobe Experience Cloud]. Wir arbeiten mit Kunden zusammen, damit sie selbst entscheiden können, wann sie für den Umzug bereit sind.

### Muss unser Supportteam etwas für diese Änderung tun?

Wenn das Support-Team für die Erstellung neuer Benutzender verantwortlich ist, muss es sich mit den [!DNL Admin Console] vertraut machen, die zum Erstellen von Benutzenden und zum Zuweisen einer Berechtigung für Workfront verwendet werden. Andernfalls gibt es wahrscheinlich keine wesentliche Änderung für Ihr internes Support-Team.

### Wie wirkt sich dies auf Integrationen aus, die wir über die API-Funktion haben?

Der vorhandene URL-Pfad steht weiterhin für API-Traffic zur Verfügung. Sie sollten nichts tun müssen, um die Endpunkte in Ihren Integrationen zu aktualisieren. Die direkte Anmeldung über Benutzername und Kennwort wird jedoch nicht unterstützt. Sie müssen einen API-Schlüssel verwenden, mit Ausnahme von [!DNL Workfront Fusion]-Connectoren.

### Was ist mit [!DNL Creative Cloud] Benutzern? Wie wirkt sich die Migration auf sie aus? Gibt es Vorteile für sie?

Die Migration nach [!DNL Creative Cloud] hat keine Auswirkungen auf [!DNL Adobe Unified Experience] Benutzer.

### Werden sich für [!DNL Workfront] mobile Benutzer die Anmeldedaten ändern?

[!DNL Workfront] Benutzer auf Mobilgeräten sollten von der Migration zu [!DNL Adobe Unified Experience] nicht betroffen sein.

### JumpSeat funktioniert nicht mit dem [!DNL Adobe Unified Experience]. Wie kann ich dies beheben?

JumpSeat funktioniert mit dem [!DNL Adobe Unified Experience], erfordert jedoch eine Konfigurationsaktualisierung. Ändern Sie im Admin-Bedienfeld von JumpSeat die Anwendungs-URL von `workfront.com` in `.workfront.adobe.com`
