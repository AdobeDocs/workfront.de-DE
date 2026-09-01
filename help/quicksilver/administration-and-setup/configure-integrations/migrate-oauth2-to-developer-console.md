---
title: Migrieren von Workfront OAuth2 zu Adobe Developer Console
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
description: Der alte benutzerdefinierte OAuth2-Programm-Service von Workfront wird eingestellt. Erfahren Sie, was sich ändert, wer betroffen ist und wie Sie Ihre benutzerdefinierten Integrationen zu Adobe Developer Console migrieren.
author: Becky
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
source-git-commit: db7e6a6fa0c5fc5332213c388d9b4db3a5c59f53
workflow-type: tm+mt
source-wordcount: '1473'
ht-degree: 1%

---

# Migrieren von Workfront OAuth2 zu Adobe Developer Console

Der alte Service für benutzerdefinierte OAuth2-Anwendungen von Workfront (die Integrationen, die Sie unter **Setup** > **System** > **OAuth2** eingerichtet haben) wird eingestellt. Künftig müssen alle benutzerdefinierten Integrationen, die sich bei Workfront authentifizieren, stattdessen den Authentifizierungsfluss von Adobe Developer Console (developer.adobe.com) verwenden.

Diese Änderung wirkt sich auf alle benutzerdefinierten Integrations-, Skript- oder Drittanbieter-Tools aus, die sich derzeit mithilfe einer von Workfront ausgestellten OAuth2-Client-ID und eines -Geheimnisses authentifizieren. Dies hat keinen Einfluss darauf, wie Sie sich bei Workfront anmelden, und es hat keine Auswirkungen auf standardmäßige, von Adobe verwaltete Integrationen wie die gebündelten Microsoft Teams- oder Slack-Integrationen, die Adobe separat migriert.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Zugriffsebenen-Konfigurationen</td> 
   <td><p>Systemadmin</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Developer Console-Rechte</td> 
   <td><p>Für den Zugriff auf Adobe Developer Console for Workfront sind vollständige Administratorrechte für die IMS-Organisation erforderlich. Dies ist breiter angelegt als die Rolle eines Workfront-Produktadministrators, da es die gesamte Adobe-Organisation und alle darin enthaltenen Produkte verwaltet.</p></td> 
  </tr> 
 </tbody> 
</table>

+++

## Wichtige Daten

| Datum | Meilenstein | Was es für Sie bedeutet |
|---|---|---|
| &#x200B;1. November 2026 | Erstellung einer neuen App deaktiviert | Sie können keine neuen benutzerdefinierten OAuth2-Programme mehr in Workfront erstellen. Bestehende Anwendungen funktionieren weiterhin. |
| &#x200B;1. Februar 2027 | Alter Service eingestellt | Vorhandene benutzerdefinierte OAuth2-Anwendungen funktionieren nicht mehr vollständig. Jede Integration, die nicht zu Adobe Developer Console migriert wurde, verliert derzeit den Zugriff auf die Workfront-API. |

>[!IMPORTANT]
>
>Es wird dringend empfohlen, die Migration vor dem 1. November 2026 zu planen und abzuschließen, damit Ihre Integrationen ohne Unterbrechung weiter ausgeführt werden und die strenge Frist vom 1. Februar 2027 nicht abläuft.

## Betroffene Organisationen

Ihre Organisation ist von dieser Änderung betroffen, wenn sie über Integrationen, Skripte oder Tools verfügt, die über eine benutzerdefinierte OAuth2-Client-ID und geheime Daten, die über den alten OAuth2-Setup-Bildschirm von Workfront ausgegeben wurden, eine Verbindung zu Workfront herstellen. Häufige Beispiele sind:

* Benutzerdefinierte Integrationen, die Ihr Engineering-Team für die Workfront-API verwaltet.
* Connectoren von Drittanbietern oder Partnern, die mit einer von Workfront ausgestellten Client-ID konfiguriert sind. Wir empfehlen, sich an Ihren Anbieter zu wenden, wenn Sie sich nicht sicher sind, wie sich dessen Integration authentifiziert.
* Interne Automatisierungs-, Reporting- oder Datensynchronisationsskripte, die die Workfront-API direkt aufrufen.

