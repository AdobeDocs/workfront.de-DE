---
product-area: documents
navigation-topic: approvals
title: Verwenden von Adobe Experience Manager mit der Frame.io-Integration
description: Verwenden von Adobe Experience Manager mit der Frame.io-Integration
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: cb2a17991a5562c6e734eaa0ada781d706dc5a77
workflow-type: tm+mt
source-wordcount: '1614'
ht-degree: 0%

---


# Verwenden von Adobe Experience Manager mit der Frame.io-Integration

Sie können die [!DNL Experience Manager Assets]&#x200B;&#x200B; verwenden, um Ihre digitalen Assets zu verwalten und zu speichern, die den Überprüfungs- und Genehmigungszyklus durchlaufen haben. Durch diese Integration können Sie die Funktionen von Adobe Experience Manager, Frame.io und Workfront nutzen, um Ihr Content-Management und Ihre Kollaborationsprozesse zu optimieren.

## Konfigurieren der Experience Manager Assets-Integration

Sie können Ihre Arbeit mit Ihren Inhalten in [!DNL Experience Manager Assets] verbinden&#x200B;:

* Pushen von Assets und Metadaten von [!DNL Adobe Workfront] nach [!DNL Experience Manager Assets]&#x200B;
* Anwendungsfälle für die Versionierung vereinfachen
* Nachverfolgen von Metadaten für Assets
* Synchronisieren von Projektmetadaten zwischen [!DNL Workfront] und [!DNL Experience Manager Assets]

>[!NOTE]
>
>Sie können auch mehrere [!DNL Experience Manager Assets]-Repositorys mit einer [!UICONTROL Workfront]-Umgebung oder mehrere [!DNL Workfront]-Umgebungen über Organisations-IDs hinweg mit einem [!DNL Experience Manager Assets]-Repository verbinden. Befolgen Sie die Konfigurationsanweisungen in diesem Artikel für jede Integration, die Sie einrichten möchten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td>
  <p>So konfigurieren Sie die Integration:</p>
   <p>Standard</p>
   <p>Plan</p>

<p>So senden Sie Dokumente an Experience Manager Assets:</p>
   <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p>
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
* Ihre Workfront-Instanz muss Adobe Enterprise Storage verwenden.


## Einrichten der Integrationsinformationen

{{step-1-to-setup}}

