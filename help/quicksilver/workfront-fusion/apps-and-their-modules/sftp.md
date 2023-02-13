---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP-Module
description: Die [!DNL Adobe Workfront Fusion SFTP] -Module ermöglichen es Ihnen, Dateiänderungen in einem ausgewählten Ordner/Unterordner zu überwachen, neue Dateien in den gewünschten Ordner hochzuladen, vorhandene Dateien, die sich bereits in einem Ordner befinden, zu ändern oder zu löschen oder die Dateiberechtigungen zu ändern.
author: Becky
feature: Workfront Fusion
exl-id: aacc61f8-ffc3-48db-9f54-188685c52067
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1883'
ht-degree: 0%

---

# SFTP-Module

Die [!DNL Adobe Workfront Fusion] SFMit TP-Modulen können Sie Dateiänderungen in einem ausgewählten Ordner/Unterordner überwachen, neue Dateien in den gewünschten Ordner hochladen, vorhandene Dateien, die sich bereits in einem Ordner befinden, ändern oder löschen oder die Dateiberechtigungen ändern.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

So verwenden Sie SFTP mit [!DNL Workfront Fusion]muss ein SFTP-Konto vorhanden sein (z. B. [!DNL GoDaddy] Webhosting).

## SFTP verbinden mit [!DNL Workfront Fusion] {#connect-sftp-to-workfront-fusion}

So verbinden Sie Ihr SFTP-Konto mit [!DNL Workfront Fusion] Sie müssen den Zielhost und die SFTP-Anmeldeinformationen (Benutzername und Kennwort oder Benutzername und Schlüssel) für die [!UICONTROL Verbindung erstellen] angezeigt.

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
     <li><strong>[!UICONTROL Benutzername und Kennwort]</strong>: Geben Sie Ihre Anmeldedaten ein.</li> 
     <li> <p><strong>[!UICONTROL Benutzername und Schlüssel]</strong>: Geben Sie Ihren Benutzernamen und den privaten Schlüssel/Zertifikat ein.</p> <p>Laden Sie den privaten Schlüssel hoch, um die clientseitige Autorisierung zu verwenden, oder laden Sie Ihr Zertifikat hoch (P12- oder PFX-Datei), wenn Sie TLS mit Ihrem selbstsignierten Zertifikat verwenden möchten. Wenn Sie die clientseitige Zertifikatsautorisierung verwenden, können Sie hier Ihr Zertifizierungsstellenzertifikat eingeben.</p> <p>[!DNL Workfront Fusion] speichert keine von Ihnen angegebenen Daten (Dateien, Kennwörter) oder speichert sie nicht. Datei und Kennwort werden nur zum Extrahieren eines privaten Schlüssels/Zertifikats verwendet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Klicken Sie nach Eingabe der Verbindungsinformationen auf **[!UICONTROL Weiter]** um eine Verbindung herzustellen.

## [!UICONTROL SFTP] Module und ihre Felder

Bei der Konfiguration [!UICONTROL SFTP] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!UICONTROL SFTP] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trigger

#### [!UICONTROL Überwachungsdateien in einem Ordner]

Gibt Dateien mit Details zurück, wenn eine Datei in einem angegebenen Ordner erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
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
   <td> <p> Legen Sie die maximale Anzahl von Dateien fest, die [!DNL Workfront Fusion] arbeitet mit</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Unterordner in einem Ordner überwachen]

Gibt Ordner mit Details zurück, wenn ein Ordner in einem angegebenen Ordner erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Geben Sie den Ordner ein oder ordnen Sie ihn zu. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl an zurückgegebenen Dateien]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ordnern fest, die [!DNL Workfront Fusion] wird während eines Zyklus zurückgegeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

