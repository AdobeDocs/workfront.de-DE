---
title: Anwenden von Filtern in erweiterten Analysen
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Mit den Filtern im erweiterten Analysebereich von Adobe Workfront können Sie sich auf bestimmte Projekte oder Datentypen konzentrieren.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1486'
ht-degree: 0%

---

# Anwenden von Filtern in erweiterten Analysen

<!-- Audited: 12/2023 -->

Mit den Filtern im erweiterten Analysebereich von Adobe Workfront können Sie sich auf bestimmte Projekte oder Datentypen konzentrieren. Die Filtertypen, die Sie verwenden, können Ihnen Einblicke geben in:

* Projekte in Ihrem Besitz
* Spezifische Portfolio- oder Programmansichten
* Wichtige Leistungsindikatoren für einen bestimmten Zeitraum (Woche, Quartal, Geschäftsjahr)

Sie können Filter nach Bedarf hinzufügen und entfernen. Workfront behält die Filter bei, die Sie anwenden, auch wenn Sie sich abmelden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>
      <p>Neu: Beliebig</p>
      <p>oder</p>
      <p>Aktuell: Unternehmen oder höher</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
      <p>Neu: Licht oder höher</p>
      <p>oder</p>
      <p>Aktuell: Überprüfung oder höher</p>
   </td> 
  </tr>
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> <p>Sie müssen auch Ansichtszugriff auf Aufgaben, Portfolios und Benutzende haben, um bestimmte Projektfeldfilteroptionen anzeigen zu können.</p> <p>Hinweis: Wenn im Abschnitt <strong>Zusätzliche Einschränkungen festlegen</strong> des Dialogfelds „Zugriffsebene bearbeiten“ Einschränkungen ausgewählt sind, werden möglicherweise nicht alle Informationen in den Filtern oder auf der Seite „Erweiterte Analyse“ angezeigt, nachdem der Filter angewendet wurde.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>Anzeigen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Voraussetzungen für die Verwendung der erweiterten Analyse finden Sie unter [Voraussetzungen](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) in [Übersicht über die erweiterte Analyse](../enhanced-analytics/enhanced-analytics-overview.md).

## Ändern des Filters für den Datumsbereich {#change-the-date-range-filter}

Standardmäßig zeigen die Visualisierungen im Bereich Erweiterte Analyse Daten der letzten 60 Tage und der nächsten 15 Tage an. Sie können einen neuen Datumsbereich auswählen und ihn auf alle Visualisierungen im erweiterten Analysebereich anwenden. Wenn Sie die Seite verlassen, wird der standardmäßige Datumsbereich angewendet, wenn Sie das nächste Mal zurücknavigieren.

