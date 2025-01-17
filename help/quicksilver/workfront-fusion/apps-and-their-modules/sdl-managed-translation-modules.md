---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: SDL Managed Translation Modules
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# [!DNL SDL Managed Translation]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [SDL Managed Translation-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/sdl-managed-translation-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Ihr [!DNL SDL Managed Translation]-Konto mit mehreren Anwendungen und Services von Drittanbietern verbinden.

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

## Informationen zur von SDL verwalteten Übersetzungs-API

Der SDL Managed Translation Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td>https://languagecloud.sdl.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.4.26</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL SDL Managed Translation] Module

>[!NOTE]
>
>Das Zeitlimit für Vorgangs-Aufrufe an [!DNL SDL Managed Translation] beträgt **Sekunden**.

### Dateien

#### [!UICONTROL Übersetzte Datei herunterladen]

Dieses Modul ruft den Inhalt einer einzelnen übersetzten Datei ab, die im angegebenen Projekt enthalten ist. Wenn sich die angeforderte Datei noch nicht im Status Herunterladen befindet, ist der Inhalt der Datei möglicherweise noch nicht vollständig übersetzt. Wenn sich die Datei im Status Download befindet und Sie sie erfolgreich abgerufen haben, stellen Sie sicher, dass Sie die Datei mit der `Cancel or Complete File`-Methode als abgeschlossen markieren.

#### [!UICONTROL Datei hochladen]

Dieses Modul ermöglicht das Hochladen von Dateien für die Übersetzung oder die Aufnahme in ein Übersetzungsprojekt als Referenzmaterial. Uploads müssen mit multipart/form-data übermittelt werden und können mehr als eine Datei enthalten. Sie legen die `ProjectOptionId` fest, die zur Bewertung der hochgeladenen Datei(en) verwendet werden sollen. Dadurch wird bestimmt, ob jede Datei, die Sie hochladen, ein möglicher Übersetzungskandidat ist oder als Referenzmaterial gehandhabt werden muss. Bei Archiven (`zip `, `rar`, `7z`, `tar` Dateien) untersucht die App den Inhalt des Archivs und zeigt an, ob das Archiv als Ganzes übersetzt werden kann oder ob es eine Mischung aus übersetzbaren und nicht übersetzbaren Dateien enthält.

>[!NOTE]
>
>Das gleichzeitige Hochladen von mehr als einer Datei wird nicht empfohlen, da dies die Auswirkungen von Fehlern erhöhen kann.

#### [!UICONTROL Referenzdatei hinzufügen]

Dieses Modul fügt eine Referenzdatei hinzu.

### Projekte

#### [!UICONTROL Erstellen eines Projekts]

Dieses Modul erstellt das angegebene Projekt.

#### Abbrechen oder Abschließen eines Projekts

Dieses Modul bricht das angegebene Projekt ab oder schließt es ab. Wenn das Projekt auf den Download wartet, durchläuft das Projekt alle letzten Schritte im Workflow und fährt schließlich bis zum Abschluss. Wenn das Projekt auf Genehmigung wartet oder die Kreditorenauswahl abgebrochen wird. Wenn sich das Projekt in einem anderen Status befindet, schlägt die Anfrage fehl.

#### [!UICONTROL Projekt-ZIP herunterladen]

Dieses Modul ruft die `zip` der übersetzten Dateien für das angegebene Projekt ab.

#### [!UICONTROL Projekt lesen]

Dieses Modul ruft das angegebene Projekt ab.

#### [!UICONTROL Projekte mit Status abrufen]

Dieses Modul ruft alle verfügbaren Projekte mit dem angegebenen Status ab. Mit dieser Methode können die Ergebnisse per Paging abgerufen werden, indem `$top`-, `$skip`- und `$orderby`-Abfrageparameter angegeben werden.

#### [!UICONTROL Projektliste abrufen]

Erstellt eine einfache Liste aller Projekte mit allgemeinen Informationen zu jedem Projekt. Mit dieser Methode können die Ergebnisse Seiten sein, indem `$top`-, `$skip`- und `$orderby`-Abfrageparameter angegeben werden.

#### [!UICONTROL Optionen zur Projekterstellung durchsuchen]

Dieses Modul erhält Optionen zur Projekterstellung.

### Sonstige

#### [!UICONTROL Erstellen eines API-Aufrufs]

Dieses Modul führt einen beliebigen autorisierten API-Aufruf aus.
