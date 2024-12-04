---
content-type: release-notes
title: Adobe Workfront - Planung der Release-Aktivität für Version 25.1
description: Dies ist die Release-Aktivität für das Adobe Workfront-Planungsprodukt für das erste Quartal 2025.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
exl-id: ef0b719c-6d2e-4d3e-9522-da6dbd71c248
source-git-commit: 5db940b197364e30ef6e1ea3e3c94ae3bda5b20c
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 0%

---

# Aktivität &quot;Erste Quartal 2025&quot; für die Adobe Workfront-Planung

<!--remove this important intro after the 25.1 release-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Workfront Planning, ein neues Angebot von Adobe Workfront.
>
>Zusätzlich zu einem Workfront-Plan müssen Sie einen Workfront-Planungsplan erwerben, um auf Workfront-Planungsfunktionen zugreifen und diese verwenden zu können.
>
>Eine vollständige Liste der Anforderungen für den Zugriff auf die Workfront-Planung finden Sie unter [Zugriffsübersicht](/help/quicksilver/planning/access/access-overview.md).
>Einen Überblick über die Workfront-Planung finden Sie unter [Übersicht über die Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-overview.md).

In diesem Artikel werden die Funktionen beschrieben, die während der Version des ersten Quartals 2025 für die Workfront-Planung verfügbar sind.

<!--keep the sentence below for all future quarterly release pages-->
<!--remove the general activity mention after First Quarter 2025 is released-->

Eine Liste aller Funktionen, die nach der allgemeinen Release vom 28. August 2024 für die Adobe Workfront-Planung freigegeben wurden, finden Sie unter [Adobe Workfront Planning release activity: article index](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).


## Vorhandene Workfront-Felder in Datensatztypen für die Workfront-Planung importieren

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Wenn Sie nun Felder zu einem Datensatztyp hinzufügen, können Sie vorhandene benutzerdefinierte oder native Workfront-Felder importieren und mit dem ausgewählten Datensatztyp verknüpfen. Durch den Import vorhandener Felder wird eine Kopie der Workfront-Felder in der Workfront-Planung erstellt. Die kopierten Felder sind unabhängig von den Originalversionen.

Vor dieser Verbesserung mussten Sie alle Felder manuell erstellen und sie mit Datensatztypen verknüpfen.

Berechnete Felder werden derzeit nicht unterstützt.

Weitere Informationen finden Sie unter [Importieren von Feldern aus Adobe Workfront](/help/quicksilver/planning/fields/import-fields-from-workfront.md)

## Datensatztypen, Datensätze und Felder durch Importieren einer CSV- oder Excel-Datei erstellen

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können jetzt neue Datensatztypen importieren, indem Sie eine CSV- oder Excel-Datei importieren.

Die folgenden Informationen werden importiert:

* Der Name des Blatts oder der Datei wird als Name des Datensatztyps importiert.

* Die erste Zeile jeder Spalte wird als neues Feld importiert. Sie können bis zu 500 Felder in jedem importierten Blatt haben.

* Jede Zeile wird als neuer Datensatz importiert. Sie können bis zu 10.000 Datensätze pro Blatt haben.

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

## Vermeiden von Zirkelverweisen in Formeln

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Wir haben eine Warnmeldung beim Bearbeiten oder Erstellen eines Formelfelds eingeführt, das möglicherweise einen kreisförmigen Verweis auf sich selbst oder freigegebene Felder erstellt. Sie können kein Formelfeld speichern, das sich entweder auf sich selbst oder auf Elemente bezieht, auf die in der Berechnung verwiesen wird.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Hinzufügen von Verbindungsansichtsseiten zur Datensatzseite, um verbundene Datensätze in einer Tabellenansicht anzuzeigen

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können dem Detailbereich eines Datensatzes Seiten hinzufügen, um verbundene Datensätze in einer Tabellenansicht anzuzeigen. Sie können pro verknüpften Datensatz eine Seite hinzufügen.

Die hinzugefügten Seiten sind schreibgeschützt.

Weitere Informationen finden Sie unter [Layout der Datensatzseite verwalten](/help/quicksilver/planning/records/manage-the-record-page.md).

## Neue Registerkarten für Workfront und Planung im Bereich &quot;Gesendet&quot;des Bereichs Anforderungen

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Workfront-Planungsanfragen finden Sie jetzt im Abschnitt &quot;Gesendet&quot;des Anforderungsbereichs von Workfront. Im Abschnitt &quot;Gesendet&quot;werden jetzt die folgenden Registerkarten angezeigt:

* Workfront: Zeigt die in Workfront gesendeten Anforderungen an.
* Planung: Zeigt Anfragen an, die mit einem Workfront Planning-Anfrageformular eingereicht wurden.

