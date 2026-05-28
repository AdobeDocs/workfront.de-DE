---
content-type: release-notes
title: Versionsaktivität für Adobe Workfront Planning im dritten Quartal 2026
description: Dies ist die Veröffentlichungsaktivität für das Adobe Workfront Planning-Produkt im dritten Quartal 2026.
author: Alina
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: ab1ac1363d6531352e905536218618196651c3b9
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 1%

---

# Versionsaktivität für Adobe Workfront Planning im dritten Quartal 2026

<!--
take the next sentence out when we start listing features
-->

<!--
There are no features released during the Third Quarter Release for 2026. When features are released for this quarter, we will document them in this article. 
-->

<!--keep the sentence below for all future quarterly release pages-->

In diesem Artikel werden die Funktionen beschrieben, die im dritten Quartal 2026 für Workfront Planning veröffentlicht werden.

Eine Liste aller für Adobe Workfront Planning veröffentlichten Funktionen finden Sie unter [Adobe Workfront Planning Release-Aktivität: Artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).



<!--

## Planning Designer now available in Beta for all Workfront Planning customers

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 
>[!BADGE In Beta]{type=Neutral}

You can now use the Adobe Planning Designer powered by AI to configure your workspaces and data structures with ease. The Planning Designer supports everything from creating and configuring workspaces to defining fields and formulas, managing records, reviewing change history and building custom views.  

Whether used directly or through the AI Assistant, the Planning Designer provides a flexible, powerful environment for building and maintaining structured, connected information. 

A Workfront administrator can manage the availability of the Planning Designer from the System Preferences area in Setup.   

For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

## New Sample workspaces tab added to the Planning landing page

>[!NOTE]
>
>Preview: May 28, 2026 
>Production fast release: June 11, 2026 
>Production for everyone: July 16, 2026 

We have added the Sample workspaces tab in the Planning landing area where you can view example of best-practice workspaces. The workspaces are not editable and we recommend that you use them as examples to create your own.  

We also recommend that you use the multi-workspace template to create, and edit and share workspaces that result as a use of that template.  The template contains the same workspaces as the Sample workspaces tab.   

Workspace managers can modify views in sample workspaces.     

For information, see Workspaces overview (/help/quicksilver/planning/architecture/workspaces-overview.md). 

-->

## Workfront Planning-API, Version 2

>[!NOTE]
>
>Verfügbar für alle Kunden: 28. Mai 2026>[!BADGE Aus Zeitplan]{type=Neutral}

Version 2 der Workfront Planning-API ist jetzt verfügbar und erweitert die Funktionen von Version 1 erheblich.

Die folgenden Verbesserungen sind in Version 2 enthalten:

* Programmgesteuertes Erstellen, Aktualisieren und Löschen von Arbeitsbereichen, Datensatztypen und Feldern.

* Einträge vollständig verwalten.
* Verbesserungen der URL-Struktur, Fehlerbehandlung, Paginierung, Filterung und Berechtigungen.
* Beinhaltet partielle Updates über PATCH
* Umfasst Masseneintragsvorgänge.

Version 1 bleibt verfügbar, obwohl wir empfehlen, zur Verwendung von Version 2 zu wechseln.

>[!NOTE]
>
>Der Workfront Planning-Connector für Fusion wurde nicht auf API-Version 2 aktualisiert und verwendet Version 1 bis auf Weiteres.

Weitere Informationen finden Sie unter [Grundlagen zur Adobe Workfront Planning-API](/help/quicksilver/planning/general/planning-api-basics.md).

