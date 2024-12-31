---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Anzeigen des Verlaufs eines Szenarios in Adobe Workfront Fusion
description: Sie können Informationen zu allen Ausführungen für ein Szenario anzeigen oder alle Ausführungen des Szenarios nach bestimmten Daten durchsuchen.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: 2e26c4e4b5f331ed2e609381ef442f45e90c4faa
workflow-type: tm+mt
source-wordcount: '972'
ht-degree: 0%

---

# Anzeigen des Verlaufs eines Szenarios in [!DNL Adobe Workfront Fusion]

Sie können Informationen zu den Ereignissen oder Ausführungen eines Szenarios anzeigen oder alle Ausführungen des Szenarios nach bestimmten Daten durchsuchen.

Eine Szenario-Ausführung stellt eine einzelne Ausführung des Szenarios dar.

Ein Szenarioereignis ist eine Änderung des Szenarios, z. B. das Bearbeiten, Aktivieren oder Deaktivieren.

>[!NOTE]
>
>Im Verlauf eines Szenarios werden alle Ereignisse und Ausführungen eines Szenarios in den letzten 30 Tagen angezeigt.

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

## Szenarioverlauf anzeigen

### Zeigen Sie den Szenarioverlauf auf der Seite [!UICONTROL Szenariodetails] an

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Szenario“ im linken Bereich und klicken Sie dann auf das Szenario.

   Oder

   Wenn Sie an dem Szenario im Szenario-Editor arbeiten, klicken Sie auf den linken Pfeil ![](assets/exit-editing-arrow.png) der oberen linken Ecke des Fensters.

1. Zeigen Sie den Ausführungsverlauf auf der Registerkarte **Verlauf** des Bedienfelds auf der rechten Seite an.

   Die folgenden Details werden für jede Ausführung des Szenarios aufgelistet:

   * Datum, an dem der Durchlauf gestartet **[!UICONTROL gestartet]**
   * **[!UICONTROL Status]** (Erfolg oder Fehlgeschlagen)
   * Ausführen **[!UICONTROL Dauer]**
   * Anzahl **[!UICONTROL Vorgänge]**
   * Größe von **[!UICONTROL Datenübertragung]**

   >[!NOTE]
   >
   >Der Szenarioverlauf zeigt neben **kürzlich ausgeführten Szenarien** Badge Verarbeitung an, während die Ausführungsdetails in den Speicher geschrieben werden. Die Verarbeitung erfolgt unmittelbar nach der Ausführung des Szenarios. und sollte nicht länger als ein paar Minuten dauern. Details zur Szenario-Ausführung sind während der Ausführung möglicherweise nicht sichtbar.

1. Um Details zu einer bestimmten Szenario-Ausführung anzuzeigen, klicken Sie im rechten Bedienfeld auf diese Ausführung.
1. Um Ereignisse anzuzeigen, klicken Sie auf **Registerkarte** Ereignisse“ im Bedienfeld auf der rechten Seite.


### Szenarioverlauf auf der Registerkarte [!UICONTROL Verlauf] anzeigen

Die Registerkarte [!UICONTROL Verlauf] zeigt mehr Details an, als auf der Seite [!UICONTROL Szenario-Detail] verfügbar sind. Sie können die Ausführungen auch auf der Registerkarte [!UICONTROL Verlauf] filtern und sortieren.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Szenario“ im linken Bereich und klicken Sie dann auf das Szenario.

   Oder

   Wenn Sie an dem Szenario im Szenario-Editor arbeiten, klicken Sie auf den linken Pfeil ![](assets/exit-editing-arrow.png) der oberen linken Ecke des Fensters.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Verlauf“ in der oberen linken Ecke der Seite
