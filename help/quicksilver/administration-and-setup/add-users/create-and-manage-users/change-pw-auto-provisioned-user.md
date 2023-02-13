---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Ändern des Kennworts für einen automatisch bereitgestellten Benutzer
description: Wenn ein neuer Benutzer häufig versucht, sein temporäres Kennwort zu ändern, gibt er seine E-Mail-Adresse ein und erhält einen Fehler wegen eines falschen Benutzernamens. Sie müssen ihren systemzugewiesenen Benutzernamen eingeben, d. h. ihre Globally Unique Identifier (GUID). Da sich eine GUID nur schwer merken und verwenden lässt, empfehlen wir, den Benutzernamen eines neuen Benutzers in die Workfront-E-Mail-Adresse zu ändern und ihm dann zu erlauben, sein Passwort zu ändern.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Ändern des Kennworts für einen automatisch bereitgestellten Benutzer

Wenn Sie Benutzer durch die automatische Bereitstellung erstellen, weist ihnen Adobe Workfront eine GUID (Globally Unique Identifier) für einen Benutzernamen zu. Eine GUID ist eine eindeutige Zeichenfolge aus zufälligen Zahlen und Buchstaben, z. B. *5489cb430012526e1ea635e8c29f377f*.

Wenn ein neuer Benutzer versucht, sein temporäres Kennwort zu ändern, gibt er oft seine E-Mail-Adresse für seinen Benutzernamen ein und erhält einen Fehler wegen eines falschen Benutzernamens. Damit der Benutzer sein Kennwort ändern kann, muss er seinen systemzugewiesenen Benutzernamen eingeben, der eine GUID ist.

Da die Verwendung von GUID-Benutzernamen schwierig sein kann, empfehlen wir, zunächst den Benutzernamen eines Benutzers in seine Workfront-E-Mail-Adresse zu ändern und ihm dann zu erlauben, sein Kennwort zu ändern.

>[!TIP]
>
>Sie finden die GUID eines Benutzers wie folgt:
>
>* Gehen Sie zum Profil des Benutzers und kopieren Sie die GUID aus der URL in Ihren Browser.
>
>  Beispiel: in der URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details`, würden Sie die Zeichenfolge aus Zahlen und Buchstaben zwischen den letzten beiden Schrägstrichen kopieren: `61941ab1000af22d7104628efa1c738b`.
>
>  Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Erstellen Sie einen Benutzerbericht mit der Spalte Benutzer > GUID . Weitere Informationen finden Sie unter [Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Abfragen der Workfront-API.
>


## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändern des Kennworts für einen automatisch bereitgestellten Benutzer

1. Bestimmen Sie den GUID-Benutzernamen eines Benutzers, indem Sie eine API-Anfrage übergeben, wie im folgenden Beispiel gezeigt:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` Wo *`<domain>`* die Domäne Ihres Unternehmens ist und *`<ID of User>`* ist die Workfront ID des Benutzers.

   Sie erhalten eine Antwort ähnlich der folgenden:

   ![](assets/get-guid.png)

   Die Rückgabe für &quot;username&quot;ist die GUID des Benutzers.

1. Ändern Sie unter Verwendung der GUID als Benutzernamen das Kennwort des Benutzers.

   Weitere Informationen zum Ändern des Kennworts finden Sie unter [Passwort zurücksetzen](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Wenn Ihr Unternehmen ein SSO-System verwendet, kann nur ein Workfront-Systemadministrator das Kennwort eines Benutzers ändern. Weitere Informationen finden Sie unter [Überblick über Single Sign-on in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Wenn sich der Benutzer bei Workfront angemeldet hat, navigieren Sie zu:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. Im **Ihre Login-E-Mail-Adresse** überprüfen, ob die E-Mail-Adresse des Benutzers korrekt ist, und klicken Sie auf **Konto aktualisieren**.

   ![](assets/guidusername-350x272.png)

   Der Benutzername des Benutzers wird in seine Workfront-E-Mail-Adresse geändert.

>[!TIP]
>
>So suchen Sie die ID eines Benutzers:
>
>1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).
>
>1. Wählen Sie den Benutzer aus.
>
>   Die Profilseite des Benutzers wird geöffnet und seine Benutzer-ID wird in der URL angezeigt.
