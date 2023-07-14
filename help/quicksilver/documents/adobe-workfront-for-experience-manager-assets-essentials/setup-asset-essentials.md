---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Integration von Experience Manager Assets Essentials konfigurieren
description: Verbinden Sie Ihre Arbeit mit Ihren Inhalten in Experience Manager Assets Essentials - EDIT ME.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: a6cb6d4780f2b1c3e77547caf7324e882d2dab4f
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 4%

---

# Integration von Experience Manager Assets Essentials konfigurieren

Verbinden Sie Ihre Arbeit mit Ihren Inhalten in Experience Manager Assets Essentials &#x200B;:

* Push-Assets und Metadaten von Adobe Workfront an Experience Manager Assets Essentials &#x200B;
* Verknüpfen von Assets aus Experience Manager Assets Essentials mit Ihren Projekten und Aufgaben in Workfront &#x200B;
* Erleichtern von Versionierungsworkflows für Assets, die an Experience Manager Assets Essentials gesendet werden

>[!NOTE]
>
>Sie können auch mehrere Experience Manager Assets-Repositorys mit einer Workfront-Umgebung oder mehrere Workfront-Umgebungen mit einem Experience Manager Assets-Repository über Organisations-IDs hinweg verbinden. Befolgen Sie die Konfigurationsanweisungen in diesem Artikel für jede Integration, die Sie einrichten möchten.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table>
  <tr>
   <td><strong>Adobe Workfront-Plan*</strong>
   </td>
   <td>Beliebig
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront-Lizenzen*</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>Experience Manager-Lizenz</strong>
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td><strong>Produkt</strong>
   </td>
   <td>Sie müssen über Experience Manager Assets Essentials verfügen und dem Produkt als Benutzer in der Admin Console hinzugefügt werden.
   </td>
  </tr>
  <tr>
   <td><strong>Konfigurationen auf Zugriffsebene</strong>
   </td>
   <td>Sie müssen Workfront-Administrator sein. Informationen zu Workfront-Administratoren finden Sie unter <strong>Gewähren eines vollen Administratorzugriffs</strong>.
   </td>
  </tr>
</table>


*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.


## Integration einrichten

1. Klicken Sie auf **Hauptmenü** rechts oben in Adobe Workfront auf und klicken Sie dann auf **Einrichtung**.
1. Auswählen  **Dokumente** ![Dokumentsymbol](assets/document-icon.png) Wählen Sie im linken Bereich die Option **Experience Manager-Integration**.
1. Auswählen **Experience Manager-Integration hinzufügen**.
1. Geben Sie Folgendes an:

   <table>
   <tr>
      <td><strong>Name</strong>
      </td>
      <td>Geben Sie den Namen ein, den Benutzer anzeigen sollen, und zwar über die Schaltfläche Neue hinzufügen im Bereich Dokumente .
      </td>
   </tr>
   <tr>
      <td><strong>Navigations-URL</strong>
      </td>
      <td>Das System füllt die Navigations-URL automatisch. Diese URL wird verwendet, um über das Hauptmenü eine Verknüpfung zur Assets Essentials-Instanz Ihres Unternehmens herzustellen, damit Sie schnell darauf zugreifen können.
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

1. Klicken **Speichern** oder zum [Einrichten von Metadaten (optional)](#set-up-metadata-optional) in diesem Artikel.


## Einrichten von Metadaten (optional)

Ordnen Sie die Workfront-Objektdaten den Medienelement-Feldern in Experience Manager Assets zu. Metadaten werden zugeordnet, wenn ein Medienelement zum ersten Mal von Workfront übertragen wird.


### Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Konfigurieren Sie ein Metadatenschema in Experience Manager Assets Essentials, wie hier beschrieben: [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Optional) Konfigurieren Sie benutzerdefinierte Formularfelder in Workfront. Workfront verfügt über viele integrierte benutzerdefinierte Felder, die Sie verwenden können. Sie können jedoch auch eigene benutzerdefinierte Felder erstellen. Weitere Informationen finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Unterstützte Workfront- und Experience Manager Assets-Felder**

**AEM Keyword**

Sie können jedes von Workfront unterstützte Feld einem Suchbegriff in Experience Manager Assets Essentials zuordnen.

Um ein Feld mit einem Suchbegriff zu verknüpfen, wählen Sie `dc:subject` im Dropdown-Menü Experience Manager Assets-Feld im Bereich Metadatenzuordnung.

Um mehrere einzeilige Textfelder Suchbegriffen zuzuordnen, geben Sie eine kommagetrennte Liste der Suchbegriffwerte auf der Workfront-Seite der Metadaten-Zuordnung ein und `dc:subject` auf der Experience Manager Assets-Seite. Jeder Feldwert wird einem separaten Suchbegriff zugeordnet. Sie können ein berechnetes Feld verwenden, um mehrere Workfront-Felder in einem einzigen, kommagetrennten Textfeld zu kombinieren.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


### Assets

Metadaten werden zugeordnet, wenn ein Asset zum ersten Mal aus Workfront gesendet wird. Dokumente mit den integrierten oder benutzerdefinierten Feldern werden automatisch den angegebenen Feldern zugeordnet, wenn ein Asset zum ersten Mal an Experience Manager Assets Essentials gesendet wird.

1. Im **Workfront-Feld** wählen Sie ein integriertes oder benutzerdefiniertes Workfront-Feld aus.
   >[!NOTE]
   >
   >Sie können ein einzelnes Workfront-Feld mehreren Experience Manager Assets-Feldern zuordnen. Sie können nicht mehrere Workfront-Felder einem einzelnen Experience Manager Assets-Feld zuordnen.
1. Im **Experience Manager** ein Experience Manager Assets-Feld auswählen.

   Um ein Workfront-Feld einem Experience Manager Assets-Tag zuzuordnen, wählen Sie `dc:subject`.
1. Wiederholen Sie die Schritte 1 und 2 nach Bedarf.
   ![Metadaten aktivieren](assets/metadata-assets-essentials.png)
1. Klicken **Speichern** oder zum [Verknüpfte Ordner einrichten (optional)](#set-up-linked-folders-optional) in diesem Artikel.


## Verknüpfte Ordner einrichten (optional)

{{setup-linked-folder}}
