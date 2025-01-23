---
content-type: release-notes
title: Adobe Workfront - Planungsversionstätigkeit für die Version 25.1
description: Dies ist die Veröffentlichungsaktivität für das Adobe Workfront Planning-Produkt für das erste Quartal 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: a6104204cae2a2d8fb021da254437008d55a43b6
workflow-type: tm+mt
source-wordcount: '2112'
ht-degree: 0%

---

# Versionsaktivität für Adobe Workfront Planning im ersten Quartal 2025

In diesem Artikel werden die Funktionen beschrieben, die in der ersten Version des Quartals 2025 für Workfront Planning veröffentlicht werden.

<!--keep the sentence below for all future quarterly release pages-->

Eine Liste aller für Adobe Workfront Planning veröffentlichten Funktionen finden Sie unter [Adobe Workfront Planning Release-Aktivität: Artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Verbindungsfelder mit Adobe Experience Manager-Assets werden jetzt in Anfrageformularen unterstützt

>[!NOTE]
>
>Vorschau-Version: 20. Dezember 2024; Produktionsversion für alle Kunden: 16. Januar 2025

In Workfront Planning können Sie jetzt Verbindungsfelder mit AEM-Assets zu einem Datensatztyp-Anfrageformular hinzufügen.

Vor dieser Verbesserung konnten diese Feldtypen nicht zu Anfrageformularen hinzugefügt werden.

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Konfigurieren von Validierungen für Workfront-Planungsanfragen

>[!NOTE]
>
>Vorschau-Version: 16. Dezember 2024; Produktionsversion für alle Kunden: 16. Januar 2025

Jetzt können Sie einem Workfront Planning-Anforderungsformular eine Genehmigung zuordnen. Sie können nur Benutzer als Genehmiger einer Anfrage hinzufügen. Nachdem die Anfrage übermittelt wurde, wird sie zunächst an alle genehmigenden Personen gesendet, um sie zu genehmigen, bevor sie einen Datensatz erstellt.

Weitere Informationen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular in Adobe Workfront Planning](/help/quicksilver/planning/requests/add-approval-to-request-form.md).


## Benachrichtigungen für die Übermittlung von Anfragen, Genehmigungen und Statusänderungen

>[!NOTE]
>
>Vorschau-Version: 16. Dezember 2024; Produktionsversion für alle Kunden: 16. Januar 2025

Nachdem Sie eine Anfrage in Workfront Planning gesendet haben, erhalten Sie jetzt eine In-App- sowie eine E-Mail-Benachrichtigung für die folgenden Aktionen:

* Ein Antragsteller erhält eine Benachrichtigung, dass eine Anfrage erfolgreich gesendet wurde

* Ein Antragsteller erhält eine Benachrichtigung, dass eine Anfrage genehmigt oder abgelehnt wurde

* Eine genehmigende Person erhält eine Benachrichtigung, dass eine Anforderung zur Genehmigung eingereicht wurde.

>[!NOTE]
>
>Damit Benutzerinnen und Benutzer E-Mail- und In-App-Benachrichtigungen empfangen können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.

Informationen zum Senden oder Genehmigen von Anfragen finden Sie in den folgenden Artikeln:

* [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md)

* [Genehmigen einer Anfrage in Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md).

## Intelligente Suche bei der Suche nach einem Feldtyp

>[!NOTE]
>
>Vorschau-Version: 5. Dezember 2024; Produktionsversion für alle Kunden: 5. Dezember 2024

Wir haben bei der Suche nach einem Feldtyp in Workfront Planning eine intelligente Suchfunktion hinzugefügt. Sie können jetzt Feldtypen finden, wenn Sie ein Keyword eingeben. Wenn Sie beispielsweise „Preis“ eingeben, werden die Feldtypen „Anzahl“ und „Währung“ gefunden. Vor dieser Verbesserung konnten Sie nur nach dem tatsächlichen Namen des Feldtyps suchen.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Benutzerdefinierter Farbwähler für farbcodierte Optionen von Ein- oder Mehrfachauswahlfeldern

