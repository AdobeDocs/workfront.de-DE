---
product-area: betas
navigation-topic: new-commenting-experience-beta
title: Neues Kommentierungserlebnis
description: Eine Aktualisierung der Kommentierungserfahrung in Adobe Workfront befindet sich derzeit in der Entwicklung. Dieses Update umfasst eine neue Benutzeroberfläche, neue Funktionen und eine verbesserte Leistung im Abschnitt Updates von ausgewählten Objekten.
author: Alina
feature: Product Announcements
role: User
exl-id: f750b35b-8021-4cc1-81d6-e1ece2530438
source-git-commit: 980e6c2cea2ceb98abda6b98811e734d895ad274
workflow-type: tm+mt
source-wordcount: '1317'
ht-degree: 2%

---

# Neues Kommentierungserlebnis

<!--take out legacy, preview, prod references from below-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.  </span>  

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](../../product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>-->

<!--

After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases.

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>  -->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Funktionen, die für das neue Kommentierungserlebnis veröffentlicht wurden.
>
>Das Betaprogramm für die neue Kommentarerfahrung begann im April 2023 und endete im Oktober 2023. Das Betaprogramm für die neue Kommentarerfahrung wurde mit der Version vom Oktober 2023 eingestellt.
>
>Ab Oktober 2023 werden alle neuen Funktionen für das neue Kommentierungserlebnis für alle Kunden veröffentlicht. Weitere Informationen finden Sie auf der aktuellen Übersichtsseite zur Version für jede Version.

<!--An update to the commenting experience in Adobe Workfront is currently in development. This update includes a new interface, new features, and improved performance in the Updates section of select objects. 

The new commenting experience will slowly become available for all the objects with an Updates section in Workfront, and later it will expand to other Adobe Experience Cloud applications.-->

<!--For additional resources for the new commenting experience, also see the following articles:

* [New commenting experience release activity](../new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md)
* [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md)
-->

## Funktionen

Das neue Kommentierungserlebnis umfasst Verbesserungen und Änderungen am Abschnitt &quot;Aktualisierungen&quot;von Adobe Workfront-Objekten.

Zu den Verbesserungen im neuen Kommentarerlebnis gehören die folgenden:

* Verbesserte Leistung und Benutzerfreundlichkeit
* Trennung von Benutzerkommentaren und Aktualisierungen der Systemaktivität
* Echtzeitanzeige beim Hinzufügen neuer Kommentare zu einem Objekt
* Kommentare nach dem Senden bearbeiten

Die folgenden Funktionen wurden entfernt oder werden aus dem neuen Erlebnis entfernt:

* Kommentar zu einer Systemaktualisierung
* Möglichkeit, Status, Bedingung, Datum der Übertragung und Prozentsatz der Fertigstellung zu bearbeiten, während Sie zu Aufgaben und Problemen kommentieren
* Benutzerdefiniertes Formular bearbeiten
* Die Informationen &quot;im Namen von &lt; Benutzername >&quot;, wenn sich ein Workfront- oder Gruppenadministrator als anderer Benutzer anmeldet und einen Kommentar in seinem Namen hinzufügt, wurden ursprünglich entfernt. Es wurde am 19. Oktober 2023 wieder eingesetzt.
* Die Option &quot;Zur Genehmigung anfordern&quot;, wenn Sie Personen taggen, während Sie einem Dokument einen Kommentar hinzufügen.
* Die Einstellung &quot;Prozentualer Abschluss bei Aktualisierungsstatus anzeigen&quot;beim Bearbeiten des Profilfelds eines Benutzers wird entfernt. Die Funktion zum Aktualisieren des prozentualen Abschlusses einer Aufgabe oder eines Problems wurde entfernt.
* Die Benachrichtigung für den Projekteigentümer im Bereich Updates, dass der Verantwortliche einer Aufgabe oder eines Problems das Commitdatum bearbeitet hat <!--ensure this is correct when re remove the legacy and leave only new commenting-->

<!--removed this note on November 28, 2023, when this limitation was removed: 

>[!NOTE]
>
>The objects listed below have only the comments and system updates starting with January 1, 2019 available in the new commenting experience.  
>
>You can view comments and system updates on these objects prior to January 1, 2019 when viewing the Updates section in the current experience:
>
>* Issues
>* Projects
>* Tasks
>* Documents

For more information, see the [New commenting experience FAQs](../../betas/new-commenting-experience-beta/new-commenting-faq.md). 
-->

Die folgende Tabelle zeigt die Funktionen, die im neuen Kommentierungserlebnis verfügbar sein werden, sowie ihre Verfügbarkeit in den Bereichen, in denen sie unterstützt werden:

<table>
  <tr>
   <td><strong>Funktion </strong>
   </td>
   <td><strong>Existiert in alten Kommentierungserlebnissen </strong>
   </td>
   <td><strong>Existiert im neuen Kommentierungserlebnis </strong>
   </td>
   <td><strong>Wird in das neue Kommentierungserlebnis eingeführt </strong>
   </td>
   <td><strong>Wann wird in das neue Kommentierungserlebnis eingeführt? </strong>
   </td>
   <td><strong>Forschung </strong>
   </td>
  </tr>
  <tr>
   <td>Kommentare erstellen/lesen/beantworten/löschen 
   </td>
   <td>✓ 
  </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Rich-Text (ohne Anführungszeichen und Emojis)
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Rich-Text (Emojis)
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Rich-Text (Blockzitate)
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2. Quartal 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>
<tr>
   <td> Kommentare einfügen
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 2. Quartal 2023
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Antworten auf Kommentare (Gefällt mir) 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Bilder an Kommentare anhängen 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Personen in Kommentaren taggen 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Entfernen von Thread-Teilnehmern
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>


<tr>
   <td>Automatisch alle Thread-Teilnehmer taggen
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Kommentare, die für ein Unternehmen privat sind 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Veröffentlichung eines Kommentars rückgängig machen 
   </td>
   <td>✓ 
   </td>
   <td>Ersetzt durch Bearbeitungskommentar 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Systemaktualisierungen deaktivieren 
   </td>
   <td>✓ 
   </td>
   <td>Ersetzt durch die Registerkarte Aktivität . 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Kommentare bearbeiten 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Kommentarentwürfe speichern, wenn Sie von der Seite weg navigieren 
   </td>
   <td>✓ 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Anzeigen neuer Kommentare in Echtzeit (einschließlich der Anzeige, wenn ein Kommentar gelöscht wird)
   </td>
   <td> 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Zeit erfassen 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>Thread-Link kopieren 
   </td>
   <td>✓ 
   </td>
   <td> Ersetzt durch Link "Kopieren"
   </td>
   <td> 
   </td>
   <td>2. Quartal 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Kommentarlink kopieren 
   </td>
   <td>✓ 
   </td>
   <td> Ersetzt durch Link "Kopieren"
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Kommentartext zitieren 
   </td>
   <td>✓ 
   </td>
   <td>✓
   </td>
   <td> 
   </td>
   <td>2. Quartal 2023 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Fließtext kopieren 
   </td>
   <td>✓ 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
    <tr>
   <td>In Kommentaren suchen 
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1. Quartal 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Bilder in Kommentare kopieren und einfügen
   </td>
   <td> 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1. Quartal 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Verschieben von Bildern in einen Kommentar
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>1. Quartal 2024 
   </td>
   <td> 
   </td>
  </tr>

<tr>
   <td>Benutzerdefiniertes Formular bearbeiten 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
  </tr>
  <tr>
   <td>Möglichkeit, Status, Bedingung, Commit-Datum beim Kommentieren zu bearbeiten 
   </td>
   <td>✓ 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
  </tr>
<tr>
   <td>Antworten auf Systemaktualisierungen 
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
<tr>
   <td>Anzeigen von "im Namen von", wenn Kommentare hinzugefügt werden, die als ein anderer Benutzer angemeldet sind
   </td>
   <td> ✓
   </td>
   <td> ✓
   </td>
   <td> 
   </td>
   <td>
   </td>
   <td> 
   </td>
  </tr>
</table>

## Veröffentlichungs-Timeline

>[!IMPORTANT]
>
>Informationen zu den Funktionen, die während des Beta-Zeitraums für das neue Kommentar-Erlebnis veröffentlicht wurden, finden Sie unter [Neue Kommentar-Erlebnis-Release-Aktivität](../../betas/new-commenting-experience-beta/new-commenting-beta-experience-release-activity.md).
>
>Weitere Informationen zum Verwalten von Aktualisierungen für Workfront-Objekte finden Sie unter [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).


Im Folgenden finden Sie einen geplanten Zeitplan mit wichtigen Meilensteinen für die Veröffentlichung des neuen Kommentierungserlebnisses in der Produktionsumgebung. Zusätzlich zu den unten stehenden Meilensteinen werden wir das Kommentierungserlebnis mit kleineren Verbesserungen weiter verbessern.

Informationen zu den Funktionen, die nach dem Schließen der Beta-Phase für das neue Kommentar-Erlebnis veröffentlicht wurden, finden Sie auf der Seite mit der aktuellen Versionsübersicht .

Im Folgenden finden Sie einen geplanten Zeitplan für die Veröffentlichung des neuen Kommentierungserlebnisses:

* Mit der Version 23.2 (6. April 2023):
   * Starten des Kommentierungserlebnisses Beta für Probleme
   * Das neue Kommentarerlebnis für Ziele freigeben (als einziges Erlebnis)
* Mit der Version 23.3 (20. Juli 2023):
   * Starten Sie die Beta-Kommentarfunktion für Projekte, Aufgaben und Dokumente.
   * Das neue Kommentarerlebnis für Karten im Bereich &quot;Foren&quot;freigeben (als einziges Erlebnis)
* In der Version vom vierten Quartal 2023 (begrenzte Version, nur für Kunden verfügbar, die die schnelle Version wählen):
   * Das neue Kommentierungserlebnis für Vorlagen, Vorlagenaufgaben, Programme, Portfolios, Teams, Benutzer und Timesheets freigeben (als einziges Erlebnis)
   * Aktualisieren Sie die Beta-Kommentarfunktion für Projekte, Aufgaben, Probleme und Dokumente, sodass sie zur Standardoption wird. Die Bezeichnung &quot;Beta&quot;wurde entfernt.
* Mit der Version vom 26. Quartal 2023 (23.10) (26. Oktober 2023)
   * Veröffentlichen Sie die neue Kommentarfunktion für Vorlagen, Vorlagenaufgaben, Programme, Portfolios, Teams, Benutzer und Timesheets (als einziges Erlebnis) für alle Kunden.
   * Machen Sie die neue Kommentarfunktion für Projekte, Aufgaben, Probleme und Dokumente zur Standardoption.

  >[!IMPORTANT]
  >
  >    Dadurch wird die Beta-Phase der neuen Kommentarerfahrung abgeschlossen.

   * Machen Sie alle Funktionen, die für das neue Kommentierungserlebnis veröffentlicht werden, von diesem Datum an Teil der aktuellen regulären monatlichen und vierteljährlichen Versionen.
* Ende 2023:
   * Behalten Sie die alte Kommentarfunktion als sekundäre Option für die folgenden Objekte bei: Projekte, Aufgaben, Probleme und Dokumente. Die neue Kommentarfunktion ist die Standardoption für alle Benutzer dieser Objekte.
   * Machen Sie das neue Kommentierungserlebnis zum einzigen Erlebnis für alle anderen Objekte.

  >[!NOTE]
  >
  >    Iterationen verfügen weiterhin über das alte Kommentierungserlebnis. Das neue Kommentarerlebnis steht nicht für Iterationen zur Verfügung.

* Zweites Quartal 2024 (April 2024):

   * Entfernen Sie die Option, um zum alten Kommentar-Stream zurückzukehren und den neuen Kommentar-Stream zum einzigen Erlebnis für alle Objekte mit Ausnahme von Iterationen zu machen.

## Neues Kommentierungserlebnis suchen

&lt;!—WICHTIG: Wenn wir das veraltete Erlebnis loswerden, verschieben Sie eine Version davon in den Arbeitsartikel Aktualisieren oder die Übersicht des Aktualisierungsabschnitts - um zu sagen, dass das Erlebnis für alle außer für Iterationen unterschiedlich ist—>

Die neue Kommentarfunktion ist derzeit für alle Kunden und für alle Umgebungen verfügbar.

Je nachdem, für welche Objekte Sie auf das Kommentierungserlebnis zugreifen, sehen Sie möglicherweise die folgende Funktion für den Abschnitt Aktualisierungen :

* Sowohl das neue als auch das alte Kommentierungserlebnis für die folgenden Objekte:

   * Projekt
   * Aufgabe (einschließlich Meldungen)
   * Problem
   * Dokument

  >[!TIP]
  >
  >Verwenden Sie die Option Neue Kommentare , um das neue Kommentarerlebnis (wenn Sie es aktivieren) oder das veraltete Kommentarerlebnis (wenn Sie es deaktivieren) anzuzeigen, wie in diesem Abschnitt beschrieben. Die neue Kommentarfunktion ist die Standardeinstellung.

   * Nur das neue Kommentarerlebnis für die unten aufgeführten Objekte. Es gibt keine Option, das veraltete Kommentierungserlebnis für diese Objekte zu aktivieren:

      * Ziel

     >[!NOTE]
     >
     >Sie müssen über eine zusätzliche Lizenz für Adobe Workfront Goals verfügen, um auf diesen Bereich von Workfront zugreifen zu können. Weitere Informationen finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
      * Karte auf einer Pinnwand
      * Team
      * Vorlage
      * Vorlagenaufgabe
      * Arbeitszeittabelle
      * Programm
      * Portfolio
      * Benutzerin oder Benutzer

* Nur das veraltete Kommentierungserlebnis für die folgenden Objekte:

   * Wiederholungen

     Es gibt keine Option, das neue Kommentarerlebnis für Iterationen zu aktivieren. Für Iterationen ist nur das veraltete Kommentierungserlebnis verfügbar.


<!--before August 17: 

The new commenting experience is currently supported for the following objects:


* When enabling the Beta experience in the Updates section for 

    * Issues, projects, tasks, and documents

    For more information about managing updates for Workfront objects, see [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). 

* By default, as the only commenting experience for

    * Goals, cards on a board

    >[!NOTE]
    >
    >You must have an additional license to Adobe Workfront Goals to be able to access this area of Workfront. For more information, see [Requirements to use Workfront Goals](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

-->

<!--Depending on the environment you access the commenting experience you can do one of the following: 

* Enable the commenting experience Beta in the Production environment
* <span class="preview">Enable the legacy commenting experience in the Preview  environment </span>
-->

So aktivieren Sie die Kommentarerlebnis-Option für Projekte, Aufgaben, Probleme und Dokumente:

1. Markieren Sie ein Objekt, für das Sie das neue Kommentierungserlebnis aktivieren möchten, und klicken Sie auf **Updates** im linken Bereich.
1. (Bedingt) Wenn sie deaktiviert ist, aktivieren Sie die **Neue Kommentare** in der oberen rechten Ecke des Bereichs Updates , um sie zu aktivieren. Dies sollte standardmäßig aktiviert sein.

   ![](assets/new-commenting-toggle-off-highlighted.png)

1. Beginnen Sie mit der Eingabe eines Updates in die **Kommentare** Registerkarte. Die Registerkarte Kommentare ist die Standardregisterkarte beim Öffnen des neuen Erlebnisses.

   Oder

   Klicken Sie auf  **Systemaktivität** um die von Workfront erzeugten Aktivitätsaktualisierungen anzuzeigen.

1. (Optional) Um das neue Kommentarerlebnis zu deaktivieren und zur alten Kommentarfunktion zurückzukehren, deaktivieren Sie die Option **Neue Kommentare** -Option.

