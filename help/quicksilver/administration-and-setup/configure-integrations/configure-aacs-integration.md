---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Konfigurieren der Integration von [!UICONTROL Experience Manager Assets as a Cloud Service]
description: Sie können Ihre Arbeit mit Ihrem Inhalt in [!DNL Experience Manager Assets] verbinden.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 99924f690c53584c090d19fff90d23d84ec306d4
workflow-type: tm+mt
source-wordcount: '1700'
ht-degree: 0%

---

# Integration von [!UICONTROL Experience Manager Assets as a Cloud Service] konfigurieren

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>Diese Funktion ist nur für Organisationen verfügbar, die in den [!DNL Adobe Admin Console] integriert wurden.

Sie können Ihre Arbeit mit Ihrem Inhalt in [!DNL Experience Manager Assets] &#x200B; verbinden:

* Assets und Metadaten von [!DNL Adobe Workfront] an [!DNL Experience Manager Assets] pushen&#x200B;
* Verknüpfen von Assets von [!DNL Experience Manager Assets] mit Ihren Projekten und Aufgaben in [!DNL Workfront&#x200B;]
* Anwendungsfälle für die Versionierung erleichtern
* Erstellen von Ordnern mit [!DNL Experience Manager Assets]
* Tracking von Metadaten für Assets und Ordner
* Projekt-Metadaten zwischen [!DNL Workfront] und [!DNL Experience Manager Assets] synchronisieren

>[!NOTE]
>
>Sie können auch mehrere [!DNL Experience Manager Assets] Repositorys mit einer [!UICONTROL Workfront] -Umgebung oder mehreren [!DNL Workfront] -Umgebungen mit einem [!DNL Experience Manager Assets] -Repository über Organisations-IDs hinweg verbinden. Befolgen Sie die Konfigurationsanweisungen in diesem Artikel für jede Integration, die Sie einrichten möchten.

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
   <td>Sie müssen über [!DNL Experience Manager Assets as a Cloud Service] verfügen und dem Produkt als Benutzer hinzugefügt werden.
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

## Voraussetzungen

Bevor Sie beginnen

* Sie müssen [!DNL Workfront] und [!DNL Adobe Experience Manager Assets] mit einer Organisations-ID in der [!DNL Adobe Admin Console] verknüpft haben. Weitere Informationen finden Sie unter [Plattformbasierte Verwaltungsunterschiede ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Integrationsinformationen einrichten

{{step-1-to-setup}}

1. Wählen Sie im linken Bereich **[!UICONTROL Dokumente]** und dann **[!UICONTROL [!DNL Experience Manager]Integration]** aus.

   >[!NOTE]
   >
   >Dieser Konfigurationsbereich wird nur angezeigt, wenn Ihre [!DNL Workfront] -Umgebung unter einem [!DNL Adobe Admin Console] enthalten ist.

1. Wählen Sie **[!UICONTROL Hinzufügen von [!DNL Experience Manager] Integration]** aus.
1. Geben Sie im Feld **[!UICONTROL Name]** den Namen ein, den Benutzer bei der Interaktion mit dieser Integration in Workfront und Experience Manager Assets sehen sollen.
1. Im Feld **[!UICONTROL Navigations-URL]** füllt das System automatisch die Navigations-URL. Diese schreibgeschützte URL wird verwendet, um für einen schnellen Zugriff über das [!UICONTROL Hauptmenü] eine Verknüpfung mit der [!DNL Experience Manager] -Instanz Ihres Unternehmens herzustellen.
1. Wählen Sie ein Repository aus dem Dropdownmenü **[!UICONTROL [!DNL Experience Manager]Assets-Repository]** aus. Das System füllt automatisch alle [!DNL Experience Manager] Repositorys aus, die mit der Organisations-ID verknüpft sind, der Ihr Benutzerprofil zugewiesen ist.
   ![ Experience Manager-Repository auswählen](assets/setup-information.png)

1. Klicken Sie auf **[!UICONTROL Speichern]** oder wechseln Sie zum Abschnitt [Metadaten einrichten (optional)](#set-up-metadata-optional) in diesem Artikel.

   >[!NOTE]
   >
   >Aufgrund der Komplexität der Integration können Sie das Repository nach dem Speichern der ursprünglichen Konfiguration nicht ändern.

## Einrichten von Metadaten (optional)

Sie können [!DNL Workfront] -Objektdaten Asset-Medienfeldern in [!DNL Experience Manager] Assets zuordnen.

>[!IMPORTANT]
>
>Sie können Metadaten nur in eine Richtung zuordnen: von [!DNL Workfront] zu [!DNL Experience Manager]. Metadaten für Dokumente, die mit [!DNL Workfront] von [!DNL Experience Manager] verknüpft sind, können nicht an [!DNL Workfront] übertragen werden.

### Konfigurieren von Metadatenfeldern

Bevor Sie mit der Zuordnung von Metadatenfeldern beginnen, müssen Sie Metadatenfelder sowohl in Workfront als auch in Experience Manager Assets konfigurieren.

So konfigurieren Sie Metadatenfelder:

1. Konfigurieren Sie ein Metadatenschema in [!DNL Experience Manager Assets], wie in [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe [!DNL Workfront]  und  [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en) beschrieben.


1. Konfigurieren Sie benutzerdefinierte Formularfelder in Workfront. [!DNL Workfront] verfügt über viele integrierte benutzerdefinierte Felder, die Sie verwenden können. Sie können jedoch auch eigene benutzerdefinierte Felder erstellen, wie in [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) beschrieben.

+++ **Erweitern, um weitere Informationen zu unterstützten Workfront- und Experience Manager Assets-Feldern anzuzeigen**

**Experience Manager Assets-Tags**

Sie können jedes von Workfront unterstützte Feld einem Tag in Experience Manager Assets zuordnen. Dazu müssen Sie sicherstellen, dass die Tag-Werte in Experience Manager Assets mit Workfront übereinstimmen.

* Die Feldwerte für Tags und Workfront müssen exakt mit der Schreibweise und dem Format übereinstimmen.
* Workfront-Feldwerte, die Experience Manager-Assets-Tags zugeordnet werden, müssen in Kleinbuchstaben geschrieben werden, selbst wenn das Tag in Experience Manager Assets Großbuchstaben zu haben scheint.
* Workfront-Feldwerte dürfen keine Leerzeichen enthalten.
* Der Feldwert in Workfront muss auch die Ordnerstruktur des Experience Manager Assets-Tags enthalten.
* Um mehrere einzeilige Textfelder Tags zuzuordnen, geben Sie eine kommagetrennte Liste der Tag-Werte auf der Workfront-Seite der Metadatenzuordnung und auf der Experience Manager Assets-Seite `xcm:keywords` ein. Jeder Feldwert wird einem separaten Tag zugeordnet. Sie können ein berechnetes Feld verwenden, um mehrere Workfront-Felder in einem einzigen, kommagetrennten Textfeld zu kombinieren.
* Sie können Werte aus Dropdown-, Optionsfeld- oder Kontrollkästchen-Feldern zuordnen, indem Sie eine kommagetrennte Liste der in diesem Feld verfügbaren Werte eingeben.


>[!INFO]
>
>**Beispiel**: Um mit dem hier in der Ordnerstruktur angezeigten Tag abzugleichen, lautet der Feldwert in Workfront `landscapes:trees/spruce`. Beachten Sie die Kleinbuchstaben im Workfront-Feldwert.
>
>Wenn das Tag am weitesten links im Tag-Baum sein soll, muss es von einem Doppelpunkt gefolgt werden. In diesem Beispiel wäre der Feldwert in Workfront `landscapes:`, wenn er dem Landschaftstag zugeordnet werden soll.
>
>![Ordnerstruktur in AEM](assets/aem-folder-structure-with-red-boxes.png)


Nachdem Sie die Tags in Experience Manager Assets erstellt haben, werden sie im Abschnitt Metadaten unter der Dropdown-Liste Tags angezeigt. Um ein Feld mit einem Tag zu verknüpfen, wählen Sie im Dropdown-Menü Experience Manager Assets-Feld im Bereich Metadatenzuordnung die Option `xcm:keywords` aus.

Weitere Informationen zu Tags in Experience Manager Assets, einschließlich der Erstellung und Verwaltung von Tags, finden Sie unter [Verwalten von Tags](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Benutzerdefinierte Experience Manager Assets-Metadatenschema-Felder**

Sie können sowohl integrierte als auch benutzerdefinierte Workfront-Felder benutzerdefinierten Metadatenschema-Feldern in Experience Manager Assets zuordnen.

Benutzerdefinierte Metadatenfelder, die in Experience Manager Assets erstellt wurden, sind in ihrem eigenen Abschnitt im Metadaten-Setup-Bereich organisiert.

![benutzerdefinierter Metadatenabschnitt](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront-Felder**

Sie können sowohl integrierte als auch benutzerdefinierte Workfront-Felder Experience Manager Assets zuordnen. Die folgenden Feldwerte müssen sowohl Groß- als auch Kleinschreibung zwischen Workfront und Experience Manager Assets berücksichtigen:

* Dropdown-Felder
* Felder mit Mehrfachauswahl

>[!TIP]
>
> Um zu überprüfen, ob die Feldwerte exakt übereinstimmen, gehen Sie zu
>
> * Einrichtung > Benutzerdefinierter Forms in Workfront oder das -Feld im -Objekt
> * Assets > Metadatenschemata in Experience Manager Assets

+++

### Zuordnen von Metadaten für Assets

Metadaten werden zugeordnet, wenn ein Asset zum ersten Mal aus [!DNL Workfront] gepusht wird. Dokumente mit den integrierten oder benutzerdefinierten Feldern werden automatisch den angegebenen Feldern zugeordnet, wenn ein Asset zum ersten Mal an [!DNL Experience Manager Assets] gesendet wird.

Zuordnen von Metadaten für Assets:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Wählen Sie in der Spalte **[!UICONTROL [!DNL Workfront]field]** ein integriertes oder benutzerdefiniertes Workfront-Feld aus.

   >[!NOTE]
   >
   >Sie können ein einzelnes [!DNL Workfront] -Feld mehreren [!UICONTROL Experience Manager Assets] -Feldern zuordnen. Sie können nicht mehrere [!DNL Workfront] -Felder einem einzelnen [!DNL Experience Manager Assets] -Feld zuordnen.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Suchen Sie im Feld [!DNL Experience Manager Assets] nach den vorausgefüllten Kategorien oder geben Sie mindestens zwei Buchstaben in das Suchfeld ein, um auf weitere Kategorien zuzugreifen.
1. Wiederholen Sie die Schritte 2 und 3 nach Bedarf.
   ![Metadatenfelder](assets/metadata-no-asset-toggle.png)
1. Klicken Sie auf [!UICONTROL Speichern] oder wechseln Sie zum Abschnitt [Einrichten von Workflows](#set-up-workflows-optional) in diesem Artikel.

<!--

### Map metadata for folders

When users create a linked folder on a project, the associated project, portfolio, and program data is mapped to folder metadata fields in [!DNL Experience Manager Assets].

>[!NOTE]
>
>This integration does not support custom metadata from [!DNL Adobe Experience Manager].

To map metadata for folders: 

1. Select **[!UICONTROL Folders]** above the metadata table.
1. In the **[!UICONTROL [!DNL Workfront] field]** column, choose a built-in or custom Workfront field.

    >[!NOTE]
    >
    >You can map a single Workfront field to multiple Experience Manager Assets fields. You can't map multiple [!DNL Workfront] fields to a single [!DNL Experience Manager Assets] field.

1. In the **[!DNL Experience Manager Assets]** field, search through the pre-populated categories or enter at least two letters in the search field to access additional categories.
1. Repeat steps 2 and 3 as needed.
![folder metadata](assets/folder-metadata.png)
1. Click **[!UICONTROL Save]** or move on to the [Project metadata sync](#project-metadata-sync) section in this article.


### Object metadata sync

An [!DNL Experience Manager] fields that is mapped to [!DNL Workfront] portfolio, program, project, task, issue, and document fields update automatically when the field is changed in [!DNL Workfront].

When this option is enabled, any asset that has been pushed to Adobe Experience manager includes a card on the Document Details page that displays a real-time view of the document's Adobe Experience Manager metadata.

>[!IMPORTANT]
>
>Users must have write access in [!DNL Experience Manager] for assets living in the object in order for the metadata to sync when it's updated.

1. Enable the **[!UICONTROL Sync object metadata]** field.
1. Click **Save** or move on to the [Set up workflows (Optional)](#set-up-workflows-optional) section in this article.-->

## Einrichten von Workflows (optional)

Ein Workflow besteht aus einer Reihe von Aktionen, die Workfront mit Adobe Experience Manager as a Cloud Service verbinden. Als Workfront-Administrator können Sie Workflows in Workfront konfigurieren und sie dann Projektvorlagen zuweisen.

Wenn ein Projekt mit einer Projektvorlage erstellt wird, der ein Workflow zugewiesen ist, werden die im Workflow definierten Aktionen ausgelöst.

Workflows sind für die Adobe Experience Manager als Ganzes aktiviert und konfiguriert. Diese Workflows können dann auf Projektvorlagen angewendet werden. Sie können auf Vorlagenebene oder auf Projektebene angepasst oder angepasst werden, wenn ein Projekt aus dieser Vorlage erstellt wird.

Die folgenden Workflows sind in der Adobe Experience Manager-Integration verfügbar:

* [Mit Adobe Experience Manager verknüpfte Ordner erstellen](#create-adobe-experience-manager-linked-folders)
* [Publish-Assets, die an Adobe Experience Manager Assets gesendet werden](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Mit Adobe Experience Manager verknüpfte Ordner erstellen

1. Schalten Sie den Ordner **[!UICONTROL Verknüpften Ordner erstellen]** ein.
1. Geben Sie einen Namen für den Ordner ein, den Sie erstellen.
1. (Bedingt) Aktivieren Sie die Option **Standardordner-Struktur** , wenn Sie möchten, dass dieser verknüpfte Ordner der Standardordner für Projekte ist, die mit Vorlagen erstellt wurden, die diese Integration verwenden. Sie können einen oder mehrere Standardordner auswählen.
1. Wählen Sie einen Ordnerpfad aus, um anzugeben, wo alle mit dieser Integration verknüpften Ordner gespeichert werden sollen.
1. (Bedingt) Gehen Sie wie folgt vor, um dieser Integration eine Ordnerstruktur (verschachtelte Ordner) hinzuzufügen:

   1. Klicken Sie auf das Symbol **Ordner hinzufügen** ![Ordner hinzufügen](assets/add-folder-aem.png).
   1. Wählen Sie im Feld **Name type** aus, wie Sie den Ordner benennen möchten:

      * **Name**: Geben Sie einen Namen für den Ordner ein.
      * **Objektdaten**: Wählen Sie die Quelle für den Ordnernamen aus, z. B. den Projektnamen.

      >[!NOTE]
      >
      >* Ordnernamen dürfen weniger als 100 Zeichen enthalten.
      >* Die folgenden Zeichen werden aus den Ordnernamen entfernt:
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. Um einen verschachtelten Ordner zum Ordnerbaum hinzuzufügen, klicken Sie auf das Menü mit drei Punkten neben dem Ordner, in dem Sie einen verschachtelten Ordner erstellen möchten, und wählen Sie **Ordner hinzufügen** aus. Füllen Sie die Felder aus, wie im vorherigen Schritt unter Schritt beschrieben.
   1. Um einen Ordner mit Workfront zu verknüpfen, wählen Sie den Ordner aus und klicken Sie auf den Ordner &quot;**Verknüpften Ordner erstellen**&quot;   Symbol ![Ordner verknüpfen](assets/link-folder.png).
   1. (Optional) Um einen Ordner zu bearbeiten, wählen Sie den Ordner aus und klicken Sie auf das Symbol **Ordner bearbeiten** ![Symbol &quot;Bearbeiten&quot;](assets/edit-icon.png).
   1. (Optional) Um einen Ordner zu löschen, wählen Sie den Ordner aus und klicken Sie auf das Symbol **Ordner löschen** ![Ordner löschen](assets/delete-folder.png) .
1. (Bedingt) Um eine weitere Ordnerstruktur hinzuzufügen, klicken Sie auf **+ Ordnerstruktur hinzufügen** und führen Sie die Schritte in Schritt 5 aus.

1. Klicken Sie auf **[!UICONTROL Speichern]** oder wechseln Sie zum Abschnitt [Publish-Assets, die an Adobe Experience Manager Assets](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) gesendet werden, in diesem Artikel.

>[!NOTE]
>
>* Durch diese Integration werden nicht mehr als 100 Ordner erstellt, unabhängig davon, wie viele Ordnerbäume erstellt werden. Eine Integration mit 4 Ordnerbäumen kann beispielsweise bis zu 100 Ordner und nicht 400 Ordner erstellen.
>* Der erste Ordner in der Ordnerstruktur wird automatisch als mit Workfront verknüpft markiert. Wenn Sie nicht möchten, dass dieser Ordner verknüpft wird, können Sie die Verknüpfung aufheben.
>* Wenn keine Ordnerstruktur angegeben wird, wird der Stammordner zum verknüpften Ordner.


### Publish-Assets, die an Adobe Experience Manager Assets gesendet werden

1. Wechsel zu **[!UICONTROL Publish-Assets automatisch]**.
1. Aktivieren Sie das Kontrollkästchen neben dem Speicherort, an dem Sie Assets veröffentlichen möchten, die an Adobe Experience Manager-Assets gesendet werden. Sie können eine oder beide Optionen aktivieren.
1. (Bedingt) Wenn Sie die Option Brand Portal aktiviert haben, wählen Sie die Brand Portal aus, in der Sie Assets veröffentlichen möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]** oder wechseln Sie zum Abschnitt [Verknüpfte Ordner einrichten (optional)](#set-up-linked-folders-optional) in diesem Artikel.

## Verknüpfte Ordner einrichten (optional)

Sie können Benutzern erlauben, mit [!DNL Experience Manager] verknüpfte Ordner zu erstellen, während sie sich in einem [!DNL Workfront] -Projekt befinden. Wenn ein Ordner verknüpft ist, werden alle dem Ordner hinzugefügten Assets automatisch sowohl in [!DNL Workfront] als auch in [!DNL Experience Manager] angezeigt. Wenn zum ersten Mal ein Asset zum verknüpften Ordner in [!DNL Workfront] hinzugefügt wird, werden die Metadaten des Assets an [!DNL Experience Manager Assets] gesendet.

Geben Sie in den folgenden Schritten an, wo die verknüpften Ordner erstellt werden sollen. Jede Integration kann nur einen Speicherort für alle verknüpften Ordner haben.

Einrichten verknüpfter Ordner:

1. Schalten Sie den Ordner **[!UICONTROL Verknüpften Ordner aktivieren]** ein.
1. Wählen Sie einen Ordnerpfad aus, um anzugeben, wo alle mit dieser Integration verknüpften Ordner gespeichert werden sollen.

   >[!NOTE]
   >
   >Benutzer benötigen Schreibzugriff in [!DNL Adobe Experience Manager Assets] auf den Ordner, der zum Erstellen eines verknüpften Ordners angegeben ist.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
