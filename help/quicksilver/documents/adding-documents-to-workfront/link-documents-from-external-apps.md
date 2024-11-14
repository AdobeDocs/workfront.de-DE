---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Verknüpfen von Dokumenten mit externen Anwendungen
description: Sie können Dokumente und Ordner aus externen Quellen mit Adobe Workfront verknüpfen.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 97823f70-6544-445a-9a81-abe1e2f3de55
source-git-commit: fde2ad9a8ef1b7f659f8f52c157726d0562b972a
workflow-type: tm+mt
source-wordcount: '2608'
ht-degree: 0%

---

# Verknüpfen von Dokumenten mit externen Anwendungen

<!-- Audited: 01/2024 -->

Sie können Dokumente und Ordner aus den folgenden Quellen mit Adobe Workfront verknüpfen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Vorhandene Drittanbieter von Cloud-Dokumenten</td> 
   <td>Dazu gehören die folgenden: 
    <ul> 
     <li>Box</li> 
     <li>Dropbox</li> 
     <li>Dropbox Business</li> 
     <li>WebDAM</li> 
     <li>Microsoft OneDrive</li> 
     <li>Microsoft SharePoint</li> 
     <li>Google Drive</li> 
     <li>Quip</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront-Korrekturabzug </td> 
   <td>Sie können Testsendungen, die ursprünglich in Workfront Proof erstellt wurden, in Workfront verfügbar machen. Für die aktuellen Lizenzen ist ein Pro Workfront-Plan oder höher erforderlich, um diese Funktion verwenden zu können. Für die neuen Lizenzen enthalten alle Pläne diese Funktion. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter <a href="https://www.workfront.com/plans">Workfront-Pläne</a>.</td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td role="rowheader">Experience Manager Assets Essentials </td> 
   <td>Sie können Dokumente über Experience Manager Assets Essentials mit Workfront verknüpfen. Weitere Informationen finden Sie unter <a href="../../documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md" class="MCXref xref"> Adobe Workfront for Experience Manager Assets Essentials</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront DAM </td> 
   <td>Dies erfordert einen zusätzlichen Kauf. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Andere Dokumentenanbieter (über benutzerdefinierte Dokumentenintegrationen)</td> 
   <td> <p class="workfront_plans">Für die aktuellen Lizenzen ist ein Pro Workfront-Plan oder höher erforderlich, um diese Funktion verwenden zu können. Für die neuen Lizenzen enthalten alle Pläne diese Funktion. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter <a href="https://www.workfront.com/plans">Workfront-Pläne</a>.</p> </td>
  </tr> 
 </tbody> 
</table>

Bevor Sie Dokumente oder Ordner verknüpfen, muss Ihr Workfront-Administrator diese Funktion für jeden Dokumentenanbieter oder für eine benutzerdefinierte Dokumentintegration aktivieren, wie unter [Dokumentintegrationen konfigurieren](../../administration-and-setup/configure-integrations/configure-document-integrations.md) beschrieben.

Sie können Dokumente, die mit einem externen Cloud-Anbieter verknüpft sind, auf die gleiche Weise wie Dokumente, die direkt in Workfront hochgeladen wurden, testen und genehmigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td>
   <td> <p> Alle</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td>
   <td><p>Neu: Mitarbeiter oder höher</p>
    <p>oder</p>
    <p>Aktuell: Anforderung oder höher</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dokumentenspeicher

Dokumente, die von einer externen Anwendung mit Workfront verknüpft sind, werden mit dem externen Cloud-Anbieter und nicht innerhalb von Workfront gespeichert.

Es gelten die folgenden Ausnahmen:

* Wenn sie vom Document Service bereitgestellt werden, können Miniaturansichten und Vorschaubilder auf Workfront-Servern gespeichert werden.
* Wenn Sie in Workfront Testsendungen verwenden, wird das Dokument kopiert und den Testservern hinzugefügt.

## Verknüpfen eines Dokuments aus einer externen Anwendung mit Workfront

Sie können vorhandene Dokumente mit einem externen Cloud-Anbieter verknüpfen. Dies umfasst alle freigegebenen Dokumente.

### Voraussetzungen {#prerequisites}

