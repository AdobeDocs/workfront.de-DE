---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Elemente mithilfe von Funktionen in [!DNL Adobe Workfront Fusion] zuordnen
description: Wenn Sie Elemente zuordnen, können Sie Funktionen verwenden, um einfache oder komplexe Formeln zu erstellen.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: d175a3d43f13338661d8b7e1cb79038a36522ff9
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Elemente mithilfe von Funktionen in [!DNL Adobe Workfront Fusion] zuordnen

Wenn Sie Elemente zuordnen, können Sie Funktionen verwenden, um einfache oder komplexe Formeln zu erstellen. Die in [!DNL Adobe Workfront Fusion] verfügbaren Funktionen ähneln den Funktionen in Excel und einigen Programmiersprachen:

* Sie bewerten allgemeine Logik, Mathematik, Text, Daten und Arrays.
* Sie können bedingte Logik und Umwandlungen von Elementwerten durchführen, z. B. das Konvertieren von Text in Großbuchstaben, das Zuschneiden von Text, das Konvertieren eines Datums in ein anderes Format und mehr.

Weitere Informationen finden Sie unter [Zuordnen von Informationen zwischen Modulen in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).


## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">

<col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td>  
   <td> <p>Alle</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td>  
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>  
   <td> 
   <p>Aktuell: Keine [!DNL Workfront Fusion] Lizenzanforderung.</p> 
   <p>Oder</p> 
   <p>Veraltet: Beliebig </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul> 
   <p>Oder</p> 
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Übersicht über die Registerkarte &quot;Zuordnung&quot;

So öffnen Sie das Bedienfeld [!UICONTROL mapping] für ein Feld:

1. Klicken Sie im linken Bereich auf **Szenarios** .
1. Wählen Sie ein Szenario.

![](assets/open-functions-bar.png)


### Registerkarten des Zuordnungsbedienfelds

Die folgenden Registerkarten befinden sich im Zuordnungsbereich:

* **Allgemeine Funktionen** ![](assets/toolbar-icon-general-function.png) - Weitere Informationen finden Sie unter [Allgemeine Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) .

* **Math-Funktionen** ![](assets/toolbar-icon-math-functions.png) - Weitere Informationen finden Sie unter [Math-Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) .

* **Text- und Binärfunktionen** ![](assets/toolbar-icon-text&binary-functions.png) - Weitere Informationen finden Sie unter [Zeichenfolgenfunktionen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) .

* **Datum und Uhrzeit** ![](assets/toolbar-icon-date&time-functions.png) - Weitere Informationen finden Sie unter [Datums- und Uhrzeitfunktionen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) und in den unten stehenden Artikeln:

   * [Token für die Datums- und Uhrzeitformatierung in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token für Datums- und Uhrzeitanalyse in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funktionen für die Arbeit mit Arrays** ![](assets/toolbar-icon-functions-for-arrays.png) - Weitere Informationen finden Sie unter [Array-Funktionen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) .

* **Andere Funktionen zuordnen** ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) zeigt die Elemente an, die Sie aus anderen Modulen zuordnen können. Diese Registerkarte ist nicht immer verfügbar.

![](assets/functions-toolbar-350x189.png)

## Funktionen in Felder einfügen

So fügen Sie eine Funktion in ein Feld ein:

1. Klicken Sie auf den Funktionsnamen.

   Oder

   Ziehen Sie die Funktion in das Feld.


>[!BEGINSHADEBOX]

**Beispiel:** Einige Datentypen verhindern, dass Benutzer mehr als eine bestimmte Anzahl von Zeichen eingeben. Mit der Teilzeichenfolgen-Funktion können Sie einen Wert auf eine bestimmte Anzahl von Zeichen beschränken.

In diesem Beispiel beschränkt die Teilzeichenfolgenfunktion den Projektnamen auf 50 Zeichen.

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## Verschachtelungsfunktionen

Sie können Funktionen untereinander verschachteln.

## [!DNL Google Sheets]-Funktionen verwenden

Wenn [!DNL Workfront Fusion] keine Funktion enthält, die Sie verwenden möchten, aber von [!DNL Google Sheets] gekennzeichnet ist, können Sie sie wie folgt verwenden:

1. Erstellen Sie in [!DNL Google Sheets] eine neue leere Tabelle.
1. Öffnen Sie in [!DNL Workfront Fusion] Ihr Szenario.
1. Fügen Sie das Modul **[!DNL Google Sheets]** >**[!UICONTROL Zelle]** aktualisieren zum Szenario hinzu.

   Anweisungen zum Hinzufügen eines Moduls finden Sie unter [Hinzufügen eines Moduls in einem Szenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) im Artikel [Erstellen eines Szenarios in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Konfigurieren Sie das Modul:

   1. Wählen Sie im Feld **[!UICONTROL Tabelle]** das neu erstellte Arbeitsblatt aus.
   1. Fügen Sie Ihre Formel, die die Funktion [!DNL Google Sheets] enthält, in das Feld **[!UICONTROL Wert]** ein.

      Sie können die Ausgabe der vorherigen Module wie gewohnt verwenden.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Fügen Sie das Modul **[!UICONTROL Google Tabellen] >[!UICONTROL Zellen abrufen]** ein, um das berechnete Ergebnis zu erhalten.
1. Konfigurieren Sie das Modul mit derselben Cell ID wie in Schritt 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
