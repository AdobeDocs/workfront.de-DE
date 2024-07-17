---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof-SPF-Datensätze
description: Workfront Proof sendet E-Mail-Benachrichtigungen von einer Workfront Proof-E-Mail-Adresse wie notification@proofing.yourdomain.com an Ihre Prüfer. Um sicherzustellen, dass die E-Mail-Server Ihrer Empfänger allen Workfront Proof-E-Mail-Benachrichtigungen vertrauen, müssen Sie einen [!DNL Sender Policy] Framework (SPF)-Datensatz für Ihre benutzerdefinierte Domäne einrichten, die mit dem [!DNL Workfront Proof] Konto verbunden ist (z. B. proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Workfront Proof-SPF-Datensätze

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] sendet E-Mail-Benachrichtigungen von einer [!DNL Workfront Proof] -E-Mail-Adresse wie notification@proofing.yourdomain.com an Ihre Validierer. Um sicherzustellen, dass die E-Mail-Server Ihrer Empfänger allen [!DNL Workfront Proof] E-Mail-Benachrichtigungen vertrauen, müssen Sie einen [!UICONTROL Sender Policy Framework] (SPF)-Datensatz für Ihre benutzerdefinierte Domäne einrichten, die mit dem [!DNL Workfront Proof]-Konto verbunden ist (z. B. **proofing.yourdomain.com**).

Um einen SPF-Datensatz einzurichten, müssen Sie den SPF-Datensatz einbeziehen, der für unsere primäre Domäne verwendet wird.

1. Fügen Sie einen **[!UICONTROL DNS-TXT]** -Eintrag für Ihre Domäne mit dem folgenden Wert hinzu:

   `v=spf1 a:mx.proofhq.com -all`

   Ihr E-Mail-Administrator oder IT-Mitarbeiter können Ihnen bei der Einrichtung helfen.

   >[!TIP]
   >
   >Sie können das kostenlose Tool unter [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) verwenden, um [!DNL Workfront] SPF-Einträge zu überprüfen.
