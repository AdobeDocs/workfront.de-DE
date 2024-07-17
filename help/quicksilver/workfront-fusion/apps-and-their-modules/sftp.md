---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP-Module
description: Mit den [!DNL Adobe Workfront Fusion SFTP] Modulen können Sie Dateiänderungen in einem ausgewählten Ordner/Unterordner überwachen, neue Dateien in den gewünschten Ordner hochladen, vorhandene Dateien, die sich bereits in einem Ordner befinden, ändern oder löschen oder die Dateiberechtigungen ändern.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1920'
ht-degree: 0%

---

# SFTP-Module

Mit den [!DNL Adobe Workfront Fusion] SFTP-Modulen können Sie Dateiänderungen in einem ausgewählten Ordner/Unterordner überwachen, neue Dateien in den gewünschten Ordner hochladen, vorhandene Dateien, die sich bereits in einem Ordner befinden, ändern oder löschen oder die Dateiberechtigungen ändern.

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

Um SFTP mit [!DNL Workfront Fusion] verwenden zu können, ist ein SFTP-Konto erforderlich (z. B. [!DNL GoDaddy] Webhosting).

## SFTP mit [!DNL Workfront Fusion] verbinden {#connect-sftp-to-workfront-fusion}

Um Ihr SFTP-Konto mit [!DNL Workfront Fusion] zu verbinden, müssen Sie den Ziel-Host und die SFTP-Anmeldeinformationen (Benutzername und Kennwort oder Benutzername und Schlüssel) im Dialogfeld [!UICONTROL Verbindung erstellen] des Moduls eingeben.

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
   <td> <p>Geben Sie den Hostnamen des SFTP-Servers ein, mit dem Sie eine Verbindung herstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Port] </td> 
   <td> <p>Geben Sie den SFTP-Server-Port ein. Beispiel: 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Authentifizierungstyp]</p> </td> 
   <td> <p>Wählen Sie die Autorisierungsmethode aus, die Sie für die Verbindung mit dem SFTP-Server verwenden möchten.</p> 
    <ul> 
     <li><strong>[!UICONTROL Benutzername und Kennwort]</strong>: Geben Sie Ihre Anmeldeinformationen ein.</li> 
     <li> <p><strong>[!UICONTROL Benutzername und Schlüssel]</strong>: Geben Sie Ihren Benutzernamen und den privaten Schlüssel/das Zertifikat ein</p> <p>Laden Sie den privaten Schlüssel hoch, um die clientseitige Autorisierung zu verwenden, oder laden Sie Ihr Zertifikat hoch (P12- oder PFX-Datei), wenn Sie TLS mit Ihrem selbstsignierten Zertifikat verwenden möchten. Wenn Sie die clientseitige Zertifikatsautorisierung verwenden, können Sie hier Ihr Zertifizierungsstellenzertifikat eingeben.</p> <p>[!DNL Workfront Fusion] speichert keine von Ihnen angegebenen Daten (Dateien, Kennwörter) oder speichert sie nicht. Datei und Kennwort werden nur zum Extrahieren eines privaten Schlüssels/Zertifikats verwendet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Klicken Sie nach Eingabe der Verbindungsinformationen auf **[!UICONTROL Weiter]** , um eine Verbindung herzustellen.

## [!UICONTROL SFTP] -Module und ihre Felder

Wenn Sie die Module [!UICONTROL SFTP] konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!UICONTROL SFTP] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trigger

#### [!UICONTROL Dateien in einem Ordner überwachen]

Gibt Dateien mit Details zurück, wenn eine Datei in einem angegebenen Ordner erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein oder ordnen Sie ihn zu. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Puffergröße [B]</td> 
   <td> <p> Geben Sie die Puffergröße in Byte ein. Der Wert definiert die Größe der übertragenen Blöcke vom Server. Einige Server können Probleme verursachen oder Dateien beschädigen, wenn der Wert zu hoch ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Dateien]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Dateien fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Unterordner in einem Ordner ansehen]

Gibt Ordner mit Details zurück, wenn ein Ordner in einem angegebenen Ordner erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein oder ordnen Sie ihn zu. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Dateien]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ordnern fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgeben wird.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

