---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Acrobat Sign-Module
description: Mit den [!DNL Adobe Acrobat Sign] Modulen können Sie ein [!DNL Adobe Workfront Fusion] Szenario starten, das auf Ereignissen in Ihrem [!DNL Adobe] Acrobat Sign-Konto basiert, Vereinbarungen und andere Datensätze erstellen, lesen oder aktualisieren, nach Datensätzen anhand von von Ihnen festgelegten Kriterien suchen und Dokumente hochladen.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 01158218-31a6-4c68-a9b7-6a678a8f40c9
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '6652'
ht-degree: 0%

---

# [!DNL Adobe Acrobat Sign] Module

Mit den [!DNL Adobe Acrobat Sign] -Modulen können Sie ein [!DNL Adobe Workfront Fusion] -Szenario starten, das auf Ereignissen in Ihrem [!DNL Adobe Acrobat Sign] -Konto basiert, Vereinbarungen und andere Datensätze erstellen, lesen oder aktualisieren, nach Datensätzen anhand von von Ihnen festgelegten Kriterien suchen und Dokumente hochladen.

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

## [!DNL Adobe Acrobat Sign] API-Informationen

Der Adobe Acrobat Sign-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v6 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.35.1</td> 
  </tr>
 </tbody> 
</table>


## [!DNL Adobe Acrobat Sign] Empfehlungen zur Verwendung des Connectors

Die [!DNL Adobe Sign]App macht die Automatisierung von eSignature-Geschäftsprozessen in [!DNL Fusion] viel einfacher und leistungsfähiger.

Neue Benutzer von [!DNL Adobe Sign] sollten einige der Einschränkungen bei der Aktualisierung von Vereinbarungen genau beachten. Vereinbarungen werden in der Regel nicht geändert, wenn sie einmal begonnen wurden. Es wird empfohlen, dass sich neue Benutzer von [!DNL Adobe Sign] auf die Erstellung neuer Vereinbarungen mithilfe des Moduls zur Vertragserstellung konzentrieren. Dies erleichtert die Arbeit mit [!DNL Adobe Sign] mit [!DNL Fusion] -Automatisierungen.

[!DNL Adobe Sign] Vereinbarungen benötigen ein Feld, mit dem sie funktionieren. Es gibt verschiedene Möglichkeiten, dies zu tun. Am einfachsten und gängigsten ist jedoch das Hochladen eines Verlaufsdokuments und das anschließende Zuordnen dieses Dokuments zu Ihrer Vereinbarung.

![](assets/adobe-sign-recommendations-350x168.png)

## [!DNL Adobe Acrobat Sign] Module und ihre Felder

Wenn Sie [!DNL Adobe Acrobat Sign] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe Acrobat Sign] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

<!--
* [Watch for agreements](#watch-for-agreements) 
* [Watch for events](#watch-for-events)
-->

+++ **[!UICONTROL Auf Vereinbarungen achten]**

Dieses Trigger-Modul startet ein Szenario, wenn eine Vereinbarung erstellt oder aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
<td>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Wählen Sie aus, ob Sie nach neuen, aktualisierten Datensätzen oder beidem suchen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type] </td> 
   <td>Wählen Sie den Typ des Datensatzes aus, den der Datensatz sehen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text suchen]</td> 
   <td> <p>Geben Sie Begriffe ein, nach denen Sie suchen möchten. Das Modul gibt Datensätze zurück, die diese Begriffe als Feldwerte enthalten.</p> <p>Weitere Informationen zum Durchsuchen von Feldern in [!DNL Adobe Acrobat Sign] finden Sie unter "Funktionsweise der Textsuche"in <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">Adobe Sign-Suche - Funktionsweise</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Verträge]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Auf Ereignisse achten]**

Dieses Trigger-Modul startet ein Szenario, wenn ein von Ihnen ausgewähltes Ereignis auftritt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td>Wählen Sie den Webhook aus, den Sie verwenden möchten, oder klicken Sie auf <b>[!UICONTROL Add]</b> und füllen Sie die folgenden Felder aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p>Geben Sie einen Namen für den Webhook ein</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bereiche]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL Konto]</p> </li> 
     <li> <p>[!UICONTROL Group]</p> </li> 
     <li> <p>[!UICONTROL Benutzer]</p> </li> 
     <li> <p>[!UICONTROL Resource]</p> <p>Wenn Sie [!UICONTROL Resource] auswählen, geben Sie die Ressourcen-ID und den Ressourcentyp ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ressourcenebene]</td> 
   <td> <p>Wählen Sie den Ressourcentyp aus, den Sie sehen möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Agreement]</p> </li> 
     <li> <p>[!UICONTROL Widgets]</p> </li> 
     <li> <p>[!UICONTROL Megasign]</p> </li> 
     <li> <p>[!UICONTROL Bibliotheksdokumente]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook-Abonnementereignisse]</td> 
   <td>Wählen Sie die [!DNL Adobe Sign]-Ereignisse aus, die das Modul überwachen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzeigename der Anwendung]</td> 
   <td>Der Anzeigename der Anwendung, über die der Webhook erstellt wird.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anwendungsname]</td> 
   <td>Der Anzeigename der Anwendung, über die der Webhook erstellt wird.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Problem-Benachrichtigungs-E-Mails]</td> 
   <td> <p>Diese Einstellung funktioniert nur für Administratorkonten</p> <p>Klicken Sie für jede E-Mail-Adresse, an die Sie Problembenachrichtigungs-E-Mails senden möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie die E-Mail-Adresse ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bedingte Parameter der [!UICONTROL Vereinbarung]</td> 
   <td>Wenn Sie bedingte Parameter hinzufügen möchten, wählen Sie "<b>[!UICONTROL Ja]</b>"für den Datensatztyp, dem Sie Parameter hinzufügen möchten, und wählen Sie dann "<b>[!UICONTROL Ja]</b>"für alle Parameter aus, die Sie aktivieren möchten.</td> 
  </tr> 
 </tbody> 
</table>

+++

### Aktionen

