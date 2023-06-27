---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Elemente mithilfe von Funktionen in zuordnen [!DNL Adobe Workfront Fusion]
description: Wenn Sie Elemente zuordnen, können Sie Funktionen verwenden, um einfache oder komplexe Formeln zu erstellen.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Elemente mithilfe von Funktionen in zuordnen [!DNL Adobe Workfront Fusion]

Wenn Sie Elemente zuordnen, können Sie Funktionen verwenden, um einfache oder komplexe Formeln zu erstellen.

Die in [!DNL Adobe Workfront Fusion] ähneln Funktionen in Excel und einigen Programmiersprachen. Sie bewerten allgemeine Logik, Mathematik, Text, Daten und Arrays. Sie können bedingte Logik und Umwandlungen von Elementwerten durchführen, z. B. das Konvertieren von Text in Großbuchstaben, das Zuschneiden von Text, das Konvertieren eines Datums in ein anderes Format und mehr. Weitere Informationen finden Sie unter [Informationen in Adobe Workfront Fusion von einem Modul zum anderen zuordnen](../../workfront-fusion/mapping/map-information-between-modules.md).

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

## Funktionen in Felder einfügen

Wenn Sie auf ein Feld klicken, wird die [!UICONTROL Mapping] angezeigt. Das Zuordnungsbedienfeld enthält mehrere Registerkarten:

![](assets/functions-toolbar-350x189.png)

Die erste Registerkarte ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (angezeigt beim Öffnen des Bedienfelds) zeigt die Elemente an, die Sie aus anderen Modulen zuordnen können.

Die anderen Registerkarten enthalten die folgenden Funktionstypen:

* **Allgemeine Funktionen** ![](assets/toolbar-icon-general-function.png) - Siehe [Allgemeine Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) für weitere Informationen.

* **Mathematische Funktionen** ![](assets/toolbar-icon-math-functions.png) - Siehe [Mathematische Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) für weitere Informationen.

* **Text- und Binärfunktionen** ![](assets/toolbar-icon-text&binary-functions.png) - Siehe [Zeichenfolgenfunktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) für weitere Informationen.

* **Datum und Uhrzeit** ![](assets/toolbar-icon-date&time-functions.png) - Siehe [Datums- und Uhrzeitfunktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) und den unten stehenden Artikeln für weitere Informationen.

   * [Token für die Datums- und Uhrzeitformatierung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token für Datums- und Uhrzeitanalyse in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funktionen zum Arbeiten mit Arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Siehe [Array-Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) für weitere Informationen.

So fügen Sie eine Funktion in ein Feld ein:

1. Klicken Sie auf den Funktionsnamen.

   Oder

   Ziehen Sie die Funktion in das Feld.

>[!INFO]
>
>**Beispiel:** Einige Datentypen verhindern, dass Benutzer mehr als eine bestimmte Anzahl von Zeichen eingeben. Mit der Teilzeichenfolgen-Funktion können Sie einen Wert auf eine bestimmte Anzahl von Zeichen beschränken.
>
>In diesem Beispiel beschränkt die Teilzeichenfolgenfunktion den Projektnamen auf 50 Zeichen.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Verschachtelungsfunktionen

Sie können Funktionen untereinander verschachteln.

## Verwendung [!DNL Google Sheets] Funktionen

Wenn [!DNL Workfront Fusion] verfügt nicht über eine Funktion, die Sie verwenden möchten, wird jedoch durch [!DNL Google Sheets], können Sie sie wie folgt verwenden:

1. In [!DNL Google Sheets]erstellen Sie eine neue leere Tabelle.
1. In [!DNL Workfront Fusion], öffnen Sie Ihr Szenario.
1. Fügen Sie die **[!DNL Google Sheets]** >**[!UICONTROL Zelle aktualisieren]** zum Szenario hinzu.

   Anweisungen zum Hinzufügen eines Moduls finden Sie unter [Hinzufügen eines Moduls in einem Szenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) im Artikel [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Konfigurieren Sie das Modul:

   1. Wählen Sie die neu erstellte Tabelle im **[!UICONTROL Tabelle]** -Feld.
   1. Fügen Sie Ihre Formel mit den Variablen [!DNL Google Sheets] -Funktion(en) in die **[!UICONTROL Wert]** -Feld.

      Sie können die Ausgabe der vorherigen Module wie gewohnt verwenden.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Fügen Sie die **[!UICONTROL Google Tabellen] >[!UICONTROL Zelle abrufen]** -Modul, um das berechnete Ergebnis abzurufen.
1. Konfigurieren Sie das Modul mit derselben Cell ID wie in Schritt 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
