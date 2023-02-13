---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Häufig gestellte Fragen zu Adobe Workfront Fusion
description: In diesem Artikel werden häufig gestellte Fragen im Zusammenhang mit [!DNL Adobe Workfront Fusion], einschließlich Informationen zu häufig in Fusion-Workflows verwendeten Objekten
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Häufig gestellte Fragen zu Adobe Workfront Fusion

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> <p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Was ist ein Szenario?

### Antwort

Ein Szenario definiert eine Abfolge von Schritten, die von ausgeführt werden sollen [!DNL Adobe Workfront Fusion]. Für jedes Szenario geben Sie die Datenquelle an, wie die Daten verarbeitet werden sollen, welche Daten verwendet werden sollen und was ignoriert werden soll. [!DNL Workfront Fusion] ermöglicht die Erstellung komplexer Szenarien nach Bedarf; selbst die komplexesten Szenarien sind möglich.

Weitere Informationen finden Sie unter [Erstellen Sie ein Szenario für die Praxisintegration in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Kann ich in einem Szenario mehrere Module verwenden? Oder nur ein Trigger und eine Aktion?

### Antwort

Sie können in einem Szenario beliebig viele Module verwenden. Sie können unabhängige Routen erstellen und angeben, durch welche Daten sie fließen sollen. Sie können auch Ergebnisse verwenden, die von einzelnen Aktionen zurückgegeben werden, und sie dann an die nächste Aktion weiterleiten.

## can [!DNL Workfront Fusion] Arbeiten mit Dateien?

### Antwort

Ja. Verwenden [!DNL Workfront Fusion], können Dateien empfangen, gespeichert, umgewandelt, konvertiert, verschlüsselt usw. werden. Außerdem [!DNL Workfront Fusion] bietet eine breite Palette integrierter Funktionen, mit denen Benutzer effektiv und kreativ mit den in den Dateien enthaltenen Daten arbeiten können.

Weitere Informationen finden Sie unter [Über die Zuordnung von Dateien in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Was passiert, wenn ich [!DNL Workfront Fusion] eine E-Mail verarbeiten, die mehr als einen Anhang enthält?

### Antwort

Wenn Sie [!UICONTROL Email] Modul [!UICONTROL Anlagen abrufen], wird jeder Anhang einzeln über die restlichen Module im Szenario gesendet. Ähnliche Module sind auch in anderen Apps verfügbar, die mehrere Dateien gleichzeitig erhalten.

Weitere Informationen finden Sie unter [[!UICONTROL Email] Module](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Einige Trigger ermöglichen die sofortige Ausführung von Szenarien. Was bedeutet &quot;sofort&quot;?

### Antwort

Allgemeine Szenarien werden in Intervallen ausgeführt, die dem von Ihnen festgelegten Zeitplan entsprechen (z. B. jede Stunde, alle 5 Minuten, einmal im Monat usw.). Es gibt spezielle Trigger, so genannte Instant Trigger (Webhooks), die Ihr Szenario sofort starten können, nachdem sie Daten von einem bestimmten Dienst erhalten haben. Sofortige Trigger können sehr nützlich sein. Es wird empfohlen, sie nach Möglichkeit zu verwenden. Sie tragen dazu bei, die Anzahl der Vorgänge zu reduzieren. Die empfangenen Daten werden sofort verarbeitet, ohne auf die nächste geplante Ausführung zu warten. Beispiel: die [!DNL Google Sheets] Modul [!UICONTROL Änderungen überwachen] startet ein Szenario unmittelbar nach der Aktualisierung einer Zelle.

## Was sind Aggregatoren?

### Antwort

Ein [!UICONTROL Aggregator] führt Daten in einer Sammlung zusammen. Ein Beispiel dafür sind Dateien, die in ein ZIP-Archiv komprimiert und als E-Mail-Anhang gesendet werden.

Weitere Informationen finden Sie unter [[!UICONTROL Aggregator] -Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Was ist eine Operation?

### Antwort

Ein Vorgang ist eine beliebige Aufgabe, die von einem Modul ausgeführt wird. Ein Vorgang tritt beispielsweise jedes Mal auf, wenn ein Trigger ausgeführt wird, und jedes Mal, wenn eine Aktion eine Aufgabe ausführt.

## Was ist Datenübertragung?

### Antwort

Die Datenübertragung bezieht sich auf die Datenmenge, die über Ihr Szenario übertragen wird. Angenommen, Sie haben ein Szenario, in dem ein 100 KB großes Bild von FTP abgerufen und auf 50 KB reduziert wird und beide Bilder in gespeichert werden. [!DNL Dropbox]. Die in diesem Szenario verwendete Datenmenge beträgt 150 KB.

## Was ist eine Verbindung?

### Antwort

Eine Verbindung ist die Verknüpfung zwischen [!DNL Workfront Fusion] und dem Drittanbieterdienst, den Sie verwenden möchten. Die Verbindung kann beim Bearbeiten eines Szenarios einfach erstellt werden. Um eine Verbindung hinzuzufügen, klicken Sie auf die Schaltfläche **[!UICONTROL Hinzufügen]** in der Moduleinstellung und befolgen Sie die schrittweisen Anweisungen.

Weitere Informationen finden Sie unter [Über die Verbindung [!DNL Adobe Workfront Fusion] an eine App oder einen Dienst](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
