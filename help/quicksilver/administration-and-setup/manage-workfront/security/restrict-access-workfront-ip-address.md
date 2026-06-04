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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/lF3yMazoaB-W2h4ePgavnN96SZ98YYiJYuC927ImYcs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 405
ht-degree: 10%

---

# Zugriff auf Adobe Workfront nach IP-Adresse beschränken

<!--
>[!IMPORTANT]
>
>This functionality is not currently available to organizations that have been onboarded to the Adobe Admin Console. It will be available in the Adobe Admin Console in a future release.
-->

Sie können eine Adobe Workfront-IP-Zulassungsliste konfigurieren, die den Zugriff auf Workfront auf 75 IP-Adressen oder IP-Adressbereiche beschränkt, die Sie angeben. Dies bietet eine zusätzliche Sicherheitsebene für das Workfront-Programm.

Diese IP-Adressen oder IP-Adressbereiche sollten von Ihrem Netzwerkadministrator bereitgestellt werden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p><p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Andere Zulassungslisten

Wenn Ihre Firewall oder Ihr Mail-Server so konfiguriert ist, dass nur bestimmte Anbieter Zugriff haben, müssen Sie bestimmte IP-Adressen zu ihrer Zulassungsliste hinzufügen. Dadurch wird die Kommunikation zwischen Ihrer Umgebung und den Adobe Workfront-Servern geöffnet. Weitere Informationen hierzu finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Wenn Ihr Unternehmen den Enterprise-Plan verwendet, können Sie die E-Mail-Workfronts von auf die Zulassungsliste setzen so konfigurieren, dass gesteuert wird, welche E-Mail-Domains E-Mails von Workfront akzeptieren dürfen und welche E-Mail-Domains sich in der E-Mail-Adresse befinden können, die Benutzende in ihrem Workfront-Benutzerprofil angeben. Weitere Informationen finden Sie unter [Konfigurieren Ihrer E-Mail](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Hinzufügen von IP-Adressen zur Zulassungsliste

Nachdem Sie der Workfront-Zulassungsliste IP-Adressen hinzugefügt haben, können nur diese IP-Adressen für den Zugriff auf Workfront verwendet werden. Benutzer, die versuchen, über eine andere IP-Adresse auf Workfront zuzugreifen, erhalten eine Fehlermeldung, die angibt, dass ihre IP-Adresse blockiert ist.

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Kundeninfos**.

1. Wählen Sie im Abschnitt **IP** Zulassungsliste) die Option **IP-Zulassungsliste aktivieren.**

   Standardmäßig ist diese Option deaktiviert.

1. Geben Sie die IP-Adresse an, mit der Sie derzeit auf das Workfront-System zugreifen.

   ODER

   Geben Sie einen IP-Adressbereich an, der die IP-Adresse enthält, mit der Sie derzeit auf das Workfront-System zugreifen.

   Die IP-Adresse, die Sie für den Zugriff auf Workfront verwenden, muss der -Zulassungsliste hinzugefügt werden, bevor die -Datei aktiviert wird.

1. Klicken Sie auf **IP-Bereich hinzufügen** und geben Sie dann die IP-Adresse oder den IP-Adressbereich an, auf die bzw. den Sie auf Workfront zugreifen möchten.
1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere IP-Adressen oder IP-Adressbereiche hinzuzufügen.

   Es können bis zu 75 Adressen oder Bereiche hinzugefügt werden.

1. Klicken Sie auf **Speichern.**