<!--
* [Create a record](#create-a-record) 
* [Create an agreement](#create-an-agreement) 
* [Create related records](#create-related-records) 
* [Custom API Call](#custom-api-call) 
* [List records](#list-records) 
* [Read a record](#read-a-record) 
* [Read related records](#read-related-records) 
* [Update a record](#update-a-record) 
* [Update related record](#update-related-record) 
* [Upload document](#upload-document)
-->

+++ **[!UICONTROL Erstellen eines Datensatzes]**

Dieses Aktionsmodul erstellt einen neuen Datensatz des ausgewählten Typs.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td>Fügen Sie die Header der Anforderung in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Group]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Library document]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Benutzer]</b> </p> </li> 
     <li> <p><b>[!UICONTROL Webformular] ([!UICONTROL Widget])</b> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gruppeninfo]</td> 
   <td> <p>Geben Sie [!UICONTROL Name] und [!UICONTROL ID] der Gruppe ein oder ordnen Sie sie zu und geben Sie an, ob diese Gruppe die Standardgruppe für das Konto ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Library document info]</td> 
   <td> <p>Füllen Sie die folgenden Felder aus:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Zu sendende Dateien]</b> </p> <p>Klicken Sie für jede Datei, die Sie hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie die Felder aus.</p> 
      <ul> 
       <li><b>[!UICONTROL Verlaufs-Dokument-ID]</b> <p>Kennung des Verlaufsdokuments eingeben</p> </li> 
       <li> <p><b>[!UICONTROL URL file transfer]</b> </p> <p>Füllen Sie die folgenden Felder aus:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL MIME-Type]</b> </p> <p>Geben Sie den MIME-Typ der Originaldatei ein. MIME-Typen (Multizweck Internet Mail Extension) sind Bezeichnungen, mit denen Software verschiedene Arten von im Internet freigegebenen Daten identifizieren kann. Webserver und Browser verwenden den MIME-Typ, um zu bestimmen, was mit einer Datei gemacht werden soll. Beispielsweise wird eine Datei mit dem MIME-Typ <code>text/html</code> in einem Browser anders verarbeitet als eine Datei mit dem MIME-Typ <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Geben Sie einen Namen für die Datei ein.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>Geben Sie die URL der Datei ein, die Sie senden möchten.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>Wählen Sie aus, ob dieses Dokument notarialisiert werden soll.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Bibliotheksvorlagenname]</b> </p> <p>Geben Sie den Namen der Bibliotheksvorlage ein oder ordnen Sie ihn zu</p> </li> 
     <li> <p><b>[!UICONTROL Freigabemodus]</b> </p> <p>Geben Sie an, wer Zugriff auf das Bibliotheksdokument haben soll.</p> </li> 
     <li> <p><b>[!UICONTROL Library document state]</b> </p> <p>Wählen Sie aus, ob das Dokument den Authoring-Status aufweist oder aktiv ist.</p> </li> 
     <li> <p><b>[!UICONTROL Bibliotheksvorlagentyp]</b> </p> <p>Klicken Sie für jeden Bibliotheksvorlagentyp, den Sie verwenden möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie den Vorlagentyp aus.</p> </li> 
     <li> <p><b>[!UICONTROL Letztes Ereignisdatum]</b> </p> <p>Geben Sie das letzte Datum ein, an dem ein Ereignis im Bibliotheksdokument aufgetreten ist.</p> <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
     <li> <p><b>[!UICONTROL Library document status]</b> </p> <p>Wählen Sie den Status des Bibliotheksdokuments aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerinformationen]</td> 
   <td> <p>Füllen Sie die folgenden Felder aus:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Email]</b> </p> <p>Geben Sie die E-Mail-Adresse des Benutzers ein.</p> </li> 
     <li> <p><b>[!UICONTROL Is Account Admin]</b> </p> <p>Aktivieren Sie diese Option, wenn der erstellte Benutzer ein Kontoadministrator ist.</p> </li> 
     <li> <p><b>[!UICONTROL Benutzer-ID]</b> </p> <p>Eindeutige Kennung des Benutzers eingeben</p> </li> 
     <li> <p><b>[!UICONTROL Konto-ID]</b> </p> <p>Geben Sie die eindeutige ID des diesem Benutzer zugeordneten [!DNL Adobe Acrobat Sign]-Kontos ein.</p> </li> 
     <li> <p><b>[!UICONTROL Vorname]</b> </p> <p>Geben Sie den Vornamen des Benutzers ein.</p> </li> 
     <li> <p><b>[!UICONTROL Nachname]</b> </p> <p>Nachnamen des Benutzers eingeben</p> </li> 
     <li> <p><b>[!UICONTROL Company]</b> </p> <p>Geben Sie den Namen des Unternehmens des Benutzers ein.</p> </li> 
     <li> <p><b>[!UICONTROL Initials]</b> </p> <p>Geben Sie die Initialen des Benutzers ein.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Geben Sie das Gebietsschema des Benutzers ein. Dadurch wird die Sprache der Benutzeroberfläche bestimmt. </p> </li> 
     <li> <p><b>[!UICONTROL Telefon]</b> </p> <p>Telefonnummer des Benutzers eingeben</p> </li> 
     <li> <p><b>Primäre Gruppen-ID</b> </p> <p>Geben Sie die Gruppe ein, der der neue Benutzer hinzugefügt wird. Wenn nichts eingegeben wird, wird der Benutzer der Standardgruppe für das Konto hinzugefügt.</p> </li> 
     <li> <p><b>[!UICONTROL Auftragstitel]</b> </p> <p>Geben Sie die Berufsbezeichnung des Benutzers ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webformularinformationen]</td> 
   <td> <p>Füllen Sie die folgenden Felder aus</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Dateiinformationen]</b> </p> <p>Klicken Sie für jede Datei, die Sie zum Webformular hinzufügen möchten, auf Hinzufügen und füllen Sie die folgenden Felder aus:</p> 
      <ul> 
       <li> <p>[!UICONTROL Dateityp]</p> <p>[!UICONTROL Document]</p> </li> 
       <li> <p>[!UICONTROL Übergangsdokument]</p> </li> 
       <li> <p>[!UICONTROL URL file info]</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Webformularname]</b> </p> <p>Geben Sie einen Namen für das Webformular ein. Dieser Name wird verwendet, um das Webformular an Orten wie E-Mails und Websites zu identifizieren.</p> </li> 
     <li> <p><b>[!UICONTROL Web form state]</b> </p> <p>Wählen Sie den Status aus, in dem das neue Webformular erstellt werden soll.</p> </li> 
     <li> <p><b>[!UICONTROL Webformularteilnehmerset info]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Member info]</b> </p> <p>Klicken Sie für jedes Mitglied, das Sie dem Teilnehmersatz hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b>. </p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>Lassen Sie diese Option leer.</p> </li> 
         <li> <p><b>[!UICONTROL Sicherheitsoption]</b> </p> <p>Wenn Sie eine Sicherheitsoption für die Authentifizierung dieses Benutzers hinzufügen möchten, wählen Sie <b>[!UICONTROL Yes]</b>, wählen Sie dann die Sicherheitsoption aus und füllen Sie alle erforderlichen Felder aus.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Rolle]</b> </p> <p>Wählen Sie die Rolle aus. Alle Mitglieder dieses Teilnehmersatzes teilen sich die Rolle.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Webformular - zusätzlicher Teilnehmer legt Informationen fest]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Member info]</b> </p> <p>Klicken Sie für jedes Mitglied, das Sie dem Teilnehmersatz hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b>.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>Lassen Sie diese Option leer.</p> </li> 
         <li> <p><b>[!UICONTROL Sicherheitsoption]</b> </p> <p>Wenn Sie eine Sicherheitsoption für die Authentifizierung dieses Benutzers hinzufügen möchten, wählen Sie <b>[!UICONTROL Yes]</b>, wählen Sie dann die Sicherheitsoption aus und füllen Sie alle erforderlichen Felder aus.</p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Rolle]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Teilnehmer-ID des Webformulars] </b> </p> <p>Geben Sie die Kennung des Webformularteilnehmers ein.</p> </li> 
       <li> <p><b>[!UICONTROL Order]</b> </p> <p>Geben Sie die Reihenfolge an, in der dieser Teilnehmersatz mit dem Webformular interagieren soll. Beispielsweise muss die Teilnehmergruppe mit dem Bestellwert 1 zuerst gehen, 2 als Nächstes gehen usw. Bestellnummern müssen mit einer beginnen und keine Lücken in der Reihe aufweisen. </p> </li> 
       <li> <p><b>[!UICONTROL Provider participant set info]</b> </p> <p>Wenn der Teilnehmer unbekannt ist, geben Sie an, ob der Provider Details für den Teilnehmer angeben muss, und geben Sie eine Nachricht mit den Details ein, die Sie für den unbekannten Teilnehmer benötigen.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Informationen zu Authentifizierungsfehlern]</b> </p> <p>Wenn Sie eine Fehler- oder Fehlerseite für Ihre Benutzer bereitstellen möchten, wählen Sie <b>[!UICONTROL Yes]</b> aus und füllen Sie dann die folgenden Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>Geben Sie die URL für die Fehlerseite ein.</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Aktivieren Sie diese Option, wenn die Fehlerseite im Webformular angezeigt werden soll.</p> </li> 
       <li> <p><b>[!UICONTROL Verzögerung]</b> </p> <p>Geben Sie die Verzögerung in Sekunden ein, bevor der Benutzer zur Fehlerseite weitergeleitet wird.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL CC info]</b> </p> <p>Klicken Sie für jede E-Mail-Adresse, an die Sie eine E-Mail erhalten möchten, wenn die endgültige Vereinbarung im Webformular unterzeichnet wird, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die E-Mail-Adresse ein.</p> </li> 
     <li> <p><b>[!UICONTROL Abschlussinfo]</b> </p> <p style="font-style: normal;">Wenn Sie eine Erfolgsseite für Ihre Benutzer bereitstellen möchten, wählen Sie <b>[!UICONTROL Yes]</b> aus und füllen Sie dann die folgenden Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL URL]</b> </p> <p>Geben Sie die URL für die Erfolgsseite ein</p> </li> 
       <li> <p><b>[!UICONTROL Deframe]</b> </p> <p>Aktivieren Sie diese Option, wenn die Erfolgsseite im Webformular angezeigt werden soll.</p> </li> 
       <li> <p><b>[!UICONTROL Verzögerung]</b> </p> <p>Geben Sie die Verzögerung in Sekunden ein, bevor der Benutzer zur Erfolgsseite weitergeleitet wird.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Gruppen-ID]</b> </p> <p>Geben Sie die Kennung der Gruppe ein, zu der das Webformular gehört. Wenn nichts eingegeben wird, gehört das Webformular zur primären Gruppe des Kontobenutzers.</p> </li> 
     <li> <p><b>[!UICONTROL Letztes Ereignisdatum]</b> </p> <p>Geben Sie das Datum ein, an dem das letzte Ereignis im Webformular aufgetreten ist. Verwenden Sie das Format <code>yyyy-MM-dd'T'HH:mm:ssZ</code>.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Geben Sie das Gebietsschema des Benutzers ein. Dadurch wird die Sprache der Benutzeroberfläche bestimmt. </p> </li> 
     <li> <p><b>[!UICONTROL Sicherheitsoption]n</b> </p> <p>Geben Sie das Kennwort ein, das zum Schützen des Dokuments verwendet wird. Sie müssen dieses Passwort separat an alle Beteiligten weitergeben.</p> </li> 
     <li> <p><b>[!UICONTROL Überprüfungsinformationen]</b> </p> <p>Wenn Ihr Konto für die Dokumentüberprüfung eingerichtet ist und die Option, pro Vereinbarung zu aktivieren, können Sie diese Option aktivieren, um diese Vereinbarung zu verwerfen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Eine Vereinbarung erstellen]**

