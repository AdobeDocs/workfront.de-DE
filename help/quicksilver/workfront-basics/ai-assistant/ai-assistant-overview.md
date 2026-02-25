---
title: KI-Assistent in Workfront
content-type: reference
description: Erfahren Sie mehr über den KI-Assistenten in Adobe Workfront
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: e8e10f02f77f6c1df9f0af380eb16cc6bbc3b5d1
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 100%

---

# KI-Assistent in Workfront

Der KI-Assistent von Workfront hilft Ihnen bei der Durchführung Ihrer Arbeit, indem er In-App-Informationen und -Vorschläge in einer Unterhaltung in natürlicher Sprache bereitstellt. Der KI-Assistent kann Ihnen ein reibungsloseres Arbeitserlebnis bieten, indem er Folgendes für Sie übernimmt

* Zusammenfassen von Arbeitselementen oder Dokumenten
* Suche nach Anweisungen oder Referenzmaterial für Arbeitsabläufe
* Generieren oder Überprüfen von Formeln für berechnete Felder

## Zugriffsanforderungen

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: Nicht verfügbar</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>oder</p>
       <p>Aktuell: Nicht verfügbar</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen für den KI-Assistenten

Damit der KI-Assistent für Ihre Organisation aktiviert werden kann, müssen **alle** folgenden Bedingungen zutreffen:

