---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Angeforderte Projekte überprüfen
description: Projektanfragen werden in Adobe Workfront als Projekte mit dem Status [!UICONTROL Angefordert] angezeigt. In diesem Artikel wird beschrieben, wie Sie Projektanfragen überprüfen können.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1acfb885-0da3-495d-ba66-e80e339e90de
source-git-commit: 7fef704355fad677f2bdf40e630ea0146a9e1d58
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Angeforderte Projekte überprüfen

<!--Audited: 10/2025-->

Wenn mehrere Projektanträge zur Prüfung eingereicht werden, kann das Projektmanagementbüro oder der Portfoliokomitee zusammentreten, um eingereichte Anträge zu prüfen und die Genehmigungen für Projektanträge zu bestimmen. Projektanfragen werden in [!UICONTROL  als Projekte mit dem Status ]Angefordert[!DNL Adobe Workfront] angezeigt.

Sie können eine Projektanfrage zur Überprüfung senden, indem Sie einen der folgenden Schritte ausführen:

* Ändern Sie den Projektstatus in **[!UICONTROL angefordert]**.
* Schließen Sie den [!UICONTROL Business Case] des Projekts ab und reichen Sie ihn zur Genehmigung ein.\
   Weitere Informationen zum Abschließen eines Business Case für ein Projekt finden Sie unter [Erstellen eines Business Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Sie können angeforderte Projekte in den folgenden [!DNL Adobe Workfront] überprüfen:

* In einem Projektbericht
* Innerhalb eines Portfolios

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>[!UICONTROL Standard] </p> 
   <p>[!UICONTROL-Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Portfolios über [!UICONTROL View] oder höher</p> <p>[!UICONTROL Bearbeiten] Zugriff auf Projekte</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Anzeigen]-Berechtigungen oder höher für das Portfolio</p> <p>[!UICONTROL Manage]-Berechtigungen für die Projekte, um ihren Status zu aktualisieren</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td><p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL View] access or higher to Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL View] permissions or higher on the portfolio</p> <p>[!UICONTROL Manage] permissions on the projects to update their status</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Überprüfen angeforderter Projekte in einem Projektbericht

Sie können einen Bericht für Projekte erstellen, um zu sehen, welche Projekte den Status &quot;[!UICONTROL &quot; ].

Weitere Informationen zur Genehmigung von Projektanfragen durch Erstellen eines Projektberichts finden Sie [[!UICONTROL  Abschnitt „Genehmigen des Business Case durch Erstellen ]](../../../manage-work/projects/define-a-business-case/approve-business-case.md#build-a-report) Projektberichts“ in [Genehmigen eines Business Case](../../../manage-work/projects/define-a-business-case/approve-business-case.md).

## Angeforderte Projekte innerhalb eines Portfolios überprüfen

1. Gehen Sie zum Portfolio, dessen angeforderte Projekte Sie überprüfen möchten.
1. Klicken Sie **[!UICONTROL linken]** auf „Projekte“
1. Wählen Sie **[!UICONTROL Dropdown]** Menü „Filter“ die Option **[!UICONTROL Angefordert]** aus.

   Nur Projekte mit dem Status **[!UICONTROL Angefordert]** werden in der Liste angezeigt.

   >[!TIP]
   >
   > Projekte haben nicht nur den Status **[!UICONTROL Angefordert]**, sondern müssen auch mit dem ausgewählten Portfolio verknüpft sein, damit sie in dieser Liste angezeigt werden.

1. Klicken Sie auf den Namen eines Projekts in der Liste, um es zu öffnen.
1. Klicken Sie **[!UICONTROL linken]** auf „Projektdetails“.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie **[!UICONTROL Business Case]** und klicken Sie dann im Bereich **[!UICONTROL Business Case-Zusammenfassung]** auf **[!UICONTROL Genehmigen]** oder [!UICONTROL Ablehnen], um den Business Case zu genehmigen oder abzulehnen.

     ![approve_or_ject_business_case.png](assets/approve-or-reject-business-case-350x563.png)

     Der Projektstatus wird in &quot;**[!UICONTROL &quot; geändert]** wenn der Business Case genehmigt wurde.

     Der Projektstatus ändert sich in **[!UICONTROL Abgelehnt]** wenn der Business-Case abgelehnt wird.

     >[!NOTE]
     >
     >Es gibt keine Benachrichtigungen, die den Benutzer, der die Genehmigung des Business-Case eingereicht hat, darüber informieren, ob seine Projektanforderung genehmigt oder abgelehnt wurde.

     Oder

   * Ändern Sie den Status des Projekts in einen beliebigen anderen Status **[!UICONTROL Dropdown]** Menü „Status“.

     ![Ändern des Projektstatus aus der Dropdown-Liste](assets/project-status-change-from-drop-down-in-header-nwe-350x294.png)