Sie müssen einen Link zum Anforderungsformular verwenden, um Anforderungen zu einem Datensatztyp für die Workfront-Planung hinzufügen zu können. Die Übermittlung einer Workfront-Planungsanfrage aus dem Workfront-Anforderungsbereich ist zu einem späteren Zeitpunkt verfügbar.

Ihr Unternehmen muss ein Workfront-Planungspaket kaufen, bevor Ihnen im Bereich Anforderungen die Registerkarte Planung zur Verfügung steht.

Weitere Informationen finden Sie unter [Planungsanfragen zur Erstellung von Datensätzen mit Adobe Workfront senden](/help/quicksilver/planning/requests/submit-requests.md).

## Zusätzliche Feldtypen werden jetzt in Anforderungsformularen unterstützt

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können jetzt die folgenden Feldtypen zu einem Anforderungsformular vom Typ Datensatz in der Workfront-Planung hinzufügen:

* Personen
* Workfront-Verbindungen

Vor dieser Verbesserung konnten diese Feldtypen nicht zu Anforderungsformularen in der Workfront-Planung hinzugefügt werden.

Weitere Informationen finden Sie unter Anforderungsformular erstellen und verwalten in der Adobe Workfront-Planung (/help/quicksilver/planning/requests/create-request-form.md).

## Beschränken der öffentlichen Freigabe von Anforderungsformularen, die bestimmte Feldtypen enthalten

>[!NOTE]
>
>Vorschau-Version: 27. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können ein Anforderungsformular nicht mehr öffentlich freigeben, wenn das Formular einen der folgenden Feldtypen enthält:

* Formel
* Workfront- und AEM Assets-Verbindungen
* Suchfelder
* Personen

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anforderungsformulars in der Adobe Workfront-Planung](/help/quicksilver/planning/requests/create-request-form.md).


## Anzeigen von Datensätzen in der Kalenderansicht nach Woche

>[!NOTE]
>
>Vorschau-Version: 26. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können Datensätze nun wöchentlich in der Kalenderansicht anzeigen. Vor dieser Verbesserung konnten Sie die Kalenderansicht nur pro Monat anzeigen.

Weitere Informationen finden Sie unter [Verwalten der Kalenderansicht](/help/quicksilver/planning/views/manage-the-calendar-view.md).

## Gelöschte Datensätze wiederherstellen

>[!NOTE]
>
>Vorschau-Version: 22. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Nachdem die Datensätze gelöscht wurden, werden sie nun 30 Tage lang vorübergehend in eine kürzlich gelöschte Klasse verschoben. Sie können auf die kürzlich gelöschte Klasse von der Seite des Datensatztyps zugreifen und sie enthält nur Datensätze eines bestimmten Typs.

Workspace-Manager können bis zu 30 Tage nach dem Löschen Datensätze aus dem Papierkorb wiederherstellen. Verbundene Datensätze und ihre Feldinformationen werden ebenfalls wiederhergestellt.

Vor dieser Verbesserung konnten gelöschte Datensätze nicht wiederhergestellt werden.

Weitere Informationen finden Sie unter [Gelöschte Datensätze wiederherstellen](/help/quicksilver/planning/records/records-information.md).

## Adobe AI Assistant verfügbar in den Datensatzdetailbereichen

>[!NOTE]
>
>Vorschau-Version: 21. November 2024; Produktion für schnelle Veröffentlichung: Mit Version 24.12 (Dezember 2024); Produktion für vierteljährliche Veröffentlichung: Mit Version 25.1 (Januar 2025)

Um Ihnen die Arbeit zu erleichtern, haben wir den Adobe AI-Assistenten zur Detailvorschau oder Datensatzseite hinzugefügt. Sie können den KI-Assistenten innerhalb einer Datensatzseite verwenden, um Informationen zum Datensatz zu aktualisieren.

