---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: Konfigurieren des  [!DNL Adobe Workfront]  für  [!DNL Salesforce]  Benutzer
description: Nach der Installation  [!DNL Adobe Workfront]  Salesforce als  [!DNL Workfront]  können Sie es für Ihre Benutzerinnen und Benutzer verfügbar machen, indem Sie es in einem neuen Abschnitt zu ihren Seiten-Layouts Opportunity und Account in Salesforce hinzufügen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 1%

---

# Konfigurieren des [!DNL Adobe Workfront] für [!DNL Salesforce] Benutzer

Um diese Funktion verwenden zu können[!UICONTROL  ist ein [!DNL Workfront]-Plan ]Pro) erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [[!DNL Workfront] Pläne.](https://business.adobe.com/products/workfront/pricing.html)

Nachdem Sie [!DNL Adobe Workfront] für [!DNL Salesforce] als [!DNL Workfront]-Admin installiert haben, können Sie es für Ihre Benutzerinnen und Benutzer verfügbar machen, indem Sie es in einem neuen Abschnitt zu deren [!UICONTROL Opportunity] und [!UICONTROL Account]
Seiten-Layouts in [!UICONTROL Salesforce].

Informationen zur Installation von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md).

Damit Benutzer [!DNL Workfront] sowohl im [!DNL Classic]- als auch im [!DNL Lightning Experience]-Framework verfügbar haben, müssen Sie die Seiten [!DNL WorkfrontOpportunities] [!DNL WorkfrontAccounts] und [!UICONTROL VisualForce] den Seiten-Layouts [!UICONTROL Opportunity] bzw. [!UICONTROL Accounts] hinzufügen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Funktionen nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

* Sie müssen über eine [!DNL Salesforce] mit Zugriff auf ein Systemadministratorkonto verfügen.
* Sie müssen über eine [!DNL Workfront] mit Zugriff auf ein Systemadministratorkonto verfügen.

## Konfigurieren des [!DNL Workfront] im [!DNL Salesforce Classic] Framework

1. Melden Sie sich bei [!DNL Salesforce] als Workfront-Administrator an.
1. Klicken Sie auf **[!UICONTROL Setup].**
1. Erweitern Sie im **[!UICONTROL Erstellen]** den Eintrag **[!UICONTROL Anpassen].**

1. Erweitern Sie **[!UICONTROL Opportunities]** und klicken Sie dann auf **[!UICONTROL Seiten-Layouts]**, um den [!DNL Workfront] Abschnitt zu einer Opportunity hinzuzufügen.

   Oder

   Erweitern Sie **[!UICONTROL Konten]** und klicken Sie dann auf **[!UICONTROL Seitenlayouts]**, um den [!DNL Workfront] Abschnitt zu einem Konto hinzuzufügen
.

1. Klicken Sie **[!UICONTROL einem]** Layout auf „Bearbeiten“.

   Oder

   Klicken Sie **[!UICONTROL Neu]**, um ein neues Layout hinzuzufügen.

1. (Optional) Ziehen Sie die Komponente **[!UICONTROL Abschnitt]** in das Layout und legen Sie sie an der gewünschten Position ab.\

1. (Optional) Geben Sie einen Namen für den neuen Abschnitt ein.

   Es wird empfohlen, diesen Abschnitt **[!DNL Workfront]** zu benennen.

1. (Optional) Geben Sie den gewünschten **[!UICONTROL Layout]** und die **[!UICONTROL Tabulatortaste]** für den neuen Abschnitt an.

   Es wird empfohlen, für den [!DNL Workfront] Abschnitt **[!UICONTROL 1-Spalten]**-Layout auszuwählen.

1. Klicken Sie **[!UICONTROL OK]**.
1. Klicken Sie im Bereich **[!UICONTROL Layout]** auf **[!UICONTROL VisualForce-Seiten].**

1. Ziehen Sie die Komponente **[!UICONTROL WorkfrontOpportunities]** in den neuen Abschnitt im Layout **[!UICONTROL Opportunitys]**.

   Oder

   Ziehen Sie die Komponente **[!UICONTROL WorkfrontAccounts]** in den neuen Abschnitt im Layout **[!UICONTROL Konto]**.\

1. Klicken Sie auf **[!UICONTROL Eigenschaften]** oben rechts in der neu hinzugefügten Komponente.\