Bevor Sie Dokumente oder Ordner verknüpfen, muss Ihr Workfront-Administrator diese Funktion für jeden Dokumentenanbieter oder für eine benutzerdefinierte Dokumentintegration aktivieren, wie unter [Dokumentintegrationen konfigurieren](../../administration-and-setup/configure-integrations/configure-document-integrations.md) beschrieben.

### Externes Dokument mit Workfront verknüpfen {#link-an-external-document-to-workfront}

Sie können Dokumente über eine externe Anwendung wie Google und Microsoft OneDrive mit Workfront verknüpfen.

>[!IMPORTANT]
>
>Dropbox speichert Dokumente basierend auf dem Dateipfad. Aus diesem Grund ist der Zugriff auf eine von Dropbox verknüpfte Datei in Workfront nicht mehr möglich, wenn sie verschoben, umbenannt oder gelöscht wird.

1. Wechseln Sie zum Bereich **Dokumente** in Workfront, in dem Sie das Dokument speichern möchten.
1. Klicken Sie auf **Neu hinzufügen** und dann auf den externen Dokumentenanbieter, mit dem Sie Dokumente mit Workfront verknüpfen möchten.

   Um beispielsweise Dokumente von Dropbox zu verknüpfen, klicken Sie auf **Von Dropbox**.

   Externe Anbieter, die Sie bereits autorisiert haben, werden oben in der Liste angezeigt.

1. (Bedingt) Wenn Sie aufgefordert werden, sich beim externen Dienst anzumelden, geben Sie Ihre Anmeldedaten für den Dienst in das Feld ein, das angezeigt wird, und klicken Sie dann auf **Anmelden**.
1. (Bedingt) Wenn Sie aufgefordert werden, die externe Anwendung zu autorisieren, klicken Sie auf die Schaltfläche **Autorisieren** .

   Du musst das nur einmal machen.

1. Geben Sie im Suchfeld des angezeigten Felds **Externe Dateien und Ordner verknüpfen** den Namen des Elements ein, nach dem Sie suchen möchten, und drücken Sie dann die Eingabetaste **Enter** , um alle Ergebnisse aus der externen Anwendung anzuzeigen, unabhängig davon, in welchem Ordner sie gespeichert sind.

   Oder

   Suchen Sie die Dokumente, die Sie verknüpfen möchten, und wählen Sie sie aus.

   Sie können zwar mehrere Dokumente auswählen, es werden jedoch nur die in der aktuellen Ansicht ausgewählten Dokumente verknüpft. Wenn Sie beispielsweise ein Dokument auswählen und dann in einen Ordner wechseln, wird das ursprünglich ausgewählte Dokument nicht verknüpft.

1. (Bedingt) Wenn Sie Workfront DAM-Kunde sind, klicken Sie auf das Symbol **Miniaturansicht** , um Dateien als Miniaturansichten anzuzeigen.

   >[!NOTE]
   >
   >Workfront DAM-Kunden können beim Verknüpfen von Dokumenten aus Workfront DAM Miniaturansichten anzeigen. Miniaturansichten werden möglicherweise auch für Workfront DAM-Kunden für andere Dienste wie Dropbox und Box angezeigt. Das Anzeigen von Miniaturansichten für andere Dienste als Workfront DAM in Workfront wird jedoch nicht unterstützt und Miniaturansichten werden beim Verknüpfen von Dokumenten von SharePoint oder Google Drive nie angezeigt.

1. Klicken Sie auf **Link**.

   In Workfront wird neben den Dokumenten das Symbol des Cloud-Anbieters angezeigt.

   >[!NOTE]
   >
   >* Wenn die zum Verknüpfen des Dokuments verwendete Download-URL 2048 Zeichen überschreitet, kann die Datei nicht verknüpft werden.
   >* Bei Dokumenten, die mit &quot;Feld&quot;verknüpft sind, wird der Link zum Dokument im Feld erst angezeigt, wenn Sie die Seite aktualisieren.

### Hinzufügen einer neuen Version eines verknüpften Dokuments {#add-a-new-version-of-a-linked-document}

Sie können eine neue Version eines mit Workfront verknüpften Dokuments aus einer externen Anwendung hinzufügen.

