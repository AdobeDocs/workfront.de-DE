---
title: Überblick über den KI-Assistenten
content-type: reference
description: Überblick über den KI-Assistenten
author: Becky
feature: Get Started with Workfront
exl-id: e5f2408b-2c29-4257-8bdc-bf20880de265
source-git-commit: d58088eed3c23652226f5d3f104705ed112c0b9f
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 1%

---

# Überblick über den KI-Assistenten

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist in der Vorschau -Umgebung für alle Kunden und in der Produktionsumgebung für Kunden verfügbar, die monatliche Versionen aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Der KI-Assistent von Workfront hilft Ihnen bei der Durchführung Ihrer Arbeit, indem er In-App-Informationen und -Vorschläge in einer Unterhaltung in natürlicher Sprache bereitstellt. Der KI-Assistent kann Ihnen ein reibungsloseres Arbeitserlebnis bieten durch

* Zusammenfassen von Arbeitselementen oder Dokumenten
* Suchen von Anweisungen oder Referenzmaterial für Arbeitsabläufe
* Formeln für berechnete Felder erzeugen oder überprüfen

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen für den KI-Assistenten

Um den KI-Assistenten für Ihre Organisation zu aktivieren **müssen** alle) der folgenden Bedingungen zutreffen:

* Ihr Unternehmen muss zu Adobe IMS (Identity Management System) migriert sein
* Adobe Unified Experience muss aktiviert sein
* Ihr Unternehmen muss über einen Select-, Prime- oder Ultimate Workfront-Plan verfügen
* Adobe muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben

  Weitere Informationen zur Unterzeichnung des Abkommens finden Sie unter [Unterzeichnung des Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement)Abkommens in diesem Artikel.

## Überlegungen zum KI-Assistenten

* Der KI-Assistent reagiert kontextabhängig auf die Seite, die Sie geöffnet haben. Wenn Sie beispielsweise auf einer Projektseite „Dieses Projekt zusammenfassen“ in den KI-Assistenten eingeben, wird eine Zusammenfassung dieses bestimmten Projekts zurückgegeben.
* Der Workfront-Administrator muss den KI-Assistenten für Benutzende in Ihrer Organisation aktivieren. Der KI-Assistent wird über Zugriffsebenen aktiviert.

  Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Der Workfront Planning AI Assistant verfügt über andere Funktionen als der Workfront AI Assistant.

  Weitere Informationen zum KI-Assistenten in Workfront Planning finden Sie unter [Übersicht zum Adobe Workfront Planning-KI-Assistenten](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).


## Verfügbare Funktionen im KI-Assistenten

Der KI-Assistent bietet derzeit die folgenden Funktionen:

* Zusammenfassen von Projekten, Aufgaben, Problemen oder Dokumenten.

  Weitere Informationen finden Sie unter [Zusammenfassen mithilfe des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Bereitstellung von Anweisungen oder Referenzinformationen aus der Workfront-Dokumentation auf Adobe Experience League.

  Weitere Informationen finden Sie unter [Hilfe vom KI-Assistenten abrufen](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

<div class="preview">

* Suchen nach bestimmten Elementen in Workfront.

  Weitere Informationen finden Sie unter [Verwenden des KI-Assistenten zur Arbeit mit Projekten, Aufgaben und Problemen](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

</div>

* Formeln für berechnete benutzerdefinierte Felder werden generiert oder verfeinert.

  >[!NOTE]
  >
  >Diese Funktion steht nur Organisationen zur Verfügung, die Prime- oder Ultimate Workfront-Pläne haben.

  Weitere Informationen finden Sie unter [Generieren oder Überarbeiten berechneter Feldformeln mit dem KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

<!--<div class="preview">
* Summarizing updates, uploaded documents, and other notable changes about your projects within the following time frames: 24 hours, 3 days, 7 days in Priorities.

For more information, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

</div>-->

## Für den KI-Assistenten verfügbare Objekttypen

Der KI-Assistent kann Daten abfragen, die den folgenden Objekttypen zugeordnet sind, wenn der Benutzer über die gültigen Berechtigungen in Workfront verfügt:

* Portfolios
* Programme
* Projekte
* Aufgaben
* Probleme
* Benutzerdefinierte Formulare
* Benutzende
* Workfront-Planungsdatensätze


## Zugriff auf KI-Assistenten

1. Klicken Sie oben auf einer Workfront-Seite auf das Symbol KI-Assistent ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Geben Sie Ihre Frage oder Eingabeaufforderung im Bedienfeld rechts am Bildschirm ein.

   Wenn Sie in dieses Bedienfeld nicht tippen können, verfügt Ihr Unternehmen über keine unterzeichnete Adobe Gen AI-Vereinbarung.

1. Wenn der KI-Assistent nicht die Antwort bereitstellt, die Sie benötigen, verfeinern Sie Ihre Eingabeaufforderung und versuchen Sie es erneut.

## Adobe Gen AI-Vertrag unterzeichnen

Wenn Ihr Unternehmen über keine unterzeichnete Adobe-Gen-KI-Vereinbarung verfügt, kann der KI-Assistent für Ihr Unternehmen nicht aktiviert werden.

Wenn ein(e) Benutzende(r) versucht, den KI-Assistenten zu verwenden, obwohl die Adobe-Gen-KI-Vereinbarung nicht unterzeichnet wurde, wird eine Meldung angezeigt:

* Benutzende: Benutzende werden darüber informiert, dass der KI-Assistent für ihr Unternehmen nicht aktiviert wurde und sie sich an ihren Workfront-Administrator wenden können, um ihn für ihr Unternehmen anzufordern.
* Administratoren: Administratoren werden darüber informiert, dass es keine unterzeichnete Adobe-Gen-AI-Vereinbarung gibt, und können verlangen, dass eine Kopie der Vereinbarung zur Unterzeichnung gesendet wird.

So fordern Sie die Adobe Gen AI-Vereinbarung an:

1. Klicken Sie als Workfront-Administrator auf das Symbol KI-Assistent ![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Beginnen Sie mit der Eingabe im Bedienfeld KI-Assistent .
1. Wenn die Adobe Gen AI-Vereinbarungsmeldung angezeigt wird, klicken Sie auf **Vereinbarung überprüfen**.
1. Geben Sie den Namen und die E-Mail-Adresse der Person in Ihrem Unternehmen ein, die die Adobe Gen AI-Vereinbarung unterzeichnen wird.

   Die Vereinbarung wird dieser Person zur Unterzeichnung übermittelt. Nachdem er signiert und zurückgegeben wurde, ist der KI-Assistent für Ihre Organisation aktiviert.
