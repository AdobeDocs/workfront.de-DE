---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Datenspeicher in [!DNL Adobe Workfront Fusion]
description: Ein Datenspeicher, der einer Datenbank oder einer einfachen Tabelle ähnelt, kann Daten aus Szenarien speichern und so die Übertragung von Daten zwischen einzelnen Szenarien oder Szenario-Läufen ermöglichen. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 85e5483b7ee1433d0b1efbaa37c6d55c7c1d5bf7
workflow-type: tm+mt
source-wordcount: '1268'
ht-degree: 1%

---

# Datenspeicher in [!DNL Adobe Workfront Fusion]

Ein Datenspeicher, der einer Datenbank oder einer einfachen Tabelle ähnelt, kann Daten aus Szenarien speichern und so die Übertragung von Daten zwischen einzelnen Szenarien oder Szenario-Läufen ermöglichen. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.

Mit den Datenspeichermodulen können Sie die folgenden Aktionen für Datensätze in Ihren [!DNL Adobe Workfront Fusion] Datenspeicher:

* Hinzufügen
* Ersetzen
* Aktualisieren
* Abrufen
* Löschen
* Suchen
* Anzahl

Informationen zur Verwendung von Datenspeichermodulen finden Sie unter [[!UICONTROL Datenspeicher] Module](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

Eine Videoeinführung zu Datenspeichern in Workfront Fusion finden Sie unter:

* [Datenspeicher](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Erstellen Sie einen Datenspeicher in [!DNL Workfront Fusion]

* [Datenspeicher einrichten](#set-up-the-data-store)
* [Einrichten der Datenstruktur](#set-up-the-data-structure)

### Datenspeicher einrichten

Bevor Sie einen Datenspeicher in einem Modul verwenden können, müssen Sie den Datenspeicher in [!DNL Workfront Fusion].

>[!NOTE]
>
>Ihre Organisation verfügt über eine begrenzte Anzahl verfügbarer Datenspeicher. Wenn Sie versuchen, mehr Datenspeicher zu erstellen, als verfügbar sind, [!DNL Workfront] gibt eine [!UICONTROL Maximale Anzahl der erreichten Filialen] Fehler.
>
>Weitere Informationen finden Sie unter [Fehler &quot;Maximale Speicheranzahl erreicht&quot;](#maximum-stores-reached-error) in diesem Artikel.

1. Melden Sie sich bei Ihrer [!DNL Workfront Fusion] -Konto.
1. Klicks **[!UICONTROL Datenspeicher]** im linken Navigationsbereich.
1. Klicks **[!UICONTROL Datenspeicher hinzufügen]** in der oberen rechten Ecke des Bildschirms.
1. Geben Sie Einstellungen für den neuen Datenspeicher ein.

   Ein fett hervorgehobener Titel auf einem Feld in einem [!DNL Workfront Fusion] -Modul gibt eine erforderliche Einstellung an.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data store name] </td> 
      <td> <p>Geben Sie einen Namen für den Datenspeicher ein. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Datenstruktur]</p> </td> 
      <td> <p>Eine Datenstruktur ist eine Liste der Spalten für eine Tabelle. Diese Liste zeigt den Spaltennamen und den Datentyp an.</p> <p>Führen Sie einen der folgenden Schritte aus:</p> 
       <ul> 
        <li style="font-weight: bold;">Wählen Sie eine bereits erstellte Datenstruktur aus.</li> 
        <li> <p style="font-weight: bold;">Neue Datenstruktur hinzufügen</p> <p>Klicks <strong>[!UICONTROL Hinzufügen]</strong> , um eine neue Datenstruktur zu erstellen.</p> <p>Weitere Informationen finden Sie unter <a href="#set-up-the-data-structure" class="MCXref xref">Einrichten der Datenstruktur</a> in diesem Artikel beschrieben.</p> </li> 
        <li style="font-weight: bold;"> <p>Lassen Sie das Feld leer</p> <p style="font-weight: normal;">Wenn Sie keine Datenstruktur auswählen oder hinzufügen, enthält die Datenbank nur den Primärschlüssel. Ein solcher Datenbanktyp ist nützlich, wenn Sie nur Schlüssel speichern möchten und nur wissen möchten, ob ein bestimmter Schlüssel in der Datenbank vorhanden ist oder nicht.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Datenspeichergröße in MB]</p> </td> 
      <td> <p>Weisen Sie die Größe für den Datenspeicher aus Ihrem gesamten internen Datenspeicher zu.</p> <p> Der Standardwert ist 10 MB. Wenn Sie weniger als 10 MB nicht zugewiesenen Datenspeicherplatz aus Ihrer 95-MB-Zuweisung haben, ist die Standardgröße die Menge an nicht zugewiesenem Speicher.  <p>Hinweis: Der reservierte Betrag kann jederzeit geändert werden.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Einrichten der Datenstruktur

1. Klicken Sie beim Erstellen oder Bearbeiten eines Datenspeichers auf **[!UICONTROL Hinzufügen]**.
1. Im **[!UICONTROL Datenstruktur hinzufügen]** konfigurieren Sie die folgenden Felder, die angezeigt werden:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data structure name]</td> 
      <td> <p> Geben Sie einen Namen für die neue Datenstruktur ein.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Spezifikation]</p> </td> 
      <td> <p>Führen Sie einen der folgenden Schritte aus, um die Spalten Ihres Datenspeichers einzurichten.</p> 
       <ul> 
        <li> <p>Klicks <strong>[!UICONTROL Element hinzufügen]</strong> um die Eigenschaften einer Spalte manuell anzugeben.</p> <p>Geben Sie die <strong>[!UICONTROL Name]</strong> und <strong>[!UICONTROL Typ]</strong> für die Datenspeicherspalte erstellen und entsprechende Eigenschaften definieren.</p> </li> 
        <li> <p>Klicks <strong>[!UICONTROL Generator]</strong> , um die Spalten aus den von Ihnen angegebenen Beispieldaten zu bestimmen.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Beispiel: </b></span></span> 
          <p>Beispielsweise werden mit den folgenden JSON-Beispieldaten drei Spalten erstellt: Name, Alter und Telefonnummer. Die Telefonnummer ist eine Sammlung von Mobiltelefon- und Festnetztelefonnummern.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>Die leeren Spalten in der Datenspeicheransicht:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>Anschließend können Sie Werte manuell oder mithilfe der Variablen [!DNL Workfront Fusion] Datenspeichermodule.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Streng] </td> 
      <td> <p>Aktivieren Sie diese Option, um sicherzustellen, dass die Payload mit den Datenstrukturen übereinstimmt. Nutzlasten, die zusätzliche Elemente enthalten, die nicht in der Datenstruktur angegeben sind, werden abgelehnt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Vorhandenen Datenspeicher bearbeiten