Informationen zu den Spezifikationen der Workfront Planning-API finden Sie in der Entwicklerdokumentation zur [Workfront ](https://developer.adobe.com/wf-planning/)-API.

## Berechtigungen für Datensätze erteilen

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Sie können jetzt einzelne Datensatzberechtigungen anpassen, um zu steuern, wer sie in einem Datensatztyp verwalten kann.

Benutzer erben standardmäßig die Datensatzberechtigungen vom Arbeitsbereich und vom Datensatztyp. Um nur ausgewählten Benutzern mit Berechtigungen für Datensatztypen Berechtigungen zum Verwalten nur bestimmter Datensätze zu erteilen, können Sie geerbte Berechtigungen für ausgewählte Datensätze deaktivieren und nur diesen Benutzern den Zugriff auf diese Datensätze verwalten gewähren. Sie können die Berechtigungen für einen Datensatz oder für mehrere Datensätze gleichzeitig stapelweise anpassen.

Sie können Benutzern die folgenden Berechtigungsebenen gewähren:

* Ansicht
* Verwalten

>[!NOTE]
>
>* Die Berechtigungen eines Benutzers auf Datensatzebene können seine Berechtigungen für den Datensatztyp nicht überschreiten. Beispielsweise kann einem Benutzer mit Ansichtszugriff auf einen Datensatztyp kein Verwaltungszugriff auf einzelne Datensätze dieses Typs gewährt werden.
>* Derzeit können Sie die Berechtigungen von Benutzenden nicht aus einem Datensatz entfernen. Jeder Benutzer, der zumindest Anzeigezugriff auf den Datensatztyp hat, kann alle Datensätze dieses Typs anzeigen.

Weitere Informationen finden Sie unter [Freigeben von Datensätzen](/help/quicksilver/planning/access/share-records.md).

## Optimierte Hinzufügung globaler Datensatztypen

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Um Klicks zu reduzieren und das schnelle Auffinden der benötigten Datensatztypen zu erleichtern, haben wir das Hinzufügen von Datensätzen verbessert, sodass es beim Hinzufügen globaler Datensatztypen zu einem anderen Arbeitsbereich schneller und intuitiver wird.

Wenn Sie einen Datensatz aus vorhandenen Datensatztypen hinzufügen, wird sofort eine Liste aller verfügbaren globalen Datensatztypen angezeigt.

Direkt auf diesem Bildschirm können Sie einen oder mehrere globale Datensatztypen auswählen und gleichzeitig hinzufügen.

Weitere Informationen finden Sie unter [Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md).


## Synchronisieren von Metadaten von Planning mit AEM Assets

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktionsschnellveröffentlichung: 28. Mai 2026>Produktion für alle: 28. Mai 2026>[!BADGE Zeitplan]{type=Neutral}

Um die Datenintegrität zu verbessern, haben wir eine nahtlose Metadatensynchronisation zwischen GenStudio for Performance Marketing-Datensatztypen und AEM Assets veröffentlicht, wenn AEM Assets in Workfront Planning mit GenStudio-Datensatztypen verknüpft ist.

Die folgenden GenStudio for Performance Marketing-Datensatztypen können mit AEM Assets verbunden werden: Kampagne, Produkt, Rolle, Region und Kanal.

Informationen, die in Workfront Planning zu einem GenStudio-Datensatztyp hinzugefügt wurden, werden auf einer separaten Registerkarte Kampagnen eines AEM Assets in AEM angezeigt. Auf dieser Registerkarte werden auch Informationen zu Produkt, Persona, Region und Kanal für diese Kampagne im schreibgeschützten Modus angezeigt.

Mit dieser Version sind wichtige Metadaten auf beiden Plattformen konsistent und spiegeln Aktualisierungen nahezu in Echtzeit wider, wodurch die manuelle Abstimmung reduziert wird.

Weitere Informationen finden Sie unter [Verwalten des GenStudio-Arbeitsbereichs in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).

## Synchronisieren von Metadaten aus Planning mit AEM-Inhaltsfragmenten

>[!NOTE]
>
>Vorschau: 28. Mai 2026>Produktionsschnellveröffentlichung: 28. Mai 2026>Produktion für alle: 28. Mai 2026>[!BADGE Zeitplan]{type=Neutral}

Um die Datenintegrität zu verbessern, haben wir eine nahtlose Metadaten-Synchronisation zwischen Planning-Datensatztypen im GenStudio-Arbeitsbereich und AEM-Inhaltsfragmenten veröffentlicht, wenn Inhaltsfragmente mit GenStudio for Performance Marketing-Kampagnen verknüpft sind.

Informationen zu GenStudio Campaign werden jetzt auf der Registerkarte Metadaten eines Inhaltsfragments in AEM angezeigt.  Auf dieser Registerkarte werden auch Informationen zu Produkt, Persona, Region und Kanal für diese Kampagne im schreibgeschützten Modus angezeigt.

Mit dieser Version sind wichtige Metadaten auf beiden Plattformen konsistent und spiegeln Aktualisierungen nahezu in Echtzeit wider, wodurch die manuelle Abstimmung reduziert wird.

Weitere Informationen finden Sie unter [Verwalten des GenStudio-Arbeitsbereichs in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md).


## Aktualisierungen der Listenansicht

>[!NOTE]
>
>Vorschau: 27. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Mehrere Feldtypen in der Listenansicht wurden aktualisiert und enthalten jetzt eine Tastaturnavigation und andere Verbesserungen.

Die Felder „Multi-Page“, „Single-Select“ und „Assignee“ bieten jetzt Tastaturnavigation in der Listenansicht:

* Verwenden Sie die Pfeile nach oben und unten auf der Tastatur, um durch die Liste der Personen zu navigieren.

* Drücken Sie die Leertaste, um eine Person auszuwählen oder eine ausgewählte Person zu entfernen.

Bei einzelnen Feldern und Feldern mit Mehrfachauswahl in der Listenansicht:

* Wenn keine Ergebnisse gefunden werden, können Sie neue Optionen direkt aus dem Editor hinzufügen. Beachten Sie, dass diese Funktion möglicherweise nicht in allen Listen verfügbar ist.

* Die Feldinteraktion ist jetzt über die Tastatur zugänglich. Dazu gehört die Navigation zwischen den Tags, Suchoptionen und der Liste mithilfe der Pfeile nach oben und unten. Drücken Sie die Leertaste, um ein Element auszuwählen oder ein ausgewähltes Element zu entfernen.

Referenzfelder wie Felder mit automatischer Textvervollständigung und externe Lookup-Felder haben einige Verbesserungen an der Benutzeroberfläche erhalten.

Auch das Ziehen und Ablegen von Spalten wurde, sofern verfügbar, visuell verbessert.

Weitere Informationen finden Sie unter [Verwalten der Listenansicht in Adobe Workfront Planning](/help/quicksilver/planning/views/manage-the-list-view.md).

## Workfront-Referenzfelder sind als Suchfelder für Planning-Verbindungen aktiviert

>[!NOTE]
>
>Vorschau: 27. Mai 2026>Produktions-Schnellversion: 11. Juni 2026\
>Produktion für alle: 16. Juli 2026

Sie können jetzt Workfront-Referenzfelder als Lookup-Felder hinzufügen, wenn Sie einen Planning-Datensatztyp mit einem Workfront-Objekttyp verbinden.

Sie können beispielsweise die Portfolio-, Programm-, Gruppen- oder Firmeninformationen aus dem Projektobjekt in Planning zu einem Projektverbindungsfeld einer Kampagne hinzufügen.

Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

## Neue Filter für die Aufschlüsselungsfunktion der Zeitleisten-Ansicht

>[!NOTE]
>
>Vorschau: 27. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Sie können jetzt Informationen in der Zeitleisten -Ansicht anhand von Kriterien filtern, die mit den Objekten übereinstimmen, die in der Aufschlüsselung der Datensätze enthalten sind.

Vor dieser Verbesserung konnten Sie Filter nur auf die Hauptdatensätze in der Zeitleisten -Ansicht anwenden.

Weitere Informationen finden Sie unter [Verwalten der Timeline-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).

## Neuer Hinweis darauf, dass sich bearbeitete und gelöschte Felder auf Anfrageformulare auswirken

>[!NOTE]
>
>Vorschau: 27. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Wir haben eine Erinnerung hinzugefügt, dass sich das Bearbeiten oder Löschen von Datensatzfeldern auf Anfrageformulare auswirken kann, die diese Felder enthalten. Jetzt haben Sie die Möglichkeit, die betroffenen Formulare zu überprüfen und sicherzustellen, dass die Änderungen, die Sie an den Feldern vornehmen möchten, keine Auswirkungen auf bestehende Informationen haben.

Weitere Informationen finden Sie unter [Bearbeiten von Feldeinstellungen](/help/quicksilver/planning/fields/edit-fields.md).

## Gesendete Planungsanfragen bearbeiten

>[!NOTE]
>
>Vorschau: 27. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Sie können jetzt Planungsanfragen bearbeiten, nachdem Sie sie übermittelt haben, bevor aus der Anfrage ein Datensatz erstellt wird.

Die folgenden Benutzer können eine gesendete Anfrage bearbeiten:

* Der Ersteller der Anfrage
* Workspace-Manager für den Arbeitsbereich, an den die Anfrage gesendet wurde
* Systemadmins

Vor dieser Verbesserung konnten Sie keine gesendeten Anfragen bearbeiten.

Weitere Informationen finden Sie unter [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).

## Neues Vorschaufenster für AEM-Inhaltsfragmente

>[!NOTE]
>
>Vorschau: 14. Mai 2026>Produktionsschnellveröffentlichung: 14. Mai 2026>Produktion für alle: 14. Mai 2026>[!BADGE Zeitplan]{type=Neutral}

Für eine bessere Sichtbarkeit bei der Arbeit mit AEM-Inhaltsfragmenten, die mit Workfront Planning-Datensätzen verbunden sind, wurde ein Vorschaufenster hinzugefügt, in dem Informationen zu den Fragmenten in Workfront Planning angezeigt werden.

Diese Funktion war bisher für AEM Assets verfügbar und wurde nun zu Inhaltsfragmenten hinzugefügt.

Weitere Informationen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).