>[!NOTE]
>
>Vorschau-Version: 5. Dezember 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Jetzt können Sie beim Erstellen oder Bearbeiten eines Einzel- oder Mehrfachauswahlfelds benutzerdefinierte Farboptionen auswählen. Wenn Sie Felder mit farbcodierten Optionen erstellen oder bearbeiten, wird durch Klicken auf das Farbsymbol ein Farbauswahlfeld geöffnet. Sie können aus vordefinierten Farben auswählen oder benutzerdefinierte Farben mithilfe von Hexadezimalcodes oder einem Farbspektrum erstellen.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Importieren vorhandener Workfront-Felder in Workfront Planning-Datensatztypen

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Wenn Sie nun Felder zu einem Datensatztyp hinzufügen, haben Sie die Möglichkeit, vorhandene benutzerdefinierte oder native Workfront-Felder zu importieren und sie mit dem ausgewählten Datensatztyp zu verknüpfen. Beim Importieren vorhandener Felder wird eine Kopie der Workfront-Felder in Workfront Planning erstellt. Die kopierten Felder sind unabhängig von ihren Originalversionen.

Vor dieser Verbesserung mussten Sie alle Felder manuell erstellen und sie mit Datensatztypen verknüpfen.

Berechnete Felder werden derzeit nicht unterstützt.

Weitere Informationen finden Sie unter [Felder aus Adobe Workfront importieren](/help/quicksilver/planning/fields/import-fields-from-workfront.md)

## Erstellen von Datensatztypen, Datensätzen und Feldern durch Importieren einer CSV- oder Excel-Datei

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können jetzt neue Datensatztypen importieren, indem Sie eine CSV- oder Excel-Datei importieren.

Die folgenden Informationen werden importiert:

* Der Name der Tabelle oder Datei wird als Name des Datensatztyps importiert.

* Die erste Zeile jeder Spalte wird als neues Feld importiert. Pro importiertem Blatt können bis zu 500 Felder vorhanden sein.

* Jede Zeile wird als neuer Datensatz importiert. Sie können bis zu 10.000 Datensätze in jedem Blatt haben.

Weitere Informationen finden Sie unter [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

## Zirkuläre Verweise in Formeln vermeiden

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Beim Bearbeiten oder Erstellen eines Formelfelds wurde eine Warnmeldung eingeführt, die möglicherweise einen Zirkelbezug zu sich selbst oder zu freigegebenen Feldern erstellt. Sie können kein Formelfeld speichern, das entweder auf sich selbst oder auf Elemente verweist, auf die in seiner Berechnung verwiesen wird.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Hinzufügen von Verbindungsansichtsseiten zur Datensatzseite, um verbundene Datensätze in einer Tabellenansicht anzuzeigen

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können dem Detailbereich eines Datensatzes Seiten hinzufügen, um verbundene Datensätze in einer Tabellenansicht anzuzeigen. Sie können eine Seite pro verbundenen Datensatz hinzufügen.

Die hinzugefügten Seiten sind schreibgeschützt.

Weitere Informationen finden Sie unter [Seitenlayout für Einträge verwalten](/help/quicksilver/planning/records/manage-the-record-page.md).

## Neue Registerkarten &quot;Workfront&quot; und „Planung“ im Abschnitt „Gesendet“ im Bereich „Anfragen“

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Workfront-Planungsanfragen finden Sie jetzt im Abschnitt Gesendet im Bereich Anfragen von Workfront. Im Abschnitt Gesendet werden jetzt die folgenden Registerkarten angezeigt:

* Workfront: Zeigt in Workfront gesendete Anfragen an.
* Planung: Zeigt über ein Workfront Planning-Anforderungsformular gesendete Anforderungen an.

Um Anfragen zu einem Workfront Planning-Datensatztyp hinzufügen zu können, müssen Sie einen Link zum Anfrageformular verwenden. Das Senden einer Workfront-Planungsanfrage über den Bereich Anfragen in Workfront wird zu einem späteren Zeitpunkt verfügbar sein.

Ihr Unternehmen muss ein Workfront Planning-Paket erwerben, bevor Ihnen die Registerkarte Planning im Bereich Requests zur Verfügung steht.

Weitere Informationen finden Sie unter [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).

## Zusätzliche Feldtypen werden jetzt in Anfrageformularen unterstützt

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

In Workfront Planning können Sie jetzt die folgenden Feldtypen zu einem Anforderungsformular für Datensatztypen hinzufügen:

* Personen
* Workfront-Verbindungen

Vor dieser Verbesserung konnten diese Feldtypen nicht zu Anfrageformularen in Workfront Planning hinzugefügt werden.

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Öffentliche Freigabe von Anfrageformularen begrenzen, die bestimmte Feldtypen enthalten

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können ein Anfrageformular nicht mehr öffentlich freigeben, wenn das Formular einen der folgenden Feldtypen enthält:

* Formel
* Verbindungen zu Workfront und AEM Assets
* Felder nachschlagen
* Personen

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).


