---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1958'
ht-degree: 0%

---

# SFTP-Module

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [SFTP-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/universal-connectors/sftp.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit den [!DNL Adobe Workfront Fusion] SFTP-Modulen können Sie Dateiänderungen in einem ausgewählten Ordner/Unterordner überwachen, neue Dateien in den gewünschten Ordner hochladen, vorhandene Dateien ändern oder löschen, die sich bereits in einem Ordner befinden, oder Dateiberechtigungen ändern.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um SFTP mit [!DNL Workfront Fusion] verwenden zu können, benötigen Sie ein SFTP-Konto (z. B. [!DNL GoDaddy] Webhosting).

## Verbinden von SFTP mit [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

Um Ihr SFTP-Konto mit [!DNL Workfront Fusion] zu verbinden, müssen Sie den Ziel-Host und die SFTP-Anmeldedaten (Benutzername und Kennwort oder Benutzername und Schlüssel) in das Dialogfeld [!UICONTROL Verbindung erstellen“ ] Moduls eingeben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindungsname]</td> 
   <td> <p> Geben Sie den Namen für Ihre SFTP-Verbindung ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
   <td> <p>Geben Sie den Host-Namen des SFTP-Servers ein, zu dem Sie eine Verbindung herstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>Geben Sie den SFTP-Server-Port ein. Beispiel: 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Authentifizierungstyp]</p> </td> 
   <td> <p>Wählen Sie die Autorisierungsmethode aus, die Sie für die Verbindung mit dem SFTP-Server verwenden möchten.</p> 
    <ul> 
     <li><strong>[!UICONTROL Benutzername und Kennwort]</strong>: Geben Sie Ihre Anmeldedaten ein.</li> 
     <li> <p><strong>[!UICONTROL Benutzername und Schlüssel]</strong>: Geben Sie Ihren Benutzernamen und den privaten Schlüssel/das Zertifikat ein</p> <p>Laden Sie den privaten Schlüssel hoch, um die Client-seitige Autorisierung zu verwenden, oder laden Sie Ihr Zertifikat (P12- oder PFX-Datei) hoch, wenn Sie TLS mit Ihrem selbstsignierten Zertifikat verwenden möchten. Wenn Sie die Client-seitige Zertifikatautorisierung verwenden, können Sie Ihr CA-Zertifikat hier eingeben.</p> <p>[!DNL Workfront Fusion] speichert und speichert keine Daten (Dateien, Passwörter), die Sie hier angeben. Datei und Passwort werden nur zum Extrahieren eines privaten Schlüssels/Zertifikats verwendet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Klicken Sie nach Eingabe der Verbindungsinformationen auf **[!UICONTROL Weiter]**, um eine Verbindung herzustellen.

## [!UICONTROL SFTP]-Module und ihre Felder

Beim Konfigurieren von [!UICONTROL SFTP]-Modulen zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können zusätzliche [!UICONTROL SFTP]-Felder angezeigt werden, abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trigger

#### [!UICONTROL Dateien in einem Ordner ansehen]

Gibt Dateien mit Details zurück, wenn eine Datei in einem angegebenen Ordner erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein, den Sie beobachten möchten, oder ordnen Sie ihn zu. Sie können einen absoluten Pfad wie <code>/home/user/</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Puffergröße [b]</td> 
   <td> <p> Geben Sie die Puffergröße in Byte ein. Der Wert definiert die Größe der vom Server übertragenen Blöcke. Einige Server können Probleme verursachen oder Dateien beschädigen, wenn der Wert zu hoch ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Dateien]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Dateien fest, mit denen [!DNL Workfront Fusion] in einem Zyklus arbeiten soll</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Überwachen von Unterordnern in einem Ordner]

Gibt Ordner mit Details zurück, wenn ein Ordner in einem angegebenen Ordner erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein, den Sie beobachten möchten, oder ordnen Sie ihn zu. Sie können einen absoluten Pfad wie <code>/home/user/</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Dateien]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ordnern fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

#### [!UICONTROL Den Inhalt eines Ordners auflisten]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen] </td> 
   <td> <p>Wählen Sie aus, ob Sie Dateien, Ordner oder beides abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein, der die Dateien oder Ordner enthält, die Sie auflisten möchten, oder ordnen Sie ihn zu. Sie können einen absoluten Pfad wie <code>/home/user/</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Geben Sie den Suchbegriff ein oder ordnen Sie ihn zu. Wenn Sie beispielsweise nach Dateien mit der Dateierweiterung .txt suchen möchten, geben Sie <code>.txt</code> ein. Sie können auch den Namen der Datei eingeben oder zuordnen, nach der Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL sortieren nach]</td> 
   <td> <p> Wählen Sie aus, ob die Ergebnisse nach Dateiname, Größe, Datum des letzten Zugriffs oder Datum der letzten Änderung sortiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sortierreihenfolge] </td> 
   <td> <p>Wählen Sie aus, ob das Ergebnis in auf- oder absteigender Reihenfolge zurückgegeben werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Die Routenausführung auch dann fortsetzen, wenn das Modul keine Ergebnisse zurückgibt]</p> </td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass das Modul das Szenario nicht beendet, wenn es keine Ergebnisse zurückgibt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Ergebnisse]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dateien abrufen]