#### [!UICONTROL Ordnerinhalt auflisten]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
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
   <td> <p>Geben Sie den Suchbegriff ein oder ordnen Sie ihn zu. Wenn Sie beispielsweise nach Dateien mit der Dateierweiterung .txt suchen möchten, geben Sie <code>.txt</code>.Sie können auch den Namen der Datei eingeben oder zuordnen, nach der Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sortieren nach]</td> 
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
   <td> <p> Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] wird während eines Zyklus zurückgegeben.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
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
   <td> <p>Geben Sie den Suchbegriff ein oder ordnen Sie ihn zu. Wenn Sie beispielsweise nach Dateien mit der Dateierweiterung .txt suchen möchten, geben Sie <code>.txt</code>.Sie können auch den Namen der Datei eingeben oder zuordnen, nach der Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sortieren nach]</td> 
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
   <td> <p> Legen Sie die maximale Anzahl von Dateien fest, die [!DNL Workfront Fusion] wird während eines Zyklus zurückgegeben.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
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

#### [!UICONTROL Datei hochladen]

Mit diesem Modul können Sie eine Datei auf den SFTP-Server hochladen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Geben Sie einen vorhandenen Ordner als Speicherort für die Datei an. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quelldatei]</td> 
   <td> <p> Ordnen Sie die Quelldatei von einem vorherigen Modul zu, z. B. [!UICONTROL Dropbox] &gt; [!UICONTROL Datei abrufen]. Sie können auch den Dateinamen und die Dateidaten eingeben oder zuordnen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Berechtigungen]</p> </td> 
   <td> <p>Legen Sie die gewünschten Berechtigungen für die Datei oder den Ordner fest. Verwenden Sie die Parameter chmod . Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Weitere Informationen zu chmod finden Sie im Abschnitt <a href="https://ss64.com/bash/chmod.html">chmod-Dokumentation</a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zu der Datei ein, die Sie verschieben möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Neuer Ordner]</td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zur Datei ein, die Sie löschen möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dateiberechtigungen aktualisieren]

Ermöglicht das Ändern der Berechtigungen der Datei.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dateipfad]</td> 
   <td> <p> Geben Sie den Pfad zu der Datei ein, die Sie verschieben möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/file.txt</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Berechtigungen]</p> </td> 
   <td> <p>Legen Sie die gewünschten Dateiberechtigungen fest. Verwenden Sie die Parameter chmod . Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Muss dem Muster entsprechen <code> /(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Weitere Informationen zu chmod finden Sie im Abschnitt <a href="https://ss64.com/bash/chmod.html">chmod-Dokumentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ordner erstellen]

Erstellt einen neuen Ordner am angegebenen Speicherort.

>[!NOTE]
>
>Wenn der Ordner bereits vorhanden ist, gibt das Modul einen Fehler aus. Um den Fluss unterbrechungsfrei fortzusetzen, fügen Sie eine Fehler-Handler-Route an das Modul an, um den Fehler zu erfassen, und wenden Sie die [!UICONTROL Fortsetzen] , um den Fluss fortzusetzen. Informationen zum Anhängen einer Fehler-Handler-Route finden Sie unter [Umgang mit Fehlern in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md). Informationen zur Fehler-Handler-Route finden Sie unter [Richtlinien zur Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td>
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
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
   <td> <p>Legen Sie die gewünschten Ordnerberechtigungen fest. Verwenden Sie die Parameter chmod . Beispiel: <code>777 </code>oder <code>-rwxrwxrwx</code>.</p> <p>Muss dem Muster entsprechen <code>/(.?([r-][w-][x-]){3})|[0-7]{3}/.</code></p> <p>Weitere Informationen zu chmod finden Sie im Abschnitt <a href="https://ss64.com/bash/chmod.html">chmod Man-Seite</a>.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres SFTP-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">SFTP verbinden mit [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Folder Path]</td> 
   <td> <p> Geben Sie den Pfad zum Ordner an, den Sie löschen möchten. Sie können einen absoluten Pfad angeben, z. B. <code>/home/user/</code>. Sie können auch einen relativen Pfad angeben, der auf einen bestimmten Ordner des angemeldeten Benutzers verweist, z. B. <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