#### [!UICONTROL Inhalt eines Ordners auflisten]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Show] </td> 
   <td> <p>Wählen Sie aus, ob Sie Dateien, Ordner oder beides abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein oder ordnen Sie ihn zu, der die Dateien oder Ordner enthält, die Sie auflisten möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Geben Sie den Suchbegriff ein oder ordnen Sie ihn zu. Wenn Sie beispielsweise nach Dateien mit der Dateierweiterung .txt suchen möchten, geben Sie <code>.txt</code> ein. Sie können auch den Namen der Datei eingeben oder zuordnen, nach der Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Sortieren nach:</td> 
   <td> <p> Wählen Sie aus, ob die Ergebnisse nach Dateiname, Größe, Datum des letzten Zugriffs oder Datum der letzten Änderung sortiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sortierreihenfolge] </td> 
   <td> <p>Wählen Sie aus, ob das Ergebnis in auf- oder absteigender Reihenfolge zurückgegeben werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Fortfahren der Routenausführung, selbst wenn das Modul keine Ergebnisse zurückgibt]</p> </td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass dieses Modul das Szenario nicht stoppt, wenn es keine Ergebnisse zurückgibt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgibt.</p> </td> 
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
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Puffergröße [B]]</td> 
   <td> <p> Geben Sie die Puffergröße in Byte ein. Der Wert definiert die Größe der übertragenen Blöcke vom Server. Einige Server können Probleme verursachen oder Dateien beschädigen, wenn der Wert zu hoch ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein oder ordnen Sie ihn zu, der die Dateien oder Ordner enthält, die Sie auflisten möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suche] </td> 
   <td> <p>Geben Sie den Suchbegriff ein oder ordnen Sie ihn zu. Wenn Sie beispielsweise nach Dateien mit der Dateierweiterung .txt suchen möchten, geben Sie <code>.txt</code> ein. Sie können auch den Namen der Datei eingeben oder zuordnen, nach der Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Sortieren nach:</td> 
   <td> <p> Wählen Sie aus, ob die Ergebnisse nach Dateiname, Größe, Datum des letzten Zugriffs oder Datum der letzten Änderung sortiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sortierreihenfolge]</td> 
   <td> <p> Wählen Sie aus, ob das Ergebnis in auf- oder absteigender Reihenfolge zurückgegeben werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Fortfahren der Routenausführung, selbst wenn das Modul keine Ergebnisse zurückgibt]</p> </td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass dieses Modul das Szenario nicht stoppt, wenn es keine Ergebnisse zurückgibt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Dateien fest, die [!DNL Workfront Fusion] während eines Zyklus zurückgibt.</p> </td> 
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
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Puffergröße [B]]</td> 
   <td> <p> Geben Sie die Puffergröße in Byte ein. Der Wert definiert die Größe der übertragenen Blöcke vom Server. Einige Server können Probleme verursachen oder Dateien beschädigen, wenn der Wert zu hoch ist.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad] </td> 
   <td> <p>Geben Sie den Pfad zur Datei ein. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL  Datei hochladen]

Mit diesem Modul können Sie eine Datei auf den SFTP-Server hochladen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Geben Sie einen vorhandenen Ordner als Speicherort für die Datei an. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p> Ordnen Sie die Quelldatei von einem vorherigen Modul zu, z. B. [!UICONTROL Dropbox] &gt; [!UICONTROL Datei abrufen]. Sie können auch den Dateinamen und die Dateidaten eingeben oder zuordnen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Berechtigungen]</p> </td> 
   <td> <p>Legen Sie die gewünschten Berechtigungen für die Datei oder den Ordner fest. Verwenden Sie die Parameter chmod . Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Weitere Informationen zu chmod finden Sie in der Dokumentation zu <a href="https://ss64.com/bash/chmod.html">chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Datei umbenennen]

Benennt eine Datei um.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zu der Datei ein, die Sie umbenennen möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
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
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zu der Datei ein, die Sie verschieben möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL New Folder]</td> 
   <td> <p> Geben Sie den Pfad zum neuen Speicherort der Datei ein. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei löschen]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zu der Datei ein, die Sie löschen möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren der Dateiberechtigungen]

Ermöglicht das Ändern der Berechtigungen der Datei.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zu der Datei ein, die Sie verschieben möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Berechtigungen]</p> </td> 
   <td> <p>Legen Sie die gewünschten Dateiberechtigungen fest. Verwenden Sie die Parameter chmod . Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Muss dem Muster entsprechen <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Weitere Informationen zu chmod finden Sie in der Dokumentation zu <a href="https://ss64.com/bash/chmod.html">chmod</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner erstellen]

Erstellt einen neuen Ordner am angegebenen Speicherort.

>[!NOTE]
>
>Wenn der Ordner bereits vorhanden ist, gibt das Modul einen Fehler aus. Um den Fluss unterbrechungsfrei fortzusetzen, fügen Sie eine Fehler-Handler-Route an das Modul an, um den Fehler zu erfassen, und wenden Sie die Anweisung [!UICONTROL Fortsetzen] an, um den Fluss fortzusetzen. Informationen zum Anhängen einer Fehler-Handler-Route finden Sie unter [Umgang mit Fehlern in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Informationen zur Route des Fehler-Handlers finden Sie unter [Richtlinien für die Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Geben Sie einen vorhandenen Ordner als Speicherort für den neuen Ordner an. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordnername]</td> 
   <td> <p> Geben Sie den Ordnernamen ein.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Berechtigungen]</p> </td> 
   <td> <p>Legen Sie die gewünschten Ordnerberechtigungen fest. Verwenden Sie die Parameter chmod . Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Muss dem Muster entsprechen <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Weitere Informationen zu chmod finden Sie auf der <a href="https://ss64.com/bash/chmod.html">chmod Man Page</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner löschen]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP mit [!DNL Workfront Fusion]</a> verbinden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Geben Sie den Pfad zum Ordner an, den Sie löschen möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