Dieses Modul listet Dateien aus einem angegebenen Ordner auf.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Puffergröße [B]]</td> 
   <td> <p> Geben Sie die Puffergröße in Byte ein. Der Wert definiert die Größe der vom Server übertragenen Blöcke. Einige Server können Probleme verursachen oder Dateien beschädigen, wenn der Wert zu hoch ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein, der die Dateien oder Ordner enthält, die Sie auflisten möchten, oder ordnen Sie ihn zu. Sie können einen absoluten Pfad wie <code>/home/user/</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Geben Sie den Suchbegriff ein oder ordnen Sie ihn zu. Wenn Sie beispielsweise nach Dateien mit der Dateierweiterung .txt suchen möchten, geben Sie <code>.txt</code> ein. Sie können auch den Namen der Datei eingeben oder zuordnen, nach der Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL sortieren nach]</td> 
   <td> <p> Wählen Sie aus, ob die Ergebnisse nach Dateiname, Größe, Datum des letzten Zugriffs oder Datum der letzten Änderung sortiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sortierreihenfolge]</td> 
   <td> <p> Wählen Sie aus, ob das Ergebnis in auf- oder absteigender Reihenfolge zurückgegeben werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Die Routenausführung auch dann fortsetzen, wenn das Modul keine Ergebnisse zurückgibt]</p> </td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass das Modul das Szenario nicht beendet, wenn es keine Ergebnisse zurückgibt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der zurückgegebenen Ergebnisse]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Dateien fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei abrufen]

Dieses Modul ruft Dateidetails ab, einschließlich der Daten einer Datei.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Puffergröße [B]]</td> 
   <td> <p> Geben Sie die Puffergröße in Byte ein. Der Wert definiert die Größe der vom Server übertragenen Blöcke. Einige Server können Probleme verursachen oder Dateien beschädigen, wenn der Wert zu hoch ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad] </td> 
   <td> <p>Geben Sie den Pfad zur Datei ein. Sie können einen absoluten Pfad wie <code>/home/user/file.txt</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei hochladen]

Mit diesem Modul können Sie eine Datei auf den SFTP-Server hochladen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Geben Sie einen vorhandenen Ordner als Speicherort für die Datei an. Sie können einen absoluten Pfad wie <code>/home/user/</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p> Ordnen Sie die Quelldatei einem vorherigen Modul zu, z. B. [!UICONTROL Dropbox] &gt; [!UICONTROL Get File]. Sie können auch den Dateinamen und die Dateidaten eingeben oder zuordnen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL-Berechtigungen]</p> </td> 
   <td> <p>Legen Sie die gewünschten Berechtigungen für die Datei oder den Ordner fest. Verwenden Sie chmod-Parameter. Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Weitere Informationen zu chmod finden Sie in der <a href="https://ss64.com/bash/chmod.html">chmod-Dokumentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei umbenennen]

Benennt eine Datei um.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zu der Datei ein, die Sie umbenennen möchten. Sie können einen absoluten Pfad wie <code>/home/user/file.txt</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Neuer Dateiname]</td> 
   <td> <p> Geben Sie den neuen Namen für die Datei ein, einschließlich der Dateierweiterung.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer Datei]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zur zu verschiebenden Datei ein. Sie können einen absoluten Pfad wie <code>/home/user/file.txt</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Neuer Ordner]</td> 
   <td> <p> Geben Sie den Pfad zum neuen Speicherort der Datei ein. Sie können einen absoluten Pfad wie <code>/home/user/</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei löschen]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zu der Datei ein, die Sie löschen möchten. Sie können einen absoluten Pfad wie <code>/home/user/file.txt</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren von Dateiberechtigungen]

Ermöglicht das Ändern der Dateiberechtigungen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zur zu verschiebenden Datei ein. Sie können einen absoluten Pfad wie <code>/home/user/file.txt</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL-Berechtigungen]</p> </td> 
   <td> <p>Legen Sie die gewünschten Dateiberechtigungen fest. Verwenden Sie die chmod-Parameter. Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Muss mit Muster übereinstimmen <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Weitere Informationen zu chmod finden Sie in der <a href="https://ss64.com/bash/chmod.html">chmod-Dokumentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner erstellen]

Erstellt einen neuen Ordner am angegebenen Speicherort.

>[!NOTE]
>
>Wenn der Ordner bereits vorhanden ist, gibt das Modul einen Fehler aus. Um den Fluss ununterbrochen fortzusetzen, fügen Sie eine Fehler-Handler-Route an das Modul an, um den Fehler zu erfassen, und verwenden Sie die [!UICONTROL Resume]-Direktive, um den Fluss fortzusetzen. Informationen zum Anhängen einer Fehler-Handler-Route finden Sie unter [Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Informationen zur Fehler-Handler-Route finden Sie unter [Anweisungen für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner] </td> 
   <td> <p>Geben Sie einen vorhandenen Ordner als Speicherort für den neuen Ordner an. Sie können einen absoluten Pfad wie <code>/home/user/file.txt</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordnername]</td> 
   <td> <p> Geben Sie den Ordnernamen ein.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL-Berechtigungen]</p> </td> 
   <td> <p>Festlegen der gewünschten Ordnerberechtigungen. Verwenden Sie chmod-Parameter. Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Muss mit Muster übereinstimmen <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Weitere Informationen zu chmod finden Sie auf der <a href="https://ss64.com/bash/chmod.html">chmod Man Page</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner löschen]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Verbinden von SFTP mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Geben Sie den Pfad zum Ordner an, den Sie löschen möchten. Sie können einen absoluten Pfad wie <code>/home/user/</code> angeben. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