1. Um eine optimale Anzeige zu erzielen, geben Sie die folgenden Eigenschaften für die [!DNL Workfront Visualforce] an:

   * **[!UICONTROL Breite (in Pixeln oder %)]**: 100 %
   * **[!UICONTROL Höhe (in Pixeln)]**: 600
   * Wählen Sie **[!UICONTROL Bildlaufleisten anzeigen]** aus.

1. Klicken Sie **[!UICONTROL OK]**.
1. Klicken Sie **[!UICONTROL Speichern]**, um Ihr Layout zu speichern.

   Alle Benutzenden, denen dieses Layout zugewiesen wurde, können jetzt den [!DNL Workfront] Abschnitt auf ihren [!UICONTROL Opportunities] oder [!UICONTROL Accounts]-Objekten sehen.

   Benutzende sehen im [!DNL Workfront] Abschnitt einen [!DNL Workfront] Anmeldebildschirm. Wenn sie kein [!DNL Workfront]-Konto haben, können sie den Abschnitt reduzieren, ihn jedoch nicht aus ihrem Layout entfernen.

## Konfigurieren des [!DNL Workfront] im [!DNL Salesforce Lightning Experience] Framework

Sie können den Abschnitt [!DNL Workfront] zum Layout eines [!DNL Salesforce] (Opportunity[!UICONTROL  oder ] hinzufügen
im [!DNL Salesforce Lightning Experience]-Framework, entweder durch Zugriff auf den [!UICONTROL Setup]-Bereich oder über ein Konto
oder [!UICONTROL Opportunity] Objekt.

* [Konfigurieren des  [!DNL Workfront] -Abschnitts auf [!UICONTROL Setup]-Ebene](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [Konfigurieren des  [!DNL Workfront] -Abschnitts auf Opportunity- oder Kontoebene](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### Konfigurieren des [!DNL Workfront] auf der [!UICONTROL -] {#configure-the-workfront-section-at-the-setup-level}

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. Klicken Sie auf **[!UICONTROL Setup]** und dann auf **[!UICONTROL Setup]**.

1. Erweitern Sie **[!UICONTROL Objekt und Felder]** und klicken Sie dann auf **[!UICONTROL Objekt-Manager]**.

1. Klicken Sie **[!UICONTROL Opportunity]**, um das Layout einer Opportunity anzupassen.

   Oder

   Klicken Sie **[!UICONTROL Konto]**, um das Layout eines Kontos anzupassen.

1. Klicken Sie **[!UICONTROL Seitenlayouts]**.
1. Klicken Sie auf den Namen eines vorhandenen Seiten-Layouts, um es zu bearbeiten.

   Oder

   Klicken Sie auf **[!UICONTROL Neu]**, um ein neues Seiten-Layout zu erstellen.

1. Fahren Sie mit [Konfigurieren des  [!DNL Workfront] -Abschnitts auf der Opportunity- oder Kontoebene](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level) fort.

### Konfigurieren des [!DNL Workfront] Abschnitts auf Opportunity- oder Kontoebene {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. Zu einem **[!UICONTROL Opportunity]** oder **[!UICONTROL Account]**.

1. Klicken Sie auf **[!UICONTROL Setup]** und dann auf **[!UICONTROL Seite bearbeiten]**.\

1. Erweitern Sie den Abschnitt **[!UICONTROL Benutzerdefiniert]**.
1. Ziehen Sie die **[!DNL Workfront]** Komponente per Drag-and-Drop auf Ihr [!UICONTROL Opportunity] oder Konto
Seite.

   Es wird empfohlen, für den Abschnitt [!DNL Workfront] die gesamte Seitenbreite statt einer der Spalten des Layouts zu verwenden.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Alle Benutzenden, denen dieses Layout zugewiesen wurde, können jetzt den [!DNL Workfront] Abschnitt auf ihren [!UICONTROL Opportunities] oder [!UICONTROL Accounts]-Objekten sehen.

   >[!NOTE]
   >
   >Benutzende sehen im [!DNL Workfront] Abschnitt einen [!DNL Workfront] Anmeldebildschirm. Wenn sie kein [!DNL Workfront]-Konto haben, können sie den Abschnitt reduzieren, ihn jedoch nicht aus ihrem Layout entfernen. Benutzer können sich mit der von Ihnen aktivierten Authentifizierungsmethode anmelden: Erweiterte Authentifizierung oder Ihre SAML-URL (Security Assertion Markup Language).