Wenn Sie nicht wissen, ob Ihr Unternehmen über diese verfügt, kann Ihr Workfront-Administrator in der OAuth2-Anwendungsliste unter **Setup** > **System** > **OAuth2** sehen, was derzeit registriert ist. Weitere Informationen finden Sie unter [Anzeigen und Verwalten von benutzerdefinierten OAuth2-Anwendungen](/help/quicksilver/administration-and-setup/configure-integrations/manage-custom-oauth2-apps.md).

## Authentifizierungstypen von Adobe Developer Console

Adobe Developer Console unterstützt mehr als eine Authentifizierungsmethode. Sie können den Typ auswählen, der Ihrer Integration entspricht:

* **Server-zu-Server**-Authentifizierung: Für eine Anwendung, die auf Ihrem Backend ausgeführt wird und Adobe-APIs im Namen Ihres Unternehmens aufruft, ohne dass Endbenutzer beteiligt sind. Dies ist die engste Übereinstimmung mit dem veralteten Workfront OAuth2-Muster, das mit Client-IDs und Geheimnissen verwendet wurde, und ist der Typ, den die meisten benutzerdefinierten Workfront-Integrationen, -Skripte und -Automatisierungen verwenden sollten.
* **Benutzerauthentifizierung**: In Fällen, in denen sich ein Adobe-Benutzer anmelden und sein Einverständnis erteilen muss, bevor Ihre Anwendung seine Daten anzeigen oder bearbeiten kann. Wenn Ihre Integration für einen bestimmten angemeldeten Workfront-Benutzer und nicht für Ihr Unternehmen als Ganzes agieren muss, verwenden Sie stattdessen diesen Typ.

  Wenn Sie Benutzerauthentifizierung auswählen, gibt es je nach Anwendungsarchitektur drei weitere Optionen:

  * **OAuth Web App**: Für Programme mit einer Frontend-Benutzeroberfläche und einem Backend-Server. Der Server speichert das Client-Geheimnis sicher und ruft Token ab.
  * **OAuth Single-Page App**: Für Web-Anwendungen, die nur mit einem Browser ausgeführt werden, ohne Backend-Server. Die Web-App selbst ruft Token ab.
  * **OAuth Native App**: Für Mobile- oder Desktop-Anwendungen, die nativ auf einem Gerät ausgeführt werden und keinen Backend-Server haben. Die native App ruft Token ab.

Die meisten Unternehmen, die eine Backend-Integration, ein Skript oder eine Automatisierung des veralteten OAuth2-Service migrieren, wünschen sich eine Server-zu-Server-Authentifizierung.

## Funktionsvergleich: veraltete OAuth2 im Vergleich zu Adobe Developer Console

Der alte Workfront OAuth2-Service (unter **Setup** > **System** > **OAuth2 Applications**) bietet drei Anwendungstypen mit einer Beschränkung von 10 OAuth2-Anwendungen pro Workfront-Instanz. So vergleichen sich diese Aspekte mit Adobe Developer Console:

