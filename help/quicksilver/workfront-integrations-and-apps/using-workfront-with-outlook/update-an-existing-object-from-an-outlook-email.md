---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Vorhandenes Objekt von einer Outlook-E-Mail aktualisieren
description: Sie können ein vorhandenes Projekt, eine Aufgabe oder ein Problem mit Informationen aus einer Outlook-E-Mail aktualisieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: 16acba0f1981b75ca141a36d096fb6f5d37c40d1
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Vorhandenes Objekt von einem [!DNL Outlook] email

Sie können ein vorhandenes Projekt, eine Aufgabe oder ein Problem mit Informationen aus einem [!DNL Outlook] E-Mail.

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
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work], [!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Ihre [!DNL Workfront] Administrator muss [!DNL Outlook for Office] mit [!DNL Workfront] bevor Sie diese Integration verwenden können.

## Vorhandenes Objekt von einem [!DNL Outlook] email

1. In [!DNL Outlook]auswählen die E-Mail, die die Informationen enthält, die Sie in eine [!DNL Adobe Workfront update].
1. Klicken Sie auf **[!DNL Workfront]** in der oberen rechten Ecke der E-Mail-Nachricht ein, um das Workfront-Add-In anzuzeigen.\
   Möglicherweise müssen Sie rechts oben in Ihrer E-Mail auf den Pfeil nach unten klicken, um auf die Variable [!DNL Workfront] Symbol.

1. Klicken Sie auf **[!UICONTROL Menü]** icon ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) , um die Liste der verfügbaren [!DNL Workfront] options.\


1. Klicken **[!UICONTROL Aktualisieren] in Workfront**.\
   Sie können die folgenden Informationen aus der E-Mail aktualisieren, bevor sie als Aufgabe gespeichert wird:

   * **[!UICONTROL Typ]**: Wählen Sie den Typ des zu aktualisierenden Objekts aus. Sie können **[!UICONTROL Projekt]**, **[!UICONTROL Aufgabe]** oder **[!UICONTROL Problem]**. Das ausgewählte Objekt bestimmt die Ergebnisse, die im **[!UICONTROL Name]** unten. Wenn Sie sich bezüglich des Objekttyps nicht sicher sind, wählen Sie **[!UICONTROL Alle]** , um gleichzeitig nach Projekten, Aufgaben und Problemen zu suchen.

   * **[!UICONTROL Name]**: Beginnen Sie mit der Eingabe des Namens des Projekts, der Aufgabe oder des Problems, das Sie aktualisieren möchten. Klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
   * **[!UICONTROL Aktualisieren]**: Standardmäßig entspricht die Aktualisierung dem E-Mail-Textkörper. Sie können die Aktualisierung nach Bedarf ändern.\

      Diese [!UICONTROL update] wird als Aktualisierungsstatus in Workfront angezeigt.

   * **[!UICONTROL Anhänge]**: Alle E-Mail-Anhänge werden im [!UICONTROL Dokumente] -Bereich der Aufgabe. Sie können alle Anlagen löschen, bevor Sie die Aktualisierung senden.

1. (Optional) Klicken Sie auf **[!UICONTROL Andere einschließen]**, geben Sie den Namen der Benutzer ein, die Sie in die Aktualisierung aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.\
   Wiederholen Sie diesen Vorgang, um weitere Benutzer einzuschließen, und klicken Sie dann auf **[!UICONTROL Fertig]**.\
   Standardmäßig erhält der Benutzer, auf den Sie antworten, eine Benachrichtigung, unabhängig davon, ob Sie sie einschließen.\

1. (Optional) Klicken Sie auf die **[!UICONTROL Sperren]** -Symbol, um diese Aktualisierung auf Benutzer in Ihrem Unternehmen zu beschränken. Wenn die Aktualisierung gesperrt ist, können Benutzer außerhalb Ihres Unternehmens die Aktualisierung nicht sehen.

   * **[!UICONTROL Entsperrt]:** Jeder Benutzer mit Zugriff auf das Projekt, die Aufgabe oder das Problem, in dem sich die Aktualisierung befindet, kann die Aktualisierung anzeigen.\

      Standardmäßig ist die Aktualisierung entsperrt.\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL Gesperrt]:** Nur Benutzer in Ihrem Unternehmen können die Aktualisierung anzeigen.\

      ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. Klicken **[!UICONTROL Aktualisieren]**.
1. (Optional) Klicken Sie auf **[!UICONTROL Anzeigen in Workfront]** , um das aktualisierte Element mit der [!DNL Workfront] Integration [!UICONTROL Outlook].
