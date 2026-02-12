---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Integration mit [!UICONTROL Experience Manager Assets as a Cloud Service] konfigurieren
description: Sie können Ihre Arbeit mit Ihren Inhalten in  [!DNL Experience Manager Assets].
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 315428ec517b3a6c0edae387b3a866093a49a2b2
workflow-type: tm+mt
source-wordcount: '1713'
ht-degree: 1%

---

# Integration mit [!UICONTROL Experience Manager Assets as a Cloud Service] konfigurieren

<!-- Audited: 1/2024 -->


>[!IMPORTANT]
>
>Diese Funktion steht nur Organisationen zur Verfügung, die in das [!DNL Adobe Admin Console] integriert wurden.

Sie können Ihre Arbeit mit Ihren Inhalten in [!DNL Experience Manager Assets] verbinden&#x200B;:

* Pushen von Assets und Metadaten von [!DNL Adobe Workfront] nach [!DNL Experience Manager Assets]&#x200B;
* Verknüpfen von Assets aus [!DNL Experience Manager Assets] mit Ihren Projekten und Aufgaben in [!DNL Workfront&#x200B;]
* Anwendungsfälle für die Versionierung vereinfachen
* Mit [!DNL Experience Manager Assets] verknüpfte Ordner erstellen
* Nachverfolgen von Metadaten für Assets und Ordner
* Synchronisieren von Projektmetadaten zwischen [!DNL Workfront] und [!DNL Experience Manager Assets]

>[!NOTE]
>
>Sie können auch mehrere [!DNL Experience Manager Assets]-Repositorys mit einer [!UICONTROL Workfront]-Umgebung oder mehrere [!DNL Workfront]-Umgebungen über Organisations-IDs hinweg mit einem [!DNL Experience Manager Assets]-Repository verbinden. Befolgen Sie die Konfigurationsanweisungen in diesem Artikel für jede Integration, die Sie einrichten möchten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table>
  <tr>
   <td>Adobe Workfront-Paket
   </td>
   <td> <p>Prime oder Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Adobe Workfront-Lizenzen
   </td>
   <td>Standard
   <p>Plan</p>
   </td>
  </tr>
  </tr>
    <tr>
   <td>Adobe Experience Manager-Lizenzen
   </td>
   <td>Standard
   </td>
  </tr>
  <tr>
   <td>Zusätzliche Produkte
   </td>
   <td>Sie müssen über [!DNL Experience Manager Assets as a Cloud Service] verfügen und als Benutzer zum Produkt hinzugefügt werden.
   </td>
  </tr>
   <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen,

* Sie müssen über [!DNL Workfront] und [!DNL Adobe Experience Manager Assets] verfügen, die mit einer Organisations-ID im [!DNL Adobe Admin Console] verknüpft sind. Weitere Informationen finden Sie unter [Unterschiede bei der plattformbasierten Administration ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Einrichten der Integrationsinformationen

{{step-1-to-setup}}

1. Wählen **[!UICONTROL im linken]** „Dokumente“ und dann **[!UICONTROL [!DNL Experience Manager]Integration]**.

   >[!NOTE]
   >
   >Dieser Konfigurationsbereich wird nur angezeigt, wenn Ihre [!DNL Workfront] unter einem [!DNL Adobe Admin Console] enthalten ist.

1. Wählen **[!UICONTROL Integration [!DNL Experience Manager] hinzufügen]**.
1. Geben Sie im Feld **[!UICONTROL Name]** den Namen ein, den Benutzer sehen sollen, wenn sie mit dieser Integration in Workfront und Experience Manager Assets interagieren.
1. Im Feld **[!UICONTROL Navigations-URL]** füllt das System automatisch die Navigations-URL. Diese schreibgeschützte URL wird verwendet, um über das Hauptmenü eine Verknüpfung mit der [!DNL Experience Manager]-Instanz Ihrer Organisation [!UICONTROL  erstellen] um Schnellzugriff zu erhalten.
1. Wählen Sie ein Repository aus dem Dropdown-Menü **[!UICONTROL [!DNL Experience Manager]Assets]** Repository aus. Das System füllt automatisch alle [!DNL Experience Manager]-Repositorys, die mit der Organisations-ID verknüpft sind, der Ihr Benutzerprofil zugewiesen ist.
   ![Wählen Sie das Experience Manager-Repository](assets/setup-information.png)

1. Klicken Sie **[!UICONTROL Speichern]** oder gehen Sie zum Abschnitt [Einrichten von Metadaten (Optional](#set-up-metadata-optional) in diesem Artikel.

   >[!NOTE]
   >
   >Aufgrund der Komplexität der Integration können Sie das Repository nach dem Speichern der ersten Konfiguration nicht mehr ändern.

## Einrichten von Metadaten (optional)

Sie können [!DNL Workfront] Objektdaten Asset-Medienfeldern in [!DNL Experience Manager] Assets zuordnen.

>[!IMPORTANT]
>
>Metadaten können nur in eine Richtung zugeordnet werden: von [!DNL Workfront] zu [!DNL Experience Manager]. Metadaten für Dokumente, die mit [!DNL Workfront] von [!DNL Experience Manager] verknüpft sind, können nicht an [!DNL Workfront] übertragen werden.

### Metadatenfelder konfigurieren

Bevor Sie mit der Zuordnung von Metadatenfeldern beginnen, müssen Sie Metadatenfelder sowohl in Workfront als auch in Experience Manager Assets konfigurieren.

So konfigurieren Sie Metadatenfelder:

1. Konfigurieren Sie ein Metadatenschema in [!DNL Experience Manager Assets], wie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe  [!DNL Workfront]  und  [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


1. Konfigurieren von benutzerdefinierten Formularfeldern in Workfront. [!DNL Workfront] verfügt über viele integrierte benutzerdefinierte Felder, die Sie verwenden können. Sie können jedoch auch eigene benutzerdefinierte Felder erstellen, wie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) beschrieben.

+++ **Erweitern Sie , um weitere Informationen zu unterstützten Feldern von Workfront und Experience Manager Assets anzuzeigen** 

**Experience Manager Assets-Tags**

Sie können jedes von Workfront unterstützte Feld einem Tag in Experience Manager Assets zuordnen. Dazu müssen Sie sicherstellen, dass die Tag-Werte in Experience Manager Assets mit Workfront übereinstimmen.

* Tags- und Workfront-Feldwerte müssen in Schreibweise, Formatierung und Format exakt übereinstimmen.
* Workfront-Feldwerte, die Experience Manager Assets-Tags zugeordnet sind, müssen vollständig in Kleinbuchstaben geschrieben sein, auch wenn das Tag in Experience Manager Assets scheinbar Großbuchstaben enthält.
* Workfront-Feldwerte dürfen keine Leerzeichen enthalten.
* Der Feldwert in Workfront muss auch die Ordnerstruktur des Experience Manager Assets-Tags enthalten.
* Um mehrere einzeilige Textfelder Tags zuzuordnen, geben Sie eine kommagetrennte Liste der Tag-Werte in die Workfront-Seite der Metadatenzuordnung ein und `xcm:keywords` auf der Experience Manager Assets-Seite. Jeder Feldwert wird einem separaten Tag zugeordnet. Sie können ein berechnetes Feld verwenden, um mehrere Workfront-Felder in einem einzigen, durch Kommas getrennten Textfeld zu kombinieren.
* Sie können Werte aus Dropdown-, Optionsfeld- oder Kontrollkästchen-Feldern zuordnen, indem Sie eine kommagetrennte Liste der verfügbaren Werte in diesem Feld eingeben.


>[!INFO]
>
>**Beispiel**: Damit das Tag mit dem übereinstimmt, das in der Ordnerstruktur hier angezeigt wird, würde der Feldwert in Workfront `landscapes:trees/spruce`. Beachten Sie die Kleinbuchstaben im Workfront-Feldwert.
>
>Wenn Sie möchten, dass das Tag in der Tag-Struktur ganz links ist, muss ihm ein Doppelpunkt folgen. In diesem Beispiel würde der Feldwert in Workfront `landscapes:`, um die Zuordnung zum Tag „Querformat“ vorzunehmen.
>
>![Ordnerstruktur in AEM](assets/aem-folder-structure-with-red-boxes.png)


Nachdem Sie die Tags in Experience Manager Assets erstellt haben, werden sie unter der Dropdown-Liste „Tags“ im Abschnitt „Metadaten“ angezeigt. Um ein Feld mit einem Tag zu verknüpfen, wählen Sie `xcm:keywords` in der Dropdown-Liste Experience Manager Assets-Feld im Bereich für die Metadatenzuordnung aus.

Weitere Informationen zu Tags in Experience Manager Assets, einschließlich der Erstellung und Verwaltung von Tags, finden Sie unter [Verwalten von Tags](https://experienceleague.adobe.com/en/docs/experience-manager-64/administering/contentmanagement/tags).

**Benutzerdefinierte Experience Manager Assets-Metadatenschemafelder**

Sie können sowohl integrierte als auch benutzerdefinierte Workfront-Felder benutzerdefinierten Metadatenschemafeldern in Experience Manager Assets zuordnen.

Benutzerdefinierte Metadatenfelder, die in Experience Manager Assets erstellt werden, sind im Bereich „Metadaten-Setup“ in einem eigenen Abschnitt organisiert.

![Benutzerdefinierter Metadatenabschnitt](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Workfront-Felder**

Sie können sowohl integrierte als auch benutzerdefinierte Workfront-Felder Experience Manager Assets zuordnen. Die folgenden Feldwerte müssen sowohl in Groß- als auch in Kleinschreibung zwischen Workfront und Experience Manager Assets übereinstimmen:

* Dropdown-Felder
* Felder mit Mehrfachauswahl

>[!TIP]
>
> Um zu überprüfen, ob die Feldwerte genau übereinstimmen, gehen Sie zu
>
> * Setup > Benutzerdefinierte Forms in Workfront oder das Feld im -Objekt
> * Assets > Metadatenschemata in Experience Manager Assets

+++

### Zuordnen von Metadaten für Assets

Metadaten werden zugeordnet, wenn ein Asset zum ersten Mal aus [!DNL Workfront] gepusht wird. Dokumente mit den integrierten oder benutzerdefinierten Feldern werden beim ersten Versand eines Assets an [!DNL Experience Manager Assets] automatisch den angegebenen Feldern zugeordnet.

Zuordnen von Metadaten für Assets:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. Wählen Sie in der **[!UICONTROL [!DNL Workfront]&quot;]**&quot; ein integriertes oder ein benutzerdefiniertes Workfront-Feld aus.

   >[!NOTE]
   >
   >Sie können ein einzelnes [!DNL Workfront] mehreren [!UICONTROL Experience Manager Assets-Feldern ]. Sie können nicht mehrere [!DNL Workfront] einem einzelnen [!DNL Experience Manager Assets] zuordnen.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Suchen Sie im Feld [!DNL Experience Manager Assets] nach den vorausgefüllten Kategorien oder geben Sie mindestens zwei Buchstaben in das Suchfeld ein, um auf zusätzliche Kategorien zuzugreifen.
1. Wiederholen Sie die Schritte 2 und 3 nach Bedarf.
   ![Metadatenfelder](assets/metadata-no-asset-toggle.png)
1. Klicken Sie [!UICONTROL Speichern] oder gehen Sie zum Abschnitt [Einrichten von Workflows](#set-up-workflows-optional) in diesem Artikel.

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

Ein Workflow ist eine Reihe von Aktionen, die Workfront mit Adobe Experience Manager as a Cloud Service verbinden. Als Workfront-Administrator können Sie Workflows in Workfront konfigurieren und dann Projektvorlagen zuweisen.

Wenn ein Projekt mithilfe einer Projektvorlage erstellt wird, der ein Workflow zugewiesen ist, werden die im Workflow definierten Aktionen ausgelöst.

Workflows sind für die Adobe Experience Manager als Ganzes aktiviert und konfiguriert. Diese Workflows können dann auf Projektvorlagen angewendet werden. Sie können auf Vorlagenebene oder auf Projektebene angepasst werden, wenn ein Projekt aus dieser Vorlage erstellt wird.

Die folgenden Workflows sind in der Adobe Experience Manager-Integration verfügbar:

* [Erstellen von mit Adobe Experience Manager verknüpften Ordnern](#create-adobe-experience-manager-linked-folders)
* [Veröffentlichen von Assets, die an Adobe Experience Manager Assets gesendet werden](#publish-assets-that-are-sent-to-adobe-experience-manager-assets)

### Erstellen von mit Adobe Experience Manager verknüpften Ordnern

Sie können pro Ordnerstruktur bis zu 100 verknüpfte Ordner erstellen.

1. Schalten Sie **[!UICONTROL Verknüpften Ordner erstellen]** ein.
1. Geben Sie einen Namen für den verknüpften Ordner ein, den Sie erstellen.
1. (Bedingt) Aktivieren Sie die Option **Standardordnerhierarchie**, wenn dieser verknüpfte Ordner der Standardordner für Projekte sein soll, die mit Vorlagen erstellt wurden, die diese Integration verwenden. Sie können einen oder mehrere Standardordner auswählen.
1. Wählen Sie einen Ordnerpfad aus, um anzugeben, wo alle verknüpften Ordner mit dieser Integration sein sollen.
1. (Bedingt) Gehen Sie wie folgt vor, um dieser Integration eine Ordnerstruktur (verschachtelte Ordner) hinzuzufügen:

   1. Klicken Sie auf **Symbol** Ordner hinzufügen![ (Ordner hinzufügen](assets/add-folder-aem.png).
   1. Wählen Sie im Feld **Name** aus, wie Sie den Ordner benennen möchten:

      * **Name**: Geben Sie einen Namen für den Ordner ein.
      * **Objektdaten**: Wählen Sie die Quelle für den Ordnernamen aus, z. B. Projektnamen.

      >[!NOTE]
      >
      >* Ordnernamen müssen weniger als 100 Zeichen lang sein.
      >* Die folgenden Zeichen werden aus Ordnernamen entfernt:
      >
      >   `/`, `:`, `[`, `]`, `|`, `*`

   1. Um einen verschachtelten Ordner zur Ordnerstruktur hinzuzufügen, klicken Sie auf das Dreipunkt-Menü neben dem Ordner, in dem Sie einen verschachtelten Ordner erstellen möchten, und wählen Sie **Ordner hinzufügen**. Füllen Sie die Felder wie im vorherigen Schritt beschrieben aus.
   1. Um einen Ordner mit Workfront zu verknüpfen, wählen Sie den Ordner aus und klicken Sie auf **Verknüpften Ordner erstellen**   Symbol ![Verknüpfungsordner](assets/link-folder.png).
   1. (Optional) Um einen Ordner zu bearbeiten, wählen Sie den Ordner aus und klicken Sie auf das **Ordner bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).
   1. (Optional) Um einen Ordner zu löschen, wählen Sie den Ordner aus und klicken Sie auf das Symbol **Ordner löschen** ![Ordner löschen](assets/delete-folder.png).
1. (Bedingt) Um eine weitere Ordnerstruktur hinzuzufügen, klicken Sie auf **+ Ordnerstruktur hinzufügen** führen Sie die Schritte in Schritt 5 aus.

1. Klicken Sie **[!UICONTROL Speichern]** oder gehen Sie zum Abschnitt [Veröffentlichen von Assets, die an Adobe Experience Manager Assets gesendet werden](#publish-assets-that-are-sent-to-adobe-experience-manager-assets) in diesem Artikel.


>[!NOTE]
>
>* Die native Workfront AEM-Integration kann **maximal 100 Ordner pro Projekt pro Integration** erstellen, unabhängig davon, wie viele Ordnerbäume enthalten sind.
>   * Beispiel: Eine Integration mit vier Ordnerbäumen in einem Projekt kann bis zu 100 Ordner insgesamt erstellen - nicht 400.
>* Der erste Ordner in jeder Ordnerstruktur wird automatisch als mit Workfront verknüpft markiert. Wenn dieser Ordner nicht verknüpft werden soll, können Sie den Link aufheben.
>* Wenn keine Ordnerstruktur bereitgestellt wird, wird der Stammordner zum verknüpften Ordner.




### Veröffentlichen von Assets, die an Adobe Experience Manager Assets gesendet werden

1. Schalten Sie **[!UICONTROL Assets automatisch veröffentlichen]** ein.
1. Aktivieren Sie das Kontrollkästchen neben dem Speicherort, an dem Sie an Adobe Experience Manager Assets gesendete Assets veröffentlichen möchten. Sie können eine oder beide Optionen aktivieren.
1. (Bedingt) Wenn Sie die Option &quot;Brand Portal&quot; aktiviert haben, wählen Sie die Brand Portal aus, in der Sie Assets veröffentlichen möchten.
1. Klicken Sie **[!UICONTROL Speichern]** oder gehen Sie zum Abschnitt [Einrichten verknüpfter Ordner (Optional](#set-up-linked-folders-optional) in diesem Artikel.

## Verknüpfte Ordner einrichten (optional)

Sie können Benutzern erlauben, in einem [!DNL Experience Manager] Projekt Ordner zu erstellen, die mit [!DNL Workfront] verknüpft sind. Wenn ein Ordner verknüpft ist, wird jedes zum Ordner hinzugefügte Asset automatisch sowohl in [!DNL Workfront] als auch in [!DNL Experience Manager] angezeigt. Wenn ein Asset zum ersten Mal zum verknüpften Ordner in [!DNL Workfront] hinzugefügt wird, werden die Metadaten des Assets an [!DNL Experience Manager Assets] gesendet.

In den folgenden Schritten geben Sie an, wo die verknüpften Ordner erstellt werden sollen. Jede Integration kann für alle verknüpften Ordner nur einen Speicherort haben.

So richten Sie verknüpfte Ordner ein:

1. Schalten Sie **[!UICONTROL Verknüpften Ordner aktivieren]** ein.
1. Wählen Sie einen Ordnerpfad aus, um anzugeben, wo alle verknüpften Ordner mit dieser Integration sein sollen.

   >[!NOTE]
   >
   >Benutzende benötigen Schreibzugriff in [!DNL Adobe Experience Manager Assets] auf den Ordner, der zum Erstellen eines verknüpften Ordners angegeben wurde.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
