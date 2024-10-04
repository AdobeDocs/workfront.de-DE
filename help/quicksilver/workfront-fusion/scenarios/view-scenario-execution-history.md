---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Verlauf eines Szenarios in Adobe Workfront Fusion anzeigen
description: Sie können Informationen zu allen Ausführungen eines Szenarios anzeigen oder alle Ausführungen des Szenarios nach bestimmten Daten durchsuchen.
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

Die Ausführung eines Szenarios stellt einen einzelnen Ablauf des Szenarios dar.

Ein Szenario-Ereignis ist eine Änderung des Szenarios, z. B. Bearbeiten, Aktivieren oder Deaktivieren.

>[!NOTE]
>
>Der Verlauf eines Szenarios zeigt alle Ereignisse und Ausführungen eines Szenarios für die letzten 30 Tage an.

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

## Szenario-Verlauf anzeigen

### Anzeigen des Szenarioverlaufs auf der Seite [!UICONTROL Szenariodetails]

1. Klicken Sie im linken Bereich auf die Registerkarte **[!UICONTROL Szenario]** und klicken Sie dann auf das Szenario.

   Oder

   Wenn Sie im Szenario-Editor an dem Szenario arbeiten, klicken Sie in der linken oberen Ecke des Fensters auf den Linkspfeil ![](assets/exit-editing-arrow.png).

1. Zeigen Sie den Ausführungsverlauf im Tab **Verlauf** des Bedienfelds auf der rechten Seite an.

   Die folgenden Details werden für jede Ausführung des Szenarios aufgelistet:

   * Datum, an dem die Ausführung **[!UICONTROL gestartet]** war
   * **[!UICONTROL Status]** (Erfolg oder fehlgeschlagen)
   * Ausführen von **[!UICONTROL Dauer]**
   * Anzahl der **[!UICONTROL Vorgänge]**
   * Größe von **[!UICONTROL Datenübertragung]**

   >[!NOTE]
   >
   >Im Szenario-Verlauf wird neben den kürzlich ausgeführten Szenarien ein **Verarbeitungs** -Zeichen angezeigt, während die Ausführungsdetails in den Speicher geschrieben werden. Die Verarbeitung erfolgt unmittelbar nach der Ausführung des Szenarios. und sollte nicht länger als einige Minuten dauern. Details zur Ausführung des Szenarios sind möglicherweise nicht sichtbar, während die Ausführung verarbeitet wird.

1. Um Details zur Ausführung eines bestimmten Szenarios anzuzeigen, klicken Sie im rechten Bereich auf diese Ausführung.
1. Um Ereignisse anzuzeigen, klicken Sie rechts im Bedienfeld auf die Registerkarte **Ereignisse** .


### Anzeigen des Szenario-Verlaufs auf der Registerkarte [!UICONTROL Verlauf]

Die Registerkarte [!UICONTROL Verlauf] enthält mehr Details als auf der Seite [!UICONTROL Szenario-Detail] verfügbar sind. Sie können die Ausführungen auch auf der Registerkarte [!UICONTROL Verlauf] filtern und sortieren.

1. Klicken Sie im linken Bereich auf die Registerkarte **[!UICONTROL Szenario]** und klicken Sie dann auf das Szenario.

   Oder

   Wenn Sie im Szenario-Editor an dem Szenario arbeiten, klicken Sie in der linken oberen Ecke des Fensters auf den Linkspfeil ![](assets/exit-editing-arrow.png).

