---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Vermerken von Arbeitselementen als abgeschlossen mithilfe des Adobe Workfront-Plug-ins
description: Sie können in Adobe Creative Cloud-Programmen bleiben und Ihre Arbeit in Adobe Workfront nahtlos abschließen.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d94a2b10-51d5-4995-b7b3-793d7911fca9
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Arbeitselemente mit dem Plug-in &quot;[!DNL Adobe Workfront]&quot; als abgeschlossen markieren

Sie können in den folgenden [!DNL Adobe Creative Cloud] Anwendungen bleiben und Ihre Arbeit nahtlos [!DNL Adobe Workfront] mit dem Plug-in abschließen:

{{cc-app-list}}

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <!-- <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> 
   <p>Standard</p>
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> -->
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td>Sie müssen zusätzlich zu einer [!DNL Adobe Creative Cloud] über eine [!DNL Workfront]-Lizenz verfügen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf [!UICONTROL -Dokumente] bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL View] Zugriff oder höher auf das Objekt, in das Sie ein Dokument hochladen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Voraussetzungen

{{cc-install-prereq}}

## Fertigstellen eines Arbeitselements

1. Klicken Sie **[!UICONTROL oben rechts auf]** Menü“ und wählen Sie dann **[!UICONTROL Arbeitsliste]** aus. Sie können auch das Menü verwenden, um zu übergeordneten Objekten zu navigieren.

   ![Zurück zur Arbeitsliste](assets/go-back-to-work-list-350x314.png)

1. Wählen Sie in **[!UICONTROL Arbeitsliste]** die Aufgabe oder das Problem aus, die bzw. das Sie als abgeschlossen markieren möchten.
1. Klicken Sie **[!UICONTROL Fertig]**.  Wenn Sie der einzige Benutzer sind, der dieser Aufgabe oder diesem Problem zugewiesen ist, wird das Element [!UICONTROL Abgeschlossen] oder [!UICONTROL Gelöst] in [!DNL Workfront] markiert.
1. (Bedingt) Wenn dieser Aufgabe oder diesem Problem mehrere Benutzer zugewiesen sind, wird durch Klicken auf [!UICONTROL Fertig] eine Dropdown-Liste geöffnet. Anschließend können Sie:

   Klicken Sie **[!UICONTROL Fertig mit meinem Teil]**, wenn andere Benutzer ebenfalls ihre Arbeit erledigen müssen, damit die Aufgabe oder das Problem abgeschlossen ist.

   Oder

   Klicken Sie **[!UICONTROL Abschließen]** (für Aufgaben) oder **[!UICONTROL Gelöst]** (für Probleme), wenn keine weitere Arbeit an der Aufgabe oder dem Problem erforderlich ist. Dadurch wird das Element [!UICONTROL Abgeschlossen] oder [!UICONTROL Aufgelöst] in [!DNL Workfront] markiert.

   >[!NOTE]
   >
   >Wenn das Arbeitselement Vorgänger hat, ist die Schaltfläche Fertig grau, bis diese Vorgänger als abgeschlossen markiert sind. Um Vorgänger in [!DNL Workfront] anzuzeigen, klicken Sie auf den Aufgabennamen.
   >![Navigieren Sie zu Workfront](assets/navigate-to-workfront.png)

<!-- I dont think we need this one ![Complete work](assets/complete-work-350x529.png) -->