Dieses Aktionsmodul erstellt eine Vereinbarung, sendet sie zur Signatur und gibt die Vereinbarung-ID zurück.

>[!NOTE]
>
>Es wird empfohlen, das zu signierende Dokument hochzuladen und es dann dem Feld [!UICONTROL Zu sendende Datei] im Modul [!UICONTROL Vereinbarung erstellen] zuzuordnen. Ein Beispiel finden Sie unter &quot;Dokument hochladen&quot;in diesem Artikel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
<td>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td>  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td>Fügen Sie die Header der Anforderung in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"Content-type":"application/json"}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zu sendende Dateien]</td> 
   <td> <p>Klicken Sie für jedes Element, das Sie in die Vereinbarung aufnehmen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie die folgenden Felder aus:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Dateityp]</b> </p> 
      <ul> 
       <li> <p><b>[!UICONTROL Document]</b> </p> <p>Füllen Sie die folgenden Felder aus:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Erstellungsdatum]</b> </p> <p>Geben Sie das Datum ein, an dem das Dokument im Format <code>yyyy-MM-dd'T'HH:mm:ssZ</code> erstellt wurde, oder ordnen Sie es zu. Beispielsweise steht <code>2016-02-25T18:46:19Z</code> für die UTC-Zeit.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>Geben Sie die Kennung des Dokuments ein oder ordnen Sie sie zu.</p> </li> 
         <li> <p><b>[!UICONTROL Titel]</b> </p> <p>Geben Sie einen eindeutigen Titel für die Datei ein oder ordnen Sie ihn zu. Bei einem benutzerdefinierten Workflow wird eine Datei dem entsprechenden Dateielement in der Workflow-Definition zugeordnet. Dies muss im Falle einer Anforderung zur Erstellung einer benutzerdefinierten Workflow-Vereinbarung angegeben werden.</p> </li> 
         <li> <p><b>[!UICONTROL Anzahl Seiten]</b> </p> <p>Geben Sie die Anzahl der Seiten im Dokument ein oder ordnen Sie sie zu.</p> </li> 
         <li> <p><b>[!UICONTROL MIME-Type]</b> </p> <p>Geben Sie den MIME-Typ der Originaldatei ein oder ordnen Sie ihn zu. MIME-Typen (Multizweck Internet Mail Extension) sind Bezeichnungen, mit denen Software verschiedene Arten von im Internet freigegebenen Daten identifizieren kann. Webserver und Browser verwenden den MIME-Typ, um zu bestimmen, was mit einer Datei gemacht werden soll. Beispielsweise wird eine Datei mit dem MIME-Typ <code>text/html</code> in einem Browser anders verarbeitet als eine Datei mit dem MIME-Typ <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Geben Sie einen Namen für das Dokument ein oder ordnen Sie ihn zu.<br></p> </li> 
        </ul> </li> 
       <li> <p><b>[!UICONTROL Library document ID]</b> </p> <p>ID des Bibliotheksdokuments eingeben</p> </li> 
       <li> <p><b>[!UICONTROL Verlaufs-Dokument-ID]</b> </p> <p>Kennung des Verlaufsdokuments eingeben</p> </li> 
       <li> <p><b>[!UICONTROL URL file transfer]</b> </p> <p>Füllen Sie die folgenden Felder aus:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL MIME-Type]</b> </p> <p>Geben Sie den MIME-Typ der Originaldatei ein. MIME-Typen (Multizweck Internet Mail Extension) sind Bezeichnungen, mit denen Software verschiedene Arten von im Internet freigegebenen Daten identifizieren kann. Webserver und Browser verwenden den MIME-Typ, um zu bestimmen, was mit einer Datei gemacht werden soll. Beispielsweise wird eine Datei mit dem MIME-Typ <code>text/html</code> in einem Browser anders verarbeitet als eine Datei mit dem MIME-Typ <code>image/jpeg</code>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Geben Sie einen Namen für die Datei ein.</p> </li> 
         <li> <p><b>[!UICONTROL URL]</b> </p> <p>Geben Sie die URL der Datei ein, die Sie senden möchten.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Titel]</b> </p> <p>Geben Sie einen Titel für die Datei ein.</p> </li> 
     <li> <p><b>[!UICONTROL Notarize]</b> </p> <p>Aktivieren Sie diese Option, um anzugeben, dass die Datei notarialisiert werden muss.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name des Vertrags]</td> 
   <td>Geben Sie einen Namen für die neue Vereinbarung ein. Dieser Name wird verwendet, um die Vereinbarung an Orten wie E-Mails und Websites zu identifizieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Teilnehmer legt Info fest]</td> 
   <td> <p>Klicken Sie für jeden Teilnehmersatz, den Sie hinzufügen möchten, auf "<b>[!UICONTROL Element hinzufügen]</b>"und füllen Sie die folgenden Felder aus.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Members]</b> </p> <p>Klicken Sie für jede Person, die Sie zum Teilnehmersatz hinzufügen möchten, auf "<b>[!UICONTROL Element hinzufügen]</b>"und geben Sie die E-Mail-Adresse der Person ein.</p> </li> 
     <li> <p><b>[!UICONTROL Order]</b> </p> <p>Geben Sie die Reihenfolge an, in der dieser Teilnehmersatz die Vereinbarung unterzeichnen soll. Beispielsweise muss die Teilnehmergruppe mit dem Bestellwert 1 zuerst signieren, 2 als Nächstes signieren usw. Bestellnummern müssen mit einer beginnen und keine Lücken in der Reihe aufweisen. </p> </li> 
     <li> <p><b>[!UICONTROL Rolle]</b> </p> <p>Wählen Sie eine Rolle für diesen Teilnehmersatz aus. Diese Rolle erhalten alle Teilnehmer des Sets.</p> </li> 
     <li> <p><b>[!UICONTROL ID]</b> </p> <p>Geben Sie die ID dieses Teilnehmersatzes ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><b>[!UICONTROL Titel]</b> </p> <p>Geben Sie einen eindeutigen Titel für den Teilnehmersatz ein oder ordnen Sie ihn zu. Bei benutzerdefinierten Workflows sollte die im Teilnahmesatz angegebene Bezeichnung dem Teilnahmeschritt im benutzerdefinierten Workflow zugeordnet werden.</p> </li> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Geben Sie einen Namen für die Teilnehmergruppe ein. Dieser Name muss innerhalb der Vereinbarung eindeutig sein.</p> </li> 
     <li> <p><b>[!UICONTROL Private Nachricht]</b> </p> <p>Geben Sie eine Nachricht für diesen Teilnehmersatz ein oder ordnen Sie sie zu. Alle Teilnehmer am Set erhalten diese Nachricht.</p> </li> 
     <li> <p><b>[!UICONTROL Sichtbare Seiten]</b> </p> <p>Wenn für diese Vereinbarung die eingeschränkte Sichtbarkeit des Dokuments aktiviert ist, geben Sie an, welche Dateien für diesen Teilnehmersatz sichtbar sind. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Signature type]</td> 
   <td> <p>Wählen Sie den Signaturtyp aus, den die Vereinbarung erfordert.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL E-Sign]</b> </p> <p>Das Abkommen muss elektronisch unterzeichnet werden.</p> </li> 
     <li> <p><b>[!UICONTROL Written]</b> </p> <p>Die Vereinbarung muss von Hand unterzeichnet werden, und die unterzeichnete Vereinbarung muss gescannt und hochgeladen werden.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL State]</td> 
   <td> <p>Wählen Sie einen Status für diese Vereinbarung aus.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Authoring]</b> </p> <p>Sie können dieser Vereinbarung weiterhin Felder bearbeiten oder hinzufügen.</p> </li> 
     <li> <p><b>[!UICONTROL Entwurf]</b> </p> <p>Sie können diese Vereinbarung schrittweise erstellen, bevor Sie sie versenden.</p> </li> 
     <li> <p><b>[!UICONTROL In Process]</b> </p> <p>Diese Vereinbarung wird unverzüglich übermittelt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CCs]</td> 
   <td> <p>Sie können diese Vereinbarung an interessierte Parteien, die nicht unterzeichnet werden müssen, wie z. B. Interessengruppen, senden. Sie erhalten zu Beginn des Signiervorgangs eine E-Mail und eine weitere, wenn die endgültige Signatur empfangen wird. Sie erhalten auch eine PDF-Kopie der Vereinbarung. </p> <p>Klicken Sie für jede Person, für die Sie diese Vereinbarung erstellen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und füllen Sie die folgenden Felder aus:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Email]</b> </p> <p>Geben Sie die E-Mail-Adresse ein oder ordnen Sie sie der Vereinbarung zu.</p> </li> 
     <li> <p><b>[!UICONTROL Titel]</b> </p> <p>Geben Sie einen Titel für diese E-Mail-Adresse ein oder ordnen Sie ihn zu, wie in der Workflow-Beschreibung dargestellt</p> </li> 
     <li> <p><b>[!UICONTROL Sichtbare Seiten]</b> </p> </li> 
     <li> <p>Wenn für diese Vereinbarung die eingeschränkte Sichtbarkeit des Dokuments aktiviert ist, geben Sie an, welche Dateien für diesen Teilnehmersatz sichtbar sind. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL E-Mail-Option]</td> 
   <td> <p>Wählen Sie für jeden E-Mail-Typ aus, ob dieser E-Mail-Typ an alle Teilnehmer gesendet wird oder nicht.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL E-Mails zum Abschluss]</b> </p> <p>Senden Sie eine E-Mail, wenn diese Vereinbarung abgeschlossen, abgebrochen, abgelaufen oder abgelehnt wird.</p> </li> 
     <li> <p><b>[!UICONTROL E-Mails im Flug]</b> </p> <p>Eine E-Mail wird gesendet, wenn diese Vereinbarung delegiert oder ersetzt wird.</p> </li> 
     <li> <p><b>[!UICONTROL Vereinbarung löst E-Mails]</b> </p> <p>Senden Sie eine E-Mail, wenn diese Vereinbarung erstellt wird oder eine entsprechende Aktion angefordert wird.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Externe ID]</td> 
   <td> <p>Geben Sie eine ID für diese Vereinbarung ein oder ordnen Sie sie zu. Sie können dies bei der Erstellung der Vereinbarung angeben und sie verwenden, um die Vereinbarung in späteren Modulen oder Abfragen zu finden.</p> <p>Hinweis: Der Wert "Externe ID"ist für alle Teilnehmer über die API sichtbar, daher sollte er nicht verwendet werden, um ein sensibles Token zu enthalten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Feldinformationen zusammenführen]</td> 
   <td> <p>Klicken Sie für jedes Feld in der Vereinbarung, für das Sie einen Standardwert festlegen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den Standardwert und den Feldnamen ein.</p> <p>Die Werte werden den Unterzeichnern für bearbeitbare Felder angezeigt. Für schreibgeschützte Felder sind die angegebenen Werte während des Signiervorgangs nicht bearbeitbar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Notar info]</td> 
   <td> <p>Füllen Sie die folgenden Felder aus:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Termin]</b> </p> <p>Geben Sie einen geplanten Zeitpunkt und einen Termin für die Ernennung ein oder ordnen Sie ihn zu, um diese Vereinbarung zu notieren.</p> </li> 
     <li> <p><b>[!UICONTROL Hinweis]</b> </p> <p>Geben Sie alle Notizen ein oder ordnen Sie sie zu der notariellen Sitzung zu.</p> </li> 
     <li> <p><b>[!UICONTROL Zahlung]</b> </p> <p>Wählen Sie aus, ob der Notar vom Unterzeichner oder vom Absender der Vereinbarung bezahlt wird.</p> </li> 
     <li> <p><b>[!UICONTROL Notar Type]</b> </p> <p>Wählen Sie den notariellen Typ aus</p> 
      <ul> 
       <li> <p>[!UICONTROL Provider notary]</p> <p>Der Notar wird vom Notar-Provider bereitgestellt.</p> </li> 
       <li> <p>[!UICONTROL BYON notary]</p> <p>Der Notar wird vom Kunden bereitgestellt.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Post-Signaturoption]</td> 
   <td> <p>Wählen Sie aus, ob die Unterzeichner nach Unterzeichnung der Vereinbarung zu einer Erfolgsseite weitergeleitet werden sollen. Wenn Sie <b>[!UICONTROL Yes]</b> auswählen, füllen Sie die folgenden Felder aus:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Umleitungsverzögerung]</b> </p> <p>Geben Sie eine Zahl ein oder ordnen Sie sie zu, die die Anzahl der Sekunden darstellt, bevor der Unterzeichner zur Erfolgsseite weitergeleitet wird. Wenn dieser Wert größer als 0 ist, wird dem Benutzer zuerst die standardmäßige [!DNL Adobe Sign] Erfolgsmeldung angezeigt und nach einer Verzögerung zu Ihrer Erfolgsseite weitergeleitet.</p> </li> 
     <li> <p><b>[!UICONTROL Umleitungs-URL]</b> </p> <p>Geben Sie eine öffentlich zugängliche URL ein oder ordnen Sie sie zu, an die der Benutzer nach erfolgreichem Abschluss des Signiervorgangs gesendet wird.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sicherheitsoption]</td> 
   <td> <p>Geben Sie das sekundäre Kennwort ein oder ordnen Sie es zu, das zum Schützen des PDF-Dokuments verwendet wird. </p> <p>Wichtig: [!DNL Adobe Sign] gibt dieses Kennwort nie frei. Daher müssen Sie es separat an alle relevanten Parteien weitergeben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Validierungsinformationen]</td> 
   <td>Wenn Ihr Konto für die Dokumentüberprüfung eingerichtet ist und die Option, pro Vereinbarung zu aktivieren, können Sie diese Option aktivieren, um diese Vereinbarung zu verwerfen.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Erstellen verwandter Datensätze]**

