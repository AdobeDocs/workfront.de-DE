---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Häufig gestellte Fragen zu Adobe Workfront Fusion
description: In diesem Artikel werden häufig gestellte Fragen zu  [!DNL Adobe Workfront Fusion] behandelt, einschließlich Informationen zu Objekten, die häufig in Fusion-Workflows verwendet werden
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

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Was ist ein Szenario?

### Antwort

Ein Szenario definiert eine Sequenz von Schritten, die von [!DNL Adobe Workfront Fusion] ausgeführt werden sollen. Für jedes Szenario geben Sie die Datenquelle an, wie die Daten verarbeitet werden sollen und welche Daten verwendet werden sollen und was ignoriert werden soll. [!DNL Workfront Fusion] können Sie so komplexe Szenarien erstellen, wie Sie benötigen. Selbst komplexeste Szenarien sind möglich.

Weitere Informationen finden Sie unter [Erstellen eines Integrationsszenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Kann ich mehr als ein Modul in einem Szenario verwenden? Oder nur ein Trigger und eine Handlung?

### Antwort

Sie können in einem Szenario beliebig viele Module verwenden. Sie können unabhängige Routen erstellen und angeben, welche Daten durch sie fließen sollen. Sie können auch die von einzelnen Aktionen zurückgegebenen Ergebnisse verwenden und sie dann an die nächste Aktion weiterleiten.

## Kann [!DNL Workfront Fusion] mit Dateien arbeiten?

### Antwort

Ja. Mithilfe von [!DNL Workfront Fusion] können Dateien empfangen, gespeichert, transformiert, konvertiert, verschlüsselt usw. werden. Darüber hinaus bietet [!DNL Workfront Fusion] eine Vielzahl integrierter Funktionen, mit denen Benutzende effektiv und kreativ mit den in den Dateien enthaltenen Daten arbeiten können.

Weitere Informationen finden Sie unter [Über Zuordnungsdateien in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## Was passiert, wenn ich eine E-Mail mit mehr als einem Anhang verarbeiten [!DNL Workfront Fusion]?

### Antwort

Wenn Sie das Modul [!UICONTROL E]Mail[!UICONTROL  zum Abrufen von ] verwenden, wird jeder Anhang einzeln über die übrigen Module im Szenario gesendet. Ähnliche Module sind auch in anderen Apps verfügbar, die mehrere Dateien gleichzeitig erhalten.

Weitere Informationen finden Sie unter [[!UICONTROL E-Mail]-Module](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Einige Trigger ermöglichen die sofortige Ausführung von Szenarien. Was bedeutet „sofort“?

### Antwort

Häufige Szenarien werden in Intervallen entsprechend dem von Ihnen angegebenen Zeitplan ausgeführt (z. B. jede Stunde, alle 5 Minuten, einmal im Monat usw.). Es gibt spezielle Trigger, so genannte Instant-Trigger (Webhooks), die Ihr Szenario sofort starten können, nachdem sie Daten von einem bestimmten Service erhalten haben. Sofortige Trigger können äußerst nützlich sein. Wir empfehlen, sie nach Möglichkeit zu verwenden. Sie tragen dazu bei, die Anzahl der Vorgänge zu reduzieren. Die empfangenen Daten werden sofort verarbeitet, ohne auf die nächste geplante Ausführung zu warten. Beispielsweise startet das [!DNL Google Sheets]-Modul [!UICONTROL Änderungen ansehen] ein Szenario unmittelbar nach der Aktualisierung einer Zelle.

## Was sind Aggregatoren?

### Antwort

Ein [!UICONTROL Aggregator] führt Daten in einer Sammlung zusammen. Ein Beispiel dafür sind Dateien, die in ein ZIP-Archiv komprimiert und als E-Mail-Anhang gesendet werden.

Weitere Informationen finden Sie unter [[!UICONTROL Aggregator]-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Was ist ein Vorgang?

### Antwort

Ein Vorgang ist jede Aufgabe, die von einem Modul ausgeführt wird. Ein Vorgang tritt beispielsweise jedes Mal auf, wenn ein Trigger ausgeführt wird und eine Aktion eine Aufgabe ausführt.

## Was ist eine Datenübertragung?

### Antwort

Die Datenübertragung bezieht sich auf die Datenmenge, die über Ihr Szenario übertragen wird. Angenommen, Sie haben ein Szenario, das ein Bild mit 100 KB von FTP abruft, seine Größe auf 50 KB reduziert und beide Bilder in [!DNL Dropbox] speichert. Die in diesem Szenario verwendete Datenmenge beträgt 250 KB.

## Was ist eine Verbindung?

### Antwort

Eine Verbindung ist die Verknüpfung zwischen Ihrem [!DNL Workfront Fusion]-Konto und dem Drittanbieterdienst, den Sie verwenden möchten. Die Verbindung kann beim Bearbeiten eines Szenarios einfach erstellt werden. Um eine Verbindung hinzuzufügen, klicken Sie auf die **[!UICONTROL Hinzufügen]**-Schaltfläche in der Moduleinstellung und folgen Sie den schrittweisen Anweisungen.

Weitere Informationen finden Sie unter [Verbindungen - Übersicht](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
