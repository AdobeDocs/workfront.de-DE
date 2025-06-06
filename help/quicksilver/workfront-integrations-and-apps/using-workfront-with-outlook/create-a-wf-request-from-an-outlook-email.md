---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Erstellen einer  [!DNL Adobe Workfront] -Anforderung aus einer Outlook-E-Mail
description: Sie können eine - [!DNL Adobe Workfront]  aus einer E-Mail in Outlook erstellen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4ecfe632-5f2e-4dc2-8c88-6a8229887f53
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Erstellen einer [!DNL Adobe Workfront]-Anfrage aus einer [!UICONTROL Outlook]-E-Mail

>[!IMPORTANT]
>
>[Microsoft deaktiviert die Unterstützung für veraltete Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), die derzeit vom Workfront Outlook-Add-in zur Authentifizierung verwendet werden. Diese Änderung durch Microsoft hat bereits Auswirkungen auf Kunden und wird bis Oktober 2025 schrittweise eingeführt.
>
>* **Nachdem Microsoft diese Token vollständig deaktiviert hat, funktioniert die Integration von Workfront für Microsoft Outlook nicht mehr.**
>
>Im Rahmen dieser Änderung hat Microsoft die Entscheidung getroffen, die Art und Weise zu ändern, wie Token wieder aktiviert werden. Nach dem **30. Juni** können Administratoren Token nicht mehr selbst erneut aktivieren - nur der Microsoft-Support kann Ausnahmen gewähren. **Am 1. Oktober 2025 werden alte Token für alle Mandanten deaktiviert. Ausnahmen werden nicht gewährt.**


Sie können in Outlook eine [!DNL Adobe Workfront] Anfrage aus einer E-Mail erstellen.

Wenn Sie eine [!DNL Workfront] Anfrage basierend auf einer E-Mail erstellen, ist der Inhalt der E-Mail (einschließlich Betreff und Textkörper) standardmäßig in der Anfrage enthalten.

>[!NOTE]
>
>Sie können keine [!DNL Workfront]-Anfrage aus einem freigegebenen [!UICONTROL Outlook]-Postfach erstellen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL Arbeit], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Ihr [!DNL Workfront] muss [!DNL Outlook for Office] mit [!DNL Workfront] aktivieren, bevor Sie diese Integration verwenden können.

## Erstellen einer Anfrage aus einer [!DNL Outlook] E-Mail

So erstellen Sie eine [!DNL Workfront] aus [!DNL Outlook]:

1. Wählen Sie die E-Mail aus, die die Informationen enthält, die Sie in eine [!DNL Workfront]-Anfrage aufnehmen möchten.
1. Klicken Sie auf das **[!DNL Workfront]** oben rechts in der E-Mail-Nachricht, um das Workfront-Add-in anzuzeigen.\
   Möglicherweise müssen Sie auf den Abwärtspfeil oben rechts in Ihrer E-Mail klicken, um auf das Symbol [!DNL Workfront] zuzugreifen.

1. Klicken Sie auf **[!UICONTROL Menü]**-Symbol ![o365_addin_menu2_icon.png](assets/o365-addin-menu2-icon.png), um die Liste der verfügbaren [!DNL Workfront] anzuzeigen.

1. Klicken Sie **[!UICONTROL Senden-Anfrage]**.
1. Wählen **[!UICONTROL im Feld „Anforderungstyp auswählen]** die Anforderungswarteschlange aus, an die Sie die Anforderung senden möchten.

1. Geben Sie die folgenden Informationen an:\
   Je nachdem, wie die Anfrage-Warteschlange eingerichtet wurde, können die verfügbaren Felder variieren. Eine vollständige Liste und Beschreibung der möglichen Felder finden Sie [ Artikel  [!DNL Adobe Workfront] Erstellen und senden](../../manage-work/requests/create-requests/create-submit-requests.md) .

   * **[!UICONTROL Betreff]:** Geben Sie einen Betreff für die Anfrage an. Standardmäßig wird der E-Mail-Betreff verwendet.
   * **[!UICONTROL Beschreibung]:** Geben Sie eine Beschreibung für die Anfrage an. Standardmäßig wird der Textkörper der E-Mail verwendet.
   * **[!UICONTROL Dokumente]:** Sie alle Dokumente an, die Sie in die Anfrage aufnehmen möchten. Sie können Dokumente per Drag-and-Drop anhängen oder indem Sie auf **[!UICONTROL Datei auswählen]** klicken, zu navigieren und das Dokument auszuwählen.\

     Standardmäßig sind alle an die E-Mail angehängten Dokumente in der Anfrage enthalten.

1. Klicken Sie **[!UICONTROL Senden-Anfrage]**.\
   Die Anfrage wird an [!DNL Workfront] in der angegebenen Anfragewarteschlange gesendet.

1. (Optional) Navigieren Sie zurück zu [!DNL Outlook] und wählen Sie die ursprüngliche E-Mail aus.\
   Beachten Sie oben im Add-In-Bedienfeld von [!DNL Workfront] die Bestätigung mit einem Link, dass die E-Mail als Anfrage zu Workfront hinzugefügt wurde. Die Relation enthält das Datum, an dem sie konvertiert wurde.\
