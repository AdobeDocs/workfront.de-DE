---
title: Eingabeaufforderungen und Best Practices des KI-Assistenten
content-type: reference
description: Erfahren Sie mehr über die Best Practices für die Verwendung des KI-Assistenten und sehen Sie sich eine Liste von Beispielen für Eingabeaufforderungen an.
author: Jenny
feature: Get Started with Workfront
exl-id: 34a60482-e060-49f9-bbaf-8aed85845e26
source-git-commit: dc472e93541641ee1c960ec7246365200f522a17
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 4%

---

# Eingabeaufforderungen und Best Practices des KI-Assistenten

Der KI-Assistent von Workfront ist ein leistungsstarkes Tool, mit dem Sie Ihre Arbeit effektiver erledigen können, indem Sie nützliche Informationen zu Ihren Kontodaten und bestimmten Objekttypen bereitstellen.

In diesem Artikel erfahren Sie mehr über die aktuellen Best Practices für den KI-Assistenten, einschließlich der Möglichkeit, klare Eingabeaufforderungen zu schreiben, welche Objekttypen Sie nach Informationen fragen können und wie Sie bei Bedarf auf zusätzliche Ressourcen zugreifen können, um Informationen zu überprüfen.

Weitere Informationen zum KI-Assistenten finden Sie unter [KI-Assistent - Übersicht](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

>[!NOTE]
>
>Wenn sich die Funktionen des KI-Assistenten weiterentwickeln, wird der Typ der Anfragen und Fragen, die Sie ihm stellen können, erweitert. Es wird empfohlen, diesen Artikel erneut zu lesen, da neue Funktionen des KI-Assistenten veröffentlicht werden, um mehr über verfügbare Eingabeaufforderungen zu erfahren, die Sie verwenden können.


## Für den KI-Assistenten verfügbare Objekttypen

Der KI-Assistent kann Daten für die folgenden Objekttypen bereitstellen:

* Portfolios
* Programme
* Projekte
* Aufgaben
* Probleme
* Benutzerdefinierte Formulare
* Benutzende
* Workfront-Planungsdatensätze

>[!NOTE]
>
>Sie müssen in Ihrer Zugriffsebene über die erforderliche Berechtigung für ein Objekt verfügen, bevor Sie dessen Daten vom KI-Assistenten anfordern können.

## Best Practices

### Eingabeaufforderungen löschen

Um auf die nützlichsten Informationen aus dem KI-Assistenten zuzugreifen, ist es wichtig, Eingabeaufforderungen zu erstellen, die Ihnen die gewünschte Antwort geben. Die folgende Liste enthält Prinzipien, die Ihnen dabei helfen, die richtigen Eingabeaufforderungen am besten zu formulieren:

* **Verwenden Sie eine klare und spezifische Sprache**: Das Vermeiden vager und allgemeiner Eingabeaufforderungen wird dem KI-Assistenten helfen, die Daten zu erhalten, die Sie erhalten möchten.
* **Zeitrahmen einschließen**: Wenn Sie dem KI-Assistenten bestimmte Zeitrahmen für ein Objekt zuweisen, können Sie die zu verarbeitenden Daten eingrenzen und zielgerichtetere Informationen in der Antwort erhalten.
* **Fragen Sie nur nach einer Sache auf einmal**: Wenn mehrere, nicht verwandte Anfragen in einer einzigen Eingabeaufforderung enthalten sind, kann der KI-Assistent nicht die richtigen Informationen bereitstellen.

Informationen zu empfohlenen Eingabeaufforderungen finden Sie im folgenden Abschnitt in diesem Artikel: [Eingabeaufforderungsbeispiele](#prompt-examples).


### Überprüfen der KI-Assistentenantworten

In dieser Phase der Entwicklung des KI-Assistenten wird empfohlen, die bereitgestellten Informationen zu überprüfen, wenn Sie nach Informationen zu Workfront-Prozessen gefragt werden. Klicken Sie dazu auf den Link des Artikels im Abschnitt Quellen in der Eingabeaufforderung.

![Abschnitt Quellen](assets/sources-section.png)

Weitere Informationen zu Eingabeaufforderungen für Workfront-Prozesse finden Sie unter [Eingabeaufforderungen zu Workfront-Aktionen](#prompts-to-learn-about-workfront-actions) in diesem Artikel.


## Beispiele für Prompts

Die folgenden Tabellen enthalten Beispiele für Eingabeaufforderungen, mit denen Sie Informationen über Ihre Arbeit generieren und mehr über bestimmte Workfront-Prozesse oder -Aktionen erfahren können, die Sie ausführen möchten.

### Eingabeaufforderungen, um Informationen über Ihre Arbeit zu finden

<table>
    <tr>
        <td><b>Objekttyp</b></td>
        <td><b>Eingabeaufforderung</b></td>
    </tr>
        <tr>
        <td>Projekte</td>
        <td><em>Welches Fälligkeitsdatum hat [PROJEKTNAME]?</em>
        </td>
    </tr>
    <tr>
        <td>Projekte</td>
        <td><em>Wie ist der Status von [PROJECT NAME]?</em>
        </td>
    </tr>
    <tr>
        <td>Projekte </td>
        <td><em>Wer ist der Projektbesitzer für [PROJECT NAME]?</em></td>
    </tr>
    <tr>
        <td>Aufgaben</td>
        <td><em>Welche Aufgaben werden mir diese Woche zugewiesen?</em></td>
    </tr>
       <tr>
        <td>Probleme </td>
        <td><em>Welche offenen Anfragen werden meinem Team zugewiesen?</em></td>
           <tr>
        <td>Benutzende</td>
        <td><em>Wer ist im Kreativ-Team von [PROJECT NAME]?</em></td>
    </tr>
           <tr>
        <td>Benutzende </td>
        <td><em>Wie viele Aufgaben sind [USER] zugewiesen?</em></td>
    </tr>
   </table>


### Eingabeaufforderungen zu Workfront-Aktionen

<table>
    <tr>
        <td><b>Objekttyp</b></td>
        <td><b>Eingabeaufforderung</b></td>
    </tr>
    <tr>
        <td>Projekte</td>
        <td><em>Wie erstelle ich ein neues Projekt aus einer Vorlage?</em>
        </td>
    </tr>
    <tr>
        <td>Projekte </td>
        <td><em>Was ist der Unterschied zwischen einem Projekt und einem Programm?</em></td>
    </tr>
    <tr>
        <td>Aufgaben</td>
        <td><em>Wie kann ich eine Aufgabe mehreren Benutzern zuweisen?</em></td>
    </tr>
       <tr>
        <td>Aufgaben</td>
        <td><em>Was bedeutet der Status Bereit zum Start?</em></td>
    </tr>
       <tr>
        <td>Probleme </td>
        <td><em>Wie wandle ich eine Anfrage in eine Aufgabe um?</em></td>
    </tr>
           <tr>
        <td>Probleme </td>
        <td><em>Was ist der Lebenszyklus eines Problems in Workfront?</em></td>
    </tr>
        </tr>
           <tr>
        <td>Probleme </td>
        <td><em>Wie eskaliere ich eine Anfrage?</em></td>
    </tr>
           <tr>
        <td>Dokumente</td>
        <td><em>Wie lade ich eine neue Version eines Dokuments hoch?</em></td>
    </tr>
           <tr>
        <td>Dokumente </td>
        <td><em>Kann ich Workflows für die Dokumentengenehmigung festlegen?</em></td>
    </tr>
   </table>


## Aktuelle Einschränkungen des KI-Assistenten

Der KI-Assistent ist ein leistungsstarkes Tool, aber es gibt bestimmte Arten von Fragen und Anfragen, für die er in diesem aktuellen Entwicklungsstadium keine Daten bereitstellen kann. Die folgende Tabelle enthält Beispiele für Eingabeaufforderungen, für die der KI-Assistent keine Daten anzeigen kann.

<table>
    <tr>
        <td><b>Eingabeaufforderungstyp</b></td>
        <td><b>Beispiel</b></td>
    </tr>
    <tr>
        <td>Fragen zu benutzerdefinierten Konfigurationen</td>
        <td><em>Welche benutzerdefinierte Integrationslogik wird in unserer Workfront-Instanz ausgeführt?</em>
        </td>
    </tr>
    <tr>
        <td>Fragen zu Daten außerhalb von Workfront </td>
        <td><em>Können Sie mir meinen Outlook-Kalender für heute zeigen?</em></td>
    </tr>
             <tr>
        <td>Fragen zu nicht integrierten Adobe-Produkten </td>
        <td><em>Wie bearbeite ich von hier aus eine PDF in Acrobat?</em></td>
         <tr>
        <td>Fragen, die menschliches Urteilsvermögen erfordern</td>
        <td><em>Sollte dieses Projekt auf Eis gelegt werden?</em></td>
    </tr>
    </tr>
       <tr>
        <td>Massenaktualisierungsanfragen</td>
        <td><em>Alle überfälligen Aufgaben für [USER] neu zuweisen.</em></td>
    </tr>
       <tr>
        <td>Anfragen für die prädiktive Analyse</td>
        <td><em>Schlagen Sie einen neuen Projektplan auf der Grundlage unserer historischen Daten vor.</em></td>
    </tr>
           <tr>
        <td>Anfragen für Informationen über Ihrer Zugriffsebene</td>
        <td><em>Listet alle Abrechnungssätze im Konto auf.</em></td>
    </tr>
           <tr>
        <td>Anfragen, die vage Informationen enthalten </td>
        <td><em>Mein Projekt reparieren.</em></td>
    </tr>
   </table>