Weitere Informationen finden Sie unter [Adobe Workfront Planning AI Assistant Overview](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

## Neues Erlebnis beim Hinzufügen einer Miniaturansicht und eines Titelbilds zu einer Datensatzseite

>[!NOTE]
>
>Vorschau-Version: 20. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Wenn Sie die Vorschau oder Seite eines Datensatzes öffnen und der Datensatz keine Miniaturansicht oder kein Titelbild aufweist, müssen Sie jetzt den Mauszeiger über den Bereich über dem Datensatznamen in der Kopfzeile bewegen, um die Optionen zum Hinzufügen eines Titelbilds und eines Miniaturbilds zum Datensatz anzuzeigen. Vor dieser Verbesserung werden die leeren Platzhalterbilder für die Miniaturansicht und das Deckblatt über dem Datensatznamen angezeigt.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Hinzufügen eines Titelbilds zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
* [Hinzufügen eines Miniaturbilds zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

## Neue Anzeigetypen für Prozentfelder in der Tabellenansicht

>[!NOTE]
>
>Vorschau-Version: 7. November 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.12 (Dezember 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Um die Lesbarkeit von Zahlen in der Tabellenansicht zu vereinfachen, können Sie jetzt aus den folgenden Optionen auswählen, um zu ändern, wie ein Feld vom Typ Prozentsatz in der Tabellenansicht angezeigt wird:

* Zahl
* Balken
* Kreis

Dieser Anzeigetyp wird nur in der Tabellenansicht unterstützt.

Vor dieser Verbesserung konnten Sie Prozentwerte nur als Zahlen anzeigen.

Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

## Verbindungsfelder werden jetzt in Anfrageformularen unterstützt

>[!NOTE]
>
>Vorschau-Version: 31. Oktober 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Sie können jetzt verbundene Felder für Workfront Planning-Datensätze zu einem Anfrage-Formular vom Typ Datensatz hinzufügen.

Sie können keine Verbindungssuchfelder oder verbundenen Felder für Workfront-Objekte im Anfrageformular hinzufügen.

Vor dieser Verbesserung konnten diese Feldtypen nicht zu Anforderungsformularen in der Workfront-Planung hinzugefügt werden.

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anforderungsformulars in der Adobe Workfront-Planung](/help/quicksilver/planning/requests/create-request-form.md).

## Verbindungswarnung beim Verbinden von Datensätzen, die bereits mit anderen Datensätzen verknüpft sind

>[!NOTE]
>
>Vorschau-Version: 31. Oktober 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Wenn Sie versuchen, Datensätze zu verbinden, die bereits an einer anderen Stelle verbunden sind und zu einem Datensatztyp gehören, der über einen Verbindungstyp &quot;Eins zu viele&quot;oder &quot;Eins zu eins&quot;verbunden ist, erhalten Sie jetzt eine Warnung, dass die Datensätze bereits verbunden sind. Wenn Sie bestätigen, dass Sie mit Ihrer Verbindung fortfahren möchten, werden die ausgewählten Datensätze aus dem ursprünglichen Datensatz entfernt und dem Datensatz hinzugefügt, den Sie gerade bearbeiten.

Informationen zu Verbindungstypen finden Sie unter [Übersicht über verbundene Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types-overview.md).

## Neues Informationssymbol mit der Beschreibung der Felder auf der Detailseite des Datensatzes

>[!NOTE]
>
>Vorschau-Version: 30. Oktober 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Rechts neben den Feldnamen auf einer Datensatzseite wurde ein Informationssymbol hinzugefügt. Wenn Sie auf das Informationssymbol klicken, wird die Beschreibung des Felds angezeigt, sobald eine Beschreibung vorhanden ist. Vor dieser Verbesserung wird die Beschreibung des Felds angezeigt, das angezeigt wird, wenn Sie mit dem Mauszeiger über den Feldnamen fahren.

Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

## Neuer Workfront-Feldtyp für Planungsverbindungen

>[!NOTE]
>
>Vorschau: 24. Oktober 2024; Produktion für schnelle Veröffentlichung: Mit der Version 24.11 (14. November 2024); Produktion für die vierteljährliche Veröffentlichung: Mit der Version 25.1 (Januar 2025)

Um mit der Überbrückung von Workfront-Objekten zu Datensätzen in der Workfront-Planung fortzufahren, haben wir in benutzerdefinierten Workfront-Formularen einen neuen Feldtyp namens &quot;Planungsverbindung&quot;hinzugefügt. Wenn Sie diesen Feldtyp in einem benutzerdefinierten Workfront-Formular und letztendlich in einem Workfront-Objekt hinzufügen, können Sie jetzt Folgendes tun:

* Zeigt Datensätze an, die mit einem Workfront-Objekt verbunden sind, im benutzerdefinierten Formular.

* Verbinden und Trennen Sie Workfront Planning-Datensätze von einem Workfront-Objekt.

Sie können das neue Feld für alle Objekttypen zu Formularen hinzufügen. Sie können die Informationen im Feld jedoch nur aus Formularen bearbeiten, die an die folgenden Workfront-Objekte angehängt sind, die über die Datensatztypen für die Workfront-Planung verbunden werden können: Portfolio, Programm, Projekt, Unternehmen, Gruppe.

Die Massenbearbeitung der Verbindungsfelder für Workfront-Objekte ist noch nicht möglich.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Sehen Sie sich eine Videodemonstration für diese Funktion an](https://video.tv.adobe.com/v/3435633/){target=_blank}
