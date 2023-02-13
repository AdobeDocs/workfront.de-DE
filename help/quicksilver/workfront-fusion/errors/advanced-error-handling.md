---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Erweiterte Fehlerbehandlung in [!DNL Adobe] Workfront Fusion
description: Erweiterte Methoden zur Fehlerbehebung umfassen Filtern und Verschachteln.
author: Becky
feature: Workfront Fusion
exl-id: 57f43fc2-23ed-44f5-8785-90739329b5ee
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '913'
ht-degree: 0%

---

# Erweiterte Fehlerbehandlung in [!DNL Adobe Workfront Fusion]

Erweiterte Methoden zur Fehlerbehebung umfassen Filtern und Verschachteln.

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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

### Hinzufügen einer [!UICONTROL Router] gefolgt von Filtern zum Fehler-Handler

>[!INFO]
>
>![](assets/router-filter-error-handling-350x254.png)
>
>In diesem Beispiel erfolgt der Fehler im [!UICONTROL Ordner erstellen] -Modul (A), das eine normale Route und eine Fehler-Handler-Route aufweist. Auf Letzteres folgt ein Router mit einer Route, die über einen Filter verfügt, der einen bestimmten Fehlertyp definiert (Datenfehler tritt auf), und der andere Router, der die Standardroute für alle anderen Fehler ist. Die erste Route endet mit der [!UICONTROL Fortsetzen] -Anweisung, die Ersatzwerte für das Szenario enthält, das von Modul A fortgesetzt werden soll ([!UICONTROL Ordner erstellen]), während die zweite Route mit der [!UICONTROL Rollback] -Anweisung, die die Ausführung des Szenarios sofort stoppt.

Siehe [Fehlerverarbeitung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) für weitere Informationen zu verschiedenen Fehlertypen und zur [!DNL Workfront Fusion] verarbeitet und bewertet sie.

### Das Beispielszenario

Sie können dieses Beispielszenario einrichten, um zu verstehen, wie diese Filter für die Fehlerbehandlung funktionieren.

Vorhandene verwenden [!DNL Dropbox] Ordner, um eine Datei hochzuladen, anstatt eine neue zu erstellen

Wenn Sie [!UICONTROL Ordner erstellen] -Modul ein [!DNL Dropbox] und ein Ordner mit demselben Namen bereits vorhanden ist, gibt das Modul einen Datenfehler aus, wie unten dargestellt:

![](assets/dropbox-350x276.png)

Das vollständige Szenario:

![](assets/dropbox-scenario-350x190.png)

1. Die [!UICONTROL Instrumente] > [!UICONTROL Variable festlegen] -Modul enthält den Ordnernamen
1. Die [!UICONTROL HTTP] >[!UICONTROL Datei abrufen] -Modul ruft die Datei ab, die in den Ordner hochgeladen werden muss
1. Die [!UICONTROL Dropbox] >[!UICONTROL Ordner erstellen] -Modul gibt einen Fehler aus, wenn bereits ein Ordner mit demselben Namen wie der im Modul zugeordnete vorhanden ist
1. Die Route des Fehler-Handlers (transparente Blasen) enthält einen Router zum Filtern der Fehler
1. Die erste Route ist für einen bestimmten Fehlertyp namens &quot;Datenfehler&quot;, den wir bereits kennen:

   1. Wenn ein Datenfehler auftritt und die Fehlerdetails den Filter durchlaufen, wird die [!UICONTROL Dropbox] >[!UICONTROL Alle Dateien/Unterordner in einem Ordnermodul auflisten] listet alle Ordner in [!DNL Dropbox]
   1. Der nachfolgende Filter entspricht den Ordnernamen.
   1. Die [!UICONTROL Fortsetzen] -Anweisung gibt die Ordner-ID und den Ordnerpfad des vorhandenen Ordners an und das Szenario, in dem die Ausführung über [!UICONTROL Dropbox] >[!UICONTROL Ordner erstellen] -Modul verwenden, anstatt zu versuchen, einen neuen Ordner zu erstellen, verwendet es diesmal die Werte aus dem [!UICONTROL Fortsetzen] Anweisung, um zum nächsten Modul zu wechseln und die Datei im vorhandenen Ordner hochzuladen.

1. Die zweite Route gilt für alle anderen Fehler und endet mit der [!UICONTROL Rollback] Anweisung, die dazu führt, dass das Szenario sofort beendet wird

Nachstehend finden Sie eine ausführliche Erklärung zur fünften Aussage:

Um den vorhandenen Ordner in Ihren nachfolgenden Modulen zu verwenden ([!UICONTROL Datei hochladen] unten), müssen Sie eine Fehler-Handler-Route zum -Modul hinzufügen und den Ordnerpfad abrufen, der der [!UICONTROL Fortsetzen] Direktive -Modul, das wie folgt aussieht:

![](assets/add-error-handler-route-350x113.png)

Der Filter für die erste Route ist so eingestellt, dass nur der spezifische Fehler (Datenfehler) verarbeitet wird, der angezeigt wird, wenn bereits ein Ordner mit demselben Namen vorhanden ist:

![](assets/condition-350x327.png)

Die [!UICONTROL Dropbox] >[!UICONTROL Alle Dateien in einem Ordner auflisten] -Modul so konfiguriert ist, dass alle Ordner im Zielordner zurückgegeben werden. Der folgende Filter wird nur an den Filter weitergegeben, den wir ursprünglich erstellt haben (der Ordnername wird in den 33 gespeichert. Ordnernamenelement):

![](assets/condition2-350x193.png)

Schließlich wird die [!UICONTROL Fortsetzen] -Anweisung stellt den Ordnerpfad als Ausgabe für das fehlerhafte Modul bereit. Beachten Sie, dass die Ordner-ID leer gelassen wurde, da sie nicht durch die[!UICONTROL Datei hochladen]&#39; module:

![](assets/flow-control-350x190.png)

## Verschachtelung

Unabhängig davon, wo sich ein Modul befindet, können Fehler-Handler-Routen für alle Module erstellt und implementiert werden, mit Ausnahme von Routern. Daher ist es möglich, eine Fehler-Handler-Route für ein Modul zu erstellen, das bereits Teil einer vorhandenen Fehler-Handler-Route ist, die für ein anderes Modul erstellt wurde.

Hier ist ein Beispiel für eine verschachtelte Fehler-Handler-Route:

![](assets/nested-error-handling-route-350x174.png)

In diesem Szenario wird die zweite Fehler-Handler-Route unter der ersten Fehler-Handler-Route verschachtelt. Wenn die [!UICONTROL Dropbox] >[!UICONTROL Ordnermodul erstellen] auf einen Fehler trifft, wechselt die Ausführung zu Route 1, wenn die [!UICONTROL Datenfehler tritt auf] übergeben wird, wird das nächste Modul ausgeführt, gefolgt von [!UICONTROL Fortsetzen] Direktionsmodul, wenn bei der [!UICONTROL Dropbox] >[!UICONTROL Alle Dateien/Unterordner auflisten] in einem Ordnermodul.

Wenn jedoch ein Fehler damit auftritt [!DNL Dropbox] -Modul, wechselt die Ausführung zu &quot;Error Handler Route 2&quot;und endet mit der [!UICONTROL Ignorieren] Richtlinie. Die [!UICONTROL Anweisung &quot;Fortsetzen&quot;] -Modul in diesem Fall nicht ausgeführt.

Dies ist eine Kombination aus Filter- und Verschachtelungs-Fehler-Handlern.

