---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Konfigurieren der Integration von Experience Manager Assets Essentials
description: Verbinden Sie Ihre Arbeit mit Ihren Inhalten in Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 1%

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

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] Plan
   </td>
   <td>Alle
   </td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] Lizenz
   </td>
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   <p>Neu: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>[!DNL Experience Manager] Lizenz
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td>Produkt
   </td>
   <td>Sie müssen über Experience Manager Assets Essentials verfügen und dem Produkt als Benutzer in der Admin Console hinzugefügt werden.
   </td>
  </tr>
  <tr>
   <td>Konfigurationen auf Zugriffsebene
   </td>
   <td>Sie müssen ein [!DNL Workfront] -Administrator sein.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Integration einrichten

{{step-1-to-setup}}

1. Wählen Sie im linken Bereich das Symbol **Dokumente** ![Dokumente](assets/document-icon.png) und dann **Experience Manager-Integration** aus.
1. Wählen Sie **Experience Manager-Integration hinzufügen** aus.
1. Geben Sie Folgendes an:

   <table>
   <tr>
      <td><strong>Name</strong>
      </td>
      <td>Geben Sie den Namen ein, den Benutzer anzeigen sollen, indem Sie im Bereich "Dokumente"auf die Schaltfläche Neu hinzufügen klicken.
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

1. Klicken Sie auf **Speichern** oder wechseln Sie zum Abschnitt [Einrichten von Metadaten (optional)](#set-up-metadata-optional) in diesem Artikel.


## Einrichten von Metadaten (optional)

Ordnen Sie Workfront-Objektdaten Asset-Medienfeldern in Experience Manager Assets zu. Metadaten werden zugeordnet, wenn ein Asset zum ersten Mal aus Workfront gesendet wird.


### Voraussetzungen

Bevor Sie beginnen, müssen Sie

* Konfigurieren Sie ein Metadatenschema in Experience Manager Assets Essentials, wie in [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe Workfront und Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en) beschrieben.
* (Optional) Konfigurieren Sie benutzerdefinierte Formularfelder in Workfront. Workfront verfügt über viele integrierte benutzerdefinierte Felder, die Sie verwenden können. Sie können jedoch auch eigene benutzerdefinierte Felder erstellen. Weitere Informationen finden Sie unter [Benutzerdefiniertes Formular erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Unterstützte Workfront- und Experience Manager Assets-Felder

### AEM Keyword

Sie können jedes von Workfront unterstützte Feld einem Suchbegriff in Experience Manager Assets Essentials zuordnen.

Um ein Feld mit einem Keyword zu verknüpfen, wählen Sie im Dropdown-Menü Experience Manager Assets-Feld im Bereich Metadatenzuordnung die Option `xcm:keywords` aus.

Um mehrere einzeilige Textfelder Suchbegriffen zuzuordnen, geben Sie eine kommagetrennte Liste der Suchbegriffwerte auf der Workfront-Seite der Metadaten-Zuordnung ein und `xcm:keywords` auf der Experience Manager Assets-Seite. Jeder Feldwert wird einem separaten Suchbegriff zugeordnet. Sie können ein berechnetes Feld verwenden, um mehrere Workfront-Felder in einem einzigen, kommagetrennten Textfeld zu kombinieren.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### Assets

Metadaten werden zugeordnet, wenn ein Asset zum ersten Mal aus Workfront gesendet wird. Dokumente mit den integrierten oder benutzerdefinierten Feldern werden automatisch den angegebenen Feldern zugeordnet, wenn ein Asset zum ersten Mal an Experience Manager Assets Essentials gesendet wird.

1. Wählen Sie in der Spalte **Workfront field** ein integriertes oder benutzerdefiniertes Workfront-Feld aus.

   >[!NOTE]
   >
   >Sie können ein einzelnes Workfront-Feld mehreren Experience Manager Assets-Feldern zuordnen. Sie können nicht mehrere Workfront-Felder einem einzelnen Experience Manager Assets-Feld zuordnen.

1. Wählen Sie im Feld **Experience Manager** ein Experience Manager Assets -Feld aus.

   Um ein Workfront-Feld einem Experience Manager Assets-Tag zuzuordnen, wählen Sie `xcm:keywords` aus.

1. Wiederholen Sie die Schritte 1 und 2 nach Bedarf.
   ![Aktivieren von Metadaten](assets/metadata-assets-essentials.png)
1. Klicken Sie auf **Speichern** oder wechseln Sie zum Abschnitt [Verknüpfte Ordner einrichten (optional)](#set-up-linked-folders-optional) in diesem Artikel.


## Verknüpfte Ordner einrichten (optional)

{{setup-linked-folder}}