1. Wechseln Sie zum Bereich **Dokumente** , in dem das Dokument verknüpft ist, und wählen Sie dann das verknüpfte Dokument aus.

   >[!IMPORTANT]
   >
   >Das Dokument muss sich außerhalb eines verknüpften Ordners befinden, um eine neue Version zu erstellen.

1. Klicken Sie auf **Neu hinzufügen** > **Version** und dann auf den externen Dokumentanbieter.

   Um beispielsweise eine neue Dokumentversion von Dropbox aus zu verknüpfen, klicken Sie auf **Von Dropbox**.

   Externe Anbieter, die Sie bereits autorisiert haben, werden oben in der Liste angezeigt.

1. (Bedingt) Wenn Sie aufgefordert werden, sich beim externen Dienst anzumelden, geben Sie Ihre Anmeldedaten für den Dienst in das Feld ein, das angezeigt wird, und klicken Sie dann auf **Anmelden**.
1. (Bedingt) Wenn Sie aufgefordert werden, die externe Anwendung zu autorisieren, klicken Sie auf **Autorisieren**.

   Du musst das nur einmal machen.

1. Geben Sie im Suchfeld des angezeigten Felds **Externe Dateien und Ordner verknüpfen** den Namen des Elements ein, nach dem Sie suchen möchten, und drücken Sie dann die Eingabetaste **Enter** , um alle Ergebnisse aus der externen Anwendung anzuzeigen, unabhängig davon, in welchem Ordner sie gespeichert sind.

   Oder

   Suchen Sie die Dokumente, die Sie verknüpfen möchten, und wählen Sie sie aus.

   Sie können mehrere Dokumente auswählen. Es werden jedoch nur Dokumente verknüpft, die in der aktuellen Ansicht ausgewählt sind. Wenn Sie beispielsweise ein Dokument auswählen und dann in einen Ordner wechseln, wird das ursprünglich ausgewählte Dokument nicht verknüpft.

1. (Bedingt) Wenn Sie Workfront DAM-Kunde sind, klicken Sie auf das Symbol **Miniaturansicht** , um Dateien als Miniaturansichten anzuzeigen.

   >[!NOTE]
   >
   >Workfront DAM-Kunden können beim Verknüpfen von Dokumenten aus Workfront DAM Miniaturansichten anzeigen. Miniaturansichten werden möglicherweise auch für Workfront DAM-Kunden für andere Dienste wie Dropbox und Box angezeigt. Das Anzeigen von Miniaturansichten für andere Dienste als Workfront DAM in Workfront wird jedoch nicht unterstützt und Miniaturansichten werden beim Verknüpfen von Dokumenten von SharePoint oder Google Drive nie angezeigt.

1. Klicken Sie auf **Link**.

   In Workfront wird neben den Dokumenten das Symbol des Cloud-Anbieters angezeigt, das angibt, dass sie mit dem externen Cloud-Anbieter verknüpft sind.

   >[!NOTE]
   >
   >Bei Dokumenten, die mit &quot;Feld&quot;verknüpft sind, wird der Link zum Dokument im Feld erst angezeigt, wenn Sie die Seite aktualisieren.

