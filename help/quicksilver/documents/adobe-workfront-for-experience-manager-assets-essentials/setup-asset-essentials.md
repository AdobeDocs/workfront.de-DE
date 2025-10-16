---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Konfigurieren der Experience Manager Assets Essentials-Integration
description: Verbinden Sie Ihre Arbeit mit Ihren Inhalten in Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 1%

---

# Integration von Experience Manager Assets Essentials konfigurieren

Verbinden Sie Ihre Arbeit mit Ihren Inhalten in Experience Manager Assets Essentials&#x200B;:

* Pushen von Assets und Metadaten von Adobe Workfront nach Experience Manager Assets Essentials&#x200B;
* Verknüpfen von Assets aus Experience Manager Assets Essentials mit Ihren Projekten und Aufgaben in Workfront&#x200B;
* Vereinfachen von Versionierungs-Workflows für Assets, die auf Experience Manager Assets Essentials gepusht werden

>[!NOTE]
>
>Sie können auch mehrere Experience Manager Assets-Repositorys über Organisations-IDs hinweg mit einer Workfront-Umgebung oder mehrere Workfront-Umgebungen mit einem Experience Manager Assets-Repository verbinden. Befolgen Sie die Konfigurationsanweisungen in diesem Artikel für jede Integration, die Sie einrichten möchten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <p>Plan</p>
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einrichten der Integration

{{step-1-to-setup}}

1. Wählen Sie **Dokumente** ![Dokumentensymbol](assets/document-icon.png) im linken Bedienfeld aus und wählen Sie dann **Experience Manager-Integration**.
1. Wählen **Experience Manager-Integration hinzufügen** aus.
1. Geben Sie Folgendes an:

   <table>
   <tr>
      <td><strong>Name</strong>
      </td>
      <td>Geben Sie den Namen, den Benutzerinnen und Benutzern angezeigt werden soll, in die Schaltfläche Neu hinzufügen im Bereich Dokumente ein.
      </td>
   </tr>
   <tr>
      <td><strong>Navigations-URL</strong>
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
   >Sie können ein einzelnes Workfront-Feld mehreren Experience Manager Assets-Feldern zuordnen. Sie können nicht mehrere Workfront-Felder einem einzelnen Experience Manager Assets-Feld zuordnen.

1. Wählen Sie im Feld **Experience Manager** ein Experience Manager Assets-Feld aus.

   Um ein Workfront-Feld einem Experience Manager Assets-Tag zuzuordnen, wählen Sie `xcm:keywords` aus.

1. Wiederholen Sie die Schritte 1 und 2 nach Bedarf.
   ![Aktivieren von Metadaten](assets/metadata-assets-essentials.png)
1. Klicken Sie **Speichern** oder gehen Sie zum Abschnitt [Einrichten verknüpfter Ordner (optional)](#set-up-linked-folders-optional) in diesem Artikel.


## Verknüpfte Ordner einrichten (optional)

{{setup-linked-folder}}
