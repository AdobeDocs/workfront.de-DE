---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Anzeigen von Arbeitselementinformationen mithilfe des Adobe Workfront-Plug-ins
description: Sie können Informationen zu Projekten, Aufgaben, Problemen und Dokumenten aus Adobe Creative Cloud-Anwendungen anzeigen.
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: a53a716f-4faf-4ea7-a4fc-ad8d87634267
source-git-commit: fc3eb30cef2e17524b5cbd50219861f293a2ea9d
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 3%

---

# Anzeigen von Arbeitselementinformationen mithilfe von [!DNL Adobe Workfront] plugin

Informationen zu Projekten, Aufgaben, Problemen und Dokumenten finden Sie in den folgenden Abschnitten: [!DNL Adobe Creative Cloud] Anwendungen:

{{cc-app-list}}

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <!--<tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Sie müssen über eine [!DNL Adobe Creative Cloud] zusätzlich zu einer [!DNL Workfront] Lizenz.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte, Aufgaben oder Probleme in der [!UICONTROL Ansicht]</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zeigen Sie den Zugriff auf das Objekt an, das Sie anzeigen möchten. </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

{{cc-install-prereq}}

## Details und benutzerdefinierte Formulardaten anzeigen

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Wählen Sie das Arbeitselement aus, das Sie anzeigen möchten.

   >[!TIP]
   >
   >Verwenden Sie die **[!UICONTROL Menü]** -Symbol, um zu den übergeordneten Objekten des Arbeitselements zu gelangen.

1. Klicken Sie auf **[!UICONTROL Details]** icon ![](assets/details.png) in der Navigationsleiste, um Folgendes anzuzeigen:

   * [!UICONTROL Beschreibung]
   * [!UICONTROL Geplantes Abschlussdatum]
   * [!UICONTROL Status]
   * [!UICONTROL Zugewiesen an]
   * [!UICONTROL Projektinhaber] (Nur Projekte)
   * Benutzerdefinierte Formulardaten

## Dokumentdetails anzeigen

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Wählen Sie das Arbeitselement aus, das Sie anzeigen möchten.

   >[!TIP]
   >
   >Verwenden Sie die **[!UICONTROL Menü]** -Symbol, um zu den übergeordneten Objekten des Arbeitselements zu gelangen.

1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png) Doppelklicken Sie in der Navigationsleiste auf ein Dokument, um es anzuzeigen:

   * [!UICONTROL Beschreibung]
   * [!UICONTROL Dateityp]
   * [!UICONTROL Teststatus] (nur für Testsendungen verfügbar)
   * [!UICONTROL Version]
   * [!UICONTROL Größe]
   * Benutzerdefinierte Formulardaten

## Testversanddetails anzeigen

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Wählen Sie das Arbeitselement aus, das Sie anzeigen möchten.

   >[!TIP]
   >
   >Verwenden Sie die **[!UICONTROL Menü]** -Symbol, um zu den übergeordneten Objekten des Arbeitselements zu gelangen.

1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png) in der Navigationsleiste und doppelklicken Sie dann auf einen Testversand.

1. Klicken Sie auf das Pfeilsymbol in der oberen rechten Ecke der Miniaturansicht, um die Details zum Testversand in [!DNL Workfront].

![Öffnen Sie die Seite mit den Testversanddetails in Workfront.](assets/go-to-proof-details.png)

## Status eines Testversands anzeigen

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Wählen Sie das Arbeitselement aus, das Sie anzeigen möchten.

   >[!TIP]
   >
   >Verwenden Sie die **[!UICONTROL Menü]** -Symbol, um zu den übergeordneten Objekten des Arbeitselements zu gelangen.

1. Klicken Sie auf **[!UICONTROL Dokument]** icon ![](assets/documents.png) in der Navigationsleiste und doppelklicken Sie dann auf einen Testversand.

1. Scrollen Sie nach unten, um den aktuellen Status des Testversands anzuzeigen. Weitere Informationen zu Gesendet, Geöffnet, Kommentar, Entscheidung (SOCD) finden Sie unter [Dokumentdetails - Übersicht](/help/quicksilver/documents/managing-documents/document-details-overview.md).

![](assets/proof-status.png)

## Anzeigen von Unteraufgaben und Problemen

1. Klicken Sie auf **[!UICONTROL Menü]** Symbol oben rechts und wählen Sie **[!UICONTROL Arbeitsliste]**. Sie können auch über das Menü zu übergeordneten Objekten navigieren.

   ![](assets/go-back-to-work-list-350x314.png)

1. Wählen Sie das Arbeitselement aus, das Sie anzeigen möchten.

   >[!TIP]
   >
   >Verwenden Sie die **[!UICONTROL Menü]** -Symbol, um zu den übergeordneten Objekten des Arbeitselements zu gelangen.

1. Klicken Sie auf **[!UICONTROL Problem]** icon ![](assets/issues.png) oder **Unteraufgabe** icon ![](assets/subtasks.png).

1. Wählen Sie die Aufgabe oder das Problem aus und klicken Sie dann auf das **[!UICONTROL Details]** icon ![](assets/details.png) in der Navigationsleiste, um Folgendes anzuzeigen:

   * [!UICONTROL Geplantes Abschlussdatum]
   * [!UICONTROL Status]
   * [!UICONTROL Zugewiesen an]
   * Benutzerdefinierte Formulardaten
