---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: SPF-Einträge in Workfront Proof
description: Workfront Proof sendet E-Mail-Benachrichtigungen von einer Workfront Proof-E-Mail-Adresse wie notification@proofing.yourdomain.com an Ihre Validierungsverantwortlichen. Um sicherzustellen, dass die E-Mail-Server der Empfänger allen Workfront Proof-E-Mail-Benachrichtigungen vertrauen, müssen Sie einen [!DNL Sender Policy] Framework (SPF)-Eintrag für Ihre benutzerdefinierte Domain einrichten, die mit dem [!DNL Workfront Proof]-Konto verbunden ist (z. B. proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
TQID: 'https://experienceleague.adobe.com/LTZzs99Zzsn5dbOlu4wP1coyJAMDnnCZZ1pTTbEjT24'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 4%
---
# SPF-Einträge in Workfront Proof

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] sendet E-Mail-Benachrichtigungen von einer [!DNL Workfront Proof] E-Mail-Adresse wie notification@proofing.yourdomain.com an Ihre Validierungsverantwortlichen. Um sicherzustellen, dass die E-Mail-Server [!DNL Workfront Proof] Empfänger allen E-Mail-Benachrichtigungen vertrauen, müssen Sie einen [!UICONTROL Sender Policy Framework]&#x200B;(SPF)-Eintrag für Ihre benutzerdefinierte Domain einrichten, die mit dem [!DNL Workfront Proof]-Konto verbunden ist (z. B. **proofing.meinedomäne.com**).

Um einen SPF-Eintrag einzurichten, müssen Sie den für Ihre primäre Domain verwendeten SPF-Eintrag einbeziehen.

1. Fügen Sie einen **[!UICONTROL DNS TXT]**-Eintrag für Ihre Domain mit dem folgenden Wert hinzu:

   `v=spf1 a:mx.proofhq.com -all`

   Ihr E-Mail-Administrator oder IT-Personal kann Ihnen bei der Einrichtung helfen.

   >[!TIP]
   >
   >Sie können das kostenlose Tool unter [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) verwenden, um [!DNL Workfront] SPF-Datensätze zu überprüfen.

