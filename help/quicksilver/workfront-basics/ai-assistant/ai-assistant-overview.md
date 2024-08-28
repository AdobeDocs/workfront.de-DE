---
title: "Übersicht über KI-Assistenzkräfte"
content-type: reference
description: Übersicht über den KI-Assistenten
author: Becky
feature: Get Started with Workfront
source-git-commit: d261fd9eb9b8b649ebe413e35161543db1db8412
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Übersicht über den KI-Assistenten

>[!IMPORTANT]
>
>Der Workfront AI-Assistent wurde vorübergehend entfernt und steht zu einem späteren Zeitpunkt zur Verfügung.

Der KI-Assistent von Workfront hilft Ihnen bei der Erledigung Ihrer Arbeit, indem er In-App-Informationen und -Vorschläge in einem in natürlicher Sprache geführten Gespräch anbietet. Der KI-Assistent bietet Ihnen eine reibungslosere Arbeitserfahrung durch

* Zusammenfassung von Arbeitselementen oder Dokumenten
* Suchen von Anweisungen oder Referenzmaterial für Arbeitsabläufe
* Formeln für berechnete Felder erstellen oder überprüfen

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).## Voraussetzungen für den AI-Assistenten

Um den KI-Assistenten für Ihre Organisation zu aktivieren, muss **alle** der folgenden Punkte gelten:

* Ihr Unternehmen muss zu Adobe IMS (Identity Management System) migriert sein.
* Das Adobe Unified Experience muss aktiviert sein
* Ihr Unternehmen muss über einen Workfront-Plan für Select, Prime oder Ultimate verfügen
* Adobe muss über eine unterzeichnete Adobe Gen-AI-Vereinbarung verfügen.

  Weitere Informationen zum Unterzeichnen der Vereinbarung finden Sie unter [Unterschreiben der Adobe Gen AI Agreement](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) in diesem Artikel.

## Überlegungen zum KI-Assistenten

* Der KI-Assistent ist kontextsensitiv gegenüber der Seite, die Sie geöffnet haben. Wenn Sie beispielsweise &quot;Projekt zusammenfassen&quot;in den KI-Assistenten auf einer Projektseite eingeben, erhalten Sie eine Zusammenfassung dieses spezifischen Projekts.
* Der Workfront-Administrator muss den KI-Assistenten für Benutzer in Ihrem Unternehmen aktivieren. Die Aktivierung des KI-Assistenten erfolgt über Zugriffsebenen.

  Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des AI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* Der Workfront Planning AI Assistant verfügt über andere Funktionen als der Workfront AI Assistant.

  Weitere Informationen zum KI-Assistenten in der Workfront-Planung finden Sie unter [Übersicht über den Adobe Workfront Planning AI Assistant - Überblick](/help/quicksilver/planning/general/planning-ai-assistant-overview.md).


## In AI Assistant verfügbare Funktionen

Der KI-Assistent bietet derzeit die folgenden Funktionen:

* Zusammenfassen von Projekten, Aufgaben, Problemen oder Dokumenten.

  Weitere Informationen finden Sie unter [Zusammenfassen mit dem AI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

* Bereitstellung von Anweisungen oder Referenzinformationen, die aus der Workfront-Dokumentation in Adobe Experience League abgerufen werden.

  Weitere Informationen finden Sie unter [Hilfe vom AI-Assistenten erhalten](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

* Erstellen oder verfeinern Sie Formeln für berechnete benutzerdefinierte Felder.

  >[!NOTE]
  >
  >Diese Funktion steht nur Unternehmen zur Verfügung, die die Pläne von Prime oder Ultimate Workfront verfolgen.

  Weitere Informationen finden Sie unter [Berechnete Feldformeln mit dem KI-Assistenten erstellen oder überarbeiten](/help/quicksilver/workfront-basics/ai-assistant/use-ai-assistant-to-check-formulas.md).

## Access AI Assistant

1. Klicken Sie oben auf einer beliebigen Workfront-Seite auf das Symbol &quot;AI Assistant&quot;![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Geben Sie Ihre Frage oder Aufforderung in das Bedienfeld rechts vom Bildschirm ein.

   Wenn Sie in dieses Bedienfeld nicht eingeben können, verfügt Ihr Unternehmen nicht über eine unterzeichnete Adobe Gen-KI-Vereinbarung für die Datei.

1. Wenn der KI-Assistent nicht die benötigte Antwort bereitstellt, verfeinern Sie Ihre Eingabeaufforderung und versuchen Sie es erneut.

## Unterschreiben der Adobe Gen AI-Vereinbarung

Wenn Ihr Unternehmen über keine unterzeichnete Adobe Gen-KI-Vereinbarung zur -Datei verfügt, kann der KI-Assistent für Ihr Unternehmen nicht aktiviert werden.

Wenn ein Benutzer versucht, AI Assistant zu verwenden, wenn die Adobe Gen AI-Vereinbarung nicht unterzeichnet wurde, wird ihm eine Meldung angezeigt:

* Benutzer: Benutzer werden darüber informiert, dass der KI-Assistent für ihre Organisation nicht aktiviert wurde und dass sie sich an ihren Workfront-Administrator wenden können, um ihn für ihre Organisation anzufordern.
* Administratoren: Administratoren werden darüber informiert, dass keine unterzeichnete Adobe Gen AI-Vereinbarung vorliegt, und können verlangen, dass eine Kopie der Vereinbarung zur Unterzeichnung gesendet wird.

So fordern Sie die Adobe Gen AI-Vereinbarung an:

1. Als Workfront-Administrator klicken Sie auf das Symbol &quot;KI-Assistent&quot;![](/help/quicksilver/workfront-basics/ai-assistant/assets/ai-assistant-icon.png).
1. Beginnen Sie mit der Eingabe im Bedienfeld &quot;AI Assistant&quot;.
1. Wenn die Meldung zur Adobe Gen AI Agreement (KI-Vereinbarung) angezeigt wird, klicken Sie auf **Review Agreement (Vereinbarung überprüfen)**.
1. Geben Sie den Namen und die E-Mail-Adresse der Person in Ihrem Unternehmen ein, die die Adobe Gen AI-Vereinbarung unterzeichnet.

   Die Vereinbarung wird dieser Person zur Unterzeichnung übermittelt. Nach der Unterzeichnung und Rückgabe wird der KI-Assistent für Ihre Organisation aktiviert.

