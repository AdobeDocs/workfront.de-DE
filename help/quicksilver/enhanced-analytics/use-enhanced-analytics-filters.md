---
title: Filter in erweiterten Analysen anwenden
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Filter im Bereich "Erweiterte Analyse"von Adobe Workfront helfen Ihnen dabei, sich auf bestimmte Projekte oder bestimmte Datentypen zu konzentrieren.
author: Nolan
feature: Reports and Dashboards
exl-id: 25854c04-d914-4302-a36b-e8134637efe1
source-git-commit: 4ade799ff735183f83f045e7eaa876961d266208
workflow-type: tm+mt
source-wordcount: '1508'
ht-degree: 0%

---

# Filter in erweiterten Analysen anwenden

Die Filter im Bereich &quot;Erweiterte Analyse&quot;von Adobe Workfront helfen Ihnen dabei, sich auf bestimmte Projekte oder bestimmte Datentypen zu konzentrieren. Die von Ihnen verwendeten Filtertypen bieten Einblicke in:

* Projekte, die Ihnen gehören
* Spezifische Portfolio- oder Programmansichten
* Wichtige Leistungsindikatoren für einen bestimmten Zeitraum (Woche, Quartal, Geschäftsjahr)

Sie können Filter nach Bedarf hinzufügen und entfernen. Workfront behält die angewendeten Filter bei, selbst wenn Sie sich abmelden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <caption style="text-align: left;">
  *Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.
 </caption> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>
      <p>Neuer Plan: Beliebig</p>
      <p>oder</p>
      <p>Aktueller Plan: Business oder höher</p></td> 
  </tr>
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>
      <p>Neuer Plan: leicht oder höher</p>
      <p>oder</p>
      <p>Aktueller Plan: Überprüfung oder höher</p>
   </td> 
  </tr>
  <tr> 
   <td><b>Zugriffsstufe*</b> </td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> <p>Sie müssen außerdem Zugriff auf "Anzeigen"auf Aufgaben, Portfolios und Benutzer haben, um bestimmte Filteroptionen für Projektfelder anzuzeigen.</p> <p>Hinweis: Wenn Einschränkungen im Abschnitt Zusätzliche Einschränkungen festlegen des Dialogfelds Zugriffsebene bearbeiten ausgewählt sind, werden möglicherweise nicht alle Informationen in den Filtern oder auf der Seite Erweiterte Analyse angezeigt, nachdem der Filter angewendet wurde. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><b>Objektberechtigungen</b> </p> </td> 
   <td> <p>Anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzungen

