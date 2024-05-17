---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: Konfigurieren der JumpSeat-Integration
description: Sie können [!DNL JumpSeat] mit [!DNL Workfront] , um benutzerdefinierte, produktinterne Anleitungen zu erstellen.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Konfigurieren der JumpSeat-Integration

Sie können [!DNL JumpSeat] mit [!DNL Workfront] , um benutzerdefinierte, produktinterne Anleitungen zu erstellen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Produkt</strong></td> 
   <td>Sie müssen über eine aktive [!DNL JumpSeat] Plan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p> Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Hinzufügen und Aktivieren [!DNL Workfront] als Anwendung in [!DNL JumpSeat]. Weitere Informationen finden Sie unter [Hinzufügen oder Löschen einer Anwendung](https://support.jumpseat.io/article/how-to-add-an-application/).

## Konfigurieren Sie die [!DNL JumpSeat] Integration

Es wird empfohlen, eine [!DNL JumpSeat] Integration in Ihre Vorschau- und Produktionsumgebungen.

>[!TIP]
>
>Sie müssen zwei separate [!DNL Workfront] Anwendungen in [!DNL JumpSeat]- eine für die Vorschau und eine für die Produktion. Siehe [Hinzufügen oder Löschen einer Anwendung](https://support.jumpseat.io/article/how-to-add-an-application/) für weitere Informationen.

So konfigurieren Sie die [!DNL JumpSeat] Integration:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]**.
1. Klicken Sie im linken Bereich auf **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat]Integration]**.
1. Geben Sie Ihre **[!UICONTROL [!DNL JumpSeat]URL]**, die Sie auf dem Erweiterungssymbol in [!DNL JumpSeat].

   **Beispiel:** [!DNL https]://{mycompanyname}.jumpsitz.io

1. Geben Sie die **[!UICONTROL [!DNL JumpSeat]Integrationstoken]**. Sie finden dies auf der **[!UICONTROL Konfiguration]** Seite in [!DNL JumpSeat].

   **Beispiel:** $2y$10$BevsKeQ8...OYR.LurSg2U64O

1. Klicks **[!UICONTROL Testen der Konfiguration]**.
1. Entscheiden Sie, ob die Integration **[!UICONTROL Aktiv]** oder **[!UICONTROL Inaaktiv]**.

   >[!IMPORTANT]
   >
   >Der in Schritt 5 ausgeführte Konfigurationstest muss bestanden werden, damit die Integration aktiviert werden kann.

   ![JumpSeat-Integrationsseite](assets/jumpseat-integration-page.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

>[!TIP]
>
>Weitere Informationen zur Konfiguration der [!DNL JumpSeat] -Integration, siehe [!DNL JumpSeat] Dokumentation für [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