Informationen zum Hinzufügen einer neuen Version eines Dokuments, das Sie aus Ihrem Dateisystem in Workfront hochgeladen haben, finden Sie unter [Dokumente zu Adobe Workfront hinzufügen](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md#add-documents-to-workfront) in [Dokumente aus Ihrem Dateisystem zu Adobe Workfront hinzufügen](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

### Verknüpfen von Workfront Proof-Dokumenten {#link-workfront-proof-documents}

Sie können Testsendungen mit Workfront verknüpfen, die ursprünglich in Workfront Proof existierten. Wenn Sie einen Testversand aus Workfront Proof verknüpfen, sind alle mit dem Testversand verknüpften Kommentare und anderen Metadaten in Workfront verfügbar.

Sie können nur die Testsendungen verknüpfen, für die Sie Zugriff auf Ansicht in Workfront Proof haben.

1. Wechseln Sie zum Bereich **Dokumente** in Workfront, in dem Sie das Dokument speichern möchten.
1. Klicken Sie auf **Neu hinzufügen** und dann auf **Aus Workfront Proof**.

   >[!NOTE]
   >
   >Die Optionen in diesem Menü variieren je nachdem, welche Drittanbieter in Ihrer Umgebung konfiguriert sind.

1. Geben Sie im angezeigten Feld **Testsendungen von Workfront Proof verknüpfen** den Namen des Testversands ein, den Sie in Workfront verfügbar machen möchten.

   Die Liste wird bei der Eingabe gefiltert.

1. Wählen Sie bis zu 10 zu verknüpfende Testsendungen aus.

   Ein abgeblendeter Testversand-Name kann nicht verknüpft werden, da der Testversand bereits mit einem Dokument in Workfront verknüpft ist.

1. Klicken Sie auf **Link**.

   Die neueste Version des Testversands ist mit Workfront verknüpft. Wenn Sie den Testversand öffnen, sind alle Versionen im Testversand-Viewer verfügbar.

### Erstellen eines Google-Dokuments aus Workfront {#create-a-google-document-from-within-workfront}

Sie können ein neues Google-Dokument in Workfront erstellen. Für andere Cloud-Anbieter können Sie keine neuen Dokumente aus Workfront erstellen.

1. Wechseln Sie zum Bereich **Dokumente** in Workfront, in dem Sie das Dokument speichern möchten.
1. Klicken Sie auf **Neu hinzufügen** > **Google-Datei** und wählen Sie dann den Typ des zu erstellenden Google-Dokuments aus.
1. Wenn das Feld **Google-Laufwerkskonto hinzufügen** angezeigt wird, klicken Sie auf **Google-Laufwerk autorisieren**.

   Ein Google-Dokument wird der Registerkarte **Dokumente** hinzugefügt.

   >[!NOTE]
   >
   > Meine Festplatte und für mich freigegeben zeigen zwei unterschiedliche Ergebnisse an. Wenn Sie eine Datei in My Drive nicht finden können, überprüfen Sie den Ordner Für mich freigegeben .

## Hochladen und Verknüpfen eines Dokuments von Workfront mit einem externen Cloud-Anbieter

Sie können ein Dokument von Workfront hochladen und mit einem externen Cloud-Anbieter verknüpfen. Dadurch wird die Dokumentenspeicherung von Workfront an den externen Cloud-Anbieter verschoben. Wenn das Dokument in der externen Anwendung geändert wird, wird es automatisch in Workfront aktualisiert.

>[!NOTE]
>
>Durch das Senden eines Assets an einen externen Dokumentanbieter wird eine neue Version des Assets erstellt.

Benutzer ohne Zugriff auf Workfront können das Dokument in der externen Anwendung sehen, wenn sie Zugriff auf die Anwendung haben.

1. Wählen Sie ein Dokument aus, das in Workfront hochgeladen wird.
1. Klicken Sie auf **Mehr** >**Senden an** und wählen Sie dann den Cloud-Anbieter aus, unter dem das verknüpfte Dokument gespeichert werden soll.

   Dazu können Sie auch das Menü Mehr ![](assets/more-icon.png) auf der Seite Dokumentdetails verwenden.

1. Wählen Sie den Ordner in der Anwendung des Providers aus, in dem Sie das Dokument speichern möchten.

   Dies kann ein beliebiger Ordner in der Anwendung des Providers sein, einschließlich eines freigegebenen Ordners.

1. Klicken Sie auf **Speichern**.

   Das Logo des externen Anbieters wird neben dem Dokumentnamen angezeigt, um anzugeben, dass das Dokument jetzt mit Workfront verknüpft und vom externen Cloud-Anbieter gespeichert ist.

   ![doc_with_google_drive_link_highlight_1_.png](assets/doc-with-google-drive-link-highlight--1--350x66.png)

## Verknüpfungsordner

Wenn Sie einen Ordner zwischen Workfront und einem externen Cloud-Anbieter verknüpfen, werden der Ordner und alle zugehörigen Inhalte verknüpft. Wenn Benutzer ohne Zugriff auf Workfront Dateien aus der externen Dokumentanwendung hinzufügen, entfernen und ändern, werden ihre Änderungen mit Workfront synchronisiert.

### Zugriffsberechtigungen für Ordner {#folder-access-rights}

Beim Synchronisieren von Ordnerinhalten aus einer externen Dokumentanwendung verwendet Workfront die Anmeldeinformationen des Benutzers, der den Ordner ursprünglich verknüpft hat. Dies führt zum folgenden Benutzererlebnis:

* Wenn Benutzer keinen Zugriff auf Dateien und Ordner in der externen Anwendung haben, aber Zugriff auf den verknüpften Ordner über Workfront haben, können sie nur die Namen der Dateien und Ordner in Workfront anzeigen, nicht deren Inhalte.
* Wenn ein Benutzer in einem verknüpften Ordner in Workfront auf Inhalte zugreift (z. B. auf einen Unterordner in einem verknüpften Ordner), die von einem anderen Benutzer mit Workfront verknüpft wurden, wird der Inhalt mit Workfront unter Verwendung der Workfront-Anmeldedaten des Benutzers, der den Ordner ursprünglich verknüpft hat, synchronisiert, nicht mit den Anmeldedaten des Benutzers, der auf den Inhalt zugreift.

>[!IMPORTANT]
>
>* Wenn der Benutzer, der den Ordner ursprünglich verknüpft hat, aus dem Workfront-System entfernt wird, können Benutzer nicht mehr über Workfront auf den Inhalt des verknüpften Ordners zugreifen. In diesem Fall muss der Ordner von einem aktiven Workfront-Benutzer, der über Berechtigungen für den Ordner in der externen Anwendung verfügt, neu verknüpft werden.
>* Wenn der Benutzer, der einen Ordner verknüpft hat, keinen Zugriff mehr auf die externe Anwendung hat, kann Workfront nicht mehr auf den Ordnerinhalt zugreifen. Dies kann beispielsweise der Fall sein, wenn der Benutzer, der den Ordner ursprünglich verknüpft hat, das Unternehmen verlässt. Um einen kontinuierlichen Zugriff sicherzustellen, muss ein Benutzer mit Zugriff auf den Ordner den Ordner erneut verknüpfen.

### Externe Ordner verknüpfen {#link-one-or-more-external-folders}

1. Wechseln Sie zu dem Bereich in Workfront, in dem Sie den Ordner ablegen möchten, und klicken Sie dann im linken Bereich auf **Dokumente** ![](assets/document-icon.png) .

1. Klicken Sie auf **Neu hinzufügen** und dann auf den externen Dokumentanbieter, von dem Sie einen Ordner mit Workfront verknüpfen möchten.
1. (Bedingt) Wenn Sie den externen Dienst noch nicht autorisiert haben, geben Sie Ihre Anmeldedaten für den externen Anbieter an und klicken Sie auf **Anmelden**.

   Externe Anbieter, die Sie bereits autorisiert haben, werden oben in der Liste angezeigt.

1. Navigieren Sie im angezeigten Feld **Externe Dateien und Ordner verknüpfen** zu den Ordnern, die Sie verknüpfen möchten, und wählen Sie sie aus.

   Oder

   Geben Sie den Namen des Ordners ein, nach dem Sie suchen möchten, und drücken Sie dann die Taste **Enter**.

   Sie können mehrere Ordner auswählen. Es werden jedoch nur Ordner verknüpft, die in der aktuellen Ansicht ausgewählt sind. Wenn Sie beispielsweise einen Ordner auswählen und dann in einen Ordner wechseln, wird der ursprünglich ausgewählte Ordner nicht verknüpft.

   >[!NOTE]
   >
   >Wenn Sie Ordner von Google Drive aus verknüpfen, können Sie nur Ordner verknüpfen, die sich in Ihrem persönlichen Laufwerk (My Drive) und Team Drive befinden. Sie können keine Ordner aus dem Bereich Für mich freigegeben verknüpfen.

1. Klicken Sie auf **Link**.

   In Workfront wird neben dem Ordner das Logo des Cloud-Anbieters angezeigt, das angibt, dass er mit dem externen Cloud-Anbieter verknüpft ist.

1. (Optional) Um den Ordner so umzubenennen, dass der Ordnername in Workfront sich vom Ordnernamen in der externen Dokumentanwendung unterscheidet, wählen Sie den Ordner im Abschnitt **Ordner** aus, klicken Sie auf das Menü Mehr ![](assets/more-icon.png) , das neben dem Ordnernamen angezeigt wird, und klicken Sie dann auf **Umbenennen**.

   ![](assets/documents-folderlink-rename-nwe-350x154.png)

Dadurch wird der Ordner in der externen Anwendung nicht umbenannt.

### Unterordner zu einem verknüpften Ordner hinzufügen  {#add-subfolders-to-a-linked-folder}

Sie können einen neuen Ordner in einem vorhandenen verknüpften Ordner erstellen. Sie können auch einen anderen Ordner in einen vorhandenen verknüpften Ordner ziehen.

1. Um einen neuen Ordner in einem vorhandenen verknüpften Ordner zu erstellen, wechseln Sie zum vorhandenen Ordner und erstellen Sie dann den neuen Ordner wie unter [Erstellen von Dokumentenordnern](../../documents/organizing-documents/create-documents-folder.md) beschrieben.

   Oder

   Um einen vorhandenen Ordner in einen vorhandenen verknüpften Ordner zu ziehen, wechseln Sie zum Bereich Dokumente , in dem Sie den Unterordner ablegen möchten, und ziehen Sie ihn in den verknüpften Ordner.

   ![](assets/documents-link-folder-move-nwe-350x113.png)

   >[!NOTE]
   >
   >Die folgenden Einschränkungen gelten beim Ziehen eines vorhandenen Workfront-Ordners in einen verknüpften Ordner:
   >
   >* Der Ordner, den Sie ziehen, kann noch nicht verknüpft sein und keine bereits verknüpften Inhalte enthalten.
   >* Der Ordner (einschließlich des Inhalts), den Sie ziehen, darf 50 MB nicht überschreiten.

## Dokument zu einem verknüpften Ordner hinzufügen

Wenn Sie ein Dokument über Workfront zu einem verknüpften Ordner hinzufügen, wird es automatisch als verknüpftes Dokument hinzugefügt.

1. Wählen Sie den verknüpften Ordner aus, in dem das Dokument gespeichert werden soll, klicken Sie auf &quot;**Neu hinzufügen&quot;> &quot;Dokument&quot;**, navigieren Sie zum Dokument und fügen Sie es dem Ordner hinzu.

   Oder

   Ziehen Sie das Dokument im Bereich **Dokumente** , in dem Sie das Dokument abrufen möchten, in einen verknüpften Ordner.

   Eine neue Dokumentversion wird automatisch in der externen Anwendung erstellt und mit Workfront verknüpft.

>[!NOTE]
>
> * Die Dokumentoptionen sind während der Verschiebung des Dokuments nicht verfügbar.
>
> * Nachdem ein Dokument in Experience Manager Assets verschoben wurde, ist es nicht mehr in der Dokumentliste in Workfront sichtbar.
>
> * Alle Aktionen oder Bearbeitungen, die Sie während des Übergangs an einem Dokument vornehmen, werden nicht im Dokument in Experience Manager Assets angezeigt und gehen daher verloren.

## Verknüpfte Dokumente oder Ordner löschen

Wenn Sie ein verknüpftes Dokument oder Ordner aus der externen Anwendung löschen, bleibt das Dokument bzw. der Ordner im Workfront-System, bis Sie es auch aus Workfront löschen.

1. Wählen Sie das verknüpfte Dokument oder Ordner aus und klicken Sie dann auf **Löschen**.
1. Klicken Sie im angezeigten Bestätigungsfeld auf **Ja, Verknüpfung aufheben**.

   Die Verknüpfung des Dokuments mit der Workfront-Site wird aufgehoben. Sie ist in der externen Anwendung nicht betroffen.

## Über das Umbenennen verknüpfter Dokumente und Ordner

Wenn Sie ein verknüpftes Dokument oder einen verknüpften Ordner umbenennen, ist die Änderung nur in der Anwendung sichtbar, in der Sie sie vornehmen. Wenn Sie beispielsweise ein verknüpftes Dokument in Workfront umbenennen, ist der neue Name nur in Workfront sichtbar.

Wenn der Name in Workfront und in der externen Anwendung übereinstimmen soll, müssen Sie ihn an beiden Stellen umbenennen.

>[!IMPORTANT]
>
>Benennen Sie ein Dokument in Workfront nicht um, das mit Dropbox verknüpft ist. Dadurch wird der Zugriff auf die Datei in Workfront verhindert. Benennen Sie die Datei stattdessen in Dropbox um und synchronisieren Sie sie dann erneut.
