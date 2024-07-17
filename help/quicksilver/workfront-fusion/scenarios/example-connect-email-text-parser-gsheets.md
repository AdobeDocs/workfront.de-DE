---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: "Adobe Workfront Fusion-Beispielszenario: E-Mail-, Text-Parser- und Google Tabellen verbinden"
description: In diesem Szenario können Sie ein Protokoll aller E-Mail-Nachrichten erstellen und diese für weitere Aktionen in einer Tabelle taggen. Sie erfasst einen E-Mail-Textkörper in zwei separaten Tabellen in einer Tabelle und verwendet dabei Reguläre Ausdrücke (Regex) als Suchmuster. Das erste Muster sucht nach einer Wortgruppe und das zweite nach derselben Wortgruppe und einer E-Mail-Adresse.
author: Becky
feature: Workfront Fusion
exl-id: ebcfa3b9-3207-441c-9ce5-9af696c0119d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 0%

---

# Beispiel für das [!DNL Adobe Workfront Fusion]-Szenario: E-Mail verbinden, [!UICONTROL Text-Parser] und [!DNL Google Sheets]

In diesem Szenario können Sie ein Protokoll aller E-Mail-Nachrichten erstellen und diese für weitere Aktionen in einer Tabelle taggen. Sie erfasst einen E-Mail-Textkörper in zwei separaten Tabellen in einer Tabelle und verwendet dabei Reguläre Ausdrücke (Regex) als Suchmuster. Das erste Muster sucht nach einer Wortgruppe und das zweite nach derselben Wortgruppe und einer E-Mail-Adresse.

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

## Voraussetzungen