Voraussetzungen für die Verwendung von Enhanced Analytics finden Sie unter [Voraussetzungen](../enhanced-analytics/enhanced-analytics-overview.md#prerequisites) in [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Datumsbereichfilter ändern {#change-the-date-range-filter}

Standardmäßig zeigen die Visualisierungen im Bereich &quot;Erweiterte Analyse&quot;Daten für die letzten 60 Tage und die nächsten 15 Tage an. Sie können einen neuen Datumsbereich auswählen und ihn auf alle Visualisierungen im Bereich &quot;Erweiterte Analyse&quot;anwenden. Wenn Sie von der Seite weg navigieren, wird der Standarddatumsbereich beim nächsten Navigieren angewendet.

>[!TIP]
>
>Sie können auch über die Tastatur einen Datumsbereich aus dem Kalender-Widget öffnen, öffnen und auswählen.\
>Weitere Informationen finden Sie unter [Tastaturbefehle](../enhanced-analytics/enhanced-analytics-overview.md#keyboard-shortcuts) im Artikel [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

So wählen Sie einen neuen Datumsbereich aus:

{{step1-to-analytics}}

1. Klicken Sie oben rechts auf das Datumsbereichsfeld, um die Kalenderansicht zu öffnen.
1. Verwenden Sie die Pfeile oberhalb des Kalenders, um den Monat Ihres Startdatums zu suchen, und wählen Sie dann das Startdatum aus.

   ![Datumsbereich auswählen](assets/filters-select-date-range-350x344.png)

1. Verwenden Sie die Pfeile über dem Kalender, um den Monat Ihres Enddatums zu suchen, und wählen Sie dann das Enddatum aus.
1. (Optional) Wenn Sie einen kleineren Datumsbereich vergrößern möchten, ziehen Sie die Maus über eine der Visualisierungen von einem bestimmten Datum zum nächsten.

   Alle Visualisierungen auf dem Bildschirm werden entsprechend dem ausgewählten Zeitrahmen aktualisiert. Neben allen vorhandenen Filtern wird ein Timeframe-Filter angezeigt. Dieser Filter wird nicht beibehalten, wenn Sie sich abmelden oder aus dem Bereich &quot;Erweiterte Analyse&quot;navigieren.

   ![Zeitrahmen-Filter](assets/timeframe-filter-350x220.png)

## Filter hinzufügen

Sie können Filter hinzufügen, die auf Standardprojektfeldern, benutzerdefinierten Formularfeldern und den für Projekte zugewiesenen Startseiten basieren.

>[!TIP]
>
>Sie können auch die Tastaturbefehle verwenden, um zu einem neuen Filter zu navigieren und ihn hinzuzufügen.\
>Weitere Informationen finden Sie unter [Tastaturbefehle](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) im Artikel [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

* [Hinzufügen eines Projektfeldfilters](#add-a-project-field-filter)
* [Hinzufügen eines benutzerdefinierten Formularfilters für ein Projekt](#add-a-project-custom-form-filter)
* [Team-Filter hinzufügen](#add-a-team-filter)

### Hinzufügen eines Projektfeldfilters {#add-a-project-field-filter}

Mit Projektfeldfiltern können Sie Daten nach Projekten und Aufgaben anhand der in Feldern eingegebenen Werte filtern, die standardmäßig in Projekten enthalten sind.

Die folgenden Projektfeldfiltertypen sind verfügbar:

| Feld | Angezeigte Daten |
|---|---|
| **Projekt** | Zeigt nur Daten für die ausgewählten Projekte an |
| **Programm** | Zeigt nur Daten für Projekte in den ausgewählten Programmen an |
| **Portfolio** | Zeigt Daten nur für Projekte in den ausgewählten Portfolios an |
| **Bedingung** | Zeigt Daten nur für Projekte an, bei denen die ausgewählte(n) Bedingung(en) zuletzt ausgewählt wurde(n) (Zielgruppe/n, Risiko/Probleme) |
| **Status** | Zeigt nur Daten zu Projekten an, die zuletzt den ausgewählten Status hatten (vollständig, aktuell, auf Abruf, abgebrochen usw.) |
| **Sponsor** | Zeigt nur Daten für Projekte mit den ausgewählten Sponsoren an |
| **Projektinhaber** | Zeigt Daten nur für Projekte mit den ausgewählten Projekteigentümern an |

Benutzerdefinierte Formularfilter funktionieren anders. Weitere Informationen finden Sie unter [Hinzufügen eines benutzerdefinierten Formularfilters für ein Projekt](#add-a-project-custom-form-filter).

So fügen Sie einen Projektfeldfilter hinzu:

{{step1-to-analytics}}

1. Klicken Sie oben links auf **Filter hinzufügen** und wählen Sie dann den gewünschten Filtertyp aus.

   >[!NOTE]
   >
   >Verschiedene Filtertypen zeigen unterschiedliche Daten an. Sie können nur einen Filtertyp in einem Filter verwenden. Nach der Auswahl ist kein Filtertyp verfügbar, der in einem anderen Projektfeldfilter verwendet werden kann.

1. Suchen Sie die Werte, für die die Daten angezeigt werden sollen, indem Sie mindestens drei Zeichen Text in die **Suche** und wählen Sie dann jeden Wert aus, den Sie in den Filter aufnehmen möchten.

   Um alle aktuellen Werte auszuwählen, klicken Sie auf **Alle auswählen**.

   ![Filterwert auswählen](assets/select-filter-value-350x251.png)

1. Klicken Sie nach Auswahl aller gewünschten Werte auf **Filter anwenden**.

   Die Projektzahl wird oben rechts aktualisiert, um Ihre angewendeten Filter widerzuspiegeln.

1. Wiederholen Sie diese Schritte für jeden Filter, den Sie hinzufügen möchten.

   Beim Hinzufügen von Filtern werden Daten in den unten stehenden Visualisierungen für bis zu 50 Projekte angezeigt.

   >[!TIP]
   >
   >Um Daten für mehr als die 50 standardmäßig angezeigten Projekte anzuzeigen, können Sie:
   >
   >   * Verwenden Sie die Pfeile unten links, um die nächsten 50 Projekte in dieser Visualisierung anzuzeigen.\
   >     ![Paginierungspfeil](assets/pagination-350x118.png)
   >   
   >   * Verwenden Sie die **Sortieren nach** Dropdown-Menü auf einer Visualisierung, um die Projekte in einer anderen Reihenfolge anzuzeigen.\
   >     ![Nach Menü sortieren](assets/sort-by-menu-350x247.png)

   Informationen zum Anpassen des Datumsbereichs finden Sie unter [Datumsbereichfilter ändern](#change-the-date-range-filter).

### Hinzufügen eines benutzerdefinierten Formularfilters für ein Projekt

Mit dem benutzerdefinierten Formularfiltertyp können Sie Daten nach Projekten und Aufgaben anhand der in benutzerdefinierten Formularfeldern in Projekten eingegebenen Werte filtern. Im Gegensatz zu anderen erweiterten Analytics-Filtertypen können Sie mehr als einen benutzerdefinierten Formularfilter hinzufügen. Jeder benutzerdefinierte Formularfilter enthält Werte, die nur in das ausgewählte Feld eines bestimmten benutzerdefinierten Formulars eingegeben werden.

Hinzufügen eines benutzerdefinierten Formularfilters:

{{step1-to-analytics}}

1. Klicken Sie in der linken oberen Ecke des Bildschirms auf **Filter hinzufügen**, wählen Sie **Benutzerdefiniertes Formular**.

   ![Benutzerdefinierter Formularfilter auswählen](assets/select-custom-form-filter-350x271.png)

1. Suchen Sie das gewünschte benutzerdefinierte Formular, indem Sie mindestens drei Textzeichen in die **Suche** und wählen Sie dann das benutzerdefinierte Formular aus.
1. Wählen Sie das gewünschte Feld aus und führen Sie je nach dem Typ des Felds, das Sie zum Filter hinzufügen, eine der folgenden Aktionen aus:

   >[!NOTE]
   >
   >Es können nicht alle benutzerdefinierten Corm-Feldtypen zu einem Filter hinzugefügt werden. Derzeit unterstützt Enhanced Analytics nur die unten aufgeführten Feldtypen.

   * **Kontrollkästchen**, **Dropdown** oder **Optionsfeld**: Wählen Sie jeden Wert im Feld aus, das Sie in Ihren Filter aufnehmen möchten, oder klicken Sie auf die Schaltfläche **Alle auswählen** aktivieren.\
     ![Kontrollkästchenwerte](assets/custom-form-filter-checkbox-350x255.png)

   * **Datum**: Navigieren Sie mit den Pfeilen zu einem bestimmten Monat und wählen Sie dann das Datum im Feld aus, das Sie in den Filter aufnehmen möchten.\
     ![Datumswert](assets/custom-form-filter-date-350x348.png)

   * **Text**: Geben Sie den Text in das Feld ein, das Sie in Ihren Filter aufnehmen möchten.\
     ![Textwert](assets/custom-form-filter-text-350x90.png)

   * **Zahl**: Geben Sie die Zahl in das Feld ein, das Sie in Ihren Filter aufnehmen möchten.\
     ![Zahlenwert](assets/custom-form-filter-number-350x93.png)

1. Klicken Sie nach Eingabe oder Auswahl der Werte, nach denen Sie filtern möchten, auf **Filter anwenden**.

   Die Projektzahl wird oben rechts aktualisiert, um Ihre angewendeten Filter widerzuspiegeln.

1. Wiederholen Sie diese Schritte für jeden Filter, den Sie hinzufügen möchten.

   Beim Hinzufügen von Filtern werden Daten in den unten stehenden Visualisierungen für bis zu 50 Projekte angezeigt.

   >[!TIP]
   >
   >Um Daten für mehr als die 50 standardmäßig angezeigten Projekte anzuzeigen, können Sie:
   >  
   >   * Verwenden Sie die Pfeile unten links, um die nächsten 50 Projekte in dieser Visualisierung anzuzeigen.\
   >     ![Paginierungspfeile](assets/pagination-350x118.png)
   >   
   >   * Verwenden Sie die **Sortieren nach** Dropdown-Menü auf einer Visualisierung, um die Projekte in einer anderen Reihenfolge anzuzeigen.\
   >     ![Nach Menü sortieren](assets/sort-by-menu-350x247.png)

   Informationen zum Anpassen des Datumsbereichs finden Sie unter [Datumsbereichfilter ändern](#change-the-date-range-filter).

### Team-Filter hinzufügen {#add-a-team-filter}

{{step1-to-analytics}}

1. Klicken Sie im linken Bereich auf **Personen**.

   ![Personen auswählen](assets/people-area-cropped-qs-350x276.png)

1. Klicken Sie oben links im Bildschirm auf **Filter hinzufügen** und wählen Sie dann die **Team** Filter.
1. Suchen Sie die Teams, für die Sie Daten anzeigen möchten, indem Sie mindestens drei Zeichen Text in die **Suche** und wählen Sie dann jedes Team aus, das Sie in den Filter aufnehmen möchten. Um alle Teams auszuwählen, klicken Sie auf **Alle auswählen**.

   ![Teams auswählen](assets/select-team-value-350x253.png)

   >[!NOTE]
   >
   >Alle Teams sind unabhängig von Ihrer Zugriffsstufe als Filteroptionen enthalten.

1. Klicken Sie nach Auswahl aller gewünschten Teams auf **Filter anwenden**.

   Beim Hinzufügen von Filtern werden die Daten in den unten stehenden Visualisierungen angezeigt.

   Informationen zum Anpassen des Datumsbereichs finden Sie unter [Datumsbereichfilter ändern](#change-the-date-range-filter).

## Filter entfernen

Sie können Filter jederzeit entfernen. Wenn Sie einen Filter entfernen, wird er beim nächsten Besuch des Bereichs &quot;Erweiterte Analyse&quot;nicht angezeigt.

>[!TIP]
>
>Sie können auch Tastaturbefehle verwenden, um zu einem vorhandenen Filter zu navigieren und ihn zu entfernen.\
>Weitere Informationen finden Sie unter [Tastaturbefehle](../enhanced-analytics/enhanced-analytics-overview.md#keyboard) im Artikel [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

So entfernen Sie einen Filter:

{{step1-to-analytics}}

1. Wenn Sie ein Projektfeld oder einen benutzerdefinierten Formularfilter entfernen möchten, verbleiben Sie im **Arbeit** Bereich.

   Oder

   Wenn Sie einen Team-Filter entfernen möchten, wählen Sie **Personen** im linken Bereich.

1. Suchen Sie den gewünschten Filter und klicken Sie auf die **X** , um es zu entfernen.

   ![Entfernen](assets/remove-filter-350x213.png)

   Der Filter ist nicht mehr aktiv und wird nur angezeigt, wenn Sie ihn erneut hinzufügen.
