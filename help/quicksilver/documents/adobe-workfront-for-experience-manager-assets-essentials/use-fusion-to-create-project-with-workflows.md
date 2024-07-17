---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verwenden von Workfront Fusion zum Erstellen eines Workfront-Projekts mit Adobe Experience Manager-Workflows
description: Wenn Sie ein Projekt mit Workfront Fusion erstellen und Adobe Experience Manager-Workflows in das Projekt einbeziehen möchten, müssen Sie eine bestimmte Konfiguration des Fusion-Moduls verwenden, die in diesem Artikel beschrieben wird.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 012aa4c15bcdb26a3e30f8c143599a7e90c9a0f3
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Verwenden Sie Workfront Fusion, um ein Workfront-Problem in ein Projekt mit Adobe Experience Manager-Workflows zu konvertieren.

Wenn Sie ein Projekt mit Workfront Fusion erstellen und Adobe Experience Manager-Workflows in das Projekt einbeziehen möchten, müssen Sie eine bestimmte Konfiguration des Fusion-Moduls verwenden, die in diesem Artikel beschrieben wird.

>[!NOTE]
>
>Workflows sind nur in einer Adobe Experience Manager as a Cloud Service-Integration verfügbar. Sie sind nicht in Integrationen mit Adobe Experience Manager Assets Essentials verfügbar.


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
    <td><strong>Adobe Workfront-Plan*</strong></td>
    <td>Alle</td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenzen*</strong></td>
   <td>Anforderung oder höher</td>
  </tr>
  <tr>
   <td><strong>Produkt</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>Sie müssen über as a Cloud Service oder Assets Essentials von Experience Manager Assets verfügen und dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</p>
       </li>
       <li>
        <p>Sie müssen über Schreibzugriff auf das Repository in Adobe Experience Manager verfügen.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <p>Neu:</p>
     <ul>
       <li>
         <p>Workfront-Plan auswählen oder als Prime-Projekt festlegen: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.</p>
       </li>
       <li> 
         <p>Ultimate Workfront Plan: Workfront Fusion ist im Lieferumfang enthalten.</p>
       </li>
     </ul>
     <p>Oder</p>
     <p>Aktuell: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen auf Zugriffsebene*</strong>
   </td>
   <td>Zugriff auf Dokumente bearbeiten
     <p>
       <strong>Hinweis: </strong>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <strong>Benutzerdefinierte Zugriffsebenen erstellen oder ändern</strong>.
     </p>
   </td>
  </tr>
</table>

## Voraussetzungen

Bevor Sie beginnen