## Suchfelder jetzt für AEM-Inhaltsfragmente in Workfront Planning verfügbar

>[!NOTE]
>
>Vorschau: 14. Mai 2026>Produktionsschnellveröffentlichung: 14. Mai 2026>Produktion für alle: 14. Mai 2026>[!BADGE Zeitplan]{type=Neutral}

Sie können jetzt die folgenden Suchfelder hinzufügen, wenn Sie einen Planning-Datensatztyp mit einem AEM-Inhaltsfragment verbinden:

* Erstellt von
* Erstellt um
* Geändert von
* Geändert um

Vor dieser Verbesserung waren Suchfelder nur für AEM-Assets und -Ordner verfügbar.

Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).



## Benutzerdefinierte Ansichten für die Detailseite eines Datensatzes

>[!NOTE]
>
>Vorschau: 14. Mai 2026>Produktions-Schnellversion: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Um eine bessere Flexibilität bei der Visualisierung Ihrer Informationen auf der Detailseite eines Datensatzes zu ermöglichen, haben wir die Möglichkeit eingeführt, benutzerdefinierte Ansichten für diese Seite zu erstellen.

Zusätzlich zum Hinzufügen von zwei bereits erstellten Detailseitenansichten, die entweder alle Datensatzfelder oder nur die in der Tabellenansicht sichtbaren Felder enthalten, können Sie jetzt benutzerdefinierte Ansichten für die Detailseiten eines Datensatzes erstellen. Die von Ihnen erstellten Ansichten sind für alle sichtbar, die auf den Datensatz zugreifen können.

Durch dieses Update wird die Einstellung **Alle Felder anzeigen** entfernt und durch benutzerdefinierte Detailansichten ersetzt.

Weitere Informationen finden Sie unter [Verwalten der Datensatzseite](/help/quicksilver/planning/records/manage-the-record-page.md).

## Hinzufügen von Gruppierungen zu einer Datensatzseite mit verbundenen Projekten

>[!NOTE]
>
>Vorschau: 14. Mai 2026\
>Produktion schnell: 11. Juni 2026>Produktion für alle: 16. Juli 2026

Sie können Ihre Informationen jetzt auf der Seite „Mit Projekten verbundene Datensätze“ eines Datensatzes in Workfront Planning gruppieren. Diese Funktion war in diesem Bereich vor dieser Verbesserung nicht vorhanden.

Weitere Informationen finden Sie unter [Verwalten der Listenansicht](/help/quicksilver/planning/views/manage-the-list-view.md).
