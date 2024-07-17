---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Konfigurieren der E-Mail-Zulassungsliste
description: Wenn Ihr Unternehmen den WorkspaceEnterprise-Plan verwendet, können Sie eine Workfront-E-Mail-Zulassungsliste erstellen, um zu steuern, welche E-Mail-Domains E-Mails von Workfront akzeptieren dürfen und welche E-Mail-Domains sich in der E-Mail-Adresse befinden können, die Benutzer in ihrem Benutzerprofil angeben. Dies ist nützlich, wenn die Sicherheitsrichtlinie Ihres Unternehmens Benutzer daran hindert, in Workfront gespeicherte Daten an externe E-Mail-Adressen zu senden. Sie können nur Ihre internen Unternehmensdomänen in die Zulassungsliste aufnehmen, um sicherzustellen, dass diese Richtlinie befolgt wird.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Konfigurieren der E-Mail-Zulassungsliste

Wenn Ihr Unternehmen den WorkspaceEnterprise-Plan verwendet, können Sie eine Workfront-E-Mail-Zulassungsliste erstellen, um Folgendes zu steuern:

* Welche E-Mail-Domains dürfen E-Mails von Workfront akzeptieren?
* Welche E-Mail-Domänen können sich in der E-Mail-Adresse befinden, die Benutzer in ihrem Benutzerprofil angeben.

Dies ist nützlich, wenn die Sicherheitsrichtlinie Ihres Unternehmens Benutzer daran hindert, in Workfront gespeicherte Daten an externe E-Mail-Adressen zu senden. Sie können nur Ihre internen Unternehmensdomänen in die Zulassungsliste aufnehmen, um sicherzustellen, dass diese Richtlinie befolgt wird.

>[!IMPORTANT]
>
>Ihr IT-Team sollte sicherstellen, dass eingehende E-Mails von `notifications@my.workfront.com` nicht im System Ihres Unternehmens blockiert werden.
>
>Sämtliche E-Mails von Workfront werden von dieser Adresse gesendet, um einen erfolgreichen E-Mail-Versand zu ermöglichen und den Versand von E-Mails zu verhindern. Dies umfasst sowohl automatisierte Warnhinweise als auch die Kommunikation zwischen Benutzern.
>
>Die Zeile Von in einer Workfront-E-Mail, die Sie von einem Benutzer namens Joan Harris erhalten, würde beispielsweise wie folgt aussehen:
>
```
>Joan Harris <notifications@my.workfront.com>
>```

Informationen zum Konfigurieren der Firewall Ihres Unternehmens für das Öffnen der Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Zugriffsanforderungen

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Andere Zulassungslisten

Wenn Ihr Unternehmen über den Unternehmensplan verfügt, können Sie eine Adobe Workfront IP-Zulassungsliste konfigurieren, die den Zugriff auf Workfront auf 45 von Ihnen festgelegte IP-Adressen oder IP-Adressbereiche beschränkt. Dies bietet eine zusätzliche Sicherheitsebene für die Workfront-Anwendung. Weitere Informationen finden Sie unter [Zugriffsbeschränkung auf Adobe Workfront nach IP-Adresse](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Wenn Ihre Firewall oder Ihr E-Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern geöffnet. Weitere Informationen dazu finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall-Benutzer](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Konfigurieren der E-Mail-Zulassungsliste

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **System** > **Kundeninformationen**.

1. Wählen Sie im Bereich **E-Mail-Zulassungsliste** die Option **Domain-Zulassungsliste aktivieren** und klicken Sie dann auf **Domäne hinzufügen**.
1. Geben Sie in das angezeigte Feld eine Domäne ein, die Sie zulassen möchten, z. B. `ourcompany.com`, und klicken Sie dann auf **Domäne hinzufügen**.

1. Wiederholen Sie den vorherigen Schritt, um alle anderen Domänen hinzuzufügen, die Sie zulassen möchten.
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.