Dieses Aktionsmodul erstellt Datensätze, die mit einem ausgewählten Modul verknüpft sind.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Datensatztyp des ursprünglichen Datensatzes aus, mit dem Sie die erstellten Datensätze verknüpfen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>Geben Sie die ID des Objekts ein oder ordnen Sie sie zu, mit dem Sie den erstellten Datensatz verknüpfen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement related field]</td> 
   <td> <p>Wählen Sie den Typ des verwandten Felds aus, das Sie erstellen möchten</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Formularfelder]</b> </p> <p>Geben Sie die Vorlagen-ID der Vorlage ein, die die zu erstellenden Felder enthält</p> </li> 
     <li> <p><b>[!UICONTROL Erinnerungen]</b> </p> <p>Füllen Sie die folgenden Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Teilnehmer-ID]</b> </p> <p>Klicken Sie für jeden Teilnehmer, der an eine Erinnerung erinnert werden soll, auf [!UICONTROL Element hinzufügen] und geben Sie die Kennung des Teilnehmers ein.</p> </li> 
       <li> <p><b>[!UICONTROL Status]</b> </p> <p>Für neue Datensätze muss der Status [!UICONTROL Active] lauten.</p> </li> 
       <li> <p><b>[!UICONTROL Erste Erinnerungsverzögerung]</b> </p> <p>Geben Sie die Verzögerung in Stunden ein, bevor Sie die erste Erinnerung senden. Der zulässige Mindestwert beträgt 1 Stunde und der Höchstwert darf nicht größer sein als die Differenz zwischen der Vertragserstellung und der Ablaufzeit der Vereinbarung in Stunden. Wenn diese Verzögerung nicht festgelegt ist, basiert die erste Erinnerung auf der Häufigkeit.</p> </li> 
       <li> <p><b>[!UICONTROL Erinnerungsfrequenz]</b> </p> <p>Legen Sie die Häufigkeit fest, mit der die Erinnerung gesendet werden soll. Wenn keine Häufigkeit angegeben wird, wird die Erinnerung einmal gesendet.</p> </li> 
       <li> <p><b>[!UICONTROL Letztes Sendedatum]</b> </p> <p>Dieses Feld wird vom System festgelegt.</p> </li> 
       <li> <p><b>[!UICONTROL Nächstes Sendedatum]</b> </p> <p>Dieses Feld muss leer sein oder auf [!UICONTROL ONCE] gesetzt sein.</p> </li> 
       <li> <p><b>[!UICONTROL Hinweis]</b> </p> <p>Geben Sie einen Hinweis ein, der in die Erinnerung eingefügt werden soll. Dies ist nützlich, um dem Teilnehmer mitzuteilen, warum seine Teilnahme erforderlich ist.</p> </li> 
       <li> <p><b>[!UICONTROL Erinnerungszähler starten von]</b> </p> <p>Wählen Sie aus, ob die Erinnerung gesendet wird, basierend darauf, wann die Vereinbarung erstellt wird, sobald sie verfügbar wird.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Signer identity report]</b> </p> <p>Geben Sie das Kennwort ein, das zum Schützen des PDF-Dokuments verwendet wird.</p> </li> 
     <li> <p><b>[!UICONTROL Ansichten]</b> </p> <p>Füllen Sie die folgenden Felder aus</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Wählen Sie den Namen der Ansicht aus, die Sie erstellen möchten.</p> </li> 
       <li> <p><b>[!UICONTROL Benutzer für automatische Anmeldung]</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, um den Benutzer automatisch bei der zurückgegebenen URL anzumelden.</p> </li> 
       <li> <p><b>[!UICONTROL Frame Parent]</b> </p> <p>Geben Sie eine kommagetrennte Liste der URLs der übergeordneten Domäne ein oder ordnen Sie sie zu, in denen die zurückgegebenen URLs gespeichert werden können. Wenn dies leer gelassen wird, sind die [!DNL Adobe Acrobat Sign]-Seiten nicht im iframe sichtbar.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Geben Sie die Sprache ein, in der Sie die Ansicht erstellen möchten. </p> </li> 
       <li> <p><b>[!UICONTROL Kein Chrome-Flag]</b> </p> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, um die eingebettete Seite ohne Navigationskopfzeile oder Fußzeile anzuzeigen.</p> </li> 
       <li> <p><b>[!UICONTROL Kann Dateien bearbeiten]</b> </p> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, wenn Sie möchten, dass der Abschnitt zum Hochladen von Dateien bearbeitet wird, indem Sie Dateien hinzufügen oder entfernen. Dies ist kein Zugriffskontrollmechanismus. Der Standardwert ist [!UICONTROL Ja].</p> </li> 
       <li> <p><b>[!UICONTROL Library document]</b> </p> <p>Wählen Sie "<b>[!UICONTROL Ja]</b>", wenn Links für Bibliotheksdokumente sichtbar sein sollen. Der Standardwert ist [!UICONTROL Ja].</p> </li> 
       <li> <p><b>[!UICONTROL Lokale Datei]</b> </p> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, wenn die lokale Schaltfläche zum Hochladen von Dateien angezeigt werden soll. Der Standardwert ist [!UICONTROL Ja].</p> </li> 
       <li> <p><b>[!UICONTROL Web Connectors]</b> </p> <p>Wählen Sie "<b>[!UICONTROL Ja]</b>", wenn die Links zum Anhängen von Dokumenten aus Web-Quellen angezeigt werden sollen. Die Standardeinstellung ist "Ja".</p> </li> 
       <li> <p><b>[!UICONTROL Ist Vorschau ausgewählt]</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, um die Seite "Erstellen"auf den Authoring-Modus zu setzen.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Member Share]</b> </p> <p>Klicken Sie für jedes Mitglied, für das Sie die Vereinbarung freigeben möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die E-Mail-Adresse des Mitglieds sowie eine Nachricht an dieses Mitglied ein.</p> </li> 
     <li> <p>[!UICONTROL Teilnehmersatz delegieren]</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Teilnehmer-Set-ID]</b> </p> <p>Geben Sie die ID des Teilnehmersatzes ein.</p> </li> 
       <li> <p><b>[!UICONTROL Member info]</b> </p> <p>Klicken Sie für jedes Mitglied, das Sie hinzufügen möchten, auf [!UICONTROL Element hinzufügen] und geben Sie die E-Mail-Adresse und Telefoninformationen für das Mitglied ein.</p> </li> 
       <li> <p><b>[!UICONTROL Private Nachricht]</b> </p> <p>Geben Sie eine Nachricht ein. Alle Mitglieder des Teilnehmersatzes erhalten diese Nachricht.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bibliotheksansichtsinformationen]</td> 
   <td> <p>Füllen Sie die folgenden Felder aus:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Geben Sie einen Namen für die Bibliotheksvorlage ein. Dieser Name wird in E-Mails und Websites verwendet.</p> </li> 
     <li> <p><b>[!UICONTROL Benutzer für automatische Anmeldung]</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, um den Benutzer automatisch bei der zurückgegebenen URL anzumelden.</p> </li> 
     <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Geben Sie eine kommagetrennte Liste der URLs der übergeordneten Domäne ein oder ordnen Sie sie zu, in denen die zurückgegebenen URLs gespeichert werden können. Wenn dies leer gelassen wird, sind die [!DNL Adobe Acrobat Sign]-Seiten nicht im iframe sichtbar.</p> </li> 
     <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Geben Sie die Sprache ein, in der Sie die Ansicht erstellen möchten. </p> </li> 
     <li> <p><b>[!UICONTROL Kein Chrome-Flag]</b> </p> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, um die eingebettete Seite ohne Navigationskopfzeile oder Fußzeile anzuzeigen.</p> </li> 
     <li> <p><b>[!UICONTROL Konfiguration der Sendeansicht]</b> </p> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, wenn Sie die [!UICONTROL Senden]-Ansicht konfigurieren möchten, und füllen Sie dann die folgenden Felder aus.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Agreement name]</b> </p> <p>Geben Sie den Vertragsnamen für das Bibliotheksdokument auf der Seite "Erstellen"ein oder ordnen Sie ihn zu.</p> </li> 
       <li> <p><b>[!UICONTROL Kann Dateien bearbeiten]</b> </p> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, wenn Sie möchten, dass der Abschnitt zum Hochladen von Dateien bearbeitet wird, indem Sie Dateien hinzufügen oder entfernen. Dies ist kein Zugriffskontrollmechanismus. Der Standardwert ist [!UICONTROL Ja].</p> </li> 
       <li> <p><b>[!UICONTROL Lokale Datei]</b> </p> <p>Wählen Sie "<b>[!UICONTROL Ja]</b>", wenn Links für Bibliotheksdokumente sichtbar sein sollen. Der Standardwert ist [!UICONTROL Ja].</p> </li> 
       <li> <p><b>[!UICONTROL Web Connectors]</b> </p> <p>Wählen Sie "<b>[!UICONTROL Ja]</b>", wenn die Links zum Anhängen von Dokumenten aus Web-Quellen angezeigt werden sollen. Der Standardwert ist [!UICONTROL Ja].</p> </li> 
       <li> <p><b>Ist die Vorschau ausgewählt</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, um die Seite "Erstellen"auf den Authoring-Modus zu setzen.</p> </li> 
      </ul> <p> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzeransichtsinformationen]</td> 
   <td> <p>Füllen Sie die folgenden Felder aus</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Name]</b> </p> <p>Wählen Sie den Namen der angeforderten Benutzeransicht aus.</p> </li> 
     <li> <p><b>[!UICONTROL Benutzer für automatische Anmeldung]</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, um den Benutzer automatisch anzumelden. Wählen Sie <b>[!UICONTROL No]</b> aus, um Anmeldeinformationen anzufordern. Der Standardwert ist [!UICONTROL No].</p> </li> 
     <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Geben Sie eine kommagetrennte Liste der URLs der übergeordneten Domäne ein oder ordnen Sie sie zu, in denen die zurückgegebenen URLs gespeichert werden können. Wenn dies leer gelassen wird, sind die [!DNL Adobe Acrobat Sign]-Seiten nicht im iframe sichtbar.</p> </li> 
     <li> <p><b>Kein Chrome-Flag</b> </p> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, um die eingebettete Seite ohne Navigationskopfzeile oder Fußzeile anzuzeigen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Widget-bezogene Felder]</td> 
   <td> <p>Wählen Sie den zugehörigen Datensatz aus, den Sie erstellen möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Ansichten]</p> <p>Füllen Sie die folgenden Felder aus.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Wählen Sie den Namen der angeforderten Webformularansicht aus.</p> </li> 
       <li> <p><b>[!UICONTROL Benutzer für automatische Anmeldung]</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, um den Benutzer automatisch anzumelden. Wählen Sie <b>[!UICONTROL No]</b> aus, um Anmeldeinformationen anzufordern. Der Standardwert ist [!UICONTROL No].</p> </li> 
       <li> <p><b>[!UICONTROL Frame parent]</b> </p> <p>Geben Sie eine kommagetrennte Liste der URLs der übergeordneten Domäne ein oder ordnen Sie sie zu, in denen die zurückgegebenen URLs gespeichert werden können. Wenn dies leer gelassen wird, sind die [!DNL Adobe Acrobat Sign]-Seiten nicht im iframe sichtbar.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Geben Sie die Sprache ein, in der Sie die Ansicht erstellen möchten. </p> </li> 
       <li> <p><b>[!UICONTROL Kein Chrome-Flag]</b> </p> <p>Wählen Sie <b>[!UICONTROL Ja]</b> aus, um die eingebettete Seite ohne Navigationskopfzeile oder Fußzeile anzuzeigen.</p> </li> 
       <li> <p>[!UICONTROL Konfiguration der personalisierten Signaturansicht]</p> <p>Wenn Sie eine personalisierte Signaturansicht konfigurieren möchten, wählen Sie <b>[!UICONTROL Yes]</b> und füllen Sie die folgenden Felder aus:</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Email]</b> </p> <p>Geben Sie die E-Mail-Adresse des Empfängers des neu erstellten Webformulars ein</p> </li> 
         <li> <p><b>[!UICONTROL Kommentar]</b> </p> <p>Geben Sie einen Kommentar ein, in dem beschrieben wird, wie der API-Aufrufer die Identität des Unterzeichners ermittelt hat. Diese Informationen werden im Audit-Protokoll [!DNL Adobe Acrobat Sign] angezeigt.</p> </li> 
         <li> <p><b>[!UICONTROL Ablauf]</b> </p> <p>Geben Sie ein Ablaufdatum für die Personalisierung dieses Webformulars ein. </p> <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Wiederverwendbar]</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, wenn der vorgesehene Unterzeichner das Formular mehrmals signieren kann.</p> </li> 
        </ul> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Member Share]</b> </p> <p>Klicken Sie für jedes Mitglied, für das Sie die Vereinbarung freigeben möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie die E-Mail-Adresse des Mitglieds sowie eine Nachricht an dieses Mitglied ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Benutzerspezifischer API-Aufruf]**
Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf ausführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein <code>https://api.[region].adobesign.com/api/rest/v6/</code></p> <p>Hinweis: Die Liste der verfügbaren Endpunkte finden Sie in der [!DNL Adobe Sign] API-Referenz.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge] </td> 
   <td> <p>Geben Sie die Abfragezeichenfolge der Anfrage ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hochladen eines Verlaufsdokuments]</td> 
   <td> <p>Wenn Sie ein Verlaufsdokument hochladen möchten, geben Sie die Quelldatei für das Dokument ein, das Sie hochladen möchten.</p> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Listeneinträge]**

