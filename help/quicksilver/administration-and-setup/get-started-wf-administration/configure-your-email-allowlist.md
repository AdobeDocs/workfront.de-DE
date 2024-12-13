---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Konfigurieren der E-Mail-Zulassungsliste
description: Wenn Ihr Unternehmen den WorkfrontEnterprise-Plan verwendet, können Sie eine Workfront-E-Mail-Zulassungsliste erstellen, um zu steuern, welche E-Mail-Domains E-Mails von Workfront akzeptieren dürfen und welche E-Mail-Domains sich in der E-Mail-Adresse befinden können, die Benutzende in ihrem Benutzerprofil angeben. Dies ist nützlich, wenn die Sicherheitsrichtlinie Ihres Unternehmens Benutzende daran hindert, in Workfront gespeicherte Daten an externe E-Mail-Adressen zu senden. Sie können nur Ihre unternehmensinternen Domains in die Zulassungsliste einbeziehen, um sicherzustellen, dass diese Richtlinie eingehalten wird.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 937965ad495453e185504d53f9d9c88c3cd7e201
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Konfigurieren der E-Mail-Zulassungsliste

Wenn Ihr Unternehmen den Workfront Enterprise-Plan verwendet, können Sie eine Workfront-E-Mail-Zulassungsliste erstellen, um Folgendes zu steuern:

* Welche E-Mail-Domains dürfen E-Mails von Workfront akzeptieren?
* Welche E-Mail-Domains können sich in der E-Mail-Adresse befinden, die Benutzer in ihrem Benutzerprofil angeben?

Dies ist nützlich, wenn die Sicherheitsrichtlinie Ihres Unternehmens Benutzende daran hindert, in Workfront gespeicherte Daten an externe E-Mail-Adressen zu senden. Sie können nur Ihre unternehmensinternen Domains in die Zulassungsliste einbeziehen, um sicherzustellen, dass diese Richtlinie eingehalten wird.

>[!IMPORTANT]
>
>Ihr IT-Team sollte sicherstellen, dass eingehende E-Mails von `notifications@my.workfront.com` im System Ihres Unternehmens nicht blockiert werden.
>
>Alle E-Mails von Workfront werden von dieser Adresse gesendet, um den erfolgreichen E-Mail-Versand zu steigern und das Spoofing von E-Mails zu beseitigen. Dazu gehören sowohl automatisierte Warnhinweise als auch die Kommunikation zwischen Benutzern.
>
>Die „Von“-Zeile in einer Workfront-E-Mail, die Sie von einem Benutzer namens Joan Harris erhalten, würde beispielsweise wie folgt aussehen:
>`Joan Harris <notifications@my.workfront.com>`

Informationen zum Konfigurieren der Firewall Ihres Unternehmens zum Öffnen der Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront auf die Zulassungsliste setzen-Servern finden Sie unter [Konfigurieren der Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Andere Zulassungslisten

Wenn Ihr Unternehmen über einen Unternehmensplan verfügt, können Sie eine Adobe Workfront-IP-Zulassungsliste konfigurieren, die den Zugriff auf Workfront auf 75 IP-Adressen oder IP-Adressbereiche beschränkt, die Sie angeben. Dies bietet eine zusätzliche Sicherheitsebene für das Workfront-Programm. Weitere Informationen finden Sie unter [Zugriff auf Adobe Workfront nach IP-Adresse beschränken](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff haben, müssen Sie der Zulassungsliste bestimmte IP-Adressen hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern geöffnet. Weitere Informationen hierzu finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Konfigurieren der E-Mail-Zulassungsliste

{{step-1-to-setup}}

1. Klicken Sie **System** > **Kundeninformationen**.
1. Auf die Zulassungsliste setzen Auf die Zulassungsliste setzen Wählen Sie im Abschnitt **E** Mail **die Option Domain aktivieren** und klicken Sie dann auf **Domain hinzufügen**.
1. Geben Sie in das angezeigte Feld eine Domain ein, die Sie zulassen möchten, z. B. `ourcompany.com`, und klicken Sie dann auf **Domain hinzufügen**.
1. Wiederholen Sie den vorherigen Schritt, um weitere Domains hinzuzufügen, die Sie zulassen möchten.
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.
