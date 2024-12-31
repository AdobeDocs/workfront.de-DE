---
title: Versionsübersicht 22.3
description: Versionsübersicht 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bfc7ce9e-b715-47b7-bab7-2e3540d0da3e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3220'
ht-degree: 0%

---

# Versionsübersicht 22.3

Diese Seite enthält Informationen zur Funktionalität, die in der Version 22.3 enthalten ist. Alle aufgelisteten Funktionen sind in der neuen Adobe Workfront-Version verfügbar. Einige Funktionen sind auch in Adobe Workfront Classic verfügbar. [Workfront Classic wird jedoch im März 2022 eingestellt](https://one.workfront.com/s/new-workfront-experience) kurz darauf folgt das Ende der Nutzungsdauer von Workfront Classic im Juli 2022.

Diese Verbesserungen wurden in der Woche vom 11. Juli 2022 in der Produktionsumgebung verfügbar gemacht.

## Adobe Workfront-Verbesserungen

* [Verbesserungen für Administratoren](#administrator-enhancements)
* [Projektverbesserungen](#project-enhancements)
* [Verbesserungen beim Ressourcen-Management](#resource-management-enhancements)
* [Verbesserungen beim Reporting](#reporting-enhancements)
* [Integrationsverbesserungen](#integration-enhancements)
* [Verbesserungen für Mobilgeräte](#mobile-enhancements)
* [Weitere Verbesserungen](#other-enhancements)

### Administrator-Verbesserungen {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Integrieren von Adobe Workfront mit JumpSeat
</a></p></p> <p>Sie können JumpSeat jetzt mit Workfront integrieren, um benutzerdefinierte, produktinterne Anleitungen für Ihre Benutzerinnen und Benutzer zu erstellen. Sie müssen über eine Adobe Workfront Enterprise-Lizenz und ein aktives JumpSeat-Abonnement verfügen, um die Integration zu aktivieren.</p>  
    </td>
    <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 2. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Verwenden entsperrter Status in einem Genehmigungsprozess
</a></p></p> <p>Diese Funktion wurde aus der Produktionsversion 22.3 entfernt. Diese Funktion soll zu einem späteren Zeitpunkt in der Produktion veröffentlicht werden.</p> 
<p>Um Ihnen mehr Kontrolle über die Genehmigungsprozesse und -status in Ihrem System zu geben, haben wir es ermöglicht, einen Genehmigungsprozess basierend auf einem entsperrten Systemstatus zu erstellen. Darüber hinaus können Sie jetzt jeden Status entsperren, der bereits in einem Genehmigungsprozess verwendet wird. Zuvor musste ein in einem Genehmigungsprozess verwendeter Systemstatus gesperrt werden. Dadurch war sie für alle Gruppen verfügbar - ohne die Möglichkeit, sie zu entfernen oder umzubenennen -, sodass Gruppenadministratoren die Statusliste ihrer Gruppe nicht an ihre spezifischen Anforderungen anpassen konnten.</p>   
   </td> 
    <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 2. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: 15. September 2022</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Standardeinstellungen für Korrekturabzüge wurden in Workfront verschoben
</a></p></p> <p>Sie können jetzt die folgenden Korrekturabzugseinstellungen im Workfront-Setup-Bereich bearbeiten:</p> 
<ul>
   <li><p>Standardeinstellungen für Korrekturabzüge</p></li>
   <li><p>Einstellungen für Korrekturabzugsentscheidungen</p></li>
   </ul> 
   </td> 
    <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 1. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Hinzufügen einer PDF-Datei zu einem benutzerdefinierten Formular
</a></p></p> <p>Wir helfen Ihnen auch weiterhin dabei, benutzerdefinierte Formulare visuell und informativer zu gestalten, indem Sie neue Asset-Widgets hinzufügen können, z. B. Bilder und Videos. Jetzt können Sie einem benutzerdefinierten Formular einen Link zu einer PDF-Datei hinzufügen. Wenn das Formular an ein Objekt angehängt ist, können Benutzende, die mit dem Objekt arbeiten, das PDF im Formular anzeigen und damit interagieren.</p>
   </td> 
    <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 2. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Editor zur Berechnung von benutzerdefinierten Formularfeldern zeigt Fehlerinformationen an
</a><span style="color: #ff0000; font-weight: bold;"> (vorübergehend nicht verfügbar)</span></p></p> <p>Die Bearbeitung von Berechnungen für benutzerdefinierte Felder ist jetzt einfacher, da hilfreiche Fehlerinformationen direkt in der Berechnung angezeigt werden. Beim Erstellen eines berechneten Felds in einem benutzerdefinierten Formular werden Fehler in rosa hervorgehoben. Wenn Sie den Mauszeiger über den hervorgehobenen Teil bewegen, wird eine QuickInfo angezeigt, die das Problem beschreibt.</p>
    </td> 
    <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 9. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Anpassung des Projekt-Headers
</a></p></p> <p>Als Workfront- oder Gruppenadministrator bzw. -administratorin können Sie jetzt die Felder anpassen, die in der Kopfzeile eines Projekts angezeigt werden, wenn Sie eine Layout-Vorlage verwenden.</p>
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
    <td>
    <ul> 
     <li> <p>Vorschau der Version: 2. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
   </td>
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Steuerelement zum Erstellen eines leeren Projekts</a></p></p> <p>Als System- oder Gruppenadministrator können Sie jetzt steuern, ob Benutzer leere Projekte erstellen können, ohne eine Vorlage zu verwenden. Im Bereich Projektvoreinstellungen von Setup wurde eine neue Einstellung eingeführt, mit der Sie die Erstellung leerer Projekte in den folgenden Bereichen deaktivieren können:</p> 
   <ul>
   <li><p>über die Option Neues Projekt in einer Projektliste</p></li>
   <li><p>Bei der Konvertierung einer Anfrage in ein Projekt über die Anfrageseite</p></li>
   </ul>
   <p>Die neue Einstellung ist „Benutzern erlauben, Projekte ohne Vorlage zu erstellen“ und sie ist standardmäßig aktiviert.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 19. Mai 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3 </p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Deaktivieren einer Gruppe auf der Seite „Gruppen“</a> </p> <p>Kürzlich haben wir die Möglichkeit hinzugefügt, Gruppen zu deaktivieren und zu reaktivieren. Um diese Aktion zu beschleunigen und zu vereinfachen, wurde sie zur Seite einer Gruppe hinzugefügt. Nachdem Sie nun auf den Namen einer Gruppe geklickt haben, um zu ihrer Seite zu gelangen, können Sie das Menü Mehr <img src="assets/more-icon.png"> neben dem Namen der Gruppe auswählen und auf Deaktivieren oder Reaktivieren klicken.</p> <p>Zuvor konnten Sie eine Gruppe nur mithilfe des Kontrollkästchens Ist aktiv auf ihrer Detailseite deaktivieren oder reaktivieren. </p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 14. April 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3 </p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-admin-enhancements.md" class="MCXref xref" xrefformat="{para}">Hinzufügen von Videos zu benutzerdefinierten Formularen</a> </p> <p>Jetzt können Sie einem benutzerdefinierten Formular einen neuen Modus für Informationen, visuelles Interesse und Kreativität bereitstellen, indem Sie ein Video hinzufügen. Wenn das Formular mit einem Objekt verbunden ist, können Benutzende, die mit dem Objekt arbeiten, das Video jederzeit abspielen.</p> <p>Zuvor konnten Sie nur textbasierte Felder und Bilder zu einem benutzerdefinierten Formular hinzufügen.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 14. April 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3 </p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projektverbesserungen {#project-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Delegation von Abwesenheitsarbeiten</a></p> <p>Jetzt können Sie die Ihnen zugewiesenen Aufgaben und Probleme vorübergehend an andere Benutzer delegieren, wenn Sie für einen kurzen Zeitraum abwesend sein möchten. Dadurch wird sichergestellt, dass Ihre Abwesenheit nicht zu einer Hürde für die Fertigstellung wird.</p> 
   <p>Vor dieser Verbesserung konnten Sie nur Genehmigungen delegieren.</p></td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 9. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Neues Erlebnis beim Konvertieren eines Problems in eine Aufgabe</a></p> <p>Damit Ihre Verwendung von Workfront mit der neuen Workfront-Version konsistent ist, haben wir die Benutzeroberfläche zum Konvertieren eines Problems in eine Aufgabe neu gestaltet.</p> 
   </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 9. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Neues Erlebnis beim Konvertieren eines Problems in ein Projekt ohne Vorlage</a></p> <p>Um die Verwendung von Workfront mit der neuen Workfront-Version konsistent zu machen, haben wir die Benutzeroberfläche zum Konvertieren eines Problems in ein Projekt ohne Verwendung einer Vorlage neu gestaltet.</p> 
   <p>Zusätzlich zu der aktualisierten Benutzeroberfläche, die der neuen Workfront-Version entspricht, haben wir auch die Möglichkeit hinzugefügt, ein Problem aus einer Liste oder einem Bericht in leere Projekte zu konvertieren.</p></td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 2. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr>
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Smart-Tagging im Aktualisierungsverlauf</a></p> <p>Wir haben das Tagging von Benutzern im Aktualisierungsverlauf verbessert, wenn Sie eine neue Aktualisierung erstellen oder auf eine vorhandene antworten. Wenn Sie einen Benutzer taggen, um ihn in ein Update aufzunehmen, zeigen wir neben seinem Namen und Avatar auch seine Primäre Rolle und seine E-Mail-Adresse an. Dies hilft bei der Unterscheidung zwischen mehreren Benutzenden mit ähnlichen oder identischen Namen.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 19. Mai 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Neue Syntax für Berechnungen in benutzerdefinierten Feldern</a> </p> <p>Um uns auf zukünftige Verbesserungen vorzubereiten, die Ihnen beim Hinzufügen von Berechnungen zu benutzerdefinierten Formularen helfen, haben wir die Syntax für referenzierte Felder standardisiert, die Sie zu einer Berechnung hinzufügen. Diese neue Syntax ist einfach zu verwenden, da das System sie für Sie eingibt, wenn Sie mit der Eingabe des Namens eines Felds beginnen und es dann auswählen.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 5. Mai 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Halten Sie genaue Informationen bereit, wenn zwei Benutzer mit einer gemeinsamen Rolle an einem Genehmigungsprozess beteiligt sind</a> </p> <p>Um die Richtigkeit Ihrer Daten für die Validierung von Arbeiten sicherzustellen, haben wir die Art und Weise geändert, wie Validierungsinformationen für einen Artikel aufgezeichnet werden, wenn dem Artikel ein Prozess mit mehreren Rollen zugeordnet ist.</p> <p>Einige Genehmigungsprozesse erfordern die Genehmigung von zwei verschiedenen Rollen, und zwei verschiedene genehmigende Personen können eine dieser Rollen gemeinsam haben. Wenn dies passiert, nachdem die Genehmigungsentscheidungen getroffen wurden, zeichnet Workfront jede genehmigende Person und ihre jeweilige Rolle auf, die mit dem Genehmigungsprozess verknüpft ist.</p> <p>Vor dieser Änderung wurden beide Genehmigungen für den zweiten Benutzer aufgezeichnet, da er eine der Genehmigungsrollen mit der ersten genehmigenden Person teilte. In diesem Fall hat die zweite genehmigende Person die Informationen der ersten genehmigenden Person überschrieben.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 21. April 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic wurde im März 2022 eingestellt</a> kurz darauf folgte das Ende der Nutzungsdauer von Workfront Classic im Juli 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Neue Erfahrung beim Konvertieren eines Problems in ein Projekt mithilfe einer Vorlage auf Anfrageebene</a> </p> <p>Um die Verwendung von Workfront mit der neuen Workfront-Version konsistent zu machen, haben wir die Benutzeroberfläche zum Konvertieren eines Problems in ein Projekt neu gestaltet, wenn eine Vorlage über die Anfrageseite konvertiert wird.</p> <p>Sie können jetzt direkt nach der Auswahl, das Problem zu konvertieren, einfacher auf Ihre Favoritenliste zugreifen.</p> <p>Die neu gestaltete Benutzeroberfläche entspricht dem Erlebnis, wenn Sie ein Projekt aus einer Vorlage erstellen, die wir kürzlich ebenfalls aktualisiert haben.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> 
    <ul> 
     <li> <p>Vorschau-Version: 8. Dezember 2021<br></p> </li> 
     <li> <p>Produktionsversion: Schrittweiser Rollout ab 28. April 2022 <span style="color: #ff0000; font-weight: bold;">Diese Funktion wurde am 4. März 2022 vorübergehend aus der Produktionsumgebung entfernt. Später wurde es ab dem 28. April 2022 im Rahmen eines schrittweisen Rollouts veröffentlicht. Der Rollout wurde am 5. Mai 2022 abgeschlossen. Dies ist jetzt für alle Kunden in der Vorschau und Produktion verfügbar.</span></p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.1-release-activity/22-1-project-enhancements.md#convert" class="MCXref xref" xrefformat="{para}">Konvertieren von Problemen in Projekte mithilfe einer Vorlage aus Listen, Berichten und Dashboards</a> </p> <p>Um Ihre Arbeit effizienter zu gestalten und Ihnen das Konvertieren von Problemen in einer schnelllebigen Umgebung zu erleichtern, haben wir die Möglichkeit hinzugefügt, ein Problem mithilfe einer Vorlage aus einer Liste, einem Bericht oder einem Dashboard in ein Projekt zu konvertieren.</p> <p>Vor dieser Verbesserung gab es diese Funktion nur, wenn Sie das Problem auf der Anfrageseite konvertierten.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> 
    <ul> 
     <li> <p>Vorschau-Version: 8. Dezember 2021<br></p> </li> 
     <li> <p>Produktionsversion: Schrittweiser Rollout ab 28. April 2022 <span style="color: #ff0000; font-weight: bold;">Diese Funktion wurde am 4. März 2022 vorübergehend aus der Produktionsumgebung entfernt. Später wurde es ab dem 28. April 2022 im Rahmen eines schrittweisen Rollouts veröffentlicht. Der Rollout wurde am 5. Mai 2022 abgeschlossen. Dies ist jetzt für alle Kunden in der Vorschau und Produktion verfügbar.</span></p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#allocati" class="MCXref xref" xrefformat="{para}">Zuordnungsstunden werden bei Änderungen an Zuweisungen nicht mehr entfernt</a> </p> <p>Um die Genauigkeit Ihrer Daten zu gewährleisten, haben wir eine Änderung vorgenommen, um die Zuordnungsstunden beizubehalten und die geplanten Stunden für Aufgaben unverändert zu lassen, wenn Änderungen an Zuweisungen für die Aufgabe vorgenommen werden.</p> <p>Die folgenden Änderungen wurden an Aufgaben mit dem Typ Einfache Dauer vorgenommen:</p> 
    <ul> 
     <li> <p>Einzelne Zuweisungen bleiben beim Ersetzen von Benutzern und Rollen erhalten.</p> </li> 
     <li> <p>Einzelne Zuweisungen bleiben bei der Rolle erhalten, wenn Benutzer entfernt werden.</p> </li> 
    </ul> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> 
    <ul> 
     <li> <p>Vorschau der Version: 10. Februar 2022<br></p> </li> 
     <li> <p>Produktionsversion: 21. April 2022 </p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic wurde im März 2022 eingestellt</a> kurz darauf folgte das Ende der Nutzungsdauer von Workfront Classic im Juli 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.2-release-activity/22-2-project-enhancements.md#share" class="MCXref xref" xrefformat="{para}">Freigeben von Ordnern nur in den obersten fünf Ebenen einer Ordnerhierarchie</a> (Dies verweist auf die Versionshinweise zu 20.2, als diese Funktion zum ersten Mal in der Vorschau eingeführt wurde.)</p> <p>Um eine optimale Leistung für Benutzer zu gewährleisten, die Ordner freigeben, beschränken wir die Freigabe derzeit auf die fünf obersten Ebenen in einer Ordnerhierarchie für ein Objekt.</p> <p>Jeder Ordner auf der sechsten Ebene oder darunter erbt seine Freigabekonfigurationen von dem Ordner direkt darüber.</p> </td> 
   <td><strong>Verfügbar zu diesen Daten:</strong> 
    <ul> 
     <li> <p>Vorschau der Version: 10. Februar 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.2 <span style="color: #ff0000; font-weight: bold;">Diese Funktion ist vorübergehend nicht verfügbar. Diese Seite wird aktualisiert, wenn die Funktion in der Produktionsumgebung verfügbar ist.</span></p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
     <li> <p>Adobe Workfront Classic (<a href="https://one.workfront.com/s/new-workfront-experience" target="_blank">Workfront Classic wird im März 2022 eingestellt</a> kurz darauf folgt das Ende der Nutzungsdauer von Workfront Classic im Juli 2022.)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr>
                    <td>
                        <a href="/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">Workfront-Kampagnen (Beta)</a> </p>
                        <p>Wir führen ein neues Objekt in Adobe Workfront ein, das das Potenzial hat, die Verwaltung der Arbeit zu ändern. </p>
                        <p>Mit Workfront Campaign können Sie Projekte aus verschiedenen Portfolios und Programmen in einem neuen Arbeitscontainer organisieren.
Campaign wurde im Juli 2022 mit der Version 22.3 zur Beta-Vorschau veröffentlicht. Weitere Informationen finden Sie unter <a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-project-enhancements.md" class="MCXref xref" xrefformat="{para}">22.3-Projektverbesserungen</a> </p>
<p>Dieser neue Container wird in zukünftigen Versionen weiterentwickelt, um Arbeitsobjekte zu verbinden, die derzeit in separaten Silos verwaltet werden.</p>

</td>
                    <td><span class="bold">Verfügbar zu diesen Daten:</span>
                        <ul>
                            <li>
                                <p>Vorschau-Version: Während des gesamten Veröffentlichungszeitraums von 22.4 <br /><span style="color: #ff0000; font-weight: bold;">Diese Funktion wird voraussichtlich am 9. Januar 2023 aus der Vorschau entfernt. Weitere Informationen finden Sie auf der Übersichtsseite zur Version <a href="../23.1-release-activity/23-1-release-overview.md">23.1.</a> </span></p>
                            </li>
                            <li>
                                <p>Produktionsversion: TBD</p>
                            </li>
                        </ul>
                    </td>
                </tr>
 </tbody> 
</table>

### Verbesserungen beim Ressourcen-Management {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-resource-management-enhancements.md" class="MCXref xref" xrefformat="{para}">Sortiereinstellungen und Verbesserungen der Benutzerfreundlichkeit im Workload Balancer</a> </p> <p>Um Ihr Benutzererlebnis bei der Verwendung des Workload Balancer zu verbessern, haben wir die folgenden Verbesserungen eingeführt, darunter eine verbesserte Sortierung in den Abschnitten „Nicht zugewiesen“ und „Zugewiesen“, ein neues Erscheinungsbild für Projektbalken, ein aktualisiertes, leichter lesbares Design für „Voraussichtliche Termine“ und mehr.</p> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 2. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Verbesserungen beim Reporting {#reporting-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-reporting-enhancements.md" class="MCXref xref" xrefformat="{para}">Entfernen und Hinzufügen von Ressourcenbudgetierungsfeldern in Listen und Berichten
</a> </p> <p>Um die Ressourcenbudgetierungsinformationen aus dem Ressourcenplaner widerzuspiegeln, wurde den Listen und Berichten das neue Feld Ressourcenplaner - budgetierte Stunden hinzugefügt. Verschiedene Felder wurden aus Listen und Berichten entfernt, da sie auf veraltete Tools verwiesen, die in früheren Versionen aus Workfront entfernt wurden.</p> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 23. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: 23. Juni 2022</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Integrationsverbesserungen {#integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Integration von <a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront für Experience Manager Assets</a> </p> <p>Wir freuen uns, Ihnen mitteilen zu können, dass die Adobe Workfront Experience Manager Assets-Integration jetzt zum Cloud Service verfügbar ist.</p>
   <p>Wir haben auch neue Funktionen für Cloud Service und Assets Essentials eingeführt.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau-Version: Nicht zutreffend<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Kombinieren Sie mehrere Dateien in einem einzigen Korrekturabzug im Creative Cloud-Plug-in</a> </p> <p>Sie können jetzt externe Dateien mit den Inhalten hochladen, die Sie im Plug-in "Adobe Workfront for Creative Cloud" erstellt haben, um Korrekturabzüge mit mehreren Dateien in Workfront zu erstellen. Externe Dateien werden als zusätzliche Korrekturabzugseiten in Workfront angezeigt. Mit dieser Verbesserung haben wir auch das Erscheinungsbild der Korrekturabzugs-Erstellung aktualisiert.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau-Version: Nicht zutreffend<br></p> </li> 
     <li> <p>Produktionsversion: TBD</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
   <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-integration-enhancements.md" class="MCXref xref" xrefformat="{para}">Die neue Integration der SharePoint (Graph API) ist jetzt verfügbar</a> </p> <p>Wir haben eine neue, einfachere SharePoint-Integration erstellt. Jetzt müssen Sie die SharePoint-Integration nicht mehr konfigurieren. Stattdessen können Sie einfach die neue SharePoint-Integration wählen, ähnlich wie bei anderen Dokumentintegrationen.</p>
   <p>Sie verlieren nicht den Zugriff auf Dokumente, die derzeit über die veraltete SharePoint-Integration verknüpft sind. Sie können jedoch keine neuen Dokumente über die Legacy-Integration verknüpfen.</p>
   <p>Workfront-Admins können SharePoint- und ältere SharePoint-Integrationen je nach den Anforderungen ihres Unternehmens separat aktivieren und deaktivieren.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 2. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Verbesserungen für Mobilgeräte {#mobile-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-mobile-enhancements.md" class="MCXref xref" xrefformat="{para}">Proofing-Verbesserungen in der Mobile App</a> </p> <p>Mit der Mobile App von Adobe Workfront können Sie jetzt Anhänge zu Korrekturabzugskommentaren anzeigen und neue Anhänge hinzufügen. Unterstützte Dateitypen für Anhänge sind Bilder, Dokumente und Videos.</p> </td>
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
   <p>Sie können auch andere Korrekturabzugsbenutzende in Kommentaren und Antworten taggen. Jeder, den Sie taggen, erhält eine E-Mail-Benachrichtigung.</p>
    <ul> 
     <li> <p>Vorschau-Version: Nicht zutreffend<br></p> </li> 
     <li> <p>Produktionsversion: Mitte bis Ende Juli 2022 im Apple App Store und Google Play Store verfügbar.</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Weitere Verbesserungen {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Funktion</strong> </p> </td> 
   <td> <p><strong>Veröffentlichungstermine und Umgebungen</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Aktualisierte Arbeitszeittabellen</a> </p> <p>Wir verbessern und aktualisieren Ihr Erlebnis bei der Arbeit mit Arbeitszeittabellen kontinuierlich. </p> </td>
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 2. Juni 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Look-and-Feel-Aktualisierungen während des Zeitrahmens der Version 22.3</a> </p> <p>Innerhalb des Zeitrahmens der Version 22.3 werden kleinere Aktualisierungen des Erscheinungsbilds verschiedener Bereiche der Anwendung vorgenommen. Diese Verbesserungen werden mindestens 2 Wochen nach der Veröffentlichung in der Vorschau in der Produktionsumgebung verfügbar gemacht.</p> </td>
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: Im gesamten Zeitrahmen der Version 22.3<br></p> </li> 
     <li> <p>Produktionsfreigabe: Mindestens 2 Wochen nach der Freigabe für die Vorschau (sofern nicht anders angegeben)</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Aktivieren der automatischen Token-Rotation in Ihren benutzerdefinierten OAuth2-Anwendungen</a></p> <p>Um Ihnen mehr Kontrolle über die Sicherheit Ihrer benutzerdefinierten OAuth2-Programme zu ermöglichen, haben wir die Option hinzugefügt, die Token-Rotation zu aktualisieren. Wenn diese Option aktiviert ist, erstellt und sendet Ihre Anwendung jedes Mal, wenn ein Aktualisierungstoken verwendet wird, automatisch ein neues Aktualisierungstoken und deaktiviert das alte.</p> <p>Die Anwendung muss das neue Aktualisierungstoken nach jeder Aktualisierung speichern. Workfront speichert dieses Aktualisierungstoken nicht.</p> <p>Zuvor waren Aktualisierungstoken abgelaufen, nachdem eine bestimmte Zeitdauer in den benutzerdefinierten OAuth2-Anwendungseinstellungen konfiguriert wurde.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 5. Mai 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/22.3-release-activity/22-3-other-enhancements.md" class="MCXref xref" xrefformat="{para}">Verwenden von PKCE in Ihren benutzerdefinierten OAuth2-Integrationen für Single-Page-Web-Anwendungen</a></p> <p>Sie können jetzt Single Page Applications (SPAs) in Ihren benutzerdefinierten Integrationen mithilfe von PKCE erstellen. PKCE ist ein sicherer Autorisierungsfluss, der gut mit dynamisch aktualisierten Programmen wie mobilen Apps funktioniert, aber für alle OAuth2-Clients nützlich ist. Anstelle eines statischen Client-Geheimnisses verwendet PKCE eine dynamisch generierte Zeichenfolge, wodurch das Risiko eines Lecks des Client-Geheimnisses vermieden wird.</p> <p>Zuvor verwendeten die verfügbaren Optionen für benutzerdefinierte OAuth2-Anwendungen entweder den Namen und das Kennwort eines Benutzers oder ein Client-Geheimnis.</p> </td> 
   <td> <p><b>Verfügbar zu diesen Daten:</b> </p> 
    <ul> 
     <li> <p>Vorschau der Version: 5. Mai 2022<br></p> </li> 
     <li> <p>Produktionsversion: Mit Version 22.3</p> </li> 
    </ul> <p><strong>In diesen Umgebungen verfügbar:</strong> </p> 
    <ul> 
     <li> <p>Das neue Adobe Workfront-Erlebnis </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront Fusion-Verbesserungen

Neue Funktionen in Workfront Fusion sind außerhalb des Veröffentlichungszeitplans für 22.3 in der Produktionsumgebung verfügbar. Weitere Informationen zu den neuesten Funktionen finden Sie unter [Versionsaktivität von Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

## Verbesserungen am Workfront-Szenarioplaner

Es gibt derzeit keine Szenario-Planer-Aktualisierungen in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features are coming to Workfront Scenario Planner release with the 21.4 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-activity.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront Scenario Planner release activity</a>.</p>
-->

## Workfront Proof-Verbesserungen

Es gibt derzeit keine Workfront Proof-Updates in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">New features in Workfront Proof are now available. For more information, see <a href="../../../product-announcements/product-releases/workfront-proof-release-activity/wp-release-22-1.md" class="MCXref xref" xrefformat="{para}">Workfront Proof release activity:&nbsp;Week of November 29, 2021</a>.</p>
-->

## Workfront-Zielverbesserungen

Es gibt derzeit keine Updates zu Workfront Goals in der Version. Dieser Bereich wird aktualisiert, sobald Aktualisierungen verfügbar sind.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Most new features coming to Workfront Goals release with the 21.2 release. For information about these new features now available in Preview, see <a href="../../../product-announcements/product-releases/goals-release-activity/goals-21.2-release/goals-release-21-2.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Adobe Workfront Goals with the 21.2 release</a>.</p>
-->

## API-Version 14

Für API-Version 14 haben wir einige Ressourcen und Endpunkte geändert. Einige der Änderungen unterstützen neue Funktionen, andere erleichtern Ihnen die Verwendung der über die API verfügbaren Informationen.

Informationen zu neuen und aktualisierten Funktionen finden Sie unter [Neue Funktionen in der API-Version 14](../../../wf-api/api/new-api-version-14.md).

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](../../../wf-api/api/api-version-support-schedule.md).

## Wartungs-Updates für Workfront 

Informationen zu den Wartungs-Updates, die während der Version 22.3 vorgenommen wurden, finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html).

## Webinar zur Version 22.3

Das Webinar zur Version 22.3 wurde am 23. Juni 2022 vorgestellt. Sie können die Aufzeichnung anzeigen [hier](https://webinars.on24.com/adobe_workfront/whatsnew223?partnerref=WF1).
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Workfront 22.2 Release Webinar will be presented on March 24, 2022 at 8:00 a.m. MST. You can register for the event on the <a href="https://webinars.on24.com/adobe_workfront/WF22point2?partnerref=WFOne" target="_blank">Events page on Workfront One</a>.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This area will be updated as more information becomes available.
</MadCap:conditionalText>
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
was presented on January 12, 2022. You can view the webinar recording on the
<a href="https://one.workfront.com/s/event">Events page on Workfront One</a>.
</MadCap:conditionalText>
</p>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Functionality being removed from Production</h2>
<h3>Feature rollback: Carry over the existing proof workflow when generating a new version</h3>
<p>Due to customer feedback, <b>Workfront is removing this change from Preview environments on March 30, 2021 and from Production environments on March 31, 2021</b>.</p>
<p>On March 11, 2021, Workfront released a change to existing proof workflows in both Workfront Classic and the new Workfront experience. The change allowed for an existing workflow to carry over to any new proof versions created by a user, regardless of the method used to generate them.</p>
<p>In the new Workfront experience after this change is removed, proofs created with the Simple proof selection will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>In Workfront Classic after this change is removed, the option to Generate Proof will not include any preset proofing settings, and new versions will not carry over existing workflows or proof settings. A user can adjust settings after proof generation.</p>
<p>Similar functionality to easily copy existing workflows might be added to Production at a future time.</p>
</div>
-->

## Schulungsaktualisierungen

Erfahren Sie mehr über die neuesten Aktualisierungen von Lernprogrammen, Lernpfaden, Videos und Handbüchern für jede Adobe Workfront-Produktversion. Weitere Informationen finden Sie auf der [Seite mit Schulungsversions-Updates](https://one.workfront.com/s/training-release-updates).

## Funktion wird nicht mehr unterstützt

### Internet Explorer 11

Nachdem die Unterstützung für Internet Explorer eingestellt wurde, unterstützt Workfront jetzt offiziell Microsoft Edge.

Weitere Informationen zu unterstützten Browsern finden Sie unter [Adobe Workfront-Browser-Anforderungen](../../../workfront-basics/workfront-browser-requirements.md).