Dieses Aktionsmodul listet alle Datensätze des ausgewählten Typs auf, auf den das Konto Zugriff hat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes aus, für den Sie verwandte Datensätze abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td> <p>Geben Sie das Gebietsschema des Benutzers ein. Dadurch wird die Sprache der Benutzeroberfläche bestimmt. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Externe ID]</td> 
   <td>Geben Sie die externe ID (eine ID, die außerhalb von [!DNL Adobe Acrobat Sign] zugewiesen ist) für die Vereinbarungen ein, die Sie zurückgeben möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gruppen-ID]</td> 
   <td>Geben Sie die Kennung der Gruppe an, die den auflistbaren Datensätzen zugeordnet ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verborgene Elemente anzeigen (Datensätze)]</td> 
   <td>Aktivieren Sie diese Option, wenn Sie ausgeblendete Datensätze in Ihre Ergebnisse aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cursor] / [!UICONTROL Startindex]</td> 
   <td> <p>Geben Sie die Nummer des ersten Datensatzes ein, den das Modul zurückgeben soll. </p> <p>Hinweis: Dieses Feld wird mit dem Feld [!UICONTROL Maximale Anzahl an zurückgegebenen Datensätzen] für die Paginierung kombiniert. Wenn beispielsweise die [!UICONTROL Maximale Anzahl an zurückgegebenen Ereignissen] 100 beträgt und der [!UICONTROL Start Index] 101 beträgt, gibt das Modul die Datensätze 101-200 oder die zweite Ergebnisseite zurück.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an zurückgegebenen Datensätzen]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie [Aktion] für das Modul während jedes Szenario-Ausführungszyklus zu.</p> <p>Hinweis: Dieses Feld wird für die Paginierung mit dem Feld [!UICONTROL Cursor] oder [!UICONTROL Startindex] kombiniert. Wenn beispielsweise die [!UICONTROL Maximale Anzahl an zurückgegebenen Ereignissen] 100 beträgt und der [!UICONTROL Start Index] 101 beträgt, gibt das Modul die Datensätze 101-200 oder die zweite Ergebnisseite zurück.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Übergeordnete Domänen-URLs von [!UICONTROL]</td> 
   <td> <p>Geben Sie eine kommagetrennte Liste der URLs der übergeordneten Domäne ein oder ordnen Sie sie zu, in denen die zurückgegebenen URLs gespeichert werden können. Wenn dies leer gelassen wird, sind die [!DNL Adobe Acrobat Sign]-Seiten nicht im iframe sichtbar.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Datensatz lesen]**

