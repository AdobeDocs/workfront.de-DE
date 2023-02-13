---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Konfigurieren [!DNL Workfront Proof] E-Mails zur Vermeidung von Spam-Filtern
description: "Der Spamfilter Ihres E-Mail-Clients erfüllt einen wichtigen Zweck: Schutz vor lästigen und möglicherweise schädlichen Spam-E-Mails. Wenn Sie jedoch nicht über die richtigen Einstellungen im Spam-Filter verfügen, kann dies verhindern, dass Ihnen Folgendes angezeigt wird: [!DNL Workfront Proof] E-Mails: Testversand von E-Mail-Benachrichtigungen, Newslettern und speziellen Mitteilungen."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Konfigurieren [!DNL Workfront Proof] E-Mails zur Vermeidung von Spam-Filtern

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Der Spamfilter Ihres E-Mail-Clients erfüllt einen wichtigen Zweck: Schutz vor lästigen und möglicherweise schädlichen Spam-E-Mails. Wenn Sie jedoch nicht über die richtigen Einstellungen im Spam-Filter verfügen, kann dies verhindern, dass Ihnen Folgendes angezeigt wird: [!DNL Workfront Proof] E-Mails: Testversand von E-Mail-Benachrichtigungen, Newslettern und speziellen Mitteilungen.

Um sicherzustellen, dass Ihre [!DNL Workfront Proof] E-Mails werden immer in Ihren Posteingang und nicht in Ihren Spam-Ordner weitergeleitet. Fügen Sie der Zulassungsliste Folgendes hinzu:

* [!DNL Workfront Proof] Mailserver: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot;E-Mail-Adressen (z. B. notification@proofhq.com)

Weitere Informationen zu URLs, die Sie zu Ihrer Zulassungsliste hinzufügen können, finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) im Artikel [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot; E-Mail-Adressen

Je nach E-Mail-Client-Typ müssen Sie möglicherweise [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot; E-Mail-Adressen an eine der folgenden Adressen senden, um zu verhindern, dass der Spam-Filter in Zukunft Ihre E-Mails an Ihren Spam-Ordner weiterleitet:

* Kontaktliste
* Ihre [!UICONTROL Sichere Absender] Liste
* Einen Filter, den Sie erstellen, um E-Mails von diesen Adressen an Ihren Posteingang zu senden

Möglicherweise müssen Sie auch vorhandene [!DNL Workfront Proof] E-Mails aus Ihrem Spam-Ordner und überprüfen Sie, ob einer der &quot;[!UICONTROL von]&quot; Adressen befinden sich auf der Blockierungsadressenliste. Auf dieser Hilfeseite werden die [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot; Adressen und zeigt, wie sie in den folgenden E-Mail-Clients zum Spam-Filter hinzugefügt werden:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Wenn Sie Fragen zu einem hier beschriebenen Verfahren haben, überprüfen Sie bitte die Hilfe Ihres E-Mail-Clients.

Weitere Informationen finden Sie unter [Konfigurieren von Spam-Einstellungen für gängige E-Mail-Clients](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## Die [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot;E-Mail-Adressen kopieren

Um sicherzustellen, dass Ihre [!DNL Workfront Proof] E-Mails erreichen Ihren Posteingang. Sie müssen zwei hinzufügen [!DNL Workfront Proof] E-Mail-Adressen separat an den Spam-Filter Ihres E-Mail-Clients:

* Die allgemeine Unterstützungsadresse, [!DNL support@proofhq.com], von denen [!DNL Workfront Proof] sendet viele E-Mail-Nachrichten
* Eine Benachrichtigungsadresse, von der aus [!DNL Workfront Proof] sendet E-Mails mit der Benachrichtigung zum Testversand an den Ersteller des Testversands und die Validierer mit Links zum Testversand. Dabei kann es sich um eine allgemeine Adresse, notification@support.proofhq.com, oder eine bestimmte Adresse handeln, wenn Sie über eine benutzerdefinierte Subdomäne oder eine weiße Bezeichnungsdomäne verfügen.

Hinzufügen [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot; Adressen an den Filter Ihres E-Mail-Clients:

1. Allgemein kopieren [!DNL Workfront Proof] support &quot;[!UICONTROL von]&quot;E-Mail-Adresse (support@proofhq.com) und fügen Sie sie in das für Ihren E-Mail-Client angegebene Feld ein.
1. Kopieren Sie die entsprechende der folgenden [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot;E-Mail-Adressen und fügen Sie sie SEPARAT in das für Ihren E-Mail-Client angegebene Feld ein:

   * notification@support.proofhq.com , wenn Sie KEINE benutzerdefinierte Subdomain oder eine White Label-Domäne haben
   * notification@yoursubdomain.proofhq.com , wenn Sie über eine benutzerdefinierte Subdomain verfügen; Ersetzen Sie den Namen Ihrer Subdomain in dieser Adresse.
   * notification@yoursubdomain.yourdomain.com , wenn Sie eine Domäne mit weißen Bezeichnungen haben; Ersetzen Sie Ihren Subdomänennamen und Domänennamen in dieser Adresse.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
