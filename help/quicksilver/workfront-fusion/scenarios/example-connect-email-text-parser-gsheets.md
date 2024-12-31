---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: 'Beispiel für ein Adobe Workfront Fusion-Szenario: Verbinden von E-Mail-, Text-Parser- und Google-Tabellen'
description: Dieses Szenario hilft Ihnen, ein Protokoll aller E-Mail-Nachrichten zu erstellen und sie für weitere Aktionen in einer Tabelle zu kennzeichnen. Es erfasst einen E-Mail-Textkörper in zwei separaten Tabellen in einer Tabelle mithilfe regulärer Ausdrücke (Regex) als Suchmuster. Im ersten Muster wird nach einer Phrase gesucht, im zweiten nach derselben Phrase und E-Mail-Adresse.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Szenario: E-Mail verbinden, [!UICONTROL Text-Parser] und [!DNL Google Sheets]

Dieses Szenario hilft Ihnen, ein Protokoll aller E-Mail-Nachrichten zu erstellen und sie für weitere Aktionen in einer Tabelle zu kennzeichnen. Es erfasst einen E-Mail-Textkörper in zwei separaten Tabellen in einer Tabelle mithilfe regulärer Ausdrücke (Regex) als Suchmuster. Im ersten Muster wird nach einer Phrase gesucht, im zweiten nach derselben Phrase und E-Mail-Adresse.

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

## Voraussetzungen

