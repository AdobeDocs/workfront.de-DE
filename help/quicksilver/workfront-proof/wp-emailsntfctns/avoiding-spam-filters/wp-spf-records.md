---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront Proof SPF-Datensätze
description: Workfront Proof sendet E-Mail-Benachrichtigungen von einer Workfront Proof-E-Mail-Adresse wie notification@proofing.yourdomain.com an Ihre Validierungsverantwortlichen. Um sicherzustellen, dass die E-Mail-Server der Empfängerinnen und Empfänger allen Workfront Proof-E-Mail-Benachrichtigungen vertrauen, müssen Sie einen  [!DNL Sender Policy] Framework (SPF)-Eintrag für Ihre benutzerdefinierte Domain einrichten, die mit dem - [!DNL Workfront Proof]  verbunden ist (z. B. proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 0%

---

# Workfront Proof SPF-Datensätze

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] sendet E-Mail-Benachrichtigungen von einer [!DNL Workfront Proof] E-Mail-Adresse wie notification@proofing.yourdomain.com an Ihre Validierungsverantwortlichen. Um sicherzustellen, dass die E-Mail-Server [!DNL Workfront Proof] Empfänger allen E-Mail-Benachrichtigungen vertrauen, müssen Sie einen [!UICONTROL Sender Policy Framework](SPF)-Eintrag für Ihre benutzerdefinierte Domain einrichten, die mit dem [!DNL Workfront Proof]-Konto verbunden ist (z. B. **proofing.meinedomäne.com**).

Um einen SPF-Eintrag einzurichten, müssen Sie den für Ihre primäre Domain verwendeten SPF-Eintrag einbeziehen.

1. Fügen Sie einen **[!UICONTROL DNS TXT]**-Eintrag für Ihre Domain mit dem folgenden Wert hinzu:

   `v=spf1 a:mx.proofhq.com -all`

   Ihr E-Mail-Administrator oder IT-Personal kann Ihnen bei der Einrichtung helfen.

   >[!TIP]
   >
   >Sie können das kostenlose Tool unter [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) verwenden, um [!DNL Workfront] SPF-Datensätze zu überprüfen.
