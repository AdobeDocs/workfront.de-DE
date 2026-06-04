---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Konfigurieren  [!DNL Workfront Proof]  E-Mails zur Vermeidung von Spam-Filtern
description: 'Der Spam-Filter Ihres E-Mail-Clients erfüllt einen wichtigen Zweck: Sie vor lästigen und möglicherweise bösartigen Spam-Mails zu schützen. Wenn Sie jedoch nicht die richtigen Einstellungen im Spam-Filter haben, können Sie die folgenden wichtigen E- [!DNL Workfront Proof] -Mails nicht sehen: Korrekturabzugs-E-Mail-Benachrichtigungen, Newsletter und spezielle Nachrichten.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
TQID: https://experienceleague.adobe.com/QMtIDexmxDDuKqTg-Z47-lMnQ27zDEdMtwg-8OUe3Uw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 496
ht-degree: 0%

---

# Konfigurieren [!DNL Workfront Proof] E-Mails zur Vermeidung von Spam-Filtern

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Der Spam-Filter Ihres E-Mail-Clients erfüllt einen wichtigen Zweck: Sie vor lästigen und möglicherweise bösartigen Spam-Mails zu schützen. Wenn Sie jedoch nicht die richtigen Einstellungen im Spam-Filter haben, können Sie die folgenden wichtigen [!DNL Workfront Proof]-E-Mails nicht sehen: Korrekturabzugs-E-Mail-Benachrichtigungen, Newsletter und spezielle Nachrichten.

Um sicherzustellen, dass Ihre [!DNL Workfront Proof]-E-Mails immer an Ihren Posteingang und nicht an Ihren Spam-Ordner weitergeleitet werden, sollten Sie der Zulassungsliste Folgendes hinzufügen:

* [!DNL Workfront Proof]-Mailserver: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot;-E-Mail-Adressen (z. B. notification@proofhq.com)

Weitere Informationen zu URLs, die Sie Ihrer Zulassungsliste hinzufügen können, finden [&#x200B; unter „Konfigurieren der Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) im Artikel [Konfigurieren der Firewall-Zulassungsliste &#x200B;](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] E[!UICONTROL Mail]Adressen „Von“

Je nach Art Ihres E-Mail-Clients müssen Sie möglicherweise [!DNL Workfront Proof] E-Mail-Adressen &quot;[!UICONTROL from]&quot; zu einer der folgenden Adressen hinzufügen, um zu verhindern, dass der Spam-Filter Ihre E-Mails in Zukunft an Ihren Spam-Ordner weiterleitet:

* Ihre Kontaktliste
* Ihre [!UICONTROL Liste sicherer &#x200B;]&quot;
* Ein Filter, den Sie erstellen, um E-Mails von diesen Adressen an Ihren Posteingang zu senden

Möglicherweise müssen Sie auch alle vorhandenen [!DNL Workfront Proof]-E-Mails aus Ihrem Spam-Ordner entfernen und überprüfen, ob eine der &quot;[!UICONTROL from]-Adressen auf der Liste der blockierten Adressen steht. Auf dieser Hilfeseite werden die [!DNL Workfront Proof] &quot;[!UICONTROL from]-Adressen aufgelistet und es wird gezeigt, wie sie in den folgenden E-Mail-Clients zum Spam-Filter hinzugefügt werden können:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Wenn Sie Fragen zu einem hier beschriebenen Verfahren haben, überprüfen Sie bitte die Hilfe Ihres E-Mail-Clients.

Weitere Informationen finden Sie unter [Konfigurieren von Spam-Einstellungen für gängige E-Mail-Clients](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## Die [!DNL Workfront Proof] zu kopierenden [!UICONTROL von]-E-Mail-Adressen

Um sicherzustellen, dass Ihre [!DNL Workfront Proof] E-Mails Ihren Posteingang erreichen, müssen Sie dem Spam-Filter Ihres E-Mail-Clients zwei [!DNL Workfront Proof] E-Mail-Adressen separat hinzufügen:

* Die allgemeine Support-Adresse [!DNL support@proofhq.com], von der [!DNL Workfront Proof] viele E-Mail-Nachrichten sendet
* Eine Benachrichtigungsadresse, von der [!DNL Workfront Proof] Benachrichtigungs-E-Mails für Korrekturabzüge an die Person sendet, die den Korrekturabzug erstellt hat, und an die Prüfer, die über Links zum Korrekturabzug verfügen. Dies kann eine allgemeine Adresse, notification@support.proofhq.com, oder eine bestimmte Adresse sein, wenn Sie eine benutzerdefinierte Subdomain oder eine White-Label-Domain haben.

So fügen Sie [!DNL Workfront Proof] Filter Ihres E[!UICONTROL Mail]Clients „Von“-Adressen hinzu:

1. Kopieren Sie die E-Mail-Adresse &quot;[!UICONTROL from]&quot; des allgemeinen [!DNL Workfront Proof]-Supports (support@proofhq.com) und fügen Sie sie in das für Ihren E-Mail-Client angegebene Feld ein.
1. Kopieren Sie die entsprechende der [!DNL Workfront Proof] E-Mail-Adressen [!UICONTROL von] und fügen Sie sie SEPARAT in das für Ihren E-Mail-Client angegebene Feld ein:

   * notification@support.proofhq.com, wenn Sie KEINE benutzerdefinierte Subdomain oder White-Label-Domain haben
   * notification@yoursubdomain.proofhq.com Wenn Sie eine benutzerdefinierte Subdomain haben, ersetzen Sie den Namen Ihrer Subdomain in dieser Adresse
   * notification@yoursubdomain.yourdomain.com Wenn Sie eine White-Label-Domain haben, ersetzen Sie in dieser Adresse Ihren Subdomain-Namen und Ihren Domain-Namen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
