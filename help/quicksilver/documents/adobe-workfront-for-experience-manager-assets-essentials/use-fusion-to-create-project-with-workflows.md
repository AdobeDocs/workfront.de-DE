---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Verwenden Sie Workfront Fusion, um ein Workfront-Projekt mit Adobe Experience Manager-Workflows zu erstellen
description: Wenn Sie ein Projekt über Workfront Fusion erstellen und Adobe Experience Manager-Workflows in das Projekt aufnehmen möchten, müssen Sie eine bestimmte Fusion-Modulkonfiguration verwenden, die in diesem Artikel beschrieben wird.
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps, Workfront Fusion
exl-id: b8132d5e-234d-47f6-a09c-ca46018a2d77
source-git-commit: 6a21465ab8c92888c83344f33574302c5cc446e8
workflow-type: tm+mt
source-wordcount: '877'
ht-degree: 0%

---

# Verwenden Sie Workfront Fusion, um ein Workfront-Problem in ein Projekt mit Adobe Experience Manager-Workflows zu konvertieren

Wenn Sie ein Projekt über Workfront Fusion erstellen und Adobe Experience Manager-Workflows in das Projekt aufnehmen möchten, müssen Sie eine bestimmte Fusion-Modulkonfiguration verwenden, die in diesem Artikel beschrieben wird.

>[!NOTE]
>
>Workflows sind nur in einer Adobe Experience Manager as a Cloud Service-Integration verfügbar. Sie sind nicht in Integrationen mit Adobe Experience Manager Assets Essentials verfügbar.


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table>
  <tr>
    <td><strong>Adobe Workfront-Paket</strong></td>
   <td> <p>Jedes Adobe Workfront-Workflow-Paket und jedes Adobe Workfront-Automatisierungs- und Integrationspaket</p><p>Workfront Ultimate</p><p>Workfront Prime und Select-Pakete, mit einem zusätzlichen Kauf von Workfront Fusion.</p> </td> 
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenzen</strong></td>
   <td><p>Mitwirkender oder höher</p><p>Anfrage oder höher</p></td>
  </tr>
  <tr>
   <td><strong>Produkt</strong></td>
   <td>
     <p><b>Adobe Experience Manager:</b></p>
     <ul>
       <li>
         <p>Sie müssen über Experience Manager Assets as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzer in der Admin Console hinzugefügt werden.</p>
       </li>
       <li>
        <p>Sie müssen Schreibzugriff auf das Repository in Adobe Experience Manager haben.</p>
       </li>
     </ul>
     <p><b>Workfront Fusion:</b></p>
     <ul>
       <li>
        <p>Wenn Ihr Unternehmen über ein Select- oder Prime Workfront-Paket verfügt, das keine Workfront-Automatisierung und -Integration enthält, muss Ihr Unternehmen Adobe Workfront Fusion erwerben.</li></ul>
       </li>
     </ul>
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen der Zugriffsebene</strong>
   </td>
   <td><p>Zugriff auf Dokumente bearbeiten</p>
   </td>
  </tr>
</table>

+++

## Voraussetzungen

Bevor Sie beginnen,