Dieses Tutorial erfordert grundlegende Kenntnisse regulärer Ausdrücke. Weitere Informationen zu Regex finden Sie unter [https://regexone.com](https://regexone.com/).

Das erste Modul hinzufügen und konfigurieren

1. Suchen Sie nach E-Mail und wählen Sie **[!UICONTROL E-Mails ansehen]** als Trigger aus.

   >[!NOTE]
   >
   >Sie können zwar ein [!DNL Google]-Konto mit dem Email-Modul verbinden, aber auch ein [!DNL Gmail]-Modul verwenden.

1. Verbinden Sie entweder ein [!DNL Google] -Konto oder einen anderen IMAP-basierten E-Mail-Client (z. B. [!DNL Outlook]).
1. Wählen Sie nach der Verbindung einen Ordner aus, dessen eingehende E-Mails Sie sehen möchten, z. B. [!UICONTROL Posteingang].
1. Wählen Sie unter [!UICONTROL Kriterien] die Option **[!UICONTROL Alle E-Mails]** aus (oder schränken Sie sie auf Lesen oder Unlesen von E-Mails ein).

   Sie können auch abgerufene E-Mails als gelesen oder ungelesen markieren.

1. Setzen Sie die [!UICONTROL maximale Anzahl von Ergebnissen] auf 1.

   ![](assets/save-max-as-1-350x304.png)

   Sie können diese Einstellung je nach der Menge der empfangenen Nachrichten ändern. Es wird jedoch empfohlen, einen niedrigen Wert festzulegen und das Szenario häufiger auszuführen.

1. Klicken Sie unten auf **[!UICONTROL Erweiterte Einstellungen anzeigen]** .

   ![](assets/show-adv-settings-350x332.png)

1. Filtern Sie E-Mails nach der [!UICONTROL Absenderadresse], dem [!UICONTROL Betreff] und dem [!UICONTROL Satz].

   So können Sie nur relevante E-Mails sehen. In diesem Beispiel haben wir nur den Filter Betreff hinzugefügt und die anderen beiden leer gelassen.

   >[!NOTE]
   >
   >Wir fügen einen Router hinzu, um mithilfe des Iterators [!UICONTROL Übereinstimmungsmuster] und eines regulären Ausdrucks (Regex) nach Wortgruppen in einer E-Mail zu suchen. Dies ermöglicht uns auch, ein Szenario mit mehreren Dienstprogrammen zu erstellen.

1. Nachdem die Konfiguration abgeschlossen ist und Sie aufgefordert werden, anzugeben, wo Sie Ihre E-Mails sehen können, klicken Sie auf **[!DNL From now on]**.

   ![](assets/from-now-on-350x236.png)

1. Suchen Sie weiter nach [!UICONTROL Flusssteuerung] und fügen Sie einen [!UICONTROL Router]](#search-for-flow-control-and-add-a-router) hinzu.[

## Suchen Sie nach [!UICONTROL Flusssteuerung] und fügen Sie einen [!UICONTROL Router] hinzu.

1. Fügen Sie nach einem Modul einen Router hinzu, um die Daten zu teilen oder zu duplizieren, bevor Sie sie an das nächste Modul senden.

   In unserem Beispiel haben wir einen [!UICONTROL Router] verwendet, um den Text des E-Mail-Textkörpers an zwei separate Tabellen in einem [!DNL Google Sheet] zu senden.

   ![](assets/search-for-flow-control-350x220.png)

## Verwenden des Moduls [!UICONTROL Text Parser]

1. Fügen Sie einen Transformator [!UICONTROL Übereinstimmungsmuster] hinzu, um nach einem Satz in einer E-Mail zu suchen.

   Wir suchen in allen eingehenden E-Mails nach der Wortgruppe &quot;[!UICONTROL text parser module]&quot;, um den Haupttext und den Namen des Absenders der E-Mails zu erfassen, die mit dieser Wortgruppe übereinstimmen.

   1. Schreiben Sie das Muster als regulären Ausdruck:

      text\sparser\smodule

   1. (Optional) Verwenden Sie eine der anderen Musteroptionen.

      ![](assets/pattern-350x318.png)

      Mehrzeilig ist nützlich, wenn Ihr Text mehrere Zeilen enthält und Sie in jeder Zeile nach dem Muster suchen müssen. Für dieses Tutorial müssen wir nach dem Muster im gesamten Text des E-Mail-Textkörpers suchen. Daher lassen wir es deaktiviert.

   1. Klicken Sie im Feld [!UICONTROL Text] auf das Attribut **Textinhalt** in der Liste.

      ![](assets/text-content-350x264.png)

      Dies ist das Attribut, das den Text aus dem E-Mail-Textkörper speichert, in dem nach dem Muster gesucht wird.

1. Fügen Sie ein weiteres [!UICONTROL Übereinstimmungsmuster] hinzu, das nach demselben Satz und einer E-Mail-Adresse sucht.

   Dies ist besonders nützlich, wenn Sie über Kundenkonten mit mehreren Benutzern verfügen. Um Zeit zu sparen, können Sie das soeben erstellte Modul [!UICONTROL Text Parser] klonen und mit dem Router verknüpfen.

   ![](assets/clone.png)

1. Bearbeiten Sie das Muster wie folgt:

   text\sparser\smodule.+\s([\w.-]+@[\w.-]+)

   ![](assets/text-parser-350x202.png)

   Dieses Muster sucht nach der Wortgruppe &quot;[!UICONTROL text parser module]&quot; und einer E-Mail-Adresse wie john.doe@gmail.com und gibt nur die E-Mail-Adresse zurück.

   >[!NOTE]
   >
   >Es ist wichtig, Ihren Regex entsprechend der Spezifikation der E-Mail-Adressen zu schreiben, die Sie akzeptieren, aber die oben genannte übernimmt die meisten Standard-E-Mail-Adressen.

   * Wenn Sie nur nach E-Mail-Adresse suchen möchten, können Sie den unten stehenden Regex verwenden:

     ([\w.-]+@[\w.-]+)

   * Sie können auch nur mithilfe des unten stehenden Regex nach Telefonnummern suchen:

     ^[+]?\(?(\d{1,3})\)?[\s-]?\(?(\d{3})\)?[\s-]?\d{3}[\s-]?\d{3,4}
Das obige Muster deckt die gängigsten Formate ab, in denen eine Telefonnummer geschrieben wird.

   Um Ihre Muster zu testen, empfehlen wir die Verwendung von [[!DNL https://regex101.com]](https://regex101.com/) mit [!DNL javascript] als Geschmack.

   Der Rest der Konfiguration bleibt derselbe wie zuvor.

## Hinzufügen der [!DNL Google Sheets]-Module

Für [!DNL Sheets] müssen wir zunächst eine Tabelle mit den erforderlichen Kopfzeilen erstellen.

1. Erstellen Sie eine Tabelle mit den Spalten, unter denen Sie die Benutzerdaten erfassen möchten. (Sie können auch eine vorhandene Datei verwenden.)

   Erstellen Sie beispielsweise eine mit dem Namen &quot;E-Mail-Daten: Support-Ticket&quot;und verwenden Sie als Spalten den Namen des Absenders, die E-Mail-Adresse des Absenders und den E-Mail-Inhalt. Nennen Sie das Arbeitsblatt &quot;enthält: Text-Parser-Modul&quot;.

1. Fügen Sie das Modul [!UICONTROL Google Tabellen] mit **[!UICONTROL Zeile hinzufügen]** als Aktion hinzu.

   ![](assets/add-a-row-350x174.png)

1. Verbinden Sie Ihr [!DNL Google] -Konto (falls noch nicht geschehen). Wählen Sie die zuvor erstellte Datei und danach das Arbeitsblatt aus, in dem Sie die Daten erfassen.

   Ihr Setup sollte wie folgt aussehen:

   ![](assets/connect-google-acct-350x279.png)

1. Ordnen Sie die Attribute in den entsprechenden Feldern (Spalten) zu, um die Moduleinrichtung abzuschließen.

   ![](assets/map-attributes-350x282.png)

1. Klonen Sie das soeben erstellte Modul und verknüpfen Sie es mit dem zweiten [!UICONTROL Text Parser] -Modul.

   1. Markieren Sie das Arbeitsblatt im Arbeitsblatt, duplizieren Sie es, und geben Sie ihm einen Namen.

      Nennen Sie ihn beispielsweise &quot;enthält: Text-Parser-Modul und E-Mail&quot;.

   1. Fügen Sie eine weitere Spalte hinzu, um die E-Mail-Adresse zu speichern, die der E-Mail-Textkörper enthält.

      Nennen Sie ihn beispielsweise &quot;Freigegebene E-Mail-Adresse&quot;.

   1. Klicken Sie auf das geklonte [!DNL Google Sheets]-Modul, um das Setup zu konfigurieren.
   1. Ändern Sie das Arbeitsblatt in das neue, soeben erstellte.
   1. Ordnen Sie die Ausgabe des Moduls [!UICONTROL Übereinstimmungsmuster] ($1) der Spalte zu, in der Sie die E-Mail-Adresse speichern möchten (Freigegebene E-Mail-Adresse).

      ![](assets/map-the-output.png)

      ![](assets/sender-name-350x411.png)

   1. Klicken Sie auf **[!UICONTROL OK]** , speichern Sie das Szenario und nehmen Sie es für einen Testlauf.

      Sie müssen zwei separate E-Mails wie folgt an die angeschlossene E-Mail-Adresse senden:

      * Enthält die Phrase &quot;[!UICONTROL text parser module]&quot;(und keine E-Mail-Adresse)

        ![](assets/text-parser-module-350x103.png)

      * Enthält den obigen Satz und eine E-Mail-Adresse

        ![](assets/above-phrase-and-email-350x106.png)

        Wenn bei der Einrichtung keine Fehler auftreten, werden Sie sehen, dass das erste Arbeitsblatt alle E-Mails erfasst, die die Wortgruppe &quot;[!UICONTROL text parser module]&quot; enthalten, während das zweite Arbeitsblatt nur die E-Mails erfasst, die die Wortgruppe &quot;[!UICONTROL text parser module]&quot; und eine E-Mail-Adresse enthalten. Weitere Informationen finden Sie in den folgenden Screenshots.

        Arbeitsblatt 1:

        ![](assets/worksheet-1-350x57.png)

        Arbeitsblatt 2:

        ![](assets/worksheet-2-350x41.png)

## Ressourcen

* [Kostenlose Übungen](https://regexone.com/) zum Erfahren von regulären Ausdrücken
* [Erfahren Sie mehr über die Telefonnummernübereinstimmung](https://regexone.com/problem/matching_phone_numbers) mit Regex
* [Informationen zur E-Mail-Übereinstimmung](https://regexone.com/problem/matching_emails) mit Regex
* [Testen Sie Ihre regulären Ausdrücke](https://regex101.com/)
