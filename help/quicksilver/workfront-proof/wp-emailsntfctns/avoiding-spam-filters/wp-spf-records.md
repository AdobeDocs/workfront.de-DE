---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: Workfront-SPF-Testdatensätze
description: Workfront Testversand sendet E-Mail-Benachrichtigungen von einer Testversand-E-Mail-Adresse wie notification@proofing.yourdomain.com an Ihre Prüfer. Um sicherzustellen, dass die E-Mail-Server Ihrer Empfänger allen Workfront-Testversand-E-Mail-Benachrichtigungen vertrauen, müssen Sie eine [!DNL Sender Policy] Framework-Datensatz (SPF) für Ihre benutzerdefinierte Domäne, die mit dem [!DNL Workfront Proof] -Konto (z. B. proofing.yourdomain.com).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 5295d451-2ad2-4835-9200-f10d4e6286a2
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Workfront-SPF-Testdatensätze

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] sendet E-Mail-Benachrichtigungen von einer [!DNL Workfront Proof] E-Mail-Adresse wie notification@proofing.yourdomain.com. Um sicherzustellen, dass die E-Mail-Server Ihrer Empfänger allen [!DNL Workfront Proof] E-Mail-Benachrichtigungen erstellen, müssen Sie eine [!UICONTROL Framework für Absenderrichtlinien] (SPF)-Datensatz für Ihre benutzerdefinierte Domäne, die mit der [!DNL Workfront Proof] -Konto (z. B. **proofing.yourdomain.com**).

Um einen SPF-Datensatz einzurichten, müssen Sie den SPF-Datensatz einbeziehen, der für unsere primäre Domäne verwendet wird.

1. Hinzufügen einer **[!UICONTROL DNS TXT]** -Eintrag für Ihre Domäne mit dem folgenden Wert:

   `v=spf1 a:mx.proofhq.com -all`

   Ihr E-Mail-Administrator oder IT-Mitarbeiter können Ihnen bei der Einrichtung helfen.

   >[!TIP]
   >
   >Sie können das kostenlose Tool unter [[!DNL https://mxtoolbox.com/spf.aspx]](https://mxtoolbox.com/spf.aspx) zur Überprüfung [!DNL Workfront] SPF-Einträge.