* Ihr Workfront-Administrator muss Workflows in einer Adobe Experience Manager-Integration konfigurieren. Weitere Informationen finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).
* Sie müssen über eine Projektvorlage verfügen, die mit einem Workflow für verknüpfte Ordner der Adobe Experience Manager-Integration konfiguriert ist.
* Sie müssen eine OAuth-Anwendung in Workfront erstellt haben, um die Verbindung für dieses Modul zu konfigurieren.

  Anweisungen finden Sie unter [Erstellen einer OAuth](#create-an-oauth-application)Anwendung) in diesem Artikel.

## Modulkonfiguration

Wenn Sie in Workfront Fusion ein Projekt erstellen möchten, das Adobe Experience Manager-Workflows enthält, müssen Sie das Aktionsmodul Workfront > Sonstige verwenden.

1. Workfront Fügen Sie das Modul **&#x200B;**&#x200B;> **Misc Action** zu Ihrem Szenario hinzu.
1. Wählen Sie im **Verbindung** die Workfront-Verbindung aus, die eine Verbindung zu dem Konto herstellt, das dieses Modul verwenden wird.

   Anweisungen zum Erstellen einer Verbindung finden Sie unter [Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) im Artikel Workfront-Module.

   Anweisungen zum Erstellen der Client-ID und des Client-Geheimnisses, das Sie benötigen, um eine Verbindung zu erstellen, finden [&#x200B; unter „Erstellen einer OAuth](#create-an-oauth-application)Anwendung“ in diesem Artikel.

1. Wählen Sie **Feld** Datensatztyp“ `Issue` aus.
1. Wählen Sie im **Aktion** die Option `convertToProject` aus.
1. Geben Sie **Feld** ID“ die ID des Problems ein, das Sie in ein Projekt konvertieren, oder ordnen Sie sie zu.
1. Aktivieren **Erweiterte Einstellungen anzeigen**.
1. Scrollen Sie zum unteren Rand des Moduls und suchen Sie das Feld **Projekt (Erweiterte Sammlung** .
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

   Informationen zum Auffinden von Ordnerbaum-IDs finden Sie unter [Suchen von &#x200B;](#locate-folder-tree-ids)-IDs“ in diesem Artikel.

   Um mehr als eine Ordnerstruktur zu verwenden, trennen Sie IDs durch ein Komma:

   `"aemNativeFolderTreeIDs": ["Folder tree ID here","Second folder tree ID here"],`
1. Ersetzen Sie `New project name here` durch den Namen, den das neue Projekt haben wird.
1. Ersetzen Sie `Template ID here` durch die ID der Vorlage, die Sie für das neue Projekt verwenden.

   Sie können die Vorlagen-ID aus einem vorherigen Modul zuordnen (z. B. einem Workfront > Suchmodul) oder sie in der URL der Vorlagenseite in Workfront suchen.

1. Klicken Sie **OK**, um die Modulkonfiguration zu speichern.

## IDs der Ordnerstruktur suchen

So suchen Sie die IDs der Ordnerstruktur:

>[!NOTE]
>
>In diesen Anweisungen wird der Chrome-Browser verwendet.

1. Öffnen Sie in Workfront die Vorlage, die Sie für dieses Projekt verwenden möchten. Diese Vorlage muss die Adobe Experience Manager-Konfiguration enthalten, die Sie für das Projekt verwenden möchten.
1. Öffnen Sie die Entwickler-Tools für Ihren Browser.
1. Öffnen Sie die **Netzwerk** in den Entwickler-Tools.
1. Geben Sie **Feld** Filter“ `object-workflow` ein.
1. Klicken Sie in der Spalte Name auf die alphanumerische ID, die angezeigt wird.

   ![Auffinden von Ordner-ID 1](assets/finding-folder-id-1.png)

1. Klicken Sie auf **Vorschau** rechts neben der alphanumerischen ID.
1. Öffnen Sie die folgenden reduzierten Abschnitte:
   1. `data`
   1. `objectWorkflow`
   1. `workflows`
   1. `enhancedLinkedFolderCreationWorkflow`
   1. `enhancedLinkedFolderCreationWorkflowConfigurations`

   Jede Ordnerstruktur wird durch eine Zahl dargestellt. 0 (Null) steht für den ersten Ordner in der Liste, 1 steht für den zweiten Ordner usw. Wenn die Vorlage nur eine Ordnerstruktur enthält, ist dies die Zahl 0.

1. Öffnen Sie die Ordnerstruktur, die Sie für das neue Projekt verwenden möchten. Notieren Sie sich den Wert des `_id`. Wenn Sie mehr als eine Ordnerstruktur verwenden möchten, notieren Sie sich alle `_id` Feldwerte für die Ordnerbäume, die Sie verwenden möchten.

   ![Auffinden der Ordner-ID 2](assets/finding-folder-id-2.png)

   Dies sind die `aemNativeFolderTreeIDs` Werte, die Sie in das Feld **Projekt (Erweiterte Sammlung)** im Modul **Workfront** > **Misc Actions** eingeben.

## Erstellen einer OAuth-Anwendung

Für die Verbindung dieses Moduls müssen Sie in Workfront eine OAuth-Anwendung einrichten. Sie müssen dies nur einmal für eine bestimmte Workfront-Verbindung in Fusion tun.

1. Beginnen Sie in Workfront mit der Erstellung einer OAuth-Anwendung, wie beschrieben unter [Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss)](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-application-using-user-credentials-authorization-code-flow) im Artikel Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen.
1. Kopieren Sie die Client-ID und den geheimen Client-Schlüssel an einen sicheren Speicherort.
1. Geben Sie **Feld** Umleitungs-URIs“ Folgendes ein:

   ```
   http://app.workfrontfusion.com/oauth/cb/workfront-workfront
   ```

1. Klicken Sie auf **Speichern**.

Diese Client-ID und dieses Client-Geheimnis werden beim Konfigurieren der Verbindung des Moduls in Fusion verwendet.

Anweisungen zum Erstellen einer Verbindung finden Sie unter [Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-modules#connect-workfront-to-workfront-fusion) im Artikel Workfront-Module.