1. Wählen **[!UICONTROL im linken]** „Dokumente“ und dann **[!UICONTROL [!DNL Experience Manager]Integration]**.
1. Wählen **[!UICONTROL Integration [!DNL Experience Manager] hinzufügen]**.
1. Geben Sie im Feld **[!UICONTROL Name]** den Namen ein, den Benutzer sehen sollen, wenn sie mit dieser Integration in Workfront und Experience Manager Assets interagieren.
1. Im Feld **[!UICONTROL Navigations-URL]** füllt das System automatisch die Navigations-URL. Diese schreibgeschützte URL wird verwendet, um über das Hauptmenü eine Verknüpfung mit der [!DNL Experience Manager]-Instanz Ihrer Organisation [!UICONTROL &#x200B; erstellen] um Schnellzugriff zu erhalten.
1. Wählen Sie ein Repository aus dem Dropdown-Menü **[!UICONTROL [!DNL Experience Manager]Assets]** Repository aus. Das System füllt automatisch alle [!DNL Experience Manager]-Repositorys, die mit der Organisations-ID verknüpft sind, der Ihr Benutzerprofil zugewiesen ist.
   ![Wählen Sie das Experience Manager-Repository](assets/setup-information.png)

1. Klicken Sie **[!UICONTROL Speichern]** oder gehen Sie zum Abschnitt [Einrichten von Metadaten (Optional](#set-up-metadata-optional) in diesem Artikel.

   >[!IMPORTANT]
   >
   >Aufgrund der Komplexität der Integration können Sie das Repository nach dem Speichern der ersten Konfiguration nicht mehr ändern.


## Einrichten von Metadaten (optional)

Sie können [!DNL Workfront] Objektdaten Asset-Medienfeldern in [!DNL Experience Manager] Assets zuordnen.

>[!NOTE]
>
>Metadaten können nur in eine Richtung zugeordnet werden: von [!DNL Workfront] zu [!DNL Experience Manager]. Metadaten für Dokumente, die mit [!DNL Workfront] von [!DNL Experience Manager] verknüpft sind, können nicht an [!DNL Workfront] übertragen werden.

### Metadatenfelder konfigurieren

Bevor Sie mit der Zuordnung von Metadatenfeldern beginnen, müssen Sie Metadatenfelder sowohl in Workfront als auch in Experience Manager Assets konfigurieren.

So konfigurieren Sie Metadatenfelder:

1. Konfigurieren Sie ein Metadatenschema in [!DNL Experience Manager Assets], wie unter [Konfigurieren der Asset-Metadatenzuordnung zwischen Adobe  [!DNL Workfront]  und  [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/de/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


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

Weitere Informationen zu Tags in Experience Manager Assets, einschließlich der Erstellung und Verwaltung von Tags, finden Sie unter [Verwalten von Tags](https://experienceleague.adobe.com/de/docs/experience-manager-64/administering/contentmanagement/tags).

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
   >Sie können ein einzelnes [!DNL Workfront] mehreren [!UICONTROL Experience Manager Assets-Feldern &#x200B;]. Sie können nicht mehrere [!DNL Workfront] einem einzelnen [!DNL Experience Manager Assets] zuordnen.
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. Suchen Sie im Feld [!DNL Experience Manager Assets] nach den vorausgefüllten Kategorien oder geben Sie mindestens zwei Buchstaben in das Suchfeld ein, um auf zusätzliche Kategorien zuzugreifen.
1. Wiederholen Sie die Schritte 2 und 3 nach Bedarf.
   ![Metadatenfelder](assets/metadata-no-asset-toggle.png)
1. Klicken Sie [!UICONTROL **Speichern**] oder wechseln Sie zum Abschnitt [Synchronisierung von Objektmetadaten](#object-metadata-sync) in diesem Artikel.



### Synchronisierung von Objektmetadaten

[!DNL Experience Manager] Felder, die [!DNL Workfront] Portfolio-, Programm-, Projekt-, Aufgaben-, Problem- und Dokumentfeldern zugeordnet sind, werden automatisch aktualisiert, wenn das Feld in [!DNL Workfront] geändert wird.

Wenn diese Option aktiviert ist, zeigt jedes Asset, das auf Adobe Experience Manager gepusht wurde, auf der Seite Dokumentdetails in Workfront eine Echtzeitansicht der Adobe Experience Manager-Metadaten des Dokuments an.

1. Aktivieren Sie das Feld **[!UICONTROL Objektmetadaten synchronisieren]** und klicken Sie dann auf **Speichern**.

>[!IMPORTANT]
>
>Benutzer müssen über Schreibzugriff in [!DNL Experience Manager] für Assets verfügen, die sich im -Objekt befinden, damit die Metadaten bei der Aktualisierung synchronisiert werden können.


## Senden eines Dokuments an Experience Manager Assets oder Assets Essentials

Sie können Dokumente von Workfront an Experience Manager Assets oder Assets Essentials senden. Dokumente, die von Workfront hochgeladen und an Assets Essentials gesendet wurden, werden weiterhin für den gesamten Dokumentspeicher gezählt.

Für Assets, die über diese Integration an Experience Manager gesendet werden, gilt eine Größenbeschränkung von **5 GB**.

<!--In the Preview environment, Assets sent to Experience Manager through this integration have a size limit of **30 GB**.-->

Metadatenfelder werden zuerst zugeordnet, wenn Sie ein Asset von Workfront an Experience Manager Assets oder Assets Essentials senden. Alle Metadaten, die für die Zuordnung übergeordneter Objekte konfiguriert wurden, werden ebenfalls gesendet. Weitere Informationen zum Konfigurieren der Metadatenzuordnung finden Sie unter [Konfigurieren der Experience Manager Assets as a Cloud Service-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) oder [Konfigurieren der Experience Manager Assets Essentials-Integration](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Beispiel** Wenn Sie zum ersten Mal ein an ein Projekt angehängtes Asset senden, werden die Metadaten Experience Manager Assets oder Assets Essentials sowie allen zugeordneten Metadaten von übergeordneten Objekten wie einem Portfolio und einem Programm zugeordnet.



### Senden eines Dokuments aus Workfront

Wenn ein(e) Benutzende(r) ein Dokument von Workfront an Experience Manager Assets oder Assets Essentials sendet, werden zugeordnete Metadaten entlang des Dokuments übertragen. Nachdem das Dokument gesendet wurde, werden Änderungen an den Metadaten des Dokuments in Workfront nicht in Assets oder Assets Essentials übernommen. Wenn ein zugeordnetes Feld in Workfront geändert wird, müssen Sie eine neue Version des Dokuments mit den aktualisierten Metadaten an Assets oder Assets Essentials senden.

Senden eines Dokuments:

1. Wechseln Sie zum Bereich **Dokumente** in Workfront und wählen Sie das Dokument aus, das Sie senden möchten.
1. Klicken Sie **Senden an** und wählen Sie dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und darf daher Assets oder Assets Essentials nicht explizit erwähnen.

   ![Senden an](assets/send-to-aem.png)

1. Wählen Sie aus, wohin das Asset gesendet werden soll, und klicken Sie dann auf **Ordner auswählen**.
1. Wenn Sie das gewünschte Ziel gefunden haben, klicken Sie auf **Speichern**.

### Neue Version senden

Sie können zu einem Dokument, das Sie zuvor in Workfront hochgeladen haben, eine neue Version hinzufügen. Weitere Informationen finden Sie unter [Hochladen einer neuen Version eines Dokuments](/help/quicksilver/documents/managing-documents/upload-new-document-version.md). Nachdem die neueste Version hochgeladen wurde, können Sie sie an Assets Essentials senden. Wenn sich ein zugeordnetes Feld in Workfront geändert hat, aktualisiert die neue Version beim Senden die Metadaten in Assets Essentials.

>[!IMPORTANT]
>
>Bevor Sie eine neue Version in Workfront hochladen, empfehlen wir, die Datei umzubenennen. Wenn Sie eine neue Version mit genau demselben Dateinamen wie eine frühere Version hochladen, kann nur die neueste Version von Workfront heruntergeladen werden. Alle Versionen können unabhängig vom Dateinamen von Experience Manager Assets oder Assets Essentials heruntergeladen werden. <!--Is this still a thing with ESM?-->

So senden Sie die neueste Version:

1. Navigieren Sie zum Bereich **Dokumente** in Workfront und suchen Sie das Dokument.
1. Wählen Sie **Senden an** und dann die Experience Manager-Integration aus, die Ihr Administrator eingerichtet hat.

   >[!NOTE]
   >
   >Der Workfront-Administrator kann einen beliebigen Namen für diese Integration auswählen und erwähnt daher möglicherweise nicht speziell Assets oder Assets Essentials.

   ![Senden an](assets/send-to-aem.png)

1. Klicken Sie auf **Speichern**. Die neue Version wird am selben Speicherort wie die vorherige Version gespeichert.
