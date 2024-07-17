---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Häufig gestellte Fragen zu Adobe Workfront Fusion
description: In diesem Artikel werden häufige Fragen im Zusammenhang mit [!DNL Adobe Workfront Fusion] behandelt, einschließlich Informationen zu häufig in Fusion-Workflows verwendeten Objekten
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '664'
ht-degree: 1%

---

# Häufig gestellte Fragen zu Adobe Workfront Fusion

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

## Was ist ein Szenario?

### Antwort

Ein Szenario definiert eine Sequenz von Schritten, die von [!DNL Adobe Workfront Fusion] ausgeführt werden sollen. Für jedes Szenario geben Sie die Datenquelle an, wie die Daten verarbeitet werden sollen, welche Daten verwendet werden sollen und was ignoriert werden soll. Mit [!DNL Workfront Fusion] können Sie so komplexe Szenarien erstellen, wie Sie benötigen. Selbst die komplexesten Szenarien sind möglich.

Weitere Informationen finden Sie unter [Erstellen eines Szenarios für die Praxisintegration in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Kann ich in einem Szenario mehrere Module verwenden? Oder nur ein Trigger und eine Aktion?

### Antwort

Sie können in einem Szenario beliebig viele Module verwenden. Sie können unabhängige Routen erstellen und angeben, durch welche Daten sie fließen sollen. Sie können auch Ergebnisse verwenden, die von einzelnen Aktionen zurückgegeben werden, und sie dann an die nächste Aktion weiterleiten.

## Kann [!DNL Workfront Fusion] mit Dateien arbeiten?

### Antwort

Ja. Mit [!DNL Workfront Fusion] können Dateien empfangen, gespeichert, umgewandelt, konvertiert, verschlüsselt usw. werden. Außerdem bietet [!DNL Workfront Fusion] eine breite Palette integrierter Funktionen, mit denen Benutzer effektiv und kreativ mit den in den Dateien enthaltenen Daten arbeiten können.

Weitere Informationen finden Sie unter [Über die Zuordnung von Dateien in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Was passiert, wenn ich von [!DNL Workfront Fusion] eine E-Mail verarbeiten lasse, die mehr als einen Anhang enthält?

### Antwort

Wenn Sie das Modul [!UICONTROL E-Mail] [!UICONTROL Anlagen abrufen] verwenden, wird jede Anlage einzeln über den Rest der Module im Szenario gesendet. Ähnliche Module sind auch in anderen Apps verfügbar, die mehrere Dateien gleichzeitig erhalten.

Weitere Informationen finden Sie unter [[!UICONTROL E-Mail] -Module](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Einige Trigger ermöglichen die sofortige Ausführung von Szenarien. Was bedeutet &quot;sofort&quot;?

### Antwort

Allgemeine Szenarien werden in Intervallen ausgeführt, die dem von Ihnen festgelegten Zeitplan entsprechen (z. B. jede Stunde, alle 5 Minuten, einmal im Monat usw.). Es gibt spezielle Trigger, so genannte Instant Trigger (Webhooks), die Ihr Szenario sofort starten können, nachdem sie Daten von einem bestimmten Dienst erhalten haben. Sofortige Trigger können sehr nützlich sein. Es wird empfohlen, sie nach Möglichkeit zu verwenden. Sie tragen dazu bei, die Anzahl der Vorgänge zu reduzieren. Die empfangenen Daten werden sofort verarbeitet, ohne auf die nächste geplante Ausführung zu warten. Beispielsweise startet das Modul [!DNL Google Sheets] [!UICONTROL Änderungen ansehen] ein Szenario unmittelbar nach der Aktualisierung einer Zelle.

## Was sind Aggregatoren?

### Antwort

Ein [!UICONTROL Aggregator] führt Daten zu einer Sammlung zusammen. Ein Beispiel dafür sind Dateien, die in ein ZIP-Archiv komprimiert und als E-Mail-Anhang gesendet werden.

Weitere Informationen finden Sie unter [[!UICONTROL Aggregator]-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Was ist eine Operation?

### Antwort

Ein Vorgang ist eine beliebige Aufgabe, die von einem Modul ausgeführt wird. Ein Vorgang tritt beispielsweise jedes Mal auf, wenn ein Trigger ausgeführt wird, und jedes Mal, wenn eine Aktion eine Aufgabe ausführt.

## Was ist Datenübertragung?

### Antwort

Die Datenübertragung bezieht sich auf die Datenmenge, die über Ihr Szenario übertragen wird. Angenommen, Sie haben ein Szenario, bei dem ein 100 KB großes Bild von FTP abgerufen, seine Größe auf 50 KB verringert und beide Bilder auf [!DNL Dropbox] gespeichert werden. Die Datenmenge, die in diesem Szenario verwendet wird, beträgt 250 KB.

## Was ist eine Verbindung?

### Antwort

Eine Verbindung ist die Verknüpfung zwischen Ihrem [!DNL Workfront Fusion]-Konto und dem zu verwendenden Drittanbieterdienst. Die Verbindung kann beim Bearbeiten eines Szenarios einfach erstellt werden. Um eine Verbindung hinzuzufügen, klicken Sie in der Moduleinstellung auf die Schaltfläche **[!UICONTROL Hinzufügen]** und befolgen Sie die schrittweisen Anweisungen.

Weitere Informationen finden Sie unter [Übersicht über Verbindungen](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
