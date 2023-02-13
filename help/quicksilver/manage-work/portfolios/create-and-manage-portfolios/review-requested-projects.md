---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Überprüfen angeforderter Projekte
description: Projektanforderungen werden als Projekte mit dem Status [!UICONTROL Angefordert] in Adobe Workfront. In diesem Artikel wird beschrieben, wie Sie Projektanforderungen überprüfen.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: cf3466759a7263c446525b97dd2748ad17d0f7a6
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Überprüfen angeforderter Projekte

Wenn mehrere Projektanforderungen zur Überprüfung eingereicht werden, kann das Projekt-Management-Büro oder der Portfolio-Ausschuss zusammentreten, um die eingereichten Anfragen zu überprüfen und die Projektanforderungsgenehmigungen zu bestimmen. Projektanforderungen werden als Projekte mit dem Status [!UICONTROL Angefordert] in [!DNL Adobe Workfront].

Sie können eine Projektanforderung zur Überprüfung senden, indem Sie einen der folgenden Schritte ausführen:

* Ändern Sie den Projektstatus in **[!UICONTROL Angefordert]**.
* Führen Sie die [!UICONTROL Geschäftsfall] des Projekts erstellen und zur Genehmigung einreichen.\
   Weitere Informationen zum Abschließen eines Geschäftsszenarios für ein Projekt finden Sie unter [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Sie können die angeforderten Projekte in den folgenden Bereichen von [!DNL Adobe Workfront]:

* In einem Projektbericht
* Innerhalb eines Portfolios

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Business] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Portfolios in der [!UICONTROL Ansicht] oder höher</p> <p>[!UICONTROL] Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL View] Berechtigungen oder höher für das Portfolio</p> <p>[!UICONTROL Verwalten] Berechtigungen für Projekte zum Aktualisieren ihres Status</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Überprüfen angeforderter Projekte in einem Projektbericht

Sie können einen Bericht für Projekte erstellen, um zu sehen, welche Projekte den Status haben [!UICONTROL Angefordert].

Weitere Informationen zum Genehmigen von Projektanforderungen durch Erstellen eines Projektberichts finden Sie im Abschnitt [[!UICONTROL Genehmigen des Geschäftsszenarios durch Erstellen eines Projektberichts]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) Abschnitt in [Geschäftsfall genehmigen](../../../manage-work/projects/define-a-business-case/approve-business-case.md). 

## Überprüfen angeforderter Projekte in einem Portfolio

1. Gehen Sie zum Portfolio, dessen angeforderte Projekte Sie überprüfen möchten.
1. Klicken Sie auf &#x200B;**[!UICONTROL Projekte]** im linken Bereich
1. Aus dem **[!UICONTROL Filter]** Dropdown-Menü auswählen **[!UICONTROL Angefordert]**.

   Nur Projekte mit dem Status **[!UICONTROL Angefordert]** in der Liste angezeigt.

   >[!TIP]
   >
   > Zusätzlich zum Status von **[!UICONTROL Angefordert]**, müssen Projekte mit dem ausgewählten Portfolio verknüpft sein, damit sie in dieser Liste angezeigt werden können.

1. Klicken Sie in der Liste auf den Namen eines Projekts, um es zu öffnen.
1. Klicken **[!UICONTROL Projektdetails]** im linken Bereich.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken **[!UICONTROL Geschäftsfall]** Klicken Sie auf **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]** im [!UICONTROL Zusammenfassung von Geschäftsfällen] -Bereich, um den Geschäftsfall zu genehmigen oder abzulehnen.

      ![approve_or_reject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

      Der Projektstatus wird in **[!UICONTROL Genehmigt]** wenn der Geschäftsfall genehmigt wurde.

      Der Projektstatus wird in **[!UICONTROL Zurückgewiesen]** wenn der Geschäftsfall abgelehnt wird.

      >[!NOTE]
      Es gibt keine Benachrichtigungen, die den Benutzer, der die Genehmigung des Geschäftsfalls eingereicht hat, darauf hinweisen, ob seine Projektanfrage genehmigt oder abgelehnt wurde. 

      Oder

   * Ändern Sie den Status des Projekts in einen anderen Status im **[!UICONTROL Status]** Dropdown-Menü.

      ![](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)
 

 
