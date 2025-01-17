---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Zuordnen von Elementen mithilfe von Funktionen in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 1%

---

# Zuordnen von Elementen mithilfe von Funktionen in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Zuordnen eines Elements mithilfe von Funktionen](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-using-functions.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Beim Zuordnen von Elementen können Sie Funktionen verwenden, um einfache oder komplexe Formeln zu erstellen. Die in [!DNL Adobe Workfront Fusion] verfügbaren Funktionen ähneln den Funktionen in Excel und in einigen Programmiersprachen:

* Sie bewerten allgemeine Logik, Mathematik, Text, Daten und Arrays.
* Mit ihnen können Sie bedingte Logik und Umwandlungen von Elementwerten durchführen, z. B. einen Text in Großbuchstaben umwandeln, Text kürzen, ein Datum in ein anderes Format konvertieren und vieles mehr.

Weitere Informationen finden Sie unter [Zuordnen von Informationen von einem Modul zu einem anderen in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).


## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">

<col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>  
   <td> <p>Beliebig</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>  
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Work] oder höher</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td>  
   <td> 
   <p>Aktuell: Keine [!DNL Workfront Fusion].</p> 
   <p>Oder</p> 
   <p>Legacy: Beliebig </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</li><li>[!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] ist enthalten.</li></ul> 
   <p>Oder</p> 
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Registerkarte „Zuordnung“ - Übersicht

So öffnen Sie [!UICONTROL  Bedienfeld ]Zuordnung“ für ein Feld:

1. Klicken Sie **linken** auf „Szenarien“.
1. Wählen Sie ein Szenario.

![](assets/open-functions-bar.png)


### Registerkarten des Zuordnungsbereichs

Die folgenden Registerkarten befinden sich im Bedienfeld „Zuordnung“:

* **Allgemeine Funktionen** ![](assets/toolbar-icon-general-function.png) - Weitere Informationen finden [Allgemeine Funktionen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

* **Mathematische Funktionen** ![](assets/toolbar-icon-math-functions.png) - Weitere Informationen finden Sie [Mathematische Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md).

* **Text- und Binärfunktionen** ![](assets/toolbar-icon-text&binary-functions.png) - Weitere Informationen finden Sie unter [Zeichenfolgenfunktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md).

* **Datum und Uhrzeit** ![](assets/toolbar-icon-date&time-functions.png) - Weitere Informationen finden Sie [Datums- und  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) in und in den folgenden Artikeln:

   * [Token zur Formatierung von Datum und Uhrzeit in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token zum Analysieren von Datum und Uhrzeit in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funktionen für die Arbeit mit Arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Weitere Informationen finden Sie unter [Array [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md)Funktionen in.

* **Andere Funktionen zuordnen** zeigt ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) die Elemente an, die Sie aus anderen Modulen zuordnen können. Diese Registerkarte ist nicht immer verfügbar.

![](assets/functions-toolbar-350x189.png)

## Funktionen in Felder einfügen

So fügen Sie eine Funktion in ein Feld ein:

1. Klicken Sie auf den Funktionsnamen.

   Oder

   Ziehen Sie die Funktion in das Feld.


>[!BEGINSHADEBOX]

**Beispiel:** Einige Datentypen verhindern, dass Benutzer mehr als eine bestimmte Anzahl von Zeichen eingeben. Sie können die Funktion Teilzeichenfolge verwenden, um einen Wert auf eine bestimmte Anzahl von Zeichen zu beschränken.

In diesem Beispiel beschränkt die Funktion Teilzeichenfolge den Projektnamen auf 50 Zeichen.

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## Verschachteln von Funktionen

Sie können Funktionen ineinander verschachteln.

## [!DNL Google Sheets] verwenden

Wenn [!DNL Workfront Fusion] keine Funktion enthält, die Sie verwenden möchten, es aber von [!DNL Google Sheets] vorgestellt wird, können Sie sie wie folgt verwenden:

1. Erstellen Sie [!DNL Google Sheets] eine neue leere Tabelle.
1. Öffnen Sie [!DNL Workfront Fusion] Ihr Szenario.
1. Fügen Sie das **[!DNL Google Sheets]** Modul **[!UICONTROL Zelle aktualisieren]** zum Szenario hinzu.

   Anweisungen zum Hinzufügen eines Moduls finden Sie unter [Hinzufügen eines Moduls in einem ](../../workfront-fusion/scenarios/create-a-scenario.md#add)) im Artikel [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Konfigurieren Sie das Modul:

   1. Wählen Sie die neu erstellte Tabelle im Feld **[!UICONTROL Tabelle]** aus.
   1. Fügen Sie die Formel, die die [!DNL Google Sheets] enthält, in das Feld **[!UICONTROL Wert]** ein.

      Sie können die Ausgabe vorhergehender Module wie gewohnt verwenden.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Fügen Sie das Modul **[!UICONTROL Google] >[!UICONTROL Zelle abrufen]** ein, um das berechnete Ergebnis zu erhalten.
1. Konfigurieren Sie das Modul mit derselben Zellen-ID, die Sie in Schritt 4 verwendet haben.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
