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
source-git-commit: 01b7eb79028eb3fe47f988a31cb62ace31bba3f1
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 4%

---

# JumpSeat-Integration konfigurieren

Sie können [!DNL JumpSeat] mit [!DNL Workfront] integrieren, um benutzerdefinierte, produktinterne Anleitungen zu erstellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td>[!UICONTROL -Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über einen aktiven [!DNL JumpSeat] verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p> Sie müssen [!DNL Workfront] sein. Informationen zu [!DNL Workfront] finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Hinzufügen und Aktivieren von [!DNL Workfront] als Anwendung in [!DNL JumpSeat]. Weitere Informationen finden Sie unter [Hinzufügen oder Löschen einer Anwendung](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>Wenn Sie sich auf der Adobe Unified Experience befinden, müssen Sie die folgende Anwendungs-URL verwenden: `.workfront.adobe.com`.



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

&#x200B;>>

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