1. (Optional) Ausführliche Informationen zu einer ausgewählten Szenario-Ausführung, einschließlich der verarbeiteten Bundles, erhalten Sie, wenn Sie auf die **[!UICONTROL Details]** in der Zeile für diese Ausführung klicken.

   Weitere Informationen zur Verarbeitung von Bundles finden Sie unter [Szenario-Ausführungsfluss in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* Der [!UICONTROL details]-Link ist nur sichtbar, wenn für die Ausführung Details verfügbar sind.
   >
   >* Der Szenarioverlauf zeigt neben Szenarien **die kürzlich ausgeführt wurden,** Badge „Verarbeitungsverlauf“ an, während die Ausführungsdetails in den Speicher geschrieben werden. Die Verarbeitung erfolgt unmittelbar nach der Ausführung des Szenarios. und sollte nicht länger als ein paar Minuten dauern. Details zur Szenario-Ausführung sind während der Ausführung möglicherweise nicht sichtbar.

1. Um Ereignisse anzuzeigen, aktivieren Sie den Umschalter **Ereignisse anzeigen**.

## Filtern des Ausführungsverlaufs des Szenarios

Sie können den Ausführungsverlauf filtern, um nur Ausführungen mit den angegebenen Werten anzuzeigen.

1. Öffnen Sie den vollständigen Seitenverlauf für ein Szenario, wie in [Ausführungsverlauf des Szenarios anzeigen auf der Registerkarte [!UICONTROL Verlauf] in ](#view-scenario-execution-history-on-the-history-tab) Artikel beschrieben.
1. Klicken Sie auf [!UICONTROL  Symbol ]Filtern![](assets/fusion-scenario-filter-icon.png) in der Kopfzeile der Spalte, nach der Sie filtern möchten.
1. Geben [!UICONTROL  im ] „Filter“ die Werte ein, nach denen gefiltert werden soll.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Das Filtersymbol ist in Spalten mit einem derzeit aktiven Filter orange.

## Sortieren des Ausführungsverlaufs des Szenarios

Sie können den Ausführungsverlauf des Szenarios sortieren.

1. Öffnen Sie den vollständigen Seitenverlauf für ein Szenario, wie in [Ausführungsverlauf des Szenarios anzeigen auf der Registerkarte [!UICONTROL Verlauf] in ](#view-scenario-execution-history-on-the-history-tab) Artikel beschrieben.
1. Klicken Sie auf [!UICONTROL  Symbol ]Sortieren“ in der Kopfzeile der Spalte, nach der Sie filtern möchten.
1. Optional: Um die Sortierreihenfolge umzukehren, klicken Sie erneut auf [!UICONTROL Sortieren]-Symbol.

## Alle Ausführungen eines Szenarios durchsuchen

1. Öffnen Sie den vollständigen Seitenverlauf für ein Szenario, wie in [Ausführungsverlauf des Szenarios anzeigen auf der Registerkarte [!UICONTROL Verlauf] in ](#view-scenario-execution-history-on-the-history-tab) Artikel beschrieben.
1. Klicken Sie **[!UICONTROL Volltextsuche]** oben in der Liste der Ausführungen auf.

   Oder

   Geben Sie **Strg+Umschalt+F** (Windows) oder **Befehl+Umschalt+F** (Mac) ein
Das Fenster [!UICONTROL Suche im Verlauf] wird geöffnet.

1. (Optional) Um nach Ausführungen zu suchen, die bestimmten Text enthalten, geben Sie den Text in der Suchleiste des Fensters **[!UICONTROL Suche im Verlauf]** ein.

   Um nach exaktem Text zu suchen, setzen Sie den Text in Anführungszeichen („Beispiel„).

   >[!INFO]
   >
   >**Beispiel:** Wenn Sie die Ausführung finden möchten, mit der ein bestimmtes Projekt erstellt wurde, geben Sie die Projekt-ID in die ] &quot;[!UICONTROL &quot; ein.
   >
   >„625ef2ef0006036bd1794b6e52d737c5“

1. (Optional) Um die Suche nach Datumsbereich zu beschränken, wählen Sie das Anfangs- und Enddatum der gewünschten Suche im Bereich [!UICONTROL Nach ]) aus.

   >[!NOTE]
   >
   >* Ausführungen sind nur für die letzten 30 Tage verfügbar.
   >
   >* [!DNL Workfront Fusion] speichert Webhook-Payloads 30 Tage lang. Wenn Sie mehr als 30 Tage nach der Erstellung auf eine Webhook-Payload zugreifen, wird der Fehler &quot;[!UICONTROL Datei konnte nicht aus dem Speicher gelesen werden“ ].


1. (Optional) Um die Suche nach Status zu begrenzen, wählen Sie den gewünschten Status in der Dropdown-Liste **[!UICONTROL Nach Status]** aus.


   Verfügbare Status sind:

   * [!UICONTROL Alle]

   * [!UICONTROL Fehler]

   * [!UICONTROL Warnung]

   * [!UICONTROL Erfolg]

1. (Optional) Ändern Sie die Reihenfolge, in der die Ergebnisse im Dropdown-Menü **[!UICONTROL Sortieren nach]**&quot; angezeigt werden.

1. (Optional) Um eine Szenario-Ausführungs-ID zu kopieren, klicken Sie auf das Symbol **[!UICONTROL Ausführungs-ID kopieren]** <img src="assets/copy-fusion-execution-id-icon.png"> in der Zeile der gewünschten Ausführung

1. (Optional) Klicken Sie auf ein Ergebnis der [!UICONTROL Volltextsuche] um das Ausgabepaket des Szenario-Moduls zu überprüfen, das die Informationen enthält.
