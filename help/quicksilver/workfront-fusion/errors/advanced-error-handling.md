---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Erweiterte Fehlerbehebung in [!DNL Adobe] Workfront Fusion
description: Erweiterte Methoden zur Fehlerbehebung umfassen das Filtern und Verschachteln.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 0%

---

# Erweiterte Fehlerbehandlung in [!DNL Adobe Workfront Fusion]

Erweiterte Methoden zur Fehlerbehebung umfassen das Filtern und Verschachteln.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
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

## Filtern

Es gibt zwei Arten von Filtern, die auf einer Fehler-Handler-Route durchgeführt werden können.

* [Hinzufügen eines Filters zur Fehler-Handler-Route](#adding-a-filter-to-the-error-handler-route)
* [Hinzufügen eines Routers gefolgt von Filtern zur Fehler-Handler-Route](#adding-a-router-followed-by-filters-to-the-error-handler)

### Hinzufügen eines Filters zur Fehler-Handler-Route

Sie können einen Filter verwenden, um zu steuern, welche Fehler von der Route des Fehler-Handlers verarbeitet werden. Auf diese Weise können Sie nur bestimmte Fehlertypen verarbeiten. Wenn ein Fehler nicht durch den Filter weitergegeben wird, wird er so behandelt, als gäbe es keine Fehler-Handler-Route, die für das angegebene Modul definiert ist.

>[!INFO]
>
>**Beispiel:**
>
>![](assets/filter-error-handling-350x238.png)

### Hinzufügen eines [!UICONTROL Routers] , gefolgt von Filtern zum Fehler-Handler

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>In diesem Beispiel erfolgt der Fehler im Modul &quot;[!UICONTROL Ordner erstellen]&quot;(A), das über eine normale Route und eine Fehler-Handler-Route verfügt. Auf Letzteres folgt ein Router mit einer Route, die über einen Filter verfügt, der einen bestimmten Fehlertyp definiert (Datenfehler tritt auf), und der andere Router, der die Standardroute für alle anderen Fehler ist. Die erste Route endet mit der Anweisung [!UICONTROL Fortsetzen] , die Ersatzwerte enthält, damit das Szenario aus Modul A fortgesetzt werden kann ([!UICONTROL Ordner erstellen]), während die zweite Route mit der Anweisung [!UICONTROL Rollback] endet, die die Ausführung des Szenarios sofort stoppt.

Weitere Informationen zu verschiedenen Fehlertypen und dazu, wie diese von [!DNL Workfront Fusion] verarbeitet und ausgewertet werden, finden Sie unter [Fehlerverarbeitung in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) .

### Beispiel-Szenario

Sie können dieses Beispielszenario einrichten, um zu verstehen, wie diese Filter für die Fehlerbehandlung funktionieren.

Verwenden Sie einen vorhandenen [!DNL Dropbox] -Ordner, um eine Datei hochzuladen, anstatt eine neue zu erstellen.

Wenn Sie das Modul [!UICONTROL Ordner ] unter [!DNL Dropbox] erstellen und bereits ein Ordner mit demselben Namen vorhanden ist, gibt das Modul einen Datenfehler aus, wie unten dargestellt:

![](assets/dropbox-350x276.png)

Das vollständige Szenario:

![](assets/dropbox-scenario-350x190.png)

1. Das Modul [!UICONTROL Tools] > [!UICONTROL Variable festlegen] enthält den Ordnernamen
1. Das Modul [!UICONTROL HTTP] >[!UICONTROL Get a file] ruft die Datei ab, die in den Ordner hochgeladen werden muss
1. Das Modul [!UICONTROL Dropbox] >[!UICONTROL Ordner erstellen] erzeugt einen Fehler, wenn bereits ein Ordner mit demselben Namen vorhanden ist wie der, der im Modul zugeordnet ist
1. Die Route des Fehler-Handlers (transparente Blasen) enthält einen Router zum Filtern der Fehler
1. Die erste Route ist für einen bestimmten Fehlertyp namens &quot;Datenfehler&quot;, den wir bereits kennen:

   1. Wenn ein Datenfehler auftritt und die Fehlerdetails durch den Filter weitergegeben werden, listet der [!UICONTROL Dropbox] >[!UICONTROL Auflisten aller Dateien/Unterordner in einem Ordnermodul] alle Ordner in [!DNL Dropbox] auf
   1. Der nachfolgende Filter entspricht den Ordnernamen.
   1. Die Anweisung [!UICONTROL Fortsetzen] gibt die Ordner-ID und den Ordnerpfad des vorhandenen Ordners an und die Szenarioausführung wird über das Modul [!UICONTROL Dropbox] >[!UICONTROL Ordner erstellen] fortgesetzt. Anstatt jedoch zu versuchen, einen neuen Ordner zu erstellen, verwendet sie dieses Mal die Werte aus der Anweisung [!UICONTROL Fortsetzen] , um zum nächsten Modul zu wechseln und die Datei in den vorhandenen Ordner hochzuladen

1. Die zweite Route gilt für alle anderen Fehler und endet mit der Anweisung [!UICONTROL Rollback] , die dazu führt, dass das Szenario sofort angehalten wird.

Nachstehend finden Sie eine ausführliche Erklärung zur fünften Aussage:

Um den vorhandenen Ordner in Ihren nachfolgenden Modulen zu verwenden ([!UICONTROL Laden Sie eine Datei hoch] unten), müssen Sie eine Fehler-Handler-Route zum Modul hinzufügen und den Ordnerpfad abrufen, der dem nachfolgenden Anweisung [!UICONTROL Fortsetzen] zugeordnet werden soll:

![](assets/add-error-handler-route-350x113.png)

Der Filter für die erste Route ist so eingestellt, dass nur der spezifische Fehler (Datenfehler) verarbeitet wird, der angezeigt wird, wenn bereits ein Ordner mit demselben Namen vorhanden ist:

![](assets/condition-350x327.png)

Das Modul [!UICONTROL Dropbox] >[!UICONTROL Alle Dateien in einem Ordner auflisten] ist so konfiguriert, dass alle Ordner im Zielordner zurückgegeben werden. Der folgende Filter wird nur an den Filter weitergegeben, den wir ursprünglich erstellt haben (der Ordnername wird in den 33 gespeichert. Ordnernamenelement):

![](assets/condition2-350x193.png)

Schließlich stellt die Anweisung [!UICONTROL Fortsetzen] den Ordnerpfad als Ausgabe für das fehlerhafte Modul bereit. Beachten Sie, dass die Ordner-ID leer gelassen wurde, da sie vom Modul &quot;[!UICONTROL Datei hochladen]&quot;nicht benötigt wird:

![](assets/flow-control-350x190.png)

## Verschachtelung

Unabhängig davon, wo sich ein Modul befindet, können Fehler-Handler-Routen für alle Module erstellt und implementiert werden, mit Ausnahme von Routern. Daher ist es möglich, eine Fehler-Handler-Route für ein Modul zu erstellen, das bereits Teil einer vorhandenen Fehler-Handler-Route ist, die für ein anderes Modul erstellt wurde.

Hier ist ein Beispiel für eine verschachtelte Fehler-Handler-Route:

![](assets/nested-error-handling-route-350x174.png)

In diesem Szenario wird die zweite Fehler-Handler-Route unter der ersten Fehler-Handler-Route verschachtelt. Wenn also beim [!UICONTROL Dropbox] >[!UICONTROL Ordnermodul erstellen] ein Fehler auftritt, wird die Ausführung zu Route 1 verschoben. Wenn der Filter [!UICONTROL Datenfehler stattfindet] übergeben wird, wird das nächste Modul ausgeführt, gefolgt vom Direktionsmodul [!UICONTROL Fortsetzen] , wenn bei [!UICONTROL Dropbox] >[!UICONTROL Alle Dateien/Unterordner auflisten] ein Fehler auftritt. 1} in einem Ordnermodul

Wenn jedoch bei diesem [!DNL Dropbox] -Modul ein Fehler auftritt, wird die Ausführung zu &quot;Error Handler Route 2&quot;verschoben und endet mit der Anweisung [!UICONTROL Ignore] . Das Modul [!UICONTROL Fortsetzungsanweisung] wird in diesem Fall nicht ausgeführt.

Dies ist eine Kombination aus Filter- und Verschachtelungs-Fehler-Handlern.