1. Klicken Sie oben links auf der Seite auf die Registerkarte **[!UICONTROL Verlauf]** .
1. (Optional) Detaillierte Informationen zu einem ausgewählten Szenario-Lauf, einschließlich der verarbeiteten Bundles, erhalten Sie, wenn Sie in der Zeile für diese Ausführung auf die Schaltfläche **[!UICONTROL Details]** klicken.

   Weitere Informationen zur Verarbeitung von Bundles finden Sie unter [Ausführungsfluss eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* Der Link [!UICONTROL details] ist nur sichtbar, wenn die Ausführung Details enthält.
   >
   >* Im Szenario-Verlauf wird neben den Szenarien, die kürzlich ausgeführt wurden, ein **Verarbeitungsverlauf** -Zeichen angezeigt, während die Ausführungsdetails in den Speicher geschrieben werden. Die Verarbeitung erfolgt unmittelbar nach der Ausführung des Szenarios. und sollte nicht länger als einige Minuten dauern. Details zur Ausführung des Szenarios sind möglicherweise nicht sichtbar, während die Ausführung verarbeitet wird.

1. Um Ereignisse anzuzeigen, aktivieren Sie den Umschalter **Ereignisse anzeigen** .

## den Ausführungsverlauf des Szenarios filtern

Sie können den Ausführungsverlauf filtern, um nur Ausführungen mit den angegebenen Werten anzuzeigen.

1. Öffnen Sie den vollständigen Seitenverlauf für ein Szenario, wie unter [Anzeigen des Ausführungsverlaufs eines Szenarios auf der Registerkarte [!UICONTROL Verlauf] ](#view-scenario-execution-history-on-the-history-tab) in diesem Artikel beschrieben.
1. Klicken Sie in der Kopfzeile der Spalte, nach der Sie filtern möchten, auf das Symbol [!UICONTROL filter] ![](assets/fusion-scenario-filter-icon.png) .
1. Geben Sie im Dialogfeld [!UICONTROL filter] die Werte ein, nach denen Sie filtern möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Das Filtersymbol ist orange in Spalten mit einem derzeit aktiven Filter.

## Sortieren des Ausführungsverlaufs des Szenarios

Sie können den Ausführungsverlauf des Szenarios sortieren.

1. Öffnen Sie den vollständigen Seitenverlauf für ein Szenario, wie unter [Anzeigen des Ausführungsverlaufs eines Szenarios auf der Registerkarte [!UICONTROL Verlauf] ](#view-scenario-execution-history-on-the-history-tab) in diesem Artikel beschrieben.
1. Klicken Sie in der Kopfzeile der Spalte, nach der Sie filtern möchten, auf das Symbol [!UICONTROL Sortieren] .
1. Optional: Um die Reihenfolge der Sortierung umzukehren, klicken Sie erneut auf das Symbol [!UICONTROL Sortieren] .

## Durchsuchen aller Ausführungen eines Szenarios

1. Öffnen Sie den vollständigen Seitenverlauf für ein Szenario, wie unter [Anzeigen des Ausführungsverlaufs eines Szenarios auf der Registerkarte [!UICONTROL Verlauf] ](#view-scenario-execution-history-on-the-history-tab) in diesem Artikel beschrieben.
1. Klicken Sie oben in der Liste der Ausführungen auf **[!UICONTROL Volltextsuche]** .

   Oder

   Geben Sie **Strg+Umschalt+F** (Windows) oder **Befehl+Umschalt+F** (Mac) ein.
Das Fenster [!UICONTROL Suche im Verlauf] wird geöffnet.

1. (Optional) Um nach Ausführungen zu suchen, die bestimmten Text enthalten, geben Sie den Text in die Suchleiste des Fensters **[!UICONTROL Suche im Verlauf]** ein.

   Um nach exaktem Text zu suchen, umgeben Sie den Text mit doppelten Anführungszeichen (&quot;Beispiel&quot;).

   >[!INFO]
   >
   >**Beispiel:** Wenn Sie die Ausführung suchen möchten, die ein bestimmtes Projekt erstellt hat, geben Sie die Projekt-ID in die Leiste [!UICONTROL Volltextsuche] ein.
   >
   >&quot;625ef2ef006036bd1794b6e52d737c5&quot;

1. (Optional) Um die Suche nach Datumsbereich zu beschränken, wählen Sie im Bereich [!UICONTROL Nach Datumsbereich] das Start- und Enddatum der gewünschten Suche aus.

   >[!NOTE]
   >
   >* Ausführungen sind nur für die letzten 30 Tage verfügbar.
   >
   >* [!DNL Workfront Fusion] speichert Webhook-Payloads für 30 Tage. Wenn Sie mehr als 30 Tage nach der Erstellung auf eine Webhook-Payload zugreifen, wird der Fehler &quot;[!UICONTROL Datei konnte nicht aus dem Speicher gelesen werden.]&quot; angezeigt.


1. (Optional) Um Ihre Suche nach Status zu beschränken, wählen Sie den gewünschten Status in der Dropdown-Liste **[!UICONTROL Nach Status]** aus.


   Verfügbare Status sind:

   * [!UICONTROL Alle]

   * [!UICONTROL Fehler]

   * [!UICONTROL Warnung]

   * [!UICONTROL Erfolg]

1. (Optional) Ändern Sie die Reihenfolge, in der die Ergebnisse in der Dropdown-Liste **[!UICONTROL Nach Datumsangaben sortieren]** angezeigt werden.

1. (Optional) Um eine Ausführungs-ID eines Szenarios zu kopieren, klicken Sie auf das Symbol **[!UICONTROL Ausführungskennung kopieren]** . <img src="assets/copy-fusion-execution-id-icon.png"> in der Zeile der gewünschten Ausführung

1. (Optional) Klicken Sie auf ein Ergebnis der [!UICONTROL Volltextsuche], um das Ausgabebundle des Szenario-Moduls zu untersuchen, das die Informationen enthält.