| Legacy-Workfront-Typ | Fluss-/Authentifizierungsmethode | Developer Console-Äquivalent | Anpassen |
|---|---|---|---|
| Machine-to-Machine-Anwendung (CLIs, Daemons, Backend-Skripte) | JWT mit öffentlichem/privatem Schlüsselpaar | Server-zu-Server-Authentifizierung | Derselbe Zweck besteht darin, nicht den Endbenutzer einzubeziehen, aber der Mechanismus ändert sich. Der ältere Fluss verwendet ein Schlüsselpaar aus öffentlichem/privatem Schlüssel und JWT, während Server-zu-Server eine Client-ID und ein Client-Geheimnis mit einer OAuth-Client-Berechtigungszuweisung verwendet. Dies ist kein Austausch von Anmeldeinformationen per Drop-in. Der Authentifizierungs-Code der Integration muss sich ändern, nicht nur die Werte der Anmeldeinformationen. Weitere Informationen finden Sie unter [Verwenden des JWT-Flusses für benutzerdefinierte OAuth 2-Anwendungen](/help/quicksilver/wf-api/api/oauth-app-jwt-flow.md). |
| Web-Anwendung (Server-seitige Apps: Go, Java, .NET, Node, PHP) | OAuth 2.0-Autorisierungs-Code-Fluss | OAuth Web App (unter Benutzerauthentifizierung) | 1:1-Treffer am ehesten. Dies hat denselben Fluss und dieselbe grundlegende Form, in der ein Backend-Server das Client-Geheimnis speichert. Weitere Informationen finden Sie unter [Autorisierungs-Code-Fluss für benutzerdefinierte OAuth 2-Anwendungen](/help/quicksilver/wf-api/api/oauth-app-code-token-flow.md). |
| Single Page Web Application (JS, Angular, React, Vue) | Autorisierungs-Code-Fluss mit PKCE, kein Client-Geheimnis | OAuth Single-Page App (unter Benutzerauthentifizierung) | Nächstgelegene 1:1-ÜbereinstimmungDies hat denselben PKCE-basierten, nicht geheimen Fluss. Weitere Informationen finden Sie unter [Verwenden des PKCE-Flusses für OAuth 2-](/help/quicksilver/wf-api/api/oauth-app-pkce-flow.md). |
| (kein älteres Äquivalent) | – | Native OAuth-App (unter Benutzerauthentifizierung) | Dies ist eine neue Funktion. Legacy Workfront OAuth2 hat keinen dedizierten Typ für native Mobile- oder Desktop-Anwendungen. |

<!--

>[!NOTE]
>
>A few legacy capabilities don't have a confirmed equivalent yet in Adobe Developer Console, and are being validated with the Developer Console team:
>
>* Per-app controls the legacy UI offers: refresh token rotation toggle, absolute vs. inactivity refresh token expiration, custom logo, privacy policy URL, and developer contact fields.
>* Whether Developer Console enforces a cap on credentials or projects similar to the legacy 10-app-per-instance limit.
>* Whether a JWT/key pair-based option remains available anywhere in Developer Console for Machine to Machine customers, or whether all such integrations must move to the client-secret-based Server-to-Server grant.

-->

## Migrationsverfahren

### Wenn Sie Workfront-Systemadministrator sind

>[!NOTE]
>
>Wenn Sie Workfront-Produktadministrator, aber kein Organisationsadministrator sind, müssen Sie mit Ihrem Organisationsadministrator zusammenarbeiten, um diese Migration abzuschließen, oder darum bitten, eine Migration durchzuführen.

