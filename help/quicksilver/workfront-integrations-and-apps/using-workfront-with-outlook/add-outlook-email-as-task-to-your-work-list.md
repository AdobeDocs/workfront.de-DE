---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Outlook-E-Mail als Aufgabe zu Ihrer Auftragsliste hinzufügen
description: Sie können E [!DNL Outlook] Mails in Aufgaben  [!DNL Adobe Workfront] . Nachdem eine E-Mail konvertiert wurde, ist die Aufgabe in Ihrer Arbeitsliste im Bereich Startseite verfügbar.
author: Becky
feature: Workfront Integrations and Apps
exl-id: fcd02116-ffeb-43d3-8541-5e30e6cfdc5e
source-git-commit: d9b0e6b1c2afd17cefe190f29a072634f0b0ce50
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---

# Hinzufügen einer [!DNL Outlook] E-Mail als Aufgabe zu Ihrer Auftragsliste

>[!IMPORTANT]
>
>[Microsoft deaktiviert die Unterstützung für veraltete Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), die derzeit vom Workfront Outlook-Add-in zur Authentifizierung verwendet werden. Diese Änderung durch Microsoft hat bereits Auswirkungen auf Kunden und wird bis Oktober 2025 schrittweise eingeführt.
>
>* **Nachdem Microsoft diese Token vollständig deaktiviert hat, funktioniert die Integration von Workfront für Microsoft Outlook nicht mehr.**
>
>Im Rahmen dieser Änderung hat Microsoft die Entscheidung getroffen, die Art und Weise zu ändern, wie Token wieder aktiviert werden. Nach dem **30. Juni** können Administratoren Token nicht mehr selbst erneut aktivieren - nur der Microsoft-Support kann Ausnahmen gewähren. **Am 1. Oktober 2025 werden alte Token für alle Mandanten deaktiviert. Ausnahmen werden nicht gewährt.**


Sie können [!DNL Outlook] E-Mails in [!DNL Adobe Workfront] Aufgaben konvertieren. Nachdem eine E-Mail konvertiert wurde, ist die Aufgabe in Ihrer -Liste im Bereich [!UICONTROL Startseite] verfügbar.

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

## Hinzufügen einer [!DNL Outlook] E-Mail als Aufgabe zu Ihrer Auftragsliste

1. Wählen Sie die E-Mail in [!DNL Outlook] aus, die Sie in eine Aufgabe konvertieren möchten.
1. Klicken Sie auf das Symbol **[!DNL Workfront]** in der oberen rechten Ecke der E-Mail-Nachricht, um das [!DNL Workfront]-Add-in anzuzeigen.\
   Möglicherweise müssen Sie auf den Abwärtspfeil oben rechts in Ihrer E-Mail klicken, um auf das Symbol [!DNL Workfront] zuzugreifen.

1. Klicken Sie auf **[!UICONTROL Menü]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) Symbol, um die Liste der verfügbaren [!DNL Workfront] anzuzeigen.\


1. Klicken Sie **[!UICONTROL Zur Arbeit hinzufügen]**.\

1. Deaktivieren Sie das **[!UICONTROL Zum Projekt hinzufügen]**.
1. (Optional) Sie können die folgenden Informationen aus der E-Mail aktualisieren, bevor sie als Aufgabe gespeichert wird:

   * **[!UICONTROL Aufgabenname]:** Standardmäßig ist der Aufgabenname mit dem E-Mail-Betreff identisch. Sie können den Aufgabennamen nach Bedarf ändern.
   * **[!UICONTROL Beschreibung]:** Standardmäßig ist die Beschreibung mit dem Textkörper der E-Mail identisch. Sie können die Beschreibung nach Bedarf ändern.
   * **[!UICONTROL Anhänge]:** Alle E-Mail-Anhänge werden im Bereich [!UICONTROL Dokumente] der Aufgabe gespeichert. Sie können alle Anhänge löschen, bevor Sie die E-Mail als Aufgabe speichern.

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.\
   Die Aufgabe wird der [!UICONTROL Arbeitsliste) &#x200B;] Bereich Startseite ohne Commit-Datum hinzugefügt.

1. (Optional) Klicken Sie auf **[!UICONTROL In Workfront anzeigen]**, um die Aufgabe innerhalb des [!DNL Workfront]-Programms auf einer neuen Registerkarte anzuzeigen.

1. (Optional) Navigieren Sie zurück zu [!DNL Outlook] und wählen Sie die ursprüngliche E-Mail aus.\
   Beachten Sie oben im Add-In-Bedienfeld [!DNL Workfront] die Bestätigung mit einem Link, dass die E-Mail als Aufgabe zu Workfront hinzugefügt wurde. Die Relation enthält das Datum, an dem sie konvertiert wurde.\