Sie können die Eigenschaften und Inhalte eines vorhandenen Datenspeichers im [!UICONTROL Datenspeicher] Gebiet von [!DNL Workfront Fusion].

* [Eigenschaften eines Datenspeichers bearbeiten](#edit-the-properties-of-a-data-store)
* [Inhalt eines Datenspeichers bearbeiten](#edit-the-contents-of-a-data-store)

### Eigenschaften eines Datenspeichers bearbeiten

Zu den Eigenschaften eines Datenspeichers gehören die vom Datenspeicher verwendete Datenstruktur sowie die Größe des Datenspeichers.

1. Klicks **[!UICONTROL Datenspeicher]** ![](assets/data-store-icon.png) im linken Navigationsbereich, um die [!UICONTROL Datenspeicher] Bereich.
1. Klicks **[!UICONTROL Bearbeiten]** ![](assets/data-store-edit.png) neben dem Datenspeicher, den Sie bearbeiten möchten.
1. (Optional) Wenn Sie die von diesem Datenspeicher verwendete Datenstruktur in eine andere vorhandene Datenstruktur ändern möchten, wählen Sie sie aus dem **[!UICONTROL Datenstruktur]** angezeigt.

   Oder

   (Optional) Wenn Sie die von diesem Datenspeicher verwendete Datenstruktur in eine völlig neue Datenstruktur ändern möchten, lesen Sie [Einrichten der Datenstruktur](#set-up-the-data-structure) in diesem Artikel.

1. (Optional) Ändern Sie die Größe des Datenspeichers, indem Sie die neue Größe in die **[!UICONTROL Datenspeichergröße in MB]** -Feld.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

### Inhalt eines Datenspeichers bearbeiten

1. Klicken Sie auf **[!UICONTROL Datenspeicher]** icon ![](assets/data-store-icon.png) im linken Navigationsbereich, um die [!UICONTROL Datenspeicher] Bereich.
1. Klicks **[!UICONTROL Durchsuchen]**  neben dem Datenspeicher, den Sie bearbeiten möchten.
1. (Optional) Ordnen Sie die Spalten neu an, indem Sie sie an die gewünschte Position ziehen.
1. (Optional) [!UICONTROL Bearbeiten] durch Klicken auf die **[!UICONTROL Bearbeiten]** -Symbol in dieser Zelle und geben Sie dann den gewünschten Wert ein.
1. (Optional) Fügen Sie dem Datenspeicher ein neues Element hinzu, indem Sie auf **[!UICONTROL Hinzufügen]** und geben Sie dann die Informationen für das neue Element ein.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Fehlerbehebung

* [Wiederherstellen verlorener Daten aus einem Datenspeicher](#restoring-lost-data-from-a-data-store)
* [Fehler wegen Platzmangels](#out-of-space-error)
* [Fehler &quot;Maximale Speicheranzahl erreicht&quot;](#maximum-stores-reached-error)

### Wiederherstellen verlorener Daten aus einem Datenspeicher

Es gibt derzeit kein Tool, das die automatische Wiederherstellung verlorener Daten automatisieren kann.

#### Workaround

1. Überprüfen Sie alle Ausführungsprotokolle von Szenarien, in denen Elemente zum Datenspeicher eingefügt wurden.

   Weitere Informationen zur Prüfung von Ausführungsprotokollen finden Sie unter [Anzeigen des Ausführungsverlaufs eines Szenarios im [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Kopieren Sie die Daten.
1. Fügen Sie die Daten erneut in Ihren Datenspeicher ein.

   Informationen zum Einfügen von Daten in einen Datenspeicher finden Sie unter [Inhalt eines Datenspeichers bearbeiten](#edit-the-contents-of-a-data-store) in diesem Artikel.

### [!UICONTROL Außerhalb des Platzes] error

Ein [!UICONTROL Nicht genügend Platz] tritt auf, da Ihren zuvor erstellten Datenspeichern bereits Ihr zugewiesener Datenspeicher zugewiesen wurde.

#### Workaround

1. Bearbeiten Sie einen Ihrer vorhandenen Datenspeicher, um weniger Speicherplatz zu verwenden. Dadurch wird Speicherplatz für Ihren neuen Datenspeicher freigesetzt.

   Weitere Informationen finden Sie unter [Eigenschaften eines Datenspeichers bearbeiten](#edit-the-properties-of-a-data-store) in diesem Artikel.

>[!NOTE]
>
>Es wird empfohlen, nicht den gesamten Speicherplatz einem Datenspeicher zuzuweisen, es sei denn, Sie sind sicher, dass Sie keine weiteren Datenspeicher benötigen.

### [!UICONTROL Maximale Anzahl der erreichten Filialen] error

A [!UICONTROL Maximale Anzahl der erreichten Filialen] Fehler tritt auf, da Ihr Unternehmen alle verfügbaren Datenspeicher verwendet hat. Eine Organisation verfügt über eine Reihe verfügbarer Datenspeicher, die der doppelten Anzahl verfügbarer Szenarien entsprechen. Daher hängt die Gesamtzahl der verfügbaren Datenspeicher vom von Ihnen erworbenen Plan ab.

Wenn Ihr Unternehmen beispielsweise einen Plan mit 15 Szenarien erworben hat, kann das Unternehmen über bis zu 30 Datenspeicher verfügen.

#### Workaround

Um die Anzahl der vorhandenen Datenspeicher zu reduzieren, sollten Sie einen der folgenden Schritte ausführen:

* Kombinieren vorhandener Datenspeicher
* Nicht verwendete Datenspeicher löschen
