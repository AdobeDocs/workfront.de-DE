---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: SDL Managed Translation Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Ihr Konto für die von SDL verwaltete Übersetzung mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# [!DNL SDL Managed Translation]-Module

In einer [!DNL Adobe Workfront Fusion] Szenario können Sie Ihre [!DNL SDL Managed Translation] -Konto für mehrere Anwendungen und Dienste von Drittanbietern.

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Module

>[!NOTE]
>
>Die Zeitüberschreitung bei Aufrufen an [!DNL SDL Managed Translation] is **120 Sekunden**.

### Dateien

#### [!UICONTROL Übersetzte Datei herunterladen]

Dieses Modul ruft den Inhalt einer einzelnen übersetzten Datei ab, die im angegebenen Projekt enthalten ist. Wenn die angeforderte Datei noch nicht den Status &quot;Downland&quot;aufweist, ist der Inhalt der Datei möglicherweise noch nicht vollständig übersetzt. Wenn sich die Datei im Status Download befindet und Sie sie erfolgreich abgerufen haben, stellen Sie sicher, dass Sie die Datei mit dem `Cancel or Complete File` -Methode.

#### [!UICONTROL Datei hochladen]

Dieses Modul ermöglicht das Hochladen von Dateien zur Übersetzung oder zur Aufnahme in ein Übersetzungsprojekt als Referenzmaterial. Uploads müssen mit mehrteiligen Formulardaten gesendet werden und können mehrere Dateien enthalten. Sie legen die `ProjectOptionId` , die zum Auswerten der hochgeladenen Datei(en) verwendet werden sollte. Dadurch wird bestimmt, ob jede hochgeladene Datei zu übersetzen ist oder als Referenzmaterial behandelt werden muss. Im Falle von Archiven (`zip `, `rar`, `7z`, `tar` -Dateien) überprüft die App den Inhalt des Archivs und zeigt an, ob das Archiv als Ganzes übersetzt werden kann oder ob es eine Mischung aus übersetzbaren und nicht übersetzbaren Dateien enthält.

>[!NOTE]
>
>Das gleichzeitige Hochladen von mehr als einer Datei wird nicht empfohlen, da dadurch die Auswirkungen von Fehlern erhöht werden können.

#### [!UICONTROL Hinzufügen einer Referenzdatei]

Dieses Modul fügt eine Referenzdatei hinzu.

### Projekte

#### [!UICONTROL Projekt erstellen]

Dieses Modul erstellt das angegebene Projekt.

#### Abbrechen oder Abschließen eines Projekts

Dieses Modul bricht das angegebene Projekt ab oder schließt es ab. Wenn das Projekt auf den Download wartet, durchläuft das Projekt alle letzten Schritte im Workflow und wechselt schließlich zum Abschluss. Wenn das Projekt auf die Genehmigung wartet oder die Auswahl des Anbieters abgebrochen wird. Wenn sich das Projekt in einem anderen Status befindet, schlägt die Anfrage fehl.

#### [!UICONTROL Projekt-Zip herunterladen]

Dieses Modul erhält die `zip` Datei der übersetzten Dateien für das angegebene Projekt.

#### [!UICONTROL Projekt lesen]

Dieses Modul ruft das angegebene Projekt ab.

#### [!UICONTROL Projekte unter Status abrufen]

Dieses Modul ruft alle verfügbaren Projekte mit dem angegebenen Status ab. Diese Methode ermöglicht die Seiten der Ergebnisse durch Angabe von `$top`, `$skip`und `$orderby` Abfrageparameter.

#### [!UICONTROL Projektliste abrufen]

Ruft eine einfache Liste aller Projekte mit allgemeinen Informationen zu den einzelnen Projekten ab. Bei dieser Methode können die Ergebnisse Seiten sein, indem Sie `$top`, `$skip`und `$orderby` Abfrageparameter.

#### [!UICONTROL Optionen zur Projekterstellung durchsuchen]

Dieses Modul erhält Projekterstellungsoptionen.

### Sonstige

#### [!UICONTROL API-Aufruf durchführen]

Dieses Modul führt einen beliebigen autorisierten API-Aufruf durch.
