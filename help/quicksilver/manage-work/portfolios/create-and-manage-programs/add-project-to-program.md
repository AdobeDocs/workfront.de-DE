---
product-area: programs;projects
navigation-topic: create and manage programs
title: Hinzufügen eines Projekts zu einem Programm
description: Sie können Ihre Projekte organisieren, indem Sie sie zu Programmen innerhalb von Portfolios hinzufügen. Sie können mehrere Projekte innerhalb eines Programms haben, aber Sie können nur ein Programm mit einem Projekt verknüpfen.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1fecc4d1-4c24-495c-98f5-824e13967369
source-git-commit: 93c36a87667097729e89a61f68cc17e9c861d547
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# Hinzufügen eines Projekts zu einem Programm

Sie können Ihre Projekte organisieren, indem Sie sie zu Programmen innerhalb von Portfolios hinzufügen. Sie können mehrere Projekte innerhalb eines Programms haben, aber Sie können nur ein Programm mit einem Projekt verknüpfen.

Sie müssen ein Portfolio und ein Programm innerhalb dieses Portfolios erstellen, bevor Sie ein Projekt zu einem Programm hinzufügen können.

Informationen zum Erstellen von Portfolios finden Sie unter [Erstellen eines Portfolios](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

Informationen zum Erstellen von Programmen finden Sie unter [Programm erstellen](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Team] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Ansicht] Zugriff auf Programme oder höher</p> <p>[!UICONTROL] Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL View] Berechtigungen für das Programm</p> <p>[!UICONTROL Verwalten] Berechtigungen für Projekte</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Projekt zu einem bestehenden Programm hinzufügen

1. Gehen Sie zu einem Programm.

   Klicken **[!UICONTROL Projekte]** im linken Bereich.

1. Klicken **[!UICONTROL Neues Projekt]** und wählen Sie eine Methode zum Hinzufügen des Projekts aus.

   >[!TIP]
   >
   >Sie können kein Projekt hinzufügen, wenn Sie die Liste der Projekte im [!UICONTROL Milestone] anzeigen.

   Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Vorhandenes Projekt]</td> 
      <td> <p>Fügen Sie ein bereits erstelltes Projekt hinzu.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Neues Projekt]</td> 
      <td> <p>Fügen Sie ein neues Projekt von Grund auf hinzu. </p> <p>Weitere Informationen zum Erstellen eines neuen Projekts finden Sie unter <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Projekt erstellen</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Projekt importieren aus [!DNL MS Project]] </td> 
      <td> <p>Fügen Sie ein Projekt hinzu, aus dem Sie zuvor exportiert haben [!DNL MS Project] und auf Ihrem Computer gespeichert haben. </p> <p>Weitere Informationen zum Erstellen eines neuen Projekts durch Importieren aus [!DNL Microsoft Project], siehe <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Importieren eines Projekts aus [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Fordern Sie an, dass das neue Projekt genehmigt wird, bevor Sie mit der Bearbeitung beginnen können.</p> <p>Informationen zum Anfordern von Projekten finden Sie unter <a href="../../../manage-work/projects/create-projects/request-project.md">Anfordern eines Projekts</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Neu aus Vorlage]</td> 
      <td> <p>Fügen Sie ein neues Projekt mithilfe einer vorhandenen Vorlage hinzu. </p> <p>Weitere Informationen zum Erstellen eines Projekts aus einer Vorlage finden Sie unter <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Erstellen eines Projekts mit einer Vorlage</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Bedingt) Wenn Sie ausgewählt haben **[!UICONTROL Vorhandenes Projekt]** führen Sie folgende Schritte aus:

   1. Im **[!UICONTROL Projekte hinzufügen]** Geben Sie den Namen des Projekts in das Feld ein und wählen Sie es aus, wenn es in der Liste angezeigt wird. Sie können mehrere Projekte gleichzeitig hinzufügen.
   1. Klicken **[!UICONTROL Projekte hinzufügen]**.**&#x200B;**&#x200B; Das Projekt wird im **[!UICONTROL Projekte]** des Programms und ist nun mit dem Programm und Portfolio verknüpft. 