## Datensätze in der Kalenderansicht nach Woche anzeigen

>[!NOTE]
>
>Vorschau-Version: 26. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Jetzt können Datensätze wöchentlich in der Kalenderansicht angezeigt werden. Vor dieser Verbesserung konnten Sie die Kalenderansicht nur nach Monat anzeigen.

Weitere Informationen finden Sie unter [Verwalten der Kalenderansicht](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Gelöschte Einträge wiederherstellen

>[!NOTE]
>
>Vorschau-Version: 22. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Nachdem Datensätze gelöscht wurden, werden sie jetzt 30 Tage lang vorübergehend in ein kürzlich gelöschtes Bin verschoben. Sie können von der Seite des Datensatztyps aus auf das kürzlich gelöschte Bin zugreifen, das nur Datensätze eines bestimmten Typs enthält.

Workspace-Manager können Datensätze bis zu 30 Tage nach dem Löschen aus dem Papierkorb wiederherstellen. Verbundene Datensätze und ihre Feldinformationen werden ebenfalls wiederhergestellt.

Vor dieser Verbesserung konnten gelöschte Datensätze nicht wiederhergestellt werden.

Weitere Informationen finden Sie unter [Wiederherstellen gelöschter Datensätze](/help/quicksilver/planning/records/records-information.md).

## Adobe-KI-Assistent in den Datensatzdetailbereichen verfügbar

>[!NOTE]
>
>Vorschau-Version: 21. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Um Ihnen die Arbeit zu erleichtern, haben wir den Adobe-KI-Assistenten zur Detailvorschau oder Datensatzseite eines Datensatzes hinzugefügt. Sie können den KI-Assistenten innerhalb einer Datensatzseite verwenden, um Informationen über den Datensatz zu aktualisieren.

Weitere Informationen finden Sie unter [Übersicht über den Adobe Workfront Planning AI-Assistenten](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

## Neues Erlebnis beim Hinzufügen einer Miniaturansicht und eines Titelbilds zu einer Datensatzseite

>[!NOTE]
>
>Vorschau-Version: 20. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Wenn Sie die Vorschau oder Seite eines Datensatzes öffnen und der Datensatz keine Miniaturansicht oder ein Titelbild hat, müssen Sie jetzt den Mauszeiger über den Bereich über dem Datensatznamen in der Kopfzeile bewegen, um die Optionen zum Hinzufügen eines Covers und eines Miniaturbilds zum Datensatz anzuzeigen. Vor dieser Verbesserung wurden die leeren Platzhalterbilder für die Miniaturansicht und das Cover über dem Datensatznamen angezeigt.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Hinzufügen eines Cover-Bildes zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [Hinzufügen eines Miniaturbilds zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## Neue Anzeigetypen für Felder vom Typ Prozentsatz in der Tabellenansicht

>[!NOTE]
>
>Vorschau-Version: 7. November 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.12 (12. Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Um die Lesbarkeit der Zahlen in der Tabellenansicht zu vereinfachen, können Sie jetzt aus den folgenden Optionen auswählen, um die Darstellung eines Felds vom Typ Prozentsatz in der Tabellenansicht zu ändern:

* Zahl
* Balken
* Kreis

Dieser Anzeigetyp wird nur in der Tabellenansicht unterstützt.

Vor dieser Verbesserung konnten Sie Prozentwerte nur als Zahlen anzeigen.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Verbindungsfelder werden jetzt in Anfrageformularen unterstützt

>[!NOTE]
>
>Vorschau-Version: 31. Oktober 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können jetzt verbundene Felder für Workfront Planning-Datensätze zu einem Datensatztyp-Anfrageformular hinzufügen.

Sie können im Anfrageformular keine Verbindungssuchfelder oder verbundenen Felder für Workfront-Objekte hinzufügen.

Vor dieser Verbesserung konnten diese Feldtypen nicht zu Anfrageformularen in Workfront Planning hinzugefügt werden.

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Verbindungswarnung beim Verbinden von Datensätzen, die bereits mit anderen Datensätzen verknüpft sind

>[!NOTE]
>
>Vorschau-Version: 31. Oktober 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Wenn Sie versuchen, Datensätze zu verbinden, die bereits an anderer Stelle verbunden sind und zu einem Datensatztyp gehören, der über eine Eins-zu-Viele- oder Eins-zu-Eins-Verbindung verbunden ist, erhalten Sie jetzt eine Warnung, dass die Datensätze bereits verbunden sind. Wenn Sie bestätigen, dass Sie mit Ihrer Verbindung fortfahren möchten, werden die ausgewählten Datensätze aus dem ursprünglichen Datensatz entfernt und dem Datensatz hinzugefügt, den Sie gerade bearbeiten.

Informationen zu Verbindungstypen finden Sie unter [Übersicht über verbundene Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Neues Informationssymbol mit der Beschreibung von Feldern auf der Detailseite des Datensatzes

>[!NOTE]
>
>Vorschau-Version: 30. Oktober 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Rechts neben den Feldnamen auf einer Datensatzseite wurde ein Informationssymbol hinzugefügt. Wenn Sie auf das Informationssymbol klicken, wird die Beschreibung des Felds angezeigt, sofern eine Beschreibung vorhanden ist. Vor dieser Verbesserung wurde die Beschreibung des Felds angezeigt, wenn Sie den Mauszeiger über den Feldnamen bewegen.

Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

## Neuer Workfront-Feldtyp für Planning-Verbindungen

>[!NOTE]
>
>Vorschau-Version: 24. Oktober 2024; Produktion für die schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Um weiterhin Workfront-Objekte mit Workfront Planning-Datensätzen zu verbinden, haben wir einen neuen Feldtyp in benutzerdefinierten Workfront-Formularen namens Planning-Verbindung hinzugefügt. Durch Hinzufügen dieses Feldtyps in einem benutzerdefinierten Workfront-Formular und letztendlich in einem Workfront-Objekt können Sie jetzt Folgendes tun:

* Zeigt Datensätze an, die mit einem Workfront-Objekt im benutzerdefinierten Formular verbunden sind.

* Verbinden Sie Workfront-Planungsdatensätze mit einem Workfront-Objekt und trennen Sie sie.

Sie können das neue Feld für alle Objekttypen zu Formularen hinzufügen. Sie können die Informationen im Feld jedoch nur aus Formularen bearbeiten, die mit den folgenden Workfront-Objekten verbunden sind, die über Workfront Planning-Datensatztypen verbunden werden können: Portfolio, Programm, Projekt, Unternehmen, Gruppe.

Die Planning-Verbindungsfelder für Workfront-Objekte können noch nicht stapelweise bearbeitet werden.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Sehen Sie sich eine Videodemonstration dieser Funktion an](https://video.tv.adobe.com/v/3435633/){target=_blank}
