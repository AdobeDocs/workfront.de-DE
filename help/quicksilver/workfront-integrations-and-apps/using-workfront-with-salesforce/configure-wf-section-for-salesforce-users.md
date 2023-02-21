---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Konfigurieren Sie die [!DNL Adobe Workfront] Abschnitt für [!DNL Salesforce] Benutzer
description: Nach der Installation [!DNL Adobe Workfront] für Salesforce als [!DNL Workfront] Administrator können Sie sie Ihren Benutzern zur Verfügung stellen, indem Sie sie in einem neuen Abschnitt zu ihren Opportunity- und Account-Seitenlayouts in Salesforce hinzufügen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# Konfigurieren Sie die [!DNL Adobe Workfront] Abschnitt für [!DNL Salesforce] Benutzer

A [!UICONTROL Pro] [!DNL Workfront] Für die Verwendung dieser Funktion ist ein Plan erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [[!DNL Workfront] Pläne.](https://www.workfront.com/plans)

Nach der Installation [!DNL Adobe Workfront] für [!DNL Salesforce] as a [!DNL Workfront] Administrator können Sie sie Ihren Benutzern zur Verfügung stellen, indem Sie sie in einem neuen Abschnitt zu ihrer [!UICONTROL Chancen] und [!UICONTROL Konto]
Seitenlayouts in [!UICONTROL Salesforce].

Informationen zur Installation [!DNL Workfront for Salesforce], siehe [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Für Benutzer, die [!DNL Workfront] in beiden [!DNL Classic] und [!DNL Lightning Experience] Frameworks, müssen Sie die [!DNL WorkfrontOpportunities] und [!DNL WorkfrontAccounts] [!UICONTROL Visualkraft] Seiten [!UICONTROL Chancen] und [!UICONTROL Konten] Seitenlayouts.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

* Sie müssen über eine [!DNL Salesforce] -Instanz mit Zugriff auf ein Systemadministratorkonto.
* Sie müssen über eine [!DNL Workfront] -Instanz mit Zugriff auf ein Systemadministratorkonto.

## Konfigurieren Sie die [!DNL Workfront] im Abschnitt [!DNL Salesforce Classic] Framework

1. Anmelden bei [!DNL Salesforce] als Workfront-Administrator.
1. Klicken **[!UICONTROL Einrichtung].**
1. Im **[!UICONTROL Build]** Abschnitt erweitern **[!UICONTROL Anpassen].**

1. Erweitern **[!UICONTROL Chancen]** Klicken Sie auf **[!UICONTROL Seitenlayouts]** , um [!DNL Workfront] auf eine Gelegenheit klicken.

   Oder

   Erweitern **[!UICONTROL Konten]** Klicken Sie auf **[!UICONTROL Seitenlayouts]** , um [!DNL Workfront] auf ein Konto hinzu.

1. Klicken **[!UICONTROL Bearbeiten]** in einem vorhandenen Layout.

   Oder

   Klicken **[!UICONTROL Neu]** um ein neues Layout hinzuzufügen.

1. (Optional) Ziehen Sie die **[!UICONTROL Abschnitt]** in das Layout ein und legen Sie es an der gewünschten Position ab.\

1. (Optional) Geben Sie einen Namen für den neuen Abschnitt an.

   Es wird empfohlen, diesen Abschnitt zu benennen. **[!DNL Workfront]**.

1. (Optional) Geben Sie die gewünschte **[!UICONTROL Layout]** und **[!UICONTROL Tab-Schlüssel-Reihenfolge]** für den neuen Abschnitt.

   Es wird empfohlen, **[!UICONTROL 1-Spalte]** Layout für [!DNL Workfront] Abschnitt.

1. Klicken **[!UICONTROL OK]**.
1. Im **[!UICONTROL Layout]** Bereich, klicken Sie **[!UICONTROL Visualforce-Seiten].**

1. Ziehen Sie die **[!UICONTROL WorkfrontOpportunities]** -Komponente in den neuen Abschnitt im **[!UICONTROL Chancen]** Layout.

   Oder

   Ziehen Sie die **[!UICONTROL WorkfrontAccounts]** -Komponente in den neuen Abschnitt im  **[!UICONTROL Konto]** Layout.\

1. Klicken Sie auf **[!UICONTROL Eigenschaften]** rechts oben in der neu hinzugefügten Komponente.\

1. Um eine optimale Anzeige zu erzielen, geben Sie die folgenden Eigenschaften für die [!DNL Workfront Visualforce] Seite:

   * **[!UICONTROL Breite (in Pixel oder %)]**: 100 %
   * **[!UICONTROL Höhe (in Pixel)]**: 600
   * Auswählen **[!UICONTROL Bildlaufleisten anzeigen]**.

1. Klicken **[!UICONTROL OK]**.
1. Klicken **[!UICONTROL Speichern]** um Ihr Layout zu speichern.

   Alle Benutzer, denen dieses Layout zugewiesen wurde, können jetzt die [!DNL Workfront] Abschnitt [!UICONTROL Chancen] oder [!UICONTROL Konten] Objekte.

   Benutzer sehen eine [!DNL Workfront] Anmeldebildschirm auf [!DNL Workfront] Abschnitt. Wenn sie keine [!DNL Workfront] -Konto verwenden, können sie den Abschnitt reduzieren, ihn jedoch nicht aus ihrem Layout entfernen.

## Konfigurieren Sie die [!DNL Workfront] im Abschnitt [!DNL Salesforce Lightning Experience] Framework

Sie können die [!DNL Workfront] -Abschnitt in das Layout eines [!DNL Salesforce] [!UICONTROL Chancen] oder Konto im [!DNL Salesforce Lightning Experience] -Framework durch Zugriff auf [!UICONTROL Einrichtung] -Bereich oder von einem Konto oder [!UICONTROL Chancen] -Objekt.

* [Konfigurieren Sie die [!DNL Workfront] im Abschnitt [!UICONTROL Einrichtung] level](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Konfigurieren Sie die [!DNL Workfront] Abschnitt auf Opportunity- oder Kontoebene](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Konfigurieren Sie die [!DNL Workfront] im Abschnitt [!UICONTROL Einrichtung] level {#configure-the-workfront-section-at-the-setup-level}

1. Anmelden [!DNL Salesforce] als Systemadministrator.
1. Klicken Sie auf **[!UICONTROL Einrichtung]** und klicken Sie auf **[!UICONTROL Einrichtung]**.

1. Erweitern **[!UICONTROL Objekt und Felder]** Klicken Sie auf **[!UICONTROL Object Manager]**.

1. Klicken **[!UICONTROL Chancen]** um das Layout einer Gelegenheit anzupassen.

   Oder

   Klicken **[!UICONTROL Konto]** , um das Layout eines Kontos anzupassen.

1. Klicken **[!UICONTROL Seitenlayouts]**.
1. Klicken Sie auf den Namen eines vorhandenen Seitenlayouts, um es zu bearbeiten.

   Oder

   Klicken **[!UICONTROL Neu]** um ein neues Seitenlayout zu erstellen.

1. Fahren Sie mit [Konfigurieren Sie die [!DNL Workfront] Abschnitt auf Opportunity- oder Kontoebene](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) unten.

### Konfigurieren Sie die [!DNL Workfront] Abschnitt auf Opportunity- oder Kontoebene {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Anmelden bei [!DNL Salesforce] als Systemadministrator.
1. Gehen Sie zu einer **[!UICONTROL Chancen]** oder **[!UICONTROL Konto]**.

1. Klicken Sie auf **[!UICONTROL Einrichtung]** und klicken Sie auf **[!UICONTROL Seite bearbeiten]**.\

1. Erweitern Sie die **[!UICONTROL Benutzerverwaltet]** Abschnitt.
1. Ziehen Sie die **[!DNL Workfront]** -Komponente in [!UICONTROL Chancen] oder Kontoseite.

   Es wird empfohlen, die gesamte Seitenbreite für die [!DNL Workfront] anstatt einer der Spalten des Layouts.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Alle Benutzer, denen dieses Layout zugewiesen wurde, können jetzt die [!DNL Workfront] Abschnitt [!UICONTROL Chancen] oder [!UICONTROL Konten] Objekte.

   >[!NOTE]
   >
   >Benutzer sehen eine [!DNL Workfront] Anmeldebildschirm auf [!DNL Workfront] Abschnitt. Wenn sie keine [!DNL Workfront] -Konto verwenden, können sie den Abschnitt reduzieren, ihn jedoch nicht aus ihrem Layout entfernen. Benutzer können sich mit der von Ihnen aktivierten Authentifizierungsmethode anmelden: Verbesserte Authentifizierung oder Ihre SAML-URL (Security Assertion Markup Language).