* Ihr Workfront-Administrator muss Workflows in einer Adobe Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Sie müssen über eine Projektvorlage verfügen, die mit einem Workflow für durch die Adobe Experience Manager-Integration verknüpfte Ordner konfiguriert wurde.
* Sie müssen eine OAuth-Anwendung in Workfront erstellt haben, um die Verbindung für dieses Modul zu konfigurieren.

  Anweisungen finden Sie unter [Erstellen einer OAuth-Anwendung](#create-an-oauth-application) in diesem Artikel.

## Modulkonfiguration

Wenn Sie in Workfront Fusion ein Projekt erstellen möchten, das Adobe Experience Manager-Workflows enthält, müssen Sie das Modul Workfront > Misc Action verwenden.

1. Fügen Sie Ihrem Szenario das Modul **Workfront** > **Misc Action** hinzu.
1. Wählen Sie im Feld **Verbindung** die Workfront-Verbindung aus, die eine Verbindung zu dem Konto herstellt, das dieses Modul verwenden soll.

   Anweisungen zum Erstellen einer Verbindung finden Sie unter [Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) im Artikel Workfront-Module.

   Anweisungen zum Erstellen der Client-ID und des Client-Geheimnisses finden Sie unter [Erstellen einer OAuth-Anwendung](#create-an-oauth-application) in diesem Artikel.

1. Wählen Sie im Feld **Record Type** die Option `Issue` aus.
1. Wählen Sie im Feld **Aktion** die Option `convertToProject` aus.
1. Geben Sie im Feld **ID** die ID des Problems ein, das Sie in ein Projekt konvertieren, oder ordnen Sie sie zu.
1. Aktivieren Sie **Erweiterte Einstellungen anzeigen**.
1. Scrollen Sie zum unteren Rand des Moduls und suchen Sie das Feld **Projekt (Erweiterte Sammlung)** .
1. Fügen Sie den folgenden Text in das Feld **Projekt (Erweiterte Sammlung)** ein.

   ```
   {
       "aemNativeFolderTreeIDs": ["Folder Tree ID here"],
       "aemNativeFolderWorkflowEnabled": "true",
       "name": "New project name here",
       "templateID": "Template ID here"
   }
   ```

1. Ersetzen Sie `Folder tree ID here` durch die Ordner-IDs.

   Informationen zum Suchen von Ordnerbaum-IDs finden Sie unter [Suchen von Ordnerbaum-IDs](#locate-folder-tree-ids) in diesem Artikel.

   Um mehr als eine Ordnerstruktur zu verwenden, trennen Sie IDs durch Kommas:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Ersetzen Sie `New project name here` durch den Namen, den das neue Projekt haben wird.
1. Ersetzen Sie `Template ID here` durch die ID der Vorlage, die Sie für das neue Projekt verwenden.

   Sie können die Vorlagen-ID einem vorherigen Modul zuordnen (z. B. Workfront > Suchmodul) oder sie in der URL der Vorlagenseite in Workfront suchen.

1. Klicken Sie auf **OK** , um die Modulkonfiguration zu speichern.

## Ordnerbaum-IDs suchen

Suchen der Ordnerbaum-IDs:

>[!NOTE]
>
>Diese Anweisungen verwenden den Chrome-Browser.

1. Öffnen Sie in Workfront die Vorlage, die Sie für dieses Projekt verwenden möchten. Diese Vorlage muss die Adobe Experience Manager-Konfiguration enthalten, die Sie für das Projekt verwenden möchten.
1. Öffnen Sie die Entwicklertools für Ihren Browser.
1. Öffnen Sie die Registerkarte **Netzwerk** in den Entwicklertools.
1. Geben Sie in das Feld **Filter** den Wert `object-workflow` ein.
1. Klicken Sie in der Spalte Name auf die alphanumerische ID, die angezeigt wird.

   ![Suchen der Ordner-ID 1](assets/finding-folder-id-1.png)

1. Klicken Sie auf die Registerkarte **Vorschau** rechts neben der alphanumerischen ID.
1. Öffnen Sie die folgenden reduzierten Abschnitte:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Jeder Ordnerbaum wird durch eine Zahl dargestellt. 0 (null) steht für den ersten Ordner in der Liste, 1 für den zweiten usw. Wenn die Vorlage nur eine Ordnerstruktur enthält, ist sie die Nummer 0.

1. Öffnen Sie die Ordnerstruktur, die Sie für das neue Projekt verwenden möchten. Notieren Sie sich den Feldwert `_id` . Wenn Sie mehr als einen Ordnerbaum verwenden möchten, notieren Sie sich alle `_id` -Feldwerte für die Ordnerbäume, die Sie verwenden möchten.

   ![Suchen der Ordner-ID 2](assets/finding-folder-id-2.png)

   Dies sind die `aemNativeFolderTreeIDs` -Werte, die Sie im Feld **Projekt (Erweiterte Sammlung)** im Fusionsmodul **Workfront** > **Misc Actions** eingeben.

## OAuth-Anwendung erstellen

Sie müssen in Workfront eine OAuth-Anwendung für die Verbindung dieses Moduls einrichten. Sie müssen dies nur einmal für eine bestimmte Workfront-Verbindung in Fusion tun.

1. Beginnen Sie in Workfront mit der Erstellung einer OAuth-Anwendung, wie unter [Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Fluss des Autorisierungscodes)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) im Artikel OAuth2-Anwendungen für [!DNL Workfront] -Integrationen erstellen beschrieben.
1. Kopieren Sie die Client-ID und das Client-Geheimnis an einen sicheren Speicherort.
1. Geben Sie im Feld **Umleitungs-URIs** Folgendes ein:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Klicken Sie auf **Speichern**.

Sie verwenden diese Client-ID und das Client-Geheimnis bei der Konfiguration der Verbindung des Moduls in Fusion.

Anweisungen zum Erstellen einer Verbindung finden Sie unter [Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#connect-workfront-to-workfront-fusion) im Artikel Workfront-Module.
