---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: JumpSeat-Integration konfigurieren
description: Sie können [!DNL JumpSeat] in [!DNL Workfront]  integrieren, um benutzerdefinierte, produktinterne Anleitungen zu erstellen.
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

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über einen aktiven [!DNL JumpSeat]-Plan verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p> Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen zu [!DNL Workfront] -Administratoren finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Fügen Sie [!DNL Workfront] als Anwendung in [!DNL JumpSeat] hinzu und aktivieren Sie es. Weitere Informationen finden Sie unter [Hinzufügen oder Löschen einer Anwendung](https://support.jumpseat.io/article/how-to-add-an-application/).

>[!IMPORTANT]
>
>Wenn Sie das Adobe Unified Experience verwenden, müssen Sie die folgende Anwendungs-URL verwenden: `.workfront.adobe.com`.



## Konfigurieren der [!DNL JumpSeat] -Integration

Es wird empfohlen, eine [!DNL JumpSeat] -Integration sowohl in der Vorschau- als auch in der Produktionsumgebung einzurichten.

>[!TIP]
>
>Sie müssen zwei separate [!DNL Workfront]-Anwendungen in [!DNL JumpSeat] hinzufügen und aktivieren - eine für die Vorschau und eine für die Produktion. Weitere Informationen finden Sie unter [Hinzufügen oder Löschen einer Anwendung](https://support.jumpseat.io/article/how-to-add-an-application/) .

So konfigurieren Sie die [!DNL JumpSeat] -Integration:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL System]** > **[!UICONTROL [!DNL JumpSeat]Integration]**.
1. Geben Sie Ihre **[!UICONTROL [!DNL JumpSeat]URL]** ein, die Sie auf Ihrem Erweiterungssymbol in [!DNL JumpSeat] finden.

>[!BEGINSHADEBOX]

**Beispiel:**

https://{mycompanyname}.jumpsitz.io

>>

>[!ENDSHADEBOX]

1. Geben Sie das Integrations-Token **[!UICONTROL [!DNL JumpSeat]ein.]** Sie finden dies auf der Seite **[!UICONTROL Konfiguration]** in [!DNL JumpSeat].

   **Beispiel:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. Klicken Sie auf **[!UICONTROL Testkonfiguration]**.
1. Wählen Sie aus, ob die Integration **[!UICONTROL aktiv]** oder **[!UICONTROL inaktiv]** sein soll.

   >[!IMPORTANT]
   >
   >Der in Schritt 5 ausgeführte Konfigurationstest muss bestanden werden, damit die Integration aktiviert werden kann.

   ![JumpSeat-Integrationsseite](assets/jumpseat-integration-page.png)

1. Klicken Sie auf **[!UICONTROL Speichern]**.

>[!TIP]
>
>Weitere Informationen zum Konfigurieren der [!DNL JumpSeat] -Integration finden Sie in der [!DNL JumpSeat] -Dokumentation für [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
