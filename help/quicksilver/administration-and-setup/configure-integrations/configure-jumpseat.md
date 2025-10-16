---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: JumpSeat-Integration konfigurieren
description: Sie können  [!DNL JumpSeat]  mit  [!DNL Workfront] , um benutzerdefinierte, produktinterne Anleitungen zu erstellen.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Nolan, Becky
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 85ccee879fd4ba5a80b6e885458839901f83d26e
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 6%

---

# JumpSeat-Integration konfigurieren

Sie können [!DNL JumpSeat] mit [!DNL Workfront] integrieren, um benutzerdefinierte, produktinterne Anleitungen zu erstellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
    <p>Workflow Ultimate</p>
   <td> <p>Prime oder Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront-Lizenzen
   </td>
   <td>Standard
   <p>Plan</p>
   </td>
  </tr>
  </tr>
  <tr>
   <td>Produkt
   </td>
   <td>Sie müssen über einen aktiven [!DNL JumpSeat] verfügen.
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Hinzufügen und Aktivieren von [!DNL Workfront] als Anwendung in [!DNL JumpSeat]. Weitere Informationen finden Sie unter [Hinzufügen oder Löschen einer Anwendung](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>Wenn Sie Adobe Unified Experience verwenden, müssen Sie die folgende Anwendungs-URL verwenden: `.workfront.adobe.com`.



## [!DNL JumpSeat] konfigurieren

Es wird empfohlen, sowohl in der Vorschau- als auch in der Produktionsumgebung eine [!DNL JumpSeat]-Integration einzurichten.

>[!TIP]
>
>Sie müssen zwei separate [!DNL Workfront]-Anwendungen in [!DNL JumpSeat] hinzufügen und aktivieren - eine für die Vorschau und eine für die Produktion. Weitere [ finden Sie unter „Hinzufügen oder ](https://support.jumpseat.io/article/how-to-add-an-application/) einer Anwendung“.

So konfigurieren Sie die [!DNL JumpSeat]:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat]Integration]**.
1. Geben Sie Ihre **[!UICONTROL [!DNL JumpSeat]URL]** ein, die Sie auf dem Symbol Ihrer Erweiterung in [!DNL JumpSeat] finden.

>[!BEGINSHADEBOX]

**Beispiel:**

https://{mycompanyname}.jumpSeat.io

>>

>[!ENDSHADEBOX]

1. Geben Sie das **[!UICONTROL [!DNL JumpSeat]Integrations-Token]**. Sie finden diese auf der Seite **[!UICONTROL Konfiguration]** in [!DNL JumpSeat].

   **Beispiel:** $2y$10$BevsKeQ8….OYR.LurSg2U64O

1. Klicken Sie **[!UICONTROL Testkonfiguration]**.
1. Wählen Sie aus, ob die Integration **[!UICONTROL aktiv]** oder **[!UICONTROL inaktiv]** sein soll.

   >[!IMPORTANT]
   >
   >Der in Schritt 5 durchgeführte Konfigurationstest muss bestanden werden, damit die Integration aktiviert werden kann.

   ![JumpSeat-Integrationsseite](assets/jumpseat-integration-page.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

>[!TIP]
>
>Weitere Informationen zum Konfigurieren der [!DNL JumpSeat] finden Sie in der [!DNL JumpSeat] für [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
