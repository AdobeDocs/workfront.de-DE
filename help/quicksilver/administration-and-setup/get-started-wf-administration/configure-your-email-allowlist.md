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
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '399'
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
>>`Joan Harris <notifications@my.workfront.com>`

Informationen zum Konfigurieren der Firewall Ihres Unternehmens zum Öffnen der Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront auf die Zulassungsliste setzen-Servern finden Sie unter [Konfigurieren der Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p> <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen ein Workfront-Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Andere Zulassungslisten

Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff haben, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern geöffnet. Weitere Informationen hierzu finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Konfigurieren der E-Mail-Zulassungsliste

{{step-1-to-setup}}

1. Klicken Sie **System** > **Kundeninformationen**.
1. Auf die Zulassungsliste setzen Auf die Zulassungsliste setzen Wählen Sie im Abschnitt **E** Mail **die Option Domain aktivieren** und klicken Sie dann auf **Domain hinzufügen**.
1. Geben Sie in das angezeigte Feld eine Domain ein, die Sie zulassen möchten, z. B. `ourcompany.com`, und klicken Sie dann auf **Domain hinzufügen**.
1. Wiederholen Sie den vorherigen Schritt, um weitere Domains hinzuzufügen, die Sie zulassen möchten.
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.