* Ihre Organisation muss zu Adobe IMS (Identity Management System) migriert worden sein
* Adobe Unified Experience muss aktiviert sein
* Ihre Organisation muss über ein Workfront-Abo des Typs Select, Prime oder Ultimate verfügen.
* Bei Adobe muss eine unterzeichnete Adobe GenAI-Vereinbarung hinterlegt sein

  Weitere Informationen zur Unterzeichnung der Vereinbarung finden Sie unter [Unterzeichnen der Adobe GenAI-Vereinbarung](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in diesem Artikel.

## Überlegungen zum KI-Assistenten

* Der KI-Assistent reagiert kontextabhängig auf die Seite, die Sie geöffnet haben. Wenn Sie beispielsweise auf einer Projektseite „Erstelle eine Zusammenfassung dieses Projekts“ in den KI-Assistenten eingeben, wird eine Zusammenfassung dieses bestimmten Projekts zurückgegeben.
* Der bzw. die Workfront-Admin muss den KI-Assistenten für Benutzende in Ihrer Organisation aktivieren. Der KI-Assistent wird über Zugriffsebenen aktiviert.

  Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Der KI-Assistent von Workfront-Planung verfügt über andere Funktionen als der KI-Assistent von Workfront.

  Weitere Informationen zum KI-Assistenten in Workfront-Planung finden Sie unter [Überblick über den KI-Assistenten von Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).

* Der KI-Assistent ist derzeit nur auf Englisch verfügbar.


## Verfügbare Funktionen im KI-Assistenten

Der KI-Assistent bietet derzeit die folgenden Funktionen:

* Zusammenfassen von Projekten, Aufgaben, Problemen oder Dokumenten.

  Weitere Informationen finden Sie unter [Erstellen von Zusammenfassungen mithilfe des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Bereitstellung von Anweisungen oder Referenzinformationen aus der Workfront-Dokumentation auf Adobe Experience League.

  Weitere Informationen finden Sie unter [Anfordern von Hilfe beim KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Suche nach bestimmten Elementen in Workfront.

  Weitere Informationen finden Sie unter [Verwenden des KI-Assistenten für die Arbeit mit Projekten, Aufgaben und Problemen](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

* Generieren oder Optimieren von Formeln für berechnete benutzerdefinierte Felder.

  >[!NOTE]
  >
  >Diese Funktion steht nur Organisationen zur Verfügung, die über ein Prime- oder Ultimate-Abo von Workfront verfügen.

  Weitere Informationen finden Sie unter [Generieren oder Überarbeiten von Formeln für berechnete Felder mit dem KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

* Zusammenfassen von Aktualisierungen, hochgeladenen Dokumenten und anderen wichtigen Änderungen an Ihren Projekten innerhalb der folgenden Zeiträume: 24 Stunden, 3 Tage, 7 Tage in „Prioritäten“.

Weitere Informationen finden Sie unter [Aktuelle Informationen zur Arbeit in „Prioritäten“](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).


## Für den KI-Assistenten verfügbare Objekttypen

Der KI-Assistent kann Daten abfragen, die den folgenden Objekttypen zugeordnet sind, wenn der Benutzer bzw. die Benutzerin über die gültigen Berechtigungen in Workfront verfügt:

* Portfolios
* Programme
* Projekte
* Aufgaben
* Probleme
* Benutzerdefinierte Formulare
* Benutzende
* Einträge in Workfront-Planung


## Zugriff auf den KI-Assistenten

1. Klicken Sie oben auf einer beliebigen Workfront-Seite auf das Symbol „KI-Assistent“ (![Symbol „KI-Assistent“](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)).
1. Geben Sie Ihre Frage oder Ihren Prompt in das Panel auf der rechten Seite des Bildschirms ein.

   Wenn Sie in diesem Panel keine Eingabe vornehmen können, verfügt Ihre Organisation nicht über eine hinterlegte unterzeichnete Adobe GenAI-Vereinbarung.

1. Wenn Ihnen der KI-Assistent nicht die gewünschte Antwort liefert, verfeinern Sie Ihren Prompt und versuchen Sie es erneut.

## Unterzeichnen der Adobe GenAI-Vereinbarung

Wenn Ihre Organisation nicht über eine hinterlegte unterzeichnete Adobe GenAI-Vereinbarung verfügt, kann der KI-Assistent für Ihre Organisation nicht aktiviert werden.

Wenn ein Benutzer bzw. eine Benutzerin versucht, den KI-Assistenten zu verwenden, obwohl die Adobe GenAI-Vereinbarung nicht unterzeichnet wurde, wird eine Meldung angezeigt:

* Benutzende: Benutzende werden darüber informiert, dass der KI-Assistent für ihre Organisation nicht aktiviert wurde und sie sich an ihren bzw. ihre Workfront-Admin wenden können, um ihn für ihre Organisation anzufordern.
* Admins: Admins werden darüber informiert, dass keine unterzeichnete Adobe GenAI-Vereinbarung vorliegt, und können verlangen, dass eine Kopie der Vereinbarung zur Unterzeichnung gesendet wird.

So fordern Sie die Adobe GenAI-Vereinbarung an:

1. Klicken Sie als Workfront-Admin auf das Symbol „KI-Assistent“ (![Symbol „KI-Assistent“](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png)).
1. Beginnen Sie mit der Eingabe im Panel des KI-Assistenten.
1. Wenn die Meldung zur Adobe GenAI-Vereinbarung angezeigt wird, klicken Sie auf **Vereinbarung prüfen**.
1. Geben Sie den Namen und die E-Mail-Adresse der Person in Ihrer Organisation ein, die die Adobe GenAI-Vereinbarung unterzeichnen wird.

   Die Vereinbarung wird dieser Person zur Unterzeichnung übermittelt. Nachdem die Vereinbarung unterzeichnet und zurückgegeben wurde, wird sie von Adobe überprüft. Danach wird der KI-Assistent für Ihre Organisation aktiviert.

   >[!NOTE]
   >
   >Warten Sie nach der Unterzeichnung und Rückgabe der Vereinbarung 1–3 Werktage, damit Adobe den KI-Assistenten überprüfen und aktivieren kann.

## Tipps zum Erstellen von Prompts im KI-Assistenten

Verwenden Sie die folgenden Keywords in Ihren Prompts, um Kontext und Hilfe beim Auffinden der richtigen Informationen bereitzustellen. Bei Keywords wird nicht zwischen Groß- und Kleinschreibung unterschieden.

Geben Sie bei der Eingabe Ihres Prompts den folgenden Text ein: `using (keyword)`.

| Keyword | Ergebnis |
| --- | --- | 
| `workfront` | Interagiert mit Workfront. |
| `planning` | Interagiert mit Workfront-Planung. |
| `help` | Gibt Informationen aus der Experience League-Dokumentation zurück. |
| `formula` | Prüft Formeln zur Verwendung in Planung, Setup oder benutzerdefinierten Formularen und gibt sie zurück. |
| `health` | Überprüft den Zustand des Projekts mit dem Project Health Advisor. |
| `summarize` | Fasst Elemente zusammen, z. B. beim Hochladen einer Datei oder beim Zusammenfassen eines Projekts. |

>[!NOTE]
>
> Nicht alle Keywords sind in allen Bereichen verfügbar.
>
>* Das Keyword `formula` ist nur in Workfront-Planung, im Setup und im Builder für benutzerdefinierte Formulare verfügbar.
>* Das Keyword `planning` ist nur in Workfront-Planung verfügbar.





