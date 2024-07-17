---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: SDL Managed Translation Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Ihr Konto für die verwaltete Übersetzung von SDL mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# [!DNL SDL Managed Translation] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Ihr [!DNL SDL Managed Translation] -Konto mit mehreren Drittanbieteranwendungen und -diensten verbinden.

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

## [!DNL SDL Managed Translation] Module

>[!NOTE]
>
>Das Vorgangstimeout für Aufrufe von [!DNL SDL Managed Translation] beträgt **120 Sekunden**.

### Dateien

#### [!UICONTROL Übersetzte Datei herunterladen]

Dieses Modul ruft den Inhalt einer einzelnen übersetzten Datei ab, die im angegebenen Projekt enthalten ist. Wenn die angeforderte Datei noch nicht den Status &quot;Downland&quot;aufweist, ist der Inhalt der Datei möglicherweise noch nicht vollständig übersetzt. Wenn die Datei den Status Download aufweist und Sie sie erfolgreich abgerufen haben, stellen Sie sicher, dass Sie die Datei mit der `Cancel or Complete File` -Methode als abgeschlossen markieren.

#### [!UICONTROL  Datei hochladen]

Dieses Modul ermöglicht das Hochladen von Dateien zur Übersetzung oder zur Aufnahme in ein Übersetzungsprojekt als Referenzmaterial. Uploads müssen mit mehrteiligen Formulardaten gesendet werden und können mehrere Dateien enthalten. Sie geben den `ProjectOptionId` an, der zum Auswerten der hochgeladenen Datei(en) verwendet werden soll. Dadurch wird bestimmt, ob jede hochgeladene Datei zu übersetzen ist oder als Referenzmaterial behandelt werden muss. Im Falle von Archiven (`zip `, `rar`, `7z`, `tar` -Dateien) prüft die App den Inhalt des Archivs und zeigt an, ob das Archiv als Ganzes übersetzt werden kann oder ob es eine Mischung aus übersetzbaren und nicht übersetzbaren Dateien enthält.

>[!NOTE]
>
>Das gleichzeitige Hochladen von mehr als einer Datei wird nicht empfohlen, da dadurch die Auswirkungen von Fehlern erhöht werden können.

#### [!UICONTROL Hinzufügen einer Referenzdatei]

Dieses Modul fügt eine Referenzdatei hinzu.

### Projekte

#### [!UICONTROL Erstellen eines Projekts]

Dieses Modul erstellt das angegebene Projekt.

#### Abbrechen oder Abschließen eines Projekts

Dieses Modul bricht das angegebene Projekt ab oder schließt es ab. Wenn das Projekt auf den Download wartet, durchläuft das Projekt alle letzten Schritte im Workflow und wechselt schließlich zum Abschluss. Wenn das Projekt auf die Genehmigung wartet oder die Auswahl des Anbieters abgebrochen wird. Wenn sich das Projekt in einem anderen Status befindet, schlägt die Anfrage fehl.

#### [!UICONTROL Projekt-ZIP herunterladen]

Dieses Modul ruft die `zip` -Datei der übersetzten Dateien für das angegebene Projekt ab.

#### [!UICONTROL Projekt lesen]

Dieses Modul ruft das angegebene Projekt ab.

#### [!UICONTROL Projekte zum Status abrufen]

Dieses Modul ruft alle verfügbaren Projekte mit dem angegebenen Status ab. Diese Methode ermöglicht die Seiten der Ergebnisse durch Angabe der Abfrageparameter `$top`, `$skip` und `$orderby`.

#### [!UICONTROL Projektliste abrufen]

Ruft eine einfache Liste aller Projekte mit allgemeinen Informationen zu den einzelnen Projekten ab. Bei dieser Methode können die Ergebnisse Seiten sein, indem die Abfrageparameter `$top`, `$skip` und `$orderby` angegeben werden.

#### [!UICONTROL Optionen zur Projekterstellung durchsuchen]

Dieses Modul erhält Projekterstellungsoptionen.

### Sonstige

#### [!UICONTROL API-Aufruf durchführen]

Dieses Modul führt einen beliebigen autorisierten API-Aufruf durch.
