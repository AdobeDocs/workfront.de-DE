---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Datenspeicher in  [!DNL Adobe Workfront Fusion]
description: Ein Datenspeicher, der einer Datenbank oder einer einfachen Tabelle ähnelt, kann Daten aus Szenarien speichern und so die Übertragung von Daten zwischen einzelnen Szenarien oder Szenario-Läufen ermöglichen. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 00a969175626d27b70d516921097725fdf818799
workflow-type: tm+mt
source-wordcount: '1336'
ht-degree: 1%

---

# Datenspeicher in [!DNL Adobe Workfront Fusion]

Ein Datenspeicher, der einer Datenbank oder einer einfachen Tabelle ähnelt, kann Daten aus Szenarien speichern und so die Übertragung von Daten zwischen einzelnen Szenarien oder Szenario-Läufen ermöglichen. Sie können einen Datenspeicher verwenden, um während der Synchronisierung neue Daten aus verschiedenen Systemen zu speichern.

Mit den Datenspeichermodulen können Sie die folgenden Aktionen für Datensätze in Ihrem [!DNL Adobe Workfront Fusion] -Datenspeicher ausführen:

* Hinzufügen
* Ersetzen
* Aktualisieren
* Abrufen
* Löschen
* Suchen
* Anzahl

Informationen zur Verwendung von Datenspeichermodulen finden Sie unter [[!UICONTROL Datenspeicher] -Module](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

Eine Videoeinführung zu Datenspeichern in Workfront Fusion finden Sie unter:

* [Datenspeicher](https://video.tv.adobe.com/v/3427029/){target=_blank}

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

## Datenspeicherplatz verfügbar

<!--If your organization is on the new Workfront plan model (Select, Prime, and Ultimate packages), your total data store size is:-->

Wenn Ihr Unternehmen das neue Workfront-Planungsmodell verwendet (Select-, Prime- und Ultimate-Packages), wirkt sich der Plan Ihres Unternehmens auf die Größe und Anzahl der in Ihrer Fusion-Instanz verfügbaren Datenspeicher aus.

### Ultimate Plan

Fusionsinstanzen im Ultimate-Paket erhalten:

* 100 MB Speicherplatz
* 50 Datenspeicher

### Auswählen und Präsentieren von Plänen

Fusionsinstanzen in den Select- oder Prime-Paketen erhalten:—>

* 100 MB für die ersten 500.000 Operationen.

* 10 MB für jeden weiteren 100.000-Betrieb.

  Beispiel: Eine Organisation mit 600.000 Vorgängen erhält 110 MB.

Ihr Unternehmen kann über bis zu 50 Datenspeicher verfügen. Die kombinierte Größe dieser Datenspeicher darf die Gesamtdatenspeichergröße Ihres Unternehmens nicht überschreiten.

## Erstellen eines Datenspeichers in [!DNL Workfront Fusion]

* [Datenspeicher einrichten](#set-up-the-data-store)
* [Einrichten der Datenstruktur](#set-up-the-data-structure)

### Datenspeicher einrichten

Bevor Sie einen Datenspeicher in einem Modul verwenden können, müssen Sie den Datenspeicher in [!DNL Workfront Fusion] erstellen.

>[!NOTE]
>
>Ihre Organisation verfügt über eine begrenzte Anzahl verfügbarer Datenspeicher. Wenn Sie versuchen, mehr Datenspeicher als verfügbar zu erstellen, gibt [!DNL Workfront] den Fehler [!UICONTROL Maximale Speicherkapazität erreicht] zurück.
>
>Weitere Informationen finden Sie unter [Maximale Speicherkapazität erreicht Fehler](#maximum-stores-reached-error) in diesem Artikel.

1. Melden Sie sich bei Ihrem [!DNL Workfront Fusion] -Konto an.
1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Datenspeicher]** .
1. Klicken Sie oben rechts im Bildschirm auf **[!UICONTROL Datenspeicher hinzufügen]** .
1. Geben Sie Einstellungen für den neuen Datenspeicher ein.

   Ein fett hervorgehobener Titel auf einem Feld in einem [!DNL Workfront Fusion]-Modul zeigt eine erforderliche Einstellung an.

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
        <li> <p style="font-weight: bold;">Neue Datenstruktur hinzufügen</p> <p>Klicken Sie auf <strong>[!UICONTROL Add]</strong> , um eine neue Datenstruktur zu erstellen.</p> <p>Weitere Informationen finden Sie im Abschnitt <a href="#set-up-the-data-structure" class="MCXref xref">Einrichten der Datenstruktur</a> in diesem Artikel.</p> </li> 
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
1. Konfigurieren Sie im angezeigten Feld **[!UICONTROL Datenstruktur hinzufügen]** die folgenden Felder:

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
        <li> <p>Klicken Sie auf <strong>[!UICONTROL Element hinzufügen]</strong> , um die Eigenschaften einer Spalte manuell anzugeben.</p> <p>Geben Sie den <strong>[!UICONTROL Namen]</strong> und den <strong>[!UICONTROL Typ]</strong> für die Datenspeicherspalte ein und definieren Sie die entsprechenden Eigenschaften.</p> </li> 
        <li> <p>Klicken Sie auf <strong>[!UICONTROL Generator]</strong> , um die Spalten aus den von Ihnen angegebenen Beispieldaten zu bestimmen.</p> 
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
          <p>Anschließend können Sie dem Datenspeicher Werte manuell oder mithilfe der [!DNL Workfront Fusion] -Datenspeichermodule hinzufügen.</p> 
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

Sie können die Eigenschaften und Inhalte eines vorhandenen Datenspeichers im Bereich [!UICONTROL Datenspeicher] von [!DNL Workfront Fusion] bearbeiten.

* [Eigenschaften eines Datenspeichers bearbeiten](#edit-the-properties-of-a-data-store)
* [Inhalt eines Datenspeichers bearbeiten](#edit-the-contents-of-a-data-store)

### Eigenschaften eines Datenspeichers bearbeiten

Zu den Eigenschaften eines Datenspeichers gehören die vom Datenspeicher verwendete Datenstruktur sowie die Größe des Datenspeichers.

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Datenspeicher]** ![](assets/data-store-icon.png) , um den Bereich [!UICONTROL Datenspeicher] zu öffnen.
1. Klicken Sie neben dem zu bearbeitenden Datenspeicher auf **[!UICONTROL Bearbeiten]** ![](assets/data-store-edit.png) .
1. (Optional) Wenn Sie die von diesem Datenspeicher verwendete Datenstruktur in eine andere vorhandene Datenstruktur ändern möchten, wählen Sie sie aus der Dropdownliste **[!UICONTROL Datenstruktur]** aus.

   Oder

   (Optional) Wenn Sie die von diesem Datenspeicher verwendete Datenstruktur in eine völlig neue Datenstruktur ändern möchten, finden Sie weitere Informationen unter [Einrichten der Datenstruktur](#set-up-the-data-structure) in diesem Artikel.

1. (Optional) Ändern Sie die Größe des Datenspeichers, indem Sie die neue Größe in das Feld **[!UICONTROL Datenspeichergröße in MB]** eingeben.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

### Inhalt eines Datenspeichers bearbeiten

1. Klicken Sie im linken Navigationsbereich auf das Symbol **[!UICONTROL Datenspeicher]** ![](assets/data-store-icon.png) , um den Bereich [!UICONTROL Datenspeicher] zu öffnen.
1. Klicken Sie neben dem zu bearbeitenden Datenspeicher auf **[!UICONTROL Durchsuchen]** .
1. (Optional) Ordnen Sie die Spalten neu an, indem Sie sie an die gewünschte Position ziehen.
1. (Optional) [!UICONTROL Bearbeiten] Sie eine einzelne Zelle, indem Sie auf das Symbol **[!UICONTROL Bearbeiten]** in dieser Zelle klicken und dann den gewünschten Wert eingeben.
1. (Optional) Fügen Sie dem Datenspeicher ein neues Element hinzu, indem Sie auf **[!UICONTROL Hinzufügen]** klicken und dann die Informationen für das neue Element eingeben.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Fehlerbehebung

* [Wiederherstellen verlorener Daten aus einem Datenspeicher](#restoring-lost-data-from-a-data-store)
* [Fehler wegen Platzmangels](#out-of-space-error)
* [Fehler &quot;Maximale Speicheranzahl erreicht&quot;](#maximum-stores-reached-error)

### Wiederherstellen verlorener Daten aus einem Datenspeicher

Es gibt derzeit kein Tool, das die automatische Wiederherstellung verlorener Daten automatisieren kann.

#### Workaround

1. Überprüfen Sie alle Ausführungsprotokolle von Szenarien, in denen Elemente zum Datenspeicher eingefügt wurden.

   Weitere Informationen zum Überprüfen von Ausführungsprotokollen finden Sie unter [Ausführungsverlauf eines Szenarios anzeigen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Kopieren Sie die Daten.
1. Fügen Sie die Daten erneut in Ihren Datenspeicher ein.

   Informationen zum Einfügen von Daten in einen Datenspeicher finden Sie unter [Bearbeiten des Inhalts eines Datenspeichers](#edit-the-contents-of-a-data-store) in diesem Artikel.

### Fehler [!UICONTROL Nicht genügend Platz]

Ein Fehler vom Typ [!UICONTROL Nicht genügend Speicherplatz] tritt auf, da Ihren zuvor erstellten Datenspeichern bereits Ihr zugewiesener Datenspeicherspeicher zugewiesen wurde.

#### Workaround

1. Bearbeiten Sie einen Ihrer vorhandenen Datenspeicher, um weniger Speicherplatz zu verwenden. Dadurch wird Speicherplatz für Ihren neuen Datenspeicher freigesetzt.

   Weitere Informationen finden Sie unter [Eigenschaften eines Datenspeichers bearbeiten](#edit-the-properties-of-a-data-store) in diesem Artikel.

>[!NOTE]
>
>Es wird empfohlen, nicht den gesamten Speicherplatz einem Datenspeicher zuzuweisen, es sei denn, Sie sind sicher, dass Sie keine weiteren Datenspeicher benötigen.

### Fehler [!UICONTROL Maximale Anzahl der erreichten Stores]

Der Fehler [!UICONTROL Maximale Speichergröße erreicht] tritt auf, da Ihr Unternehmen alle verfügbaren Datenspeicher verwendet hat. Eine Organisation verfügt über eine Reihe verfügbarer Datenspeicher, die der doppelten Anzahl verfügbarer Szenarien entsprechen. Daher hängt die Gesamtzahl der verfügbaren Datenspeicher vom von Ihnen erworbenen Plan ab.

Wenn Ihr Unternehmen beispielsweise einen Plan mit 15 Szenarien erworben hat, kann das Unternehmen über bis zu 30 Datenspeicher verfügen.

#### Workaround

Um die Anzahl der vorhandenen Datenspeicher zu reduzieren, sollten Sie einen der folgenden Schritte ausführen:

* Kombinieren vorhandener Datenspeicher
* Nicht verwendete Datenspeicher löschen
