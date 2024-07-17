---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: FTP-Module
description: Mit FTP-Modulen können Sie Dateiänderungen in einem ausgewählten Ordner überwachen, neue Dateien in den gewünschten Ordner hochladen und vorhandene Dateien, die sich bereits in einem Ordner befinden, ändern oder löschen.
author: Becky
feature: Workfront Fusion
exl-id: 360825a4-4580-4039-894e-583e82132ed6
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '1335'
ht-degree: 0%

---

# FTP-Module

Mit FTP-Modulen können Sie Dateiänderungen in einem ausgewählten Ordner überwachen, neue Dateien in den gewünschten Ordner hochladen und vorhandene Dateien, die sich bereits in einem Ordner befinden, ändern oder löschen.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [Fusion App] mit [!DNL Workfront Fusion] verwenden zu können, benötigen Sie ein FTP-Konto.

## Erstellen einer Verbindung in einem FTP-Modul {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindungsname]</td> 
   <td> <p> Geben Sie den Namen für Ihre FTP-Verbindung ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Host] </td> 
   <td> <p>Geben Sie den FTP-Server-Hostnamen ein. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Port] </td> 
   <td> <p>Geben Sie die Port-Nummer des FTP-Servers ein. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzername] </td> 
   <td> <p>Geben Sie Ihren FTP-Konto-Benutzernamen ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kennwort] </td> 
   <td> <p>Geben Sie Ihr FTP-Kontokennwort ein.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Verwenden einer sicheren Verbindung (TLS)</p> </td> 
   <td> <p>Wählen Sie aus, ob Sie eine sichere Verbindung verwenden möchten.</p> <p style="font-weight: bold;">[!UICONTROL Nein]</p> <p>Die Verbindung ist nicht gesichert.</p> <p style="font-weight: bold;">[!UICONTROL Explizite Verschlüsselung oder implizite Verschlüsselung]</p> <p>Die Verbindung wird mithilfe von SSL gesichert.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Nicht autorisierte Zertifikate zurückweisen]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um das FTP-Serverzertifikat zu überprüfen. Wenn die Überprüfung fehlschlägt, wird die Verbindung nicht erstellt. Um die Überprüfung zu bestehen, muss das Zertifikat eines der folgenden Kriterien erfüllen:</p> 
    <ul> 
     <li>von einer <a href="https://en.wikipedia.org/wiki/Certificate_authority">Zertifizierungsstelle für Stammzertifikate</a> signiert werden</li> 
     <li>von einer Zwischenzertifizierungsstelle unterzeichnet werden (weitere Informationen finden Sie unter <a href="https://knowledge.digicert.com/solution/SO16297.html">Funktionsweise der Zertifikatsketten</a>). In diesem Fall sollten alle Zwischenzertifikate auf dem FTP-Server installiert sein.</li> 
     <li>ein selbst signiertes Zertifikat sein, das im Feld [!UICONTROL Selbstsigniertes Zertifikat] bereitgestellt wird (siehe unten)</li> </ul>

Wenn diese Option deaktiviert ist, wird das FTP-Serverzertifikat nicht überprüft. Wir empfehlen dringend, die Option nicht zu deaktivieren, da sie die Verbindung unsicher macht und ein ernsthaftes Sicherheitsrisiko darstellt.</td>
</tr> 
  <tr> 
   <td> <p>[!UICONTROL Selbstsigniertes Zertifikat]</p> </td> 
   <td> <p>Klicken Sie auf die Schaltfläche <b>[!UICONTROL Extract]</b> , um das Upload-Dialogfeld zu öffnen.</p> <p>Laden Sie das Zertifikat hoch, um das TLS mit Ihrem selbstsignierten Zertifikat zu verwenden. [!DNL Workfront Fusion] speichert oder speichert keine von Ihnen bereitgestellten Daten, z. B. Dateien und Kennwörter. Datei und Kennwort werden nur zum Extrahieren des Zertifikats verwendet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## FTP-Module und ihre Felder