>[!TIP]
>
>Sie können auch Tasten auf der Tastatur verwenden, um zu einem Datumsbereich im Kalender-Widget zu navigieren, ihn zu öffnen und ihn auszuwählen.\
>Weitere Informationen finden Sie im Abschnitt [Tastaturbefehle](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) im Artikel [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

Einen neuen Datumsbereich auswählen:

{{step1-to-analytics}}

1. Klicken Sie oben rechts auf das Datumsbereichsfeld, um die Kalenderansicht zu öffnen.
1. Verwenden Sie die Pfeile über dem Kalender, um den Monat Ihres Startdatums zu finden, und wählen Sie dann das Startdatum aus.

   ![Datumsbereich auswählen](assets/filters-select-date-range-350x344.png)

1. Verwenden Sie die Pfeile über dem Kalender, um den Monat Ihres Enddatums zu finden, und wählen Sie dann das Enddatum aus.
1. (Optional) Um einen kleineren Datumsbereich einzoomen, ziehen Sie die Maus von einem bestimmten Datum in eine andere Visualisierung.

   Alle Visualisierungen auf dem Bildschirm werden entsprechend dem ausgewählten Zeitrahmen aktualisiert, und neben allen vorhandenen Filtern wird ein Zeitrahmen-Filter angezeigt. Dieser Filter wird nicht beibehalten, wenn Sie sich abmelden oder den erweiterten Analysebereich verlassen.

   ![Zeitrahmen-Filter](assets/timeframe-filter-350x220.png)

## Filter hinzufügen

Sie können Filter hinzufügen, die auf standardmäßigen Projektfeldern, benutzerdefinierten Formularfeldern und den Projekten zugewiesenen Home-Teams basieren.

>[!TIP]
>
>Mit den Tasten auf der Tastatur können Sie auch zu navigieren und einen neuen Filter hinzufügen.\
>Weitere Informationen finden Sie im Abschnitt [Tastaturbefehle](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) im Artikel [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

* [Projektfeldfilter hinzufügen](#add-a-project-field-filter)
* [Hinzufügen eines benutzerdefinierten Projektformularfilters](#add-a-project-custom-form-filter)
* [Team-Filter hinzufügen](#add-a-team-filter)

### Hinzufügen eines Projektfeldfilters {#add-a-project-field-filter}

Mit Projektfeldfiltern können Sie Daten nach Projekten und Aufgaben anhand der Werte filtern, die in Felder eingegeben wurden, die standardmäßig in Projekten enthalten sind.

Die folgenden Projektfeldfiltertypen sind verfügbar:

| Feld | Angezeigte Daten |
|---|---|
| **Projekt** | Zeigt nur Daten für das/die ausgewählte(n) Projekt(e) an |
| **Programm** | Zeigt Daten nur für Projekte in den ausgewählten Programmen an |
| **Portfolio** | Zeigt Daten nur für Projekte in den ausgewählten Portfolios an |
| **Bedingung** | Zeigt Daten nur für Projekte an, die zuletzt die ausgewählte(n) Bedingung(en) hatten (zielgerichtet, gefährdet oder in Schwierigkeiten) |
| **Status** | Zeigt Daten nur für Projekte an, die zuletzt die ausgewählten Status hatten (abgeschlossen, aktuell, gehalten, abgebrochen usw.) |
| **Sponsor** | Zeigt Daten nur für Projekte mit dem/den ausgewählten Sponsor(n) an |
| **Projektbesitzer** | Zeigt Daten nur für Projekte mit dem/den ausgewählten Projektbesitzer(n) an |

Benutzerdefinierte Formularfilter funktionieren anders. Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Formularfilters](#add-a-project-custom-form-filter).

So fügen Sie einen Projektfeldfilter hinzu

{{step1-to-analytics}}

1. Klicken Sie oben links auf **Filter hinzufügen** und wählen Sie dann den gewünschten Filtertyp aus.

   >[!NOTE]
   >
   >Verschiedene Filtertypen zeigen unterschiedliche Daten an. In einem Filter kann nur ein Filtertyp verwendet werden. Nach der Auswahl steht ein Filtertyp nicht mehr zur Verwendung in einem anderen Projektfeldfilter zur Verfügung.

1. Suchen Sie die Werte, für die Sie Daten anzeigen möchten, indem Sie mindestens drei Textzeichen in das Feld **Suchen** eingeben und dann jeden Wert auswählen, den Sie in den Filter aufnehmen möchten.

   Um alle aktuellen Werte auszuwählen, klicken Sie auf **Alle auswählen**.

   ![Filterwert auswählen](assets/select-filter-value-350x251.png)

1. Klicken Sie nach Auswahl aller gewünschten Werte auf **Filter anwenden**.

   Die Projektanzahl oben rechts wird aktualisiert und zeigt Ihre angewendeten Filter an.

1. Wiederholen Sie diese Schritte für jeden Filter, den Sie hinzufügen möchten.

   Beim Hinzufügen von Filtern werden Daten in den Visualisierungen unten für bis zu 50 Projekte angezeigt.

   >[!TIP]
   >
   >Um Daten für mehr als die 50 standardmäßig angezeigten Projekte anzuzeigen, haben Sie folgende Möglichkeiten:
   >
   >   * Verwenden Sie die Pfeile unten links, um die nächsten 50 Projekte in dieser Visualisierung anzuzeigen.\
   >     ![Paginierungspfeil](assets/pagination-350x118.png)
   >   
   >   * Verwenden Sie das **Sortieren nach** Dropdown-Menü in einer Visualisierung, um die Projekte in einer anderen Reihenfolge anzuzeigen.\
   >     ![Nach Menü sortieren](assets/sort-by-menu-350x247.png)

   Informationen zum Anpassen des Datumsbereichs finden Sie unter [Ändern des Datumsbereichsfilters](#change-the-date-range-filter).

### Hinzufügen eines benutzerdefinierten Projektformularfilters

Mit dem Filtertyp für benutzerdefinierte Formulare können Sie Daten für Projekte und Aufgaben basierend auf den Werten filtern, die in benutzerdefinierte Formularfelder in Projekte eingegeben wurden. Im Gegensatz zu anderen erweiterten Analytics-Filtertypen können Sie mehr als einen benutzerdefinierten Formularfilter hinzufügen. Jeder benutzerdefinierte Formularfilter enthält Werte, die nur innerhalb des ausgewählten Felds in einem bestimmten benutzerdefinierten Formular eingegeben werden.

So fügen Sie einen benutzerdefinierten Formularfilter hinzu:

{{step1-to-analytics}}

1. Klicken Sie oben links im Bildschirm auf **Filter hinzufügen** und wählen Sie dann **Benutzerdefiniertes Formular** aus.

   ![Benutzerdefinierten Formularfilter auswählen](assets/select-custom-form-filter-350x271.png)

1. Suchen Sie das gewünschte benutzerdefinierte Formular, indem Sie mindestens drei Textzeichen in das Feld **Suche** eingeben und dann das benutzerdefinierte Formular auswählen.
1. Wählen Sie das gewünschte Feld aus und führen Sie dann eine der folgenden Aktionen je nach dem Feldtyp aus, den Sie dem Filter hinzufügen:

   >[!NOTE]
   >
   >Nicht alle benutzerdefinierten Formularfeldtypen können einem Filter hinzugefügt werden. Derzeit unterstützt Enhanced Analytics nur die unten aufgeführten Feldtypen.

   * **Kontrollkästchen**, **Dropdown** oder **Optionsfeld**: Wählen Sie jeden Wert in dem Feld aus, das Sie in Ihren Filter einbeziehen möchten, oder klicken Sie auf das Kontrollkästchen **Alle auswählen**.\
     ![Kontrollkästchenwerte](assets/custom-form-filter-checkbox-350x255.png)

   * **Datum**: Navigieren Sie mit den Pfeilen zu einem bestimmten Monat und wählen Sie dann das Datum in dem Feld aus, das Sie in Ihren Filter aufnehmen möchten.\
     ![Datumswert](assets/custom-form-filter-date-350x348.png)

   * **Text**: Geben Sie den Text in dem Feld ein, das Sie in Ihren Filter aufnehmen möchten.\
     ![Textwert](assets/custom-form-filter-text-350x90.png)

   * **Zahl**: Geben Sie die Zahl in dem Feld ein, das Sie in Ihren Filter aufnehmen möchten.\
     ![Zahlenwert](assets/custom-form-filter-number-350x93.png)

1. Nachdem Sie die Werte eingegeben oder ausgewählt haben, nach denen Sie filtern möchten, klicken Sie auf **Filter anwenden**.

   Die Projektanzahl oben rechts wird aktualisiert und zeigt Ihre angewendeten Filter an.

1. Wiederholen Sie diese Schritte für jeden Filter, den Sie hinzufügen möchten.

   Beim Hinzufügen von Filtern werden Daten in den Visualisierungen unten für bis zu 50 Projekte angezeigt.

   >[!TIP]
   >
   >Um Daten für mehr als die 50 standardmäßig angezeigten Projekte anzuzeigen, haben Sie folgende Möglichkeiten:
   >  
   >   * Verwenden Sie die Pfeile unten links, um die nächsten 50 Projekte in dieser Visualisierung anzuzeigen.\
   >     ![Paginierungspfeile](assets/pagination-350x118.png)
   >   
   >   * Verwenden Sie das **Sortieren nach** Dropdown-Menü in einer Visualisierung, um die Projekte in einer anderen Reihenfolge anzuzeigen.\
   >     ![Nach Menü sortieren](assets/sort-by-menu-350x247.png)

   Informationen zum Anpassen des Datumsbereichs finden Sie unter [Ändern des Datumsbereichsfilters](#change-the-date-range-filter).

### Team-Filter hinzufügen {#add-a-team-filter}

{{step1-to-analytics}}

1. Klicken Sie im linken Bedienfeld auf **Personen**.

   ![Personen auswählen](assets/people-area-cropped-qs-350x276.png)

1. Klicken Sie oben links im Bildschirm auf **Filter hinzufügen** und wählen Sie dann den Filter **Team** aus.
1. Suchen Sie die Teams, für die Sie Daten anzeigen möchten, indem Sie mindestens drei Textzeichen in das Feld **Suchen** eingeben und dann jedes Team auswählen, das Sie in den Filter aufnehmen möchten. Um alle Teams auszuwählen, klicken Sie auf **Alle auswählen**.

   ![Teams auswählen](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Alle Teams sind als Filteroptionen enthalten, unabhängig von Ihrer Zugriffsebene.

1. Klicken Sie nach Auswahl aller gewünschten Teams auf **Filter anwenden**.

   Beim Hinzufügen von Filtern werden Daten in den folgenden Visualisierungen angezeigt.

   Informationen zum Anpassen des Datumsbereichs finden Sie unter [Ändern des Datumsbereichsfilters](#change-the-date-range-filter).

## Filter entfernen

Sie können einen Filter jederzeit entfernen. Wenn Sie einen Filter entfernen, wird er beim nächsten Besuch des Bereichs Erweiterte Analyse nicht angezeigt.

>[!TIP]
>
>Sie können auch Tasten auf der Tastatur verwenden, um zu einem vorhandenen Filter zu navigieren und ihn zu entfernen.\
>Weitere Informationen finden Sie im Abschnitt [Tastaturbefehle](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) im Artikel [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

So entfernen Sie einen Filter:

{{step1-to-analytics}}

1. Wenn Sie ein Projektfeld oder einen benutzerdefinierten Formularfilter entfernen möchten, verbleiben Sie im Bereich **Arbeit**.

   Oder

   Wenn Sie einen Team-Filter entfernen möchten, wählen Sie **linken Bereich** Personen“ aus.

1. Suchen Sie den gewünschten Filter und klicken Sie auf das **X**, um ihn zu entfernen.

   ![Entfernen](assets/remove-filter-350x213.png)

   Der Filter ist nicht mehr aktiv und wird nur angezeigt, wenn Sie ihn erneut hinzufügen.
