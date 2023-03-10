---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Ausführungsverlauf eines Szenarios in Adobe Workfront Fusion anzeigen
description: Sie können Informationen zu allen Ausführungen eines Szenarios anzeigen oder alle Ausführungen des Szenarios nach bestimmten Daten durchsuchen.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# Anzeigen des Ausführungsverlaufs eines Szenarios im [!DNL Adobe Workfront Fusion]

Sie können Informationen zu allen Ausführungen eines Szenarios anzeigen oder alle Ausführungen des Szenarios nach bestimmten Daten durchsuchen.

Der Ausführungsverlauf eines Szenarios zeigt alle Ausführungen eines Szenarios für die letzten 30 Tage an.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Alle Ausführungen eines Szenarios anzeigen

### Anzeigen des Ausführungsverlaufs eines Szenarios [!UICONTROL Details des Szenarios] page

1. Klicken Sie auf **[!UICONTROL Szenario]** im linken Bereich auf und klicken Sie dann auf das Szenario.

   Oder

   Wenn Sie im Szenario-Editor an dem Szenario arbeiten, klicken Sie auf den Pfeil nach links ![](assets/exit-editing-arrow.png) in der Nähe der linken oberen Ecke des Fensters.

1. Zeigen Sie die Informationen in der Liste auf der rechten Seite an.

   ![](assets/open-history-tab-350x202.png)

   F

   Sie können auch auf klicken, um eine vollständige Seitenansicht dieser Informationen anzuzeigen. Mit der Vollseitenansicht können Sie den Verlauf filtern, um bestimmte Ausführungen anzuzeigen.

   Die folgenden Details werden für jede Ausführung des Szenarios aufgelistet:

   * Datum, an dem die Ausführung ausgeführt wurde **[!UICONTROL Gestartet]**
   * **[!UICONTROL Status]** (Erfolg oder fehlgeschlagen)
   * Ausführen **[!UICONTROL Dauer]**
   * Anzahl der **[!UICONTROL Aktivitäten]**
   * Größe **[!UICONTROL Datenübertragung]**
   * Link zu **[!UICONTROL Details]**

### Anzeigen des Ausführungsverlaufs eines Szenarios [!UICONTROL Geschichte] tab

Die [!UICONTROL Geschichte] zeigt mehr Details an, als auf der Registerkarte verfügbar sind [!UICONTROL Details des Szenarios] Seite. Sie können die Ausführungen auch nach der [!UICONTROL Geschichte] Registerkarte.

1. Klicken Sie auf **[!UICONTROL Szenario]** im linken Bereich auf und klicken Sie dann auf das Szenario.

   Oder

   Wenn Sie im Szenario-Editor an dem Szenario arbeiten, klicken Sie auf den Pfeil nach links ![](assets/exit-editing-arrow.png) in der Nähe der linken oberen Ecke des Fensters.

