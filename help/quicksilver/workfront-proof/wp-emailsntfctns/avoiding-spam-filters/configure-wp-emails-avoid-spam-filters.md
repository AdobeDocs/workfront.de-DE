---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Konfigurieren von [!DNL Workfront Proof] E-Mails zur Vermeidung von Spam-Filtern
description: "Der Spam-Filter Ihres E-Mail-Clients dient einem wichtigen Zweck: Sie vor lästigen und möglicherweise schädlichen Spam-E-Mails zu schützen. Wenn Sie jedoch nicht über die richtigen Einstellungen im Spam-Filter verfügen, können Sie dadurch die folgenden wichtigen [!DNL Workfront Proof] E-Mails nicht sehen: E-Mail-Benachrichtigungen, Newsletter und spezielle Nachrichten."
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1fce3d83-fdce-4ded-8e78-3468243a59e1
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# [!DNL Workfront Proof] E-Mails konfigurieren, um Spamfilter zu vermeiden

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Der Spam-Filter Ihres E-Mail-Clients dient einem wichtigen Zweck: Sie vor lästigen und möglicherweise schädlichen Spam-E-Mails zu schützen. Wenn Sie jedoch nicht über die richtigen Einstellungen im Spam-Filter verfügen, können Sie dadurch die folgenden wichtigen [!DNL Workfront Proof] E-Mails nicht sehen: E-Mail-Benachrichtigungen, Newsletter und spezielle Nachrichten.

Um sicherzustellen, dass Ihre [!DNL Workfront Proof] -E-Mails immer in Ihren Posteingang statt in Ihren Spam-Ordner geleitet werden, sollten Sie der Zulassungsliste Folgendes hinzufügen:

* [!DNL Workfront Proof] mail server: **[!DNL mx.proofhq.com]**
* [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot; E-Mail-Adressen (z. B. notification@proofhq.com)

Weitere Informationen zu URLs, die Sie zu Ihrer Zulassungsliste hinzufügen können, finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) im Artikel [Konfigurieren der Zulassungsliste Ihrer Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot; E-Mail-Adressen

Je nach E-Mail-Client-Typ müssen Sie möglicherweise eine der folgenden E-Mail-Adressen mit dem Namen [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot;hinzufügen, um zu verhindern, dass der Spam-Filter in Zukunft Ihre E-Mails an Ihren Spam-Ordner weiterleitet:

* Kontaktliste
* Ihre Liste [!UICONTROL Safe Senders]
* Einen Filter, den Sie erstellen, um E-Mails von diesen Adressen an Ihren Posteingang zu senden

Möglicherweise müssen Sie auch vorhandene [!DNL Workfront Proof] -E-Mails aus Ihrem Spam-Ordner entfernen und überprüfen, ob sich eine der &quot;[!UICONTROL von]&quot;-Adressen auf der Liste der blockierten Adressen befindet. Auf dieser Hilfeseite werden die [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot;-Adressen aufgelistet und gezeigt, wie sie in den folgenden E-Mail-Clients zum Spam-Filter hinzugefügt werden:

* [!DNL Gmail]
* [!DNL Microsoft Outlook 2003 - 2007]
* [!DNL Windows Live Hotmail]
* [!DNL Yahoo Mail]
* [!DNL Aol]

>[!NOTE]
>
>Wenn Sie Fragen zu einem hier beschriebenen Verfahren haben, überprüfen Sie bitte die Hilfe Ihres E-Mail-Clients.

Weitere Informationen finden Sie unter [Konfigurieren von Spam-Einstellungen für gängige E-Mail-Clients](../../../workfront-proof/wp-emailsntfctns/avoiding-spam-filters/configure-spam-settings-clients.md).

## Die zu kopierenden [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot;-E-Mail-Adressen

Um sicherzustellen, dass Ihre [!DNL Workfront Proof] -E-Mails Ihren Posteingang erreichen, müssen Sie zwei [!DNL Workfront Proof] -E-Mail-Adressen separat zum Spam-Filter Ihres E-Mail-Clients hinzufügen:

* Die allgemeine Supportadresse [!DNL support@proofhq.com], von der [!DNL Workfront Proof] viele E-Mail-Nachrichten sendet
* Eine Benachrichtigungsadresse, von der [!DNL Workfront Proof] dem Testversand-Ersteller und den Validierungsverantwortlichen E-Mails mit Links zum Testversand sendet. Dabei kann es sich um eine allgemeine Adresse, notification@support.proofhq.com, oder eine bestimmte Adresse handeln, wenn Sie über eine benutzerdefinierte Subdomäne oder eine weiße Bezeichnungsdomäne verfügen.

So fügen Sie die Adressen [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot;zum Filter Ihres E-Mail-Clients hinzu:

1. Kopieren Sie die allgemeine E-Mail-Adresse &quot;[!UICONTROL von]&quot; [!DNL Workfront Proof] Support &quot;&quot;(support@proofhq.com) und fügen Sie sie in das für Ihren E-Mail-Client angegebene Feld ein.
1. Kopieren Sie die entsprechende E-Mail-Adresse [!DNL Workfront Proof] &quot;[!UICONTROL von]&quot;und fügen Sie sie SEPARAT in das für Ihren E-Mail-Client angegebene Feld ein:

   * notification@support.proofhq.com , wenn Sie KEINE benutzerdefinierte Subdomain oder eine White Label-Domäne haben
   * notification@yoursubdomain.proofhq.com , wenn Sie über eine benutzerdefinierte Subdomain verfügen; ersetzen Sie den Namen Ihrer Subdomain in dieser Adresse
   * notification@yoursubdomain.yourdomain.com , wenn Sie eine weiße Beschriftungsdomäne haben; ersetzen Sie Ihren Subdomänennamen und Domänennamen in dieser Adresse.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See the relevant section below for your email client to find out where to paste in these two Workfront Proof "[!UICONTROL from]" addresses.</p>
-->
