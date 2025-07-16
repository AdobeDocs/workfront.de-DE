---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Zugriff auf Adobe Workfront nach IP-Adresse beschränken
description: Sie können eine Adobe Workfront-IP-Zulassungsliste konfigurieren, die den Zugriff auf Workfront auf 75 IP-Adressen oder IP-Adressbereiche beschränkt, die Sie angeben. Dies bietet eine zusätzliche Sicherheitsebene für das Workfront-Programm.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 65121fae364683373d2bc9abbe6672755d0cd09c
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Zugriff auf Adobe Workfront nach IP-Adresse beschränken

>[!IMPORTANT]
>
>Diese Funktion ist derzeit nicht für Organisationen verfügbar, die in die Adobe Admin Console integriert wurden. Sie wird in einer zukünftigen Version in der Adobe Admin Console verfügbar sein.

Sie können eine Adobe Workfront-IP-Zulassungsliste konfigurieren, die den Zugriff auf Workfront auf 75 IP-Adressen oder IP-Adressbereiche beschränkt, die Sie angeben. Dies bietet eine zusätzliche Sicherheitsebene für das Workfront-Programm.

Diese IP-Adressen oder IP-Adressbereiche sollten von Ihrem Netzwerkadministrator bereitgestellt werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Unternehmen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Andere Zulassungslisten

Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff haben, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern geöffnet. Weitere Informationen hierzu finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Wenn Ihr Unternehmen den Enterprise-Plan verwendet, können Sie die E-Mail-Workfronts von auf die Zulassungsliste setzen so konfigurieren, dass gesteuert wird, welche E-Mail-Domains E-Mails von Workfront akzeptieren dürfen und welche E-Mail-Domains sich in der E-Mail-Adresse befinden können, die Benutzende in ihrem Workfront-Benutzerprofil angeben. Auf die Zulassungsliste setzen Weitere Informationen finden Sie unter [Konfigurieren Ihrer E-Mail](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Hinzufügen von IP-Adressen zur Zulassungsliste

Nachdem Sie der Workfront-Zulassungsliste IP-Adressen hinzugefügt haben, können nur diese IP-Adressen für den Zugriff auf Workfront verwendet werden. Benutzer, die versuchen, über eine andere IP-Adresse auf Workfront zuzugreifen, erhalten eine Fehlermeldung, die angibt, dass ihre IP-Adresse blockiert ist.

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Kundeninformationen.**

1. Wählen Sie im Abschnitt **IP** Zulassungsliste) die Option **IP-Zulassungsliste aktivieren.**

   Diese Option ist standardmäßig deaktiviert.

1. Geben Sie die IP-Adresse an, mit der Sie derzeit auf das Workfront-System zugreifen.

   Oder

   Geben Sie einen IP-Adressbereich an, der die IP-Adresse enthält, mit der Sie derzeit auf das Workfront-System zugreifen.

   Die IP-Adresse, die Sie für den Zugriff auf Workfront verwenden, muss der -Zulassungsliste auf die Zulassungsliste setzte hinzugefügt werden, bevor die -Datei aktiviert wird.

1. Klicken Sie auf **IP-Bereich hinzufügen** und geben Sie dann die IP-Adresse oder den IP-Adressbereich an, auf die bzw. den Sie auf Workfront zugreifen möchten.
1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere IP-Adressen oder IP-Adressbereiche hinzuzufügen.

   Es können bis zu 75 Adressen oder Bereiche hinzugefügt werden.

1. Klicken Sie auf **Speichern.**
