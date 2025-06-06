---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Hinzufügen einer Outlook-E-Mail zu einem Projekt als Aufgabe oder Problem
description: Sie können E-Mails in  [!DNL Adobe Workfront]  oder Probleme konvertieren. Nachdem eine E-Mail konvertiert wurde, wird die Aufgabe oder das Problem in dem Projekt angezeigt, das beim Konvertieren ausgewählt wurde.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 00755c27-9fc9-4357-a39b-4f9772484252
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 0%

---

# Hinzufügen einer [!DNL Outlook] E-Mail zu einem Projekt als Aufgabe oder Problem

>[!IMPORTANT]
>
>[Microsoft deaktiviert die Unterstützung für veraltete Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), die derzeit vom Workfront Outlook-Add-in zur Authentifizierung verwendet werden. Diese Änderung durch Microsoft hat bereits Auswirkungen auf Kunden und wird bis Oktober 2025 schrittweise eingeführt.
>
>* **Nachdem Microsoft diese Token vollständig deaktiviert hat, funktioniert die Integration von Workfront für Microsoft Outlook nicht mehr.**
>
>Im Rahmen dieser Änderung hat Microsoft die Entscheidung getroffen, die Art und Weise zu ändern, wie Token wieder aktiviert werden. Nach dem **30. Juni** können Administratoren Token nicht mehr selbst erneut aktivieren - nur der Microsoft-Support kann Ausnahmen gewähren. **Am 1. Oktober 2025 werden alte Token für alle Mandanten deaktiviert. Ausnahmen werden nicht gewährt.**


Sie können E-Mails in [!DNL Adobe Workfront] Aufgaben oder Probleme konvertieren. Nachdem eine E-Mail konvertiert wurde, wird die Aufgabe oder das Problem in dem Projekt angezeigt, das beim Konvertieren ausgewählt wurde.

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

## Hinzufügen einer [!DNL Outlook] E-Mail zu einem Projekt als Aufgabe oder Problem

1. Wählen Sie die E-Mail in [!DNL Outlook] aus, die Sie in eine Aufgabe oder ein Problem konvertieren möchten.
1. Klicken Sie auf das **[!DNL Workfront]** oben rechts in der E-Mail-Nachricht, um das Workfront-Add-in anzuzeigen.

   Möglicherweise müssen Sie auf den Abwärtspfeil oben rechts in Ihrer E-Mail klicken, um auf das Symbol [!DNL Workfront] zuzugreifen.

1. Klicken Sie auf **[!UICONTROL Menü]**-Symbol ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png), um die Liste der verfügbaren [!DNL Workfront] anzuzeigen.



1. Klicken Sie **[!UICONTROL Zur Arbeit hinzufügen]**.

1. Wählen Sie das Feld **[!UICONTROL Zu Projekt hinzufügen]** aus.
1. Geben Sie den Namen eines Projekts in das Feld **[!UICONTROL Projekt]** ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. Wählen Sie das **[!UICONTROL Aufgabe]** aus, wenn Sie dem ausgewählten Projekt eine Aufgabe hinzufügen möchten.

   Oder

   Wählen Sie das **[!UICONTROL Problem]** aus, wenn Sie dem ausgewählten Projekt ein Problem hinzufügen möchten.

1. (Optional) Geben Sie im Feld „Zuweisen zu“ an **[!UICONTROL wem diese Aufgabe oder dieses Problem zugewiesen]**.

   >[!TIP]
   >
   >Sie können die Aufgabe oder das Problem einem Team zuweisen, wenn Sie möchten, dass mehrere Personen darüber informiert sind. Wenn die E-Mail-Benachrichtigungen der Team-Mitglieder aktiviert sind, erhalten sie eine E-Mail über die neue Aufgabe oder das neue Problem, die bzw. das ihnen zugewiesen wurde.


1. (Optional) Geben Sie den **[!UICONTROL Fällig am“]**. Dies wird zum [!UICONTROL geplanten Abschlussdatum] der Aufgabe oder des Problems.
1. (Optional) Aktualisieren Sie die folgenden Informationen aus der E-Mail, bevor sie als Aufgabe oder Problem gespeichert wird (den erforderlichen Feldern wird ein Sternchen vorangestellt).

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Aufgaben- oder Problemname]</td>
        <td>Standardmäßig entspricht der Aufgabenname dem E-Mail-Betreff. Sie können den Aufgabennamen nach Bedarf ändern.</td>
        <td></td>
      </tr>
      <tr>
        <td>[!UICONTROL Beschreibung]</td>
        <td>Standardmäßig entspricht die Beschreibung dem Textkörper der E-Mail. Sie können die Beschreibung nach Bedarf ändern.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Anlagen]</td>
        <td>Alle E-Mail-Anhänge werden im Bereich [!UICONTROL -Dokumente] der Aufgabe oder des Problems gespeichert. Sie können alle Anhänge löschen, bevor Sie die E-Mail als Aufgabe oder Problem speichern.</td>
      </tr>
   </table>

1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.

   Die Aufgabe oder das Problem wird dem angegebenen Projekt hinzugefügt

1. (Optional) Klicken Sie auf **[!UICONTROL In[!DNL Workfront]]** anzeigen , um die Aufgabe innerhalb des [!DNL Workfront]-Programms auf einer neuen Registerkarte anzuzeigen.

1. (Optional) Gehen Sie zurück zu [!DNL Outlook] und wählen Sie die konvertierte E-Mail aus.

   Beachten Sie oben im Add-In-Bedienfeld [!DNL Workfront] die Bestätigung mit einem Link, dass die E-Mail zu [!DNL Workfront] als Aufgabe oder Problem hinzugefügt wurde. Die Relation enthält das Datum, an dem sie konvertiert wurde.



