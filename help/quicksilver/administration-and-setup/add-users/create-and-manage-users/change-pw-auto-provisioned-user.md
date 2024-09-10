---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Ändern des Kennworts für einen automatisch bereitgestellten Benutzer
description: Es wird empfohlen, den Benutzernamen eines neuen Benutzers in seine Workfront-E-Mail-Adresse zu ändern und ihm dann zu erlauben, sein Passwort zu ändern.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 14124911-e5e1-4a4f-9b25-8b4fab0329e1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '464'
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
>  In der URL `https://acme.workfront.com/user/61941ab1000af22d7104628efa1c738b/details` würden Sie beispielsweise die Zeichenfolge aus Zahlen und Buchstaben zwischen den letzten beiden Schrägstrichen kopieren: `61941ab1000af22d7104628efa1c738b`.
>
>  Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
>
>* Erstellen Sie einen Benutzerbericht mit der Spalte Benutzer > GUID . Weitere Informationen finden Sie unter [Erstellen eines Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).
>
>* Abfragen der Workfront-API.
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ändern des Kennworts für einen automatisch bereitgestellten Benutzer

1. Bestimmen Sie den GUID-Benutzernamen eines Benutzers, indem Sie eine API-Anfrage übergeben, wie im folgenden Beispiel gezeigt:

   https://`<domain>`.my.workfront.com/attask/api/v14.0/USER/search?fields=username&amp;ID=`<ID of User>` Wobei *`<domain>`* die Domäne Ihres Unternehmens und *`<ID of User>`* die Workfront ID des Benutzers ist.

   Sie erhalten eine Antwort ähnlich der folgenden:

   ![](assets/get-guid.png)

   Die Rückgabe für &quot;username&quot;ist die GUID des Benutzers.

1. Ändern Sie unter Verwendung der GUID als Benutzernamen das Kennwort des Benutzers.

   Weitere Informationen zum Ändern des Kennworts finden Sie unter [Kennwort zurücksetzen](../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md).

   Wenn Ihr Unternehmen ein SSO-System verwendet, kann nur ein Workfront-Systemadministrator das Kennwort eines Benutzers ändern. Weitere Informationen finden Sie unter [Überblick über die einmalige Anmeldung in Adobe Workfront](../../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)

1. Wenn sich der Benutzer bei Workfront angemeldet hat, navigieren Sie zu:

```
   https://<your domain>.my.workfront.com/login/convertUsername
```

1. Überprüfen Sie im Feld **Ihre E-Mail-Adresse für die Anmeldung** , ob die E-Mail-Adresse des Benutzers korrekt ist, und klicken Sie dann auf **Konto aktualisieren**.

   ![](assets/guidusername-350x272.png)

   Der Benutzername des Benutzers wird in seine Workfront-E-Mail-Adresse geändert.

>[!TIP]
>
>So suchen Sie die ID eines Benutzers:
>
>1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Benutzer** ![](assets/users-icon-in-main-menu.png).![](assets/main-menu-icon.png)
>
>1. Wählen Sie den Benutzer aus.
>
>   Die Profilseite des Benutzers wird geöffnet und seine Benutzer-ID wird in der URL angezeigt.
>