1. Melden Sie sich bei [developer.adobe.com](https://developer.adobe.com) an und erstellen Sie ein neues Projekt. Projekte sind die Art und Weise, wie die Konsole verschiedene Integrationen oder Client-Programme organisiert.
1. Fügen Sie im Projekt eine API hinzu und wählen Sie **Adobe Workfront**. Diese API befindet sich unter der Kategorie Experience Cloud . Alle Workfront-APIs, einschließlich Planung, Workflow sowie Prüfung und Genehmigungen, nutzen diese API gemeinsam.
1. Wählen Sie die Option **Server-zu-Server**-Authentifizierung aus und wählen Sie dann die richtige Instanz aus, wenn Ihre IMS-Organisation über mehr als eine Workfront-Instanz verfügt.

   Anleitungen für die Auswahl eines Authentifizierungstyps finden Sie unter [Grundlegendes zu Adobe Developer Console-](#understand-adobe-developer-console-authentication-types)) in diesem Artikel.
1. Öffnen Sie auf der Projektseite die Details Ihrer neuen OAuth Server-zu-Server-Anmeldedaten, um Ihre Client-ID, Ihr Client-Geheimnis und die zum Generieren von Zugriffs-Token erforderlichen Informationen zu finden.
1. Aktualisieren Sie Ihre Integration, Ihr Skript oder Ihr Tool, um sich mit diesen neuen Anmeldeinformationen anstelle der alten Workfront OAuth2-Client-ID und des alten Geheimnisses zu authentifizieren.
1. Bestätigen des Zugriffs in Workfront. Beim Erstellen des API-Clients wird dieser automatisch als Workfront-Benutzer &quot;`techacct`&quot; hinzugefügt. Standardmäßig wird sie als Mitwirkende mit eingeschränktem Zugriff hinzugefügt, aber Sie können ihre Zugriffsebene wie für jeden anderen Benutzer anpassen.
1. (Optional) Um dem `techacct` Benutzer Administratorrechte zu gewähren, fügen Sie die E-Mail-Adresse des technischen Kontos als Administrator des entsprechenden Produktprofils in Admin Console hinzu.
1. Testen Sie die Integration End-to-End.
1. Beenden Sie den alten OAuth2-Anwendungseintrag in Workfront, nachdem Sie bestätigt haben, dass die neue Verbindung funktioniert.

Ausführliche Informationen und Screenshots in Einzelschritten finden Sie unter [Zugriff erhalten](https://developer.adobe.com/workfront-apis/guides/gaining_access/) in der Dokumentation zu Developer Console von Adobe.

### Wenn Sie kein Systemadministrator sind

Sie müssen sich an den IMS-Organisationsadministrator Ihres Unternehmens wenden, um die Migration abzuschließen, da das Einrichten der neuen Anmeldeinformationen in Adobe Developer Console diese Zugriffsebene erfordert. Wenn Sie eine Integration verwalten oder verwalten, aber wissen, wer der IMS-Organisationsadministrator Ihrer Organisation ist, wenden Sie sich an einen der folgenden Ansprechpartner:

* Ihr Workfront-Accountteam
* Ihr internes IT-Team
* Ihr technischer Ansprechpartner

## Wenn Sie nicht migrieren

Integrationen, die nach dem 1. Februar 2027 noch das veraltete Client-ID-/Geheimmuster für OAuth2 verwenden, können sich nicht mehr gegenüber der Workfront-API authentifizieren und ein abhängiger Workflow, eine Synchronisierung oder eine Automatisierung schlagen fehl. Nach diesem Datum ist keine Verlängerung geplant, migrieren Sie also Ihre Integrationen weit früher als geplant.

## Häufig gestellte Fragen

**Wirkt sich dies auf die von Adobe bereitgestellten Integrationspakete aus, z. B. Slack oder Microsoft Teams?**

Nein. Globale Anwendungen, die von Adobe verwaltet werden, werden von Adobe direkt migriert und erfordern keine Benutzeraktion.

**Wird meine vorhandene Integration vor dem 1. Februar 2027 nicht mehr funktionieren?**

Nein. Vorhandene benutzerdefinierte OAuth2-Anwendungen funktionieren weiterhin normal bis zum 1. Februar 2027. Nur die Möglichkeit, neue benutzerdefinierte OAuth2-Programme zu erstellen, ist ab dem 1. November 2026 betroffen.

**Ist die Migration mit Kosten verbunden?**

Nein, die Authentifizierung über Adobe Developer Console verursacht keine zusätzlichen Kosten.

**Wo erhalte ich Hilfe?**

Wenden Sie sich an Ihr Workfront-Account-Team oder eröffnen Sie einen Support-Fall, wenn Sie Fragen zu Ihrer spezifischen Integration oder Ihrem Zeitplan haben. Die offizielle, aktuelle Anleitung zum Setup mit Screenshots finden Sie unter [Zugriff erhalten](https://developer.adobe.com/workfront-apis/guides/gaining_access/) in der Dokumentation zu Developer Console von Adobe.