* [Trigger](#triggers)
* [Aktionen](#actions)

### Trigger

#### [!UICONTROL Dateien ansehen]

[!UICONTROL Dateien ansehen] ist das einzige Trigger-Modul für FTP. Er überwacht den Dateiinhalt des ausgewählten Ordners. Der Trigger wird ausgeführt, wenn eine neue Datei in den angegebenen Ordner eingefügt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#create-a-connection" class="MCXref xref">[!UICONTROL Verbindung in einem FTP-Modul erstellen</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Ordner]</p> </td> 
   <td> <p>Wählen Sie den Ordner aus, den Sie sehen möchten.</p> <p><b>Hinweis:</b> Pro Szenario ist nur ein Ordner zulässig. Unterordner werden ignoriert.</p> <p><b>Tipp:</b> Erstellen Sie für jeden Ordner ein unabhängiges Szenario, um mehrere Ordner zu verfolgen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Dateien] </td> 
   <td> <p>Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll. Wenn der Wert zu hoch eingestellt ist, kann die Verbindung auf der Seite des angegebenen Drittanbieterdienstes unterbrochen werden (Timeout). [!DNL Workfront Fusion] hat keinen Einfluss darauf. Es wird empfohlen, einen niedrigeren Wert festzulegen und entweder einen höheren Wert für die maximale Anzahl von Zyklen zu definieren oder das Szenario häufiger auszuführen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Berechtigungen ändern]](#change-permissions)
* [[!UICONTROL Erstellen eines Ordners]](#create-a-folder)
* [[!UICONTROL Datei löschen]](#delete-a-file)
* [[!UICONTROL Ordner löschen]](#delete-a-folder)
* [[!UICONTROL Datei abrufen]](#get-a-file)
* [[!UICONTROL Liste der Dateien in einem Ordner]](#list-of-files-in-a-folder)
* [[!UICONTROL Verschieben einer Datei oder eines Ordners]](#move-a-file-or-folder)
* [[!UICONTROL  Hochladen] einer Datei](#upload-a-file)

#### [!UICONTROL Berechtigungen ändern]

Dieses Aktionsmodul ändert die Berechtigungseinstellungen einer Datei oder eines Ordners.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Verbindung]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#Create" class="MCXref xref" >[!UICONTROL Verbindung in einem FTP-Modul erstellen</a> in diesem Artikel.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Berechtigungseinstellungen ändern]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>Wählen Sie aus, ob Sie die Einstellungen für eine Datei oder einen Ordner ändern möchten.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Dateipfad]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Geben Sie den Dateipfad für den Ordner oder die Datei ein oder ordnen Sie ihn zu.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">[!UICONTROL Berechtigungen]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Legen Sie die gewünschten Datei- oder Ordnerberechtigungen fest. Verwenden Sie die Parameter chmod . Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p>
               <p>Berechtigungen müssen mit dem Muster <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code> übereinstimmen.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Erstellen eines Ordners]

Dieses Aktionsmodul erstellt einen neuen Ordner.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">[!UICONTROL Verbindung]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#Create" class="MCXref xref" >[!UICONTROL Verbindung in einem FTP-Modul erstellen</a> in diesem Artikel.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">[!UICONTROL Ordnerpfad]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Geben Sie den Dateipfad ein oder ordnen Sie ihn dem neuen Ordner zu.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Neuer Ordnername]</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>Geben Sie einen Namen für den neuen Ordner ein oder ordnen Sie ihn zu.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Datei löschen]

Löscht eine Datei aus dem angegebenen Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#Create" class="MCXref xref" >[!UICONTROL Verbindung in einem FTP-Modul erstellen</a> in diesem Artikel.</td>
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den FTP-Ordner aus, aus dem Sie eine Datei löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateiname]</td> 
   <td> <p> Geben Sie den Dateinamen einschließlich der Dateinamenerweiterung ein. Beispiel: <code>[!DNL image].png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner löschen]

Dieses Aktionsmodul löscht den angegebenen Ordner dauerhaft.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Verbindung]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#Create" class="MCXref xref" >[!UICONTROL Verbindung in einem FTP-Modul erstellen</a> in diesem Artikel.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Ordner]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>Wählen Sie den FTP-Ordner aus, aus dem Sie eine Datei löschen möchten.</p>
            </td>
         </tr>
   </tbody>
</table>

#### [!UICONTROL Datei abrufen]

Ruft eine Datei vom FTP-Server ab, die weiter verarbeitet werden kann, z. B. Hochladen auf [!DNL Dropbox].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#creating-the-ftp-connection" class="MCXref xref">Erstellen der FTP-Verbindung</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad der Datei ein, die Sie abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Liste der Dateien in einem Ordner]

Ruft Datei- und/oder Ordnerinformationen ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#creating-the-ftp-connection" class="MCXref xref">Erstellen der FTP-Verbindung</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den FTP-Ordner aus, in dem Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Wählen Sie aus, ob Sie Informationen zu Dateien oder Ordnern oder beidem abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Geben Sie den Suchbegriff ein. Wenn kein Suchbegriff eingegeben wird, werden alle Dateien und Ordner aus dem angegebenen Ordner abgerufen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Dateien]</td> 
   <td> <p> Legen Sie die maximale Anzahl der von diesem Modul abgerufenen Dateien fest.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer Datei oder eines Ordners]

Dieses Aktionsmodul verschiebt eine Datei oder einen Ordner an einen anderen Speicherort.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Verbindung]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#Create" class="MCXref xref" >[!UICONTROL Verbindung in einem FTP-Modul erstellen</a> in diesem Artikel.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">[!UICONTROL Alter Dateipfad]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>Geben Sie den Pfad ein, aus dem Sie die Datei verschieben möchten. Beispiel: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">[!UICONTROL Neuer Dateipfad]</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>Geben Sie den Pfad ein, in den Sie die Datei verschieben möchten. Beispiel: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### [!UICONTROL  Datei hochladen]

Lädt eine Datei auf den FTP-Server hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Herstellen einer Verbindung zum FTP-Konto finden Sie unter <a href="#creating-the-ftp-connection" class="MCXref xref">Erstellen der FTP-Verbindung</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den FTP-Ordner aus, in den Sie die Datei hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei] </td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL An eine bereits vorhandene Datei anhängen]</td> 
   <td> <p>Wenn diese Option aktiviert ist und die Datei bereits auf dem FTP-Server vorhanden ist, wird der Inhalt der Datei an die vorhandene Datei angehängt. Wenn diese Option nicht aktiviert ist, wird der Inhalt der Datei überschrieben.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner erstellen, falls nicht vorhanden] </td> 
   <td> <p>Wenn diese Option aktiviert ist und der Ordner, den Sie in das Feld Ordner eingegeben haben, nicht auf dem FTP-Server vorhanden ist, erstellt das Modul den Ordner</p> </td> 
  </tr> 
 </tbody> 
</table>

## Fehlerbehebung {#troubleshooting}

Wenn bei der Erstellung der Verbindung oder während des Vorgangs eines Moduls Probleme mit der FTP-App auftreten, versuchen Sie, einen der beliebten FTP-Clients zu verwenden und versuchen Sie, dieselbe Aktion durchzuführen (z. B. eine Verbindung zu erstellen oder Dateien in einem Ordner aufzulisten). mit dem FTP-Client. Wenn Sie dieselben Probleme auch mit dem FTP-Client haben, kann dies auf eine Fehlkonfiguration des FTP-Servers zurückzuführen sein.
