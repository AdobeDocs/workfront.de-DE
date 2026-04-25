---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configure the Experience Manager Assets Essentials Integration
description: Connect your work with your content in Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 6%

---

# Integration von Experience Manager Assets Essentials konfigurieren

Connect your work with your content in Experience Manager Assets Essentials&#x200B;:

* Push assets and metadata from Adobe Workfront to Experience Manager Assets Essentials&#x200B;
* Link assets from Experience Manager Assets Essentials to your projects and tasks in Workfront&#x200B;
* Facilitate versioning workflows for assets pushed to Experience Manager Assets Essentials

>[!NOTE]
>
>You can also connect several Experience Manager Assets repositories to one Workfront environment, or several Workfront environments to one Experience Manager Assets repository across Organization IDs. Follow the configuration instructions in this article for each integration you&#39;d like to set up.<br>
>Diese Funktion ist im Bereich Neue Dokumente nicht verfügbar.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table>
  <tr>
   <td><strong>Adobe Workfront-Paket</strong>
   </td>
   <td>Beliebig
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenzen</strong>
   </td>
   <td>
   <p>Standard</p>
   <p>Abo</p>
   </td>
  </tr>
  <tr>
   <td><strong>Zusätzliche Produkte</strong>
   </td>
   <td>Sie müssen über Experience Manager Assets as a Cloud Service oder Assets Essentials verfügen und Sie müssen dem Produkt als Benutzer hinzugefügt werden.
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager-Berechtigungen</strong>
   </td>
   <td>Sie müssen über Schreibzugriff auf den Zielordner in der Experience Manager-Integration verfügen.
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen der Zugriffsebene</strong>
   </td>
   <td>Sie müssen ein Workfront-Administrator sein, um eine Experience Manager-Integration konfigurieren zu können. Nach der Konfiguration können Benutzer mit Planlizenz verknüpfte Ordner für einzelne Projekte einrichten.
   </td>
  </tr>
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).



+++

## Set up the integration

{{step-1-to-setup}}

1. Select  **Documents** ![documents icon](assets/document-icon.png) in the left panel, then select **Experience Manager Integration**.
1. Select **Add Experience Manager Integration**.
1. Specify the following:

   <table>
   <tr>
      <td><strong>Name</strong>
      </td>
      <td>Enter the name you want users to see in the Add new button in the Documents area.
      </td>
   </tr>
   <tr>
      <td><strong>Navigation URL</strong>
      </td>
      <td>Das System füllt automatisch die Navigations-URL. Diese URL wird verwendet, um über das Hauptmenü eine Verknüpfung zur Assets Essentials-Instanz Ihres Unternehmens herzustellen und so einen schnellen Zugriff zu ermöglichen.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Experience Manager Assets-Repository</strong>
      </td>
      <td>
      Das System füllt automatisch das mit Ihrer Organisations-ID verknüpfte Experience Manager-Repository.
      </td>
   </tr>
   </table>

1. Klicken Sie **Speichern** oder gehen Sie zum Abschnitt [Einrichten von Metadaten (optional)](#set-up-metadata-optional) in diesem Artikel.


## Einrichten von Metadaten (optional)

Ordnen Sie Workfront-Objektdaten Asset-Medienfeldern in Experience Manager Assets zu. Metadaten werden zugeordnet, wenn ein Asset zum ersten Mal von Workfront gepusht wird.


### Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Konfigurieren Sie ein Metadatenschema in Experience Manager Assets Essentials, wie in [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping) beschrieben.
* (Optional) Konfigurieren von benutzerdefinierten Formularfeldern in Workfront. Workfront verfügt über viele integrierte benutzerdefinierte Felder, die Sie verwenden können. Sie können jedoch auch eigene benutzerdefinierte Felder erstellen. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Unterstützte Workfront- und Experience Manager Assets-Felder

### AEM-Schlüsselwort

Sie können jedes von Workfront unterstützte Feld einem Keyword in Experience Manager Assets Essentials zuordnen.

Um ein Feld mit einem Keyword zu verknüpfen, wählen Sie `xcm:keywords` in der Dropdown-Liste Experience Manager Assets-Feld im Bereich für die Metadatenzuordnung aus.

Um mehrere einzeilige Textfelder Schlüsselwörtern zuzuordnen, geben Sie eine kommagetrennte Liste der Schlüsselwortwerte in die Workfront-Seite der Metadatenzuordnung ein und `xcm:keywords` auf der Experience Manager Assets-Seite. Jeder Feldwert wird einem separaten Keyword zugeordnet. Sie können ein berechnetes Feld verwenden, um mehrere Workfront-Felder in einem einzigen, durch Kommas getrennten Textfeld zu kombinieren.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=de).
-->


### Assets

Metadaten werden zugeordnet, wenn ein Asset zum ersten Mal von Workfront gepusht wird. Dokumente mit den integrierten oder benutzerdefinierten Feldern werden beim ersten Versand eines Assets an Experience Manager Assets Essentials automatisch den angegebenen Feldern zugeordnet.

1. Wählen Sie in der **&#x200B;**&#x200B;Workfront ein integriertes oder benutzerdefiniertes Workfront-Feld aus.

   >[!NOTE]
   >
   >Sie können ein einzelnes Workfront-Feld mehreren Experience Manager Assets-Feldern zuordnen. You can&#39;t map multiple Workfront fields to a single Experience Manager Assets field.

1. In the **Experience Manager** field, choose an Experience Manager Assets field.

   To map a Workfront field to an Experience Manager Assets tag, select `xcm:keywords`.

1. Repeat steps 1 and 2 as needed.
   ![enable metadata](assets/metadata-assets-essentials.png)
1. Click **Save** or move on to the [Set up linked folders (optional)](#set-up-linked-folders-optional) section in this article.


## Set up linked folders (optional)

{{setup-linked-folder}}
