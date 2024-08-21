---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Zugriff auf Adobe Workfront nach IP-Adresse einschränken
description: Sie können eine Adobe Workfront IP-Zulassungsliste konfigurieren, die den Zugriff auf Workfront auf 45 von Ihnen angegebene IP-Adressen oder IP-Adressbereiche beschränkt. Dies bietet eine zusätzliche Sicherheitsebene für die Workfront-Anwendung.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Zugriff auf Adobe Workfront nach IP-Adresse einschränken

Sie können eine Adobe Workfront IP-Zulassungsliste konfigurieren, die den Zugriff auf Workfront auf 45 von Ihnen angegebene IP-Adressen oder IP-Adressbereiche beschränkt. Dies bietet eine zusätzliche Sicherheitsebene für die Workfront-Anwendung.

Diese IP-Adressen oder IP-Adressbereiche sollten von Ihrem Netzwerkadministrator bereitgestellt werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Unternehmen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Andere Zulassungslisten

Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff erhalten, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern geöffnet. Weitere Informationen dazu finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall-Benutzer](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Wenn Ihr Unternehmen den Enterprise-Plan verwendet, können Sie die Workfront-E-Mail-Zulassungsliste so konfigurieren, dass gesteuert wird, welche E-Mail-Domänen E-Mails von Workfront akzeptieren dürfen und welche E-Mail-Domänen sich in der E-Mail-Adresse befinden können, die Benutzer in ihrem Workfront-Benutzerprofil angeben. Weitere Informationen finden Sie unter [Konfigurieren der E-Mail-Zulassungsliste](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Hinzufügen von IP-Adressen zur Zulassungsliste

Nachdem Sie IP-Adressen zur Workfront-Zulassungsliste hinzugefügt haben, können nur diese IP-Adressen für den Zugriff auf Workfront verwendet werden. Benutzer, die versuchen, von einer anderen IP-Adresse aus auf Workfront zuzugreifen, erhalten eine Fehlermeldung, die darauf hinweist, dass ihre IP-Adresse gesperrt ist.

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Kundeninformationen.**

1. Wählen Sie im Bereich **IP-Zulassungsliste** die Option **IP-Zulassungsliste aktivieren** aus.

   Diese Option ist standardmäßig deaktiviert.

1. Geben Sie die IP-Adresse an, die Sie derzeit für den Zugriff auf das Workfront-System verwenden.

   Oder

   Geben Sie einen IP-Adressbereich an, der die IP-Adresse enthält, die Sie derzeit für den Zugriff auf das Workfront-System verwenden.

   Die IP-Adresse, die Sie für den Zugriff auf Workfront verwenden, muss der Zulassungsliste hinzugefügt werden, bevor die Zulassungsliste aktiviert wird.

1. Klicken Sie auf **IP-Bereich hinzufügen** und geben Sie dann die IP-Adresse oder den IP-Adressbereich an, über die Sie auf Workfront zugreifen können möchten.
1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere IP-Adressen oder IP-Adressbereiche hinzuzufügen.

   Sie können bis zu 45 Adressen oder Bereiche hinzufügen.

1. Klicken Sie auf **Speichern.**
