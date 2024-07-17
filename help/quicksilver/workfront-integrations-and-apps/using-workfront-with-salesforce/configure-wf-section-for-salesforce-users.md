---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: ' [!DNL Adobe Workfront] -Abschnitt für  [!DNL Salesforce] Benutzer konfigurieren'
description: Nachdem Sie [!DNL Adobe Workfront] für Salesforce als [!DNL Workfront] Administrator installiert haben, können Sie es Ihren Benutzern zur Verfügung stellen, indem Sie es in einem neuen Abschnitt zu ihren Opportunity- und Account-Seitenlayouts in Salesforce hinzufügen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: ad2fc27db2a19ea231e925d5991dbef27ea48030
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# Konfigurieren des Bereichs [!DNL Adobe Workfront] für [!DNL Salesforce] Benutzer

Für die Verwendung dieser Funktion ist ein [!UICONTROL Pro] [!DNL Workfront] Plan erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [[!DNL Workfront] Pläne.](https://www.workfront.com/plans)

Nachdem Sie [!DNL Adobe Workfront] für [!DNL Salesforce] als [!DNL Workfront] -Administrator installiert haben, können Sie es Ihren Benutzern zur Verfügung stellen, indem Sie es in einem neuen Abschnitt zu ihren [!UICONTROL Möglichkeiten] und [!UICONTROL Konten] hinzufügen.
Seitenlayouts in [!UICONTROL Salesforce].

Weitere Informationen zum Installieren von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Damit Benutzer sowohl in den [!DNL Classic] - als auch in den [!DNL Lightning Experience] -Frameworks über [!DNL Workfront] verfügen, müssen Sie die Seiten [!DNL WorkfrontOpportunities] und [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] zu den Seitenlayouts [!UICONTROL Opportunity] bzw. [!UICONTROL Accounts] hinzufügen.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

* Sie müssen über eine [!DNL Salesforce] -Instanz mit Zugriff auf ein Systemadministratorkonto verfügen.
* Sie müssen über eine [!DNL Workfront] -Instanz mit Zugriff auf ein Systemadministratorkonto verfügen.

## Konfigurieren Sie den Abschnitt [!DNL Workfront] im Framework [!DNL Salesforce Classic] .

1. Melden Sie sich bei [!DNL Salesforce] als Workfront-Administrator an.
1. Klicken Sie auf **[!UICONTROL Setup].**
1. Erweitern Sie im Abschnitt **[!UICONTROL Build]** den Eintrag **[!UICONTROL Anpassen].**

1. Erweitern Sie **[!UICONTROL Möglichkeiten]** und klicken Sie dann auf **[!UICONTROL Seitenlayouts]** , um den Abschnitt [!DNL Workfront] einer Gelegenheit hinzuzufügen.

   Oder

   Erweitern Sie **[!UICONTROL Konten]** und klicken Sie dann auf **[!UICONTROL Seitenlayouts]** , um den Abschnitt [!DNL Workfront] einem Konto hinzuzufügen.
.

1. Klicken Sie in einem vorhandenen Layout auf **[!UICONTROL Bearbeiten]** .

   Oder

   Klicken Sie auf **[!UICONTROL Neu]** , um ein neues Layout hinzuzufügen.

1. (Optional) Ziehen Sie die Komponente **[!UICONTROL Abschnitt]** in das Layout und legen Sie sie an der gewünschten Position ab.\

1. (Optional) Geben Sie einen Namen für den neuen Abschnitt an.

   Es wird empfohlen, diesen Abschnitt &quot;**[!DNL Workfront]**&quot; zu nennen.

1. (Optional) Geben Sie die gewünschte **[!UICONTROL Layout]**- und **[!UICONTROL Tab-Taste-Reihenfolge]** für den neuen Abschnitt an.

   Es wird empfohlen, das Layout **[!UICONTROL 1-Spalte]** für den Abschnitt [!DNL Workfront] zu wählen.

1. Klicken Sie auf **[!UICONTROL OK]**.
1. Klicken Sie im Bereich **[!UICONTROL Layout]** auf **[!UICONTROL Visualforce-Seiten].**

1. Ziehen Sie die Komponente **[!UICONTROL WorkfrontOpportunities]** in den neuen Abschnitt im Layout **[!UICONTROL Opportunities]** .

   Oder

   Ziehen Sie die Komponente **[!UICONTROL WorkfrontAccounts]** in den neuen Abschnitt im Layout **[!UICONTROL Konto]**.\

1. Klicken Sie oben rechts in der neu hinzugefügten Komponente auf das Symbol **[!UICONTROL Eigenschaften]** .\

1. Um eine optimale Anzeige zu erzielen, geben Sie die folgenden Eigenschaften für die Seite [!DNL Workfront Visualforce] an:

   * **[!UICONTROL Breite (in Pixel oder %)]**: 100 %
   * **[!UICONTROL Höhe (in Pixel)]**: 600
   * Wählen Sie **[!UICONTROL Bildlaufleisten anzeigen]** aus.

1. Klicken Sie auf **[!UICONTROL OK]**.
1. Klicken Sie auf **[!UICONTROL Speichern]** , um Ihr Layout zu speichern.

   Alle Benutzer, denen dieses Layout zugewiesen wurde, können jetzt den Abschnitt &quot;[!DNL Workfront]&quot;in ihren Objekten [!UICONTROL Chancen] oder [!UICONTROL Konten] sehen.

   Benutzer sehen einen [!DNL Workfront] Anmeldebildschirm im Abschnitt [!DNL Workfront] . Wenn sie kein [!DNL Workfront] -Konto haben, können sie den Abschnitt reduzieren, ihn jedoch nicht aus ihrem Layout entfernen.

## Konfigurieren Sie den Abschnitt [!DNL Workfront] im Framework [!DNL Salesforce Lightning Experience] .

Sie können den Abschnitt [!DNL Workfront] zum Layout einer [!DNL Salesforce] [!UICONTROL Chance] oder eines Kontos hinzufügen
im Framework [!DNL Salesforce Lightning Experience] entweder durch Zugriff auf den Bereich [!UICONTROL Setup] oder über ein Konto
oder das Objekt [!UICONTROL Opportunity].

* [Konfigurieren Sie den Abschnitt  [!DNL Workfront]  auf der Ebene [!UICONTROL Setup] .](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Konfigurieren Sie den Abschnitt [!DNL Workfront] auf Opportunity- oder Kontoebene.](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Konfigurieren Sie den Abschnitt &quot;[!DNL Workfront]&quot;auf der Ebene &quot;[!UICONTROL Setup]&quot;. {#configure-the-workfront-section-at-the-setup-level}

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. Klicken Sie auf das Symbol **[!UICONTROL Einrichten]** und dann auf **[!UICONTROL Einrichten]**.

1. Erweitern Sie **[!UICONTROL Objekt und Felder]** und klicken Sie dann auf **[!UICONTROL Objektmanager]**.

1. Klicken Sie auf **[!UICONTROL Gelegenheit]** , um das Layout einer Gelegenheit anzupassen.

   Oder

   Klicken Sie auf **[!UICONTROL Konto]** , um das Layout eines Kontos anzupassen.

1. Klicken Sie auf **[!UICONTROL Seitenlayouts]**.
1. Klicken Sie auf den Namen eines vorhandenen Seitenlayouts, um es zu bearbeiten.

   Oder

   Klicken Sie auf **[!UICONTROL Neu]** , um ein neues Seitenlayout zu erstellen.

1. Fahren Sie mit [Konfigurieren Sie den Abschnitt  [!DNL Workfront] auf der Opportunity- oder Kontoebene](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) weiter unten.

### Konfigurieren Sie den Abschnitt &quot;[!DNL Workfront]&quot; auf Opportunity- oder Kontoebene. {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. Wechseln Sie zu einem **[!UICONTROL Opportunity]**- oder **[!UICONTROL Konto]**.

1. Klicken Sie auf das Symbol **[!UICONTROL Einrichten]** und dann auf **[!UICONTROL Seite bearbeiten]**.\

1. Erweitern Sie den Abschnitt **[!UICONTROL Benutzerspezifisch verwaltet]** .
1. Ziehen Sie die Komponente **[!DNL Workfront]** per Drag-and-Drop auf Ihre [!UICONTROL Chancen] oder Ihr Konto
Seite.

   Es wird empfohlen, für den Abschnitt &quot;[!DNL Workfront]&quot;die gesamte Breite der Seite anstelle einer der Spalten des Layouts zu verwenden.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Alle Benutzer, denen dieses Layout zugewiesen wurde, können jetzt den Abschnitt &quot;[!DNL Workfront]&quot;in ihren Objekten [!UICONTROL Chancen] oder [!UICONTROL Konten] sehen.

   >[!NOTE]
   >
   >Benutzer sehen einen [!DNL Workfront] Anmeldebildschirm im Abschnitt [!DNL Workfront] . Wenn sie kein [!DNL Workfront] -Konto haben, können sie den Abschnitt reduzieren, ihn jedoch nicht aus ihrem Layout entfernen. Benutzer können sich mit der Authentifizierungsmethode anmelden, die Sie aktiviert haben: Erweiterte Authentifizierung oder Ihre SAML-URL (Security Assertion Markup Language).