1. Klicken Sie auf **[!UICONTROL Geschichte]** Registerkarte oben links auf der Seite
1. (Optional) Detaillierte Informationen zu einem ausgewählten Szenario-Lauf, einschließlich der verarbeiteten Bundles, finden Sie unter **[!UICONTROL Details]** Link.

   Weitere Informationen zur Verarbeitung von Bundles finden Sie unter [Ausführungsfluss des Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >Die [!UICONTROL details] -Link nur sichtbar ist, wenn Details zur Ausführung verfügbar sind.

## den Ausführungsverlauf des Szenarios filtern

Sie können den Ausführungsverlauf filtern, um nur Ausführungen mit den angegebenen Werten anzuzeigen.

1. Öffnen Sie den vollständigen Seitenverlauf für ein Szenario, wie unter [Anzeigen des Ausführungsverlaufs eines Szenarios [!UICONTROL Geschichte] tab](#view-scenario-execution-history-on-the-history-tab) in diesem Artikel.
1. Klicken Sie auf [!UICONTROL filter] icon ![](assets/fusion-scenario-filter-icon.png) in der Kopfzeile der Spalte, nach der Sie filtern möchten.
1. Im [!UICONTROL filter] eingeben, geben Sie die Werte ein, nach denen Sie filtern möchten.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

Das Filtersymbol ist orange in Spalten mit einem derzeit aktiven Filter.

## Sortieren des Ausführungsverlaufs des Szenarios

Sie können den Ausführungsverlauf des Szenarios sortieren.

1. Öffnen Sie den vollständigen Seitenverlauf für ein Szenario, wie unter [Anzeigen des Ausführungsverlaufs eines Szenarios [!UICONTROL Geschichte] tab](#view-scenario-execution-history-on-the-history-tab) in diesem Artikel.
1. Klicken Sie auf [!UICONTROL Sortieren] in der Kopfzeile der Spalte, nach der Sie filtern möchten.
1. Optional: Um die Sortierreihenfolge umzukehren, klicken Sie auf die [!UICONTROL Sortieren] erneut.

## Durchsuchen aller Ausführungen eines Szenarios

1. Klicken Sie auf **[!UICONTROL Szenario]** icon ![](assets/scenarios-icon.png) Klicken Sie im linken Bereich auf das Szenario.

   Oder

   Wenn Sie im Szenario-Editor an dem Szenario arbeiten, klicken Sie auf den Pfeil nach links ![](assets/exit-editing-arrow.png) in der Nähe der linken oberen Ecke des Fensters.

1. Klicken Sie auf **[!UICONTROL Geschichte]** Registerkarte in der oberen linken Ecke des Bildschirms.
1. Klicken **[!UICONTROL Volltextsuche]** oben in der Liste der Ausführungen.

   Oder

   Typ **Strg+Umschalt+F** (Windows) oder **Befehl+Umschalt+F** (Mac) Die [!UICONTROL Suche im Verlauf] geöffnet.

1. (Optional) Um nach Ausführungen zu suchen, die bestimmten Text enthalten, geben Sie den Text in die Suchleiste des **[!UICONTROL Suche im Verlauf]** Fenster.

   Um nach exaktem Text zu suchen, umgeben Sie den Text mit doppelten Anführungszeichen (&quot;Beispiel&quot;).

   >[!INFO]
   >
   >**Beispiel:** Wenn Sie die Ausführung suchen möchten, die ein bestimmtes Projekt erstellt hat, geben Sie die Projekt-ID in das [!UICONTROL Volltextsuche] Bar.
   >
   >&quot;625ef2ef006036bd1794b6e52d737c5&quot;

1. (Optional) Um die Suche nach Datumsbereich zu begrenzen, wählen Sie in der [!UICONTROL Nach Datumsbereich] Bereich.

   >[!NOTE]
   >
   >* Ausführungen sind nur für die letzten 30 Tage verfügbar.
   >
   >* [!DNL Workfront Fusion] speichert Webhook-Payloads für 30 Tage. Wenn Sie mehr als 30 Tage nach der Erstellung auf eine Webhook-Payload zugreifen, tritt der Fehler auf &quot;[!UICONTROL Datei konnte nicht aus Speicher gelesen werden.]&quot;



1. (Optional) Um die Suche nach Status zu begrenzen, wählen Sie den gewünschten Status in der **[!UICONTROL Nach Status]** Dropdown-Liste.


   Verfügbare Status sind:

   * [!UICONTROL Alle]

   * [!UICONTROL Fehler]

   * [!UICONTROL Warnung]

   * [!UICONTROL Glückwunsch]

1. (Optional) Ändern Sie die Reihenfolge, in der die Ergebnisse im **[!UICONTROL Nach Datum sortieren]** Dropdown-Liste.

1. (Optional) Um eine Ausführungs-ID für ein Szenario zu kopieren, klicken Sie auf die **[!UICONTROL Ausführungs-ID kopieren]** icon <img src="assets/copy-fusion-execution-id-icon.png"> in der Zeile der gewünschten Ausführung

1. (Optional) Klicken Sie auf ein Ergebnis der [!UICONTROL Volltextsuche] um das Ausgabebundle des Szenario-Moduls zu untersuchen, das die Informationen enthält.