Dieses Aktionsmodul ruft Informationen aus einem einzelnen Datensatz ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes aus, für den Sie verwandte Datensätze abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datensatz-ID]</td> 
   <td>Geben Sie die Kennung des Datensatzes ein oder ordnen Sie ihn zu.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Verwandte Datensätze lesen]**

Lesen Sie zusätzliche Informationen zu einem einzelnen Datensatz.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes aus, für den Sie verwandte Datensätze abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datensatz-ID] (Beispiel: [!UICONTROL Konto-ID])</td> 
   <td>Geben Sie die Kennung des Datensatzes ein, für den Sie verwandte Datensätze abrufen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Andere Felder]</td> 
   <td>Geben Sie Informationen in bestimmte Felder basierend auf dem Datensatztyp und den zugehörigen Feldern ein.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Datensatz aktualisieren]**

Dieses Aktionsmodul aktualisiert einen einzelnen Datensatz in [!DNL Adobe Acrobat Sign].

>[!IMPORTANT]
>
>* Wenn Sie wesentliche Änderungen an einem Abkommen erwarten, empfehlen wir als Best Practice die Schaffung eines neuen Abkommens, anstatt das bestehende Abkommen zu aktualisieren.
>* Einige Updates stellen erforderliche Felder bereit. Achten Sie bei der Konfiguration der Aktualisierung darauf, alle erforderlichen Felder auszufüllen. Erforderliche Felder sind in [!DNL Workfront Fusion] -Modulen fett gedruckt.
>



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datensatz-ID] </td> 
   <td>Geben Sie die Kennung des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Andere Felder]</td> 
   <td> <p>Geben Sie Informationen in bestimmte Felder basierend auf dem Datensatztyp und den zugehörigen Feldern ein.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Agreement]</b> </p> <p>Wenn Sie wesentliche Änderungen an einem Abkommen erwarten, empfehlen wir als Best Practice die Schaffung eines neuen Abkommens, anstatt das bestehende Abkommen zu aktualisieren.</p> </li> 
     <li> <p><b>[!UICONTROL Library document]</b> </p> <p>Wählen Sie die zu aktualisierenden Felder aus und füllen Sie dann die ausgewählten Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Status]</b> </p> <p>Wählen Sie den neuen Status für das Bibliotheksdokument aus.</p> </li> 
       <li> <p><b>[!UICONTROL Name]</b> </p> <p>Geben Sie den Namen der Bibliotheksvorlage ein oder ordnen Sie ihn zu</p> </li> 
       <li> <p><b>[!UICONTROL Freigabemodus]</b> </p> <p>Geben Sie an, wer Zugriff auf das Bibliotheksdokument haben soll.</p> </li> 
       <li> <p><b>[!UICONTROL Bibliotheksvorlagentyp]</b> </p> <p>Klicken Sie für jeden Bibliotheksvorlagentyp, den Sie verwenden möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und wählen Sie den Vorlagentyp aus.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Benutzer]</b> </p> <p>Wählen Sie die zu aktualisierenden Felder aus und füllen Sie dann die ausgewählten Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Vorname]</b> </p> <p>Geben Sie den Vornamen des Benutzers ein.</p> </li> 
       <li> <p><b>[!UICONTROL Nachname]</b> </p> <p>Nachnamen des Benutzers eingeben</p> </li> 
       <li> <p><b>[!UICONTROL Company]</b> </p> <p>Geben Sie den Namen des Unternehmens des Benutzers ein.</p> </li> 
       <li> <p><b>[!UICONTROL Telefon]</b> </p> <p>Telefonnummer des Benutzers eingeben</p> </li> 
       <li> <p><b>[!UICONTROL Primäre Gruppen-ID]</b> </p> <p>Geben Sie die Gruppe ein, der der neue Benutzer hinzugefügt wird. Wenn nichts eingegeben wird, wird der Benutzer der Standardgruppe für das Konto hinzugefügt.</p> </li> 
       <li> <p><b>[!UICONTROL Auftragstitel]</b> </p> <p>Geben Sie die Berufsbezeichnung des Benutzers ein.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Webformular] ([!UICONTROL Widget])</b> </p> <p>Geben Sie Informationen in bestimmte Felder basierend auf dem Datensatztyp und den zugehörigen Feldern ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Aktualisieren des zugehörigen Eintrags]**