Dieses Tutorial erfordert grundlegende Kenntnisse über reguläre Ausdrücke. Weitere Informationen zu Regex finden Sie unter [https://regexone.com](https://regexone.com/).

Das erste Modul hinzufügen und konfigurieren

1. Suchen Sie nach E-Mail und wählen Sie **[!UICONTROL E-Mails ansehen]** als Trigger aus.

   >[!NOTE]
   >
   >Sie können ein [!DNL Google]-Konto zwar über das E--Modul verbinden, aber auch ein [!DNL Gmail]-Modul verwenden.

1. Verbinden Sie entweder ein [!DNL Google] oder einen anderen IMAP-basierten E-Mail-Client (z. B. [!DNL Outlook]).
1. Wählen Sie nach der Verbindung einen Ordner aus, dessen eingehende E-Mails überwacht werden sollen, z. B[!UICONTROL  „Posteingang].
1. Wählen Sie [!UICONTROL Kriterien] die Option **[!UICONTROL Alle E-Mails]** (oder schränken Sie sie auf das Lesen oder Unlesen von E-Mails ein).

   Sie können auch abgerufene E-Mails als gelesen oder ungelesen markieren.

1. Legen Sie [!UICONTROL Maximale Ergebnisanzahl“ auf ] fest.

   ![](assets/save-max-as-1-350x304.png)

   Sie können dies je nach Anzahl der Nachrichten, die Sie erhalten, ändern. Es wird jedoch empfohlen, einen niedrigen Wert festzulegen und das Szenario häufiger auszuführen.

1. Klicken **[!UICONTROL unten auf]** Erweiterte Einstellungen anzeigen“.

   ![](assets/show-adv-settings-350x332.png)

1. E-Mails nach [!UICONTROL Absenderadresse], [!UICONTROL Betreff] und [!UICONTROL Phrase] filtern

   Dadurch haben Sie die Möglichkeit, nur relevante E-Mails anzusehen. In diesem Beispiel haben wir nur einen Filter „Betreff“ hinzugefügt und die anderen 2 leer gelassen.

   >[!NOTE]
   >
   >Wir fügen einen Router hinzu, um in einer E-Mail mit dem Iterator [!UICONTROL Match Pattern] und einem regulären Ausdruck (Regex) als Suchmuster nach Phrasen zu suchen. Dies ermöglicht es uns auch, ein Szenario mit mehreren Dienstprogrammen zu erstellen.

1. Nachdem die Konfiguration abgeschlossen ist und Sie aufgefordert werden, anzugeben, wo Sie mit der Überwachung Ihrer E-Mails beginnen möchten, klicken Sie auf **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Fahren Sie mit [Suche nach [!UICONTROL Flusskontrolle] fort und fügen Sie einen [!UICONTROL  hinzu]](#search-for-flow-control-and-add-a-router)

## Suchen Sie nach [!UICONTROL Flusssteuerung] und fügen Sie einen [!UICONTROL Router] hinzu

1. Fügen Sie nach einem Modul einen Router hinzu, um die Daten aufzuteilen oder zu duplizieren, bevor Sie sie an das nächste Modul senden.

   Hier verwenden wir einen [!UICONTROL Router], um den Text des E-Mail-Textkörpers an zwei separate Tabellen in einem [!DNL Google Sheet] zu senden.

   ![](assets/search-for-flow-control-350x220.png)

## Verwenden des [!UICONTROL Text Parser]-Moduls

1. Fügen Sie einen Transformator [!UICONTROL Übereinstimmungsmuster] hinzu, um in einer E-Mail nach einer Phrase zu suchen.

   Wir werden in allen eingehenden E-Mails nach dem [!UICONTROL  „Text Parser Module] suchen, um den Textkörper und den Namen des Absenders der E-Mails zu erfassen, die mit dieser Phrase übereinstimmen.

   1. Schreiben Sie das Muster als regulären Ausdruck:

      text\sparser\smodule

   1. (Optional) Verwenden Sie eine der anderen Optionen für das Muster.

      ![](assets/pattern-350x318.png)

      Multiline ist nützlich, wenn Ihr Text mehrere Zeilen enthält und Sie in jeder Zeile nach dem Muster suchen müssen. Für dieses Tutorial müssen wir nach dem Muster im gesamten Text der E-Mail suchen und lassen es daher deaktiviert.

   1. Klicken Sie [!UICONTROL  Feld ]Text“ auf das Attribut **Textinhalt** in der Liste.

      ![](assets/text-content-350x264.png)

      Dies ist das Attribut, das den Text aus dem E-Mail-Textkörper speichert, in dem wir nach dem Muster suchen werden.

1. Fügen Sie ein weiteres [!UICONTROL Übereinstimmungsmuster] hinzu, das nach derselben Phrase und einer E-Mail-Adresse sucht.

   Dies ist besonders nützlich, wenn Sie Kundenkonten mit mehreren Benutzern haben. Um Zeit zu sparen, können Sie das soeben erstellte [!UICONTROL Text Parser]-Modul klonen und mit dem Router verknüpfen.

   ![](assets/clone.png)

1. Bearbeiten Sie das Muster wie folgt:

   text\sparser\sModule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Dieses Muster sucht nach dem Satz &quot;[!UICONTROL Text Parser Module]&quot; und einer E-Mail-Adresse wie john.doe@gmail.com und gibt nur die E-Mail-Adresse zurück.

   >[!NOTE]
   >
   >Es ist wichtig, Ihren Regex in Übereinstimmung mit der Spezifikation der von Ihnen akzeptierten E-Mail-Adressen zu schreiben, aber die oben genannte übernimmt die meisten Standard-E-Mail-Adressen.

   * Wenn Sie nur nach einer E-Mail-Adresse suchen möchten, können Sie den folgenden Regex verwenden:

     ([\w.-]+@[\w.-]+)

   * Sie können auch nur nach Telefonnummern suchen, indem Sie den folgenden Regex verwenden:

     ^[+]?\(?(\d{1,3})\)?[\S-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}
Das obige Muster deckt die gängigsten Formate ab, in denen eine Telefonnummer geschrieben wird.

   Um Ihre Muster zu testen, empfehlen wir die Verwendung von [[!DNL https://regex101.com]](https://regex101.com/) mit [!DNL javascript] als Geschmack.

   Der Rest der Konfiguration bleibt die gleiche wie zuvor.

## [!DNL Google Sheets] hinzufügen

[!DNL Sheets] müssen wir zunächst eine Tabelle mit den erforderlichen Kopfzeilen erstellen.

1. Erstellen Sie eine Tabelle mit den Spalten, in denen die Benutzerdaten erfasst werden sollen. (Sie können auch eine vorhandene Datei verwenden).

   Erstellen Sie beispielsweise eine namens „E-Mail-Daten: Support-Ticket“ mit den Spalten „Absendername“, „Absender-E-Mail“ und „E-Mail-Inhalt“. Benennen Sie das Arbeitsblatt mit „enthält: Text-Parser-Modul“.

1. Fügen Sie das Modul [!UICONTROL Google Sheets] mit **[!UICONTROL Zeile hinzufügen]** als Aktion hinzu.

   ![](assets/add-a-row-350x174.png)

1. Verbinden Sie Ihr [!DNL Google]-Konto (falls noch nicht geschehen). Wählen Sie die zuvor erstellte Datei und dann das Arbeitsblatt aus, in dem Sie die Daten erfassen möchten.

   Das Setup sollte wie folgt aussehen:

   ![](assets/connect-google-acct-350x279.png)

1. Ordnen Sie die Attribute in den entsprechenden Feldern (Spalten) zu, um die Moduleinrichtung abzuschließen.

   ![](assets/map-attributes-350x282.png)

1. Klonen Sie das soeben erstellte Modul und verknüpfen Sie es mit dem zweiten [!UICONTROL Text Parser]-Modul.

   1. Gehen Sie zu Ihrem Arbeitsblatt, duplizieren Sie das zuvor erstellte Arbeitsblatt und geben Sie ihm einen Namen.

      Geben Sie ihm beispielsweise den Namen „enthält: Text-Parser-Modul und E-Mail“.

   1. Fügen Sie eine weitere Spalte hinzu, um die E-Mail-Adresse zu speichern, die der Textkörper der E-Mail enthält.

      Nennen Sie sie beispielsweise „E-Mail-Adresse freigegeben“.

   1. Klicken Sie auf das geklonte [!DNL Google Sheets], um die Einrichtung zu konfigurieren.
   1. Ändern Sie das Arbeitsblatt in das soeben erstellte.
   1. Ordnen Sie die Ausgabe aus dem [!UICONTROL Match Pattern]-Modul ($1) der Spalte zu, in der Sie die E-Mail-Adresse speichern möchten (freigegebene E-Mail-Adresse).

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Klicken Sie **[!UICONTROL OK]**, speichern Sie das Szenario und nehmen Sie es für einen Testlauf.

      Sie müssen wie folgt zwei separate E-Mails an die verbundene E-Mail-Adresse senden:

      * Enthält die Phrase &quot;[!UICONTROL Text Parser Module]&quot; (und keine E-Mail-Adresse)

        ![](assets/text-parser-module-350x103.png)

      * Enthält den obigen Satz und eine E-Mail-Adresse

        ![](assets/above-phrase-and-email-350x106.png)

        Wenn in Ihrer Einrichtung keine Fehler auftreten, werden Sie feststellen, dass das erste Arbeitsblatt alle E-Mails erfasst, die die Phrase &quot;[!UICONTROL Text Parser Module]&quot; enthalten, während das zweite Arbeitsblatt nur diejenigen erfasst, die die Phrase &quot;[!UICONTROL Text Parser Module]&quot; und eine E-Mail-Adresse enthalten. Die folgenden Screenshots sind verfügbar.

        Arbeitsblatt 1:

        ![](assets/worksheet-1-350x57.png)

        Arbeitsblatt 2:

        ![](assets/worksheet-2-350x41.png)

## Ressourcen

* [Kostenlose Übungen](https://regexone.com/) um mehr über reguläre Ausdrücke zu erfahren
* [Erfahren Sie mehr über den Abgleich von Telefonnummern](https://regexone.com/problem/matching_phone_numbers) mithilfe von Regex
* [Erfahren Sie mehr über E-Mail-](https://regexone.com/problem/matching_emails) mithilfe von Regex
* [Testen regulärer Ausdrücke](https://regex101.com/)