Dieses Aktionsmodul aktualisiert Datensätze, die sich auf ein bestimmtes Objekt beziehen.

>[!IMPORTANT]
>
>* Wenn Sie wesentliche Änderungen an einem Abkommen erwarten, empfehlen wir als Best Practice die Schaffung eines neuen Abkommens, anstatt das bestehende Abkommen zu aktualisieren.
>* Einige Updates stellen erforderliche Felder bereit. Achten Sie bei der Konfiguration der Aktualisierung darauf, alle erforderlichen Felder auszufüllen. Erforderliche Felder sind in [!DNL Workfront Fusion] -Modulen fett gedruckt.
>



<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Datensatztyp des Datensatzes aus, mit dem die zugehörigen Felder verknüpft sind.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Agreement]/[!UICONTROL Library document]/[!UICONTROL User]/[!UICONTROL Widget ID]</td> 
   <td>Geben Sie die ID des Objekts ein oder ordnen Sie sie zu, mit dem Sie den erstellten Datensatz verknüpfen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Andere Felder]</td> 
   <td> <p>Geben Sie Informationen in bestimmte Felder basierend auf dem Datensatztyp und den zugehörigen Feldern ein.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Agreement]</b> </p> <p>Wenn Sie wesentliche Änderungen an einem Abkommen erwarten, empfehlen wir als Best Practice die Schaffung eines neuen Abkommens, anstatt das bestehende Abkommen zu aktualisieren.</p> </li> 
     <li> <p><b>[!UICONTROL Library document]</b> </p> <p>Wählen Sie die zu aktualisierenden Felder aus und füllen Sie dann die ausgewählten Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL State]</b> </p> <p>Wählen Sie den neuen Status für das Bibliotheksdokument aus.</p> </li> 
       <li> <p><b>[!UICONTROL Hinweis]</b> </p> <p>Geben Sie den Text der Notiz ein oder ordnen Sie ihn zu.</p> </li> 
       <li> <p><b>[!UICONTROL Sichtbarkeit]</b> </p> <p>Wählen Sie aus, ob das Bibliotheksdokument ein- oder ausgeblendet wird.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Benutzer]</b> </p> <p>Wählen Sie die zu aktualisierenden Felder aus und füllen Sie dann die ausgewählten Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Group info list]</b> </p> <p>Füllen Sie die folgenden Felder aus</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Status]</b> </p> <p>Wählen Sie den neuen Status für den Benutzer aus.</p> </li> 
         <li> <p><b>[!UICONTROL ID]</b> </p> <p>Eindeutige Kennung der Gruppe eingeben</p> </li> 
         <li> <p><b>[!UICONTROL Is group admin]</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, um diesen Benutzer zu einem Gruppenadministrator zu machen.</p> </li> 
         <li> <p><b>Is primary group</b> </p> <p>Wählen Sie <b>[!UICONTROL Yes]</b> aus, um diese Gruppe auf die primäre Gruppe des Benutzers zu aktualisieren.</p> </li> 
         <li> <p><b>[!UICONTROL Erstellungsdatum]</b> </p> <p>Geben Sie das Datum ein, an dem die Gruppe erstellt wurde.</p> <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Typerzwang in [!UICONTROL Adobe Workfront Fusion]</a>.</p> </li> 
         <li> <p><b>[!UICONTROL Name]</b> </p> <p>Geben Sie den Namen der Gruppe ein oder ordnen Sie ihn zu.</p> </li> 
         <li> <p><b>[!UICONTROL Bibliothek - Dokumenterstellung sichtbar]</b> </p> <p>Diese Einstellungen bestimmen, ob der Benutzer Bibliotheksdokumente erstellen kann</p> 
          <ul> 
           <li> <p>[!UICONTROL Wert]</p> <p>Zulassen</p> </li> 
           <li> <p>[!UICONTROL Vererbt]</p> <p>Gruppeneinstellung übernehmen aus Gruppe oder Konto</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL Auf Workflows beschränkter Versand]</b> </p> <p>Diese Einstellungen bestimmen, ob der Benutzer Vereinbarungen nur mithilfe von Workflows erstellen kann.</p> 
          <ul> 
           <li> <p>[!UICONTROL Wert]</p> <p>Zulassen</p> </li> 
           <li> <p>[!UICONTROL Vererbt]</p> <p>Gruppeneinstellung übernehmen aus Gruppe oder Konto</p> </li> 
          </ul> </li> 
         <li> <p><b>[!UICONTROL Benutzer kann senden]</b> </p> 
          <ul> 
           <li> <p>[!UICONTROL Wert]</p> <p>Zulassen</p> </li> 
           <li> <p>[!UICONTROL Vererbt]</p> <p>Gruppeneinstellung übernehmen aus Gruppe oder Konto</p> </li> 
          </ul> </li> 
        </ul> </li> 
      </ul> 
      <ul> 
       <li> <p><b>[!UICONTROL State]</b> </p> <p>Wählen Sie den neuen Status für den Benutzer aus und geben Sie einen Kommentar dazu ein, warum Sie den Benutzer aktivieren oder deaktivieren möchten.</p> </li> 
       <li> <p><b>[!UICONTROL Locale]</b> </p> <p>Geben Sie das Gebietsschema des Benutzers ein. Dadurch wird die Sprache der Benutzeroberfläche bestimmt. </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Webformular] ([!UICONTROL Widget])</b> </p> <p>Geben Sie Informationen in bestimmte Felder basierend auf dem Datensatztyp und den zugehörigen Feldern ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Dokument hochladen]**

Laden Sie ein Verlaufsdokument hoch. Ein vorübergehendes Dokument ist 7 Tage nach dem Hochladen verfügbar.

>[!NOTE]
>
>Es wird empfohlen, das zu signierende Dokument hochzuladen und es anschließend dem Feld Zu sendende Datei im Modul Vereinbarung erstellen zuzuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datensatz-ID]</td> 
   <td>Geben Sie die Kennung des Datensatzes ein oder ordnen Sie ihn zu</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME type]</td> 
   <td>Geben Sie den MIME-Typ der Originaldatei ein. MIME-Typen (Multizweck Internet Mail Extension) sind Bezeichnungen, mit denen Software verschiedene Arten von im Internet freigegebenen Daten identifizieren kann. Webserver und Browser verwenden den MIME-Typ, um zu bestimmen, was mit einer Datei gemacht werden soll. Beispielsweise wird eine Datei mit dem MIME-Typ <code>text/html</code> in einem Browser anders verarbeitet als eine Datei mit dem MIME-Typ <code>image/jpeg</code>.</td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** In diesem Workflow wird das zu signierende Dokument (das zuvor von Workfront heruntergeladen wurde) als Übergangsdokument hochgeladen.

![](assets/sign-example-1-350x308.png)

Das Modul [!UICONTROL Dokument hochladen] gibt dem Dokument eine [!DNL Adobe Acrobat Sign] -ID, auf die in späteren Modulen verwiesen werden kann. Bei der Erstellung der Vereinbarung ist die ID des hochgeladenen Dokuments im Feld [!UICONTROL Zu sendende Dateien] enthalten.

![](assets/sign-example-2-350x356.png)

+++

### Suchvorgänge

+++ **[!UICONTROL Suchvereinbarungen]**

Dieses Suchmodul sucht nach Vereinbarungen basierend auf von Ihnen angegebenen Kriterien.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Acrobat Sign]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Textfilter]</td> 
   <td> <p>Suchen Sie in den Vertragsmetadaten nach Text. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Suchtext]</b> </p> <p>Geben Sie Text ein, den Sie in den Vertragsmetadaten finden möchten. Jedes Wort wird als separates Textelement behandelt. </p> </li> 
     <li> <p><b>[!UICONTROL Text in]</b> suchen </p> <p>Wählen Sie die Metadatenfelder aus, in denen Sie Text finden möchten. Wenn Sie nichts auswählen, durchsucht das Modul alle Metadaten.</p> </li> 
    </ul> <p>Das Modul gibt eine Vereinbarung zurück, die den eingegebenen Text in einem der ausgewählten Felder enthält. Beispiel: Wenn Sie "Frühjahrskampagne"eingeben und die Optionen Titel und Hinweis auswählen, werden alle Vereinbarungen mit den Wörtern "Frühling"oder "Kampagne"entweder im Titel oder in der Notiz zurückgegeben.</p> <p>Weitere Informationen zum Durchsuchen von Feldern in [!DNL Adobe Acrobat Sign] finden Sie unter "Funktionsweise der Textsuche"in <a href="https://helpx.adobe.com/sign/using/adobesign-search-users-agreements.html#HowSearchWorks">[!DNL Adobe Sign] Suche - Funktionsweise</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Erstellungsdatum]</td> 
   <td>Wählen Sie Datumswerte aus. Das Modul gibt nur Datensätze zurück, für die das erstellte Datum diesen Kriterien entspricht.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ablaufdatum]</td> 
   <td>Wählen Sie Datumswerte aus. Das Modul gibt nur Datensätze zurück, für die das Ablaufdatum diesen Kriterien entspricht.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Änderungsdatum]</p> </td> 
   <td>Wählen Sie Datumswerte aus. Das Modul gibt nur Datensätze zurück, für die das geänderte Datum diesen Kriterien entspricht.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Externe ID]</td> 
   <td> <p> Externe ID ist eine vom Absender zugewiesene ID der Vereinbarung, die in beliebiger Form, in der Regel aber in Form von "&lt;groupID&gt;:&lt;ID&gt;"vorliegen kann.</p> <p>Klicken Sie für jede externe ID, die Sie hinzufügen möchten, auf "<b>[!UICONTROL Hinzufügen]</b>"und geben Sie die externe ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gruppen-ID]</td> 
   <td> <p>Die Gruppen-ID ist eine Kennung, die bei der Erstellung der Gruppe zugewiesen wurde.</p> <p>Klicken Sie für jede externe ID, die Sie hinzufügen möchten, auf "<b>[!UICONTROL Hinzufügen]</b>"und geben Sie die externe ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td> <p>Dies ist die der jeweiligen Vereinbarung zugewiesene ID. </p> <p>Klicken Sie für jede externe ID, die Sie hinzufügen möchten, auf "<b>[!UICONTROL Hinzufügen]</b>"und geben Sie die externe ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Übergeordnete ID von [!UICONTROL]</td> 
   <td> <p>Dies ist die ID, die dem übergeordneten Objekt der Vereinbarung zugewiesen ist. </p> <p>Klicken Sie für jede externe ID, die Sie hinzufügen möchten, auf "<b>[!UICONTROL Hinzufügen]</b>"und geben Sie die externe ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Teilnehmer-E-Mail]</td> 
   <td> <p>Die E-Mail-Adresse eines Teilnehmers. </p> <p>Klicken Sie für jede externe ID, die Sie hinzufügen möchten, auf "<b>[!UICONTROL Hinzufügen]</b>"und geben Sie die externe ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rolle]</td> 
   <td>Wählen Sie die Rollen aus, die die zurückgegebenen Ergebnisse enthalten sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sortieren nach</td> 
   <td>Wenn das Modul die Ergebnisse sortieren soll, wählen Sie das Feld aus, nach dem die Ergebnisse sortiert werden sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortierreihenfolge]r</td> 
   <td>Wenn das Modul die Ergebnisse sortieren soll, wählen Sie aus, ob die Sortierung aufsteigend oder absteigend erfolgen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status]</td> 
   <td>Wählen Sie die Status aus, die die zurückgegebenen Ergebnisse enthalten sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
   <td>Wählen Sie die Vertragstypen aus, die die zurückgegebenen Ergebnisse enthalten sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Untertypen]</td> 
   <td>Wählen Sie die Untertypen der Vereinbarung aus, die die zurückgegebenen Ergebnisse enthalten sollen. Untertypen sind nur bei Vereinbarungen mit Bibliotheksvorlagen möglich.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzer-ID]</td> 
   <td> <p>Die Benutzer-ID des Benutzers, für den die Vereinbarung freigegeben ist.</p> <p>Klicken Sie für jede Benutzer-ID, die Sie hinzufügen möchten, auf "<b>[!UICONTROL Hinzufügen]</b>"und geben Sie die Benutzer-ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sichtbarkeit]</td> 
   <td>Wählen Sie die Sichtbarkeitsstufe aus, die die zurückgegebenen Ergebnisse enthalten sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startindex]</td> 
   <td> <p>Geben Sie die Position des ersten Ergebnisses ein, das Sie zurückgeben möchten. Kombinieren Sie dies mit den maximal zurückgegebenen Ergebnissen von [!UICONTROL], um Ergebnisse zu paginieren.</p> <p>Beispiel: Wenn Sie 100 Ergebnisse gleichzeitig zurückgeben, geben Sie 100 ein, um die Ergebnisse 100-200 zurückzugeben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie [Aktion] für das Modul während jedes Szenario-Ausführungszyklus zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++
