---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: 2019.4 Weitere Verbesserungen
description: Auf dieser Seite werden verschiedene Verbesserungen beschrieben, die mit der Version 2019.4 vorgenommen wurden. Es wird in der Woche vom 11. November 2019 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# 2019.4 Weitere Verbesserungen

Auf dieser Seite werden verschiedene Verbesserungen beschrieben, die mit der Version 2019.4 vorgenommen wurden. Es wird in der Woche vom 11. November 2019 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen in Version 2019.4 finden Sie unter [Übersicht über die Version 2019.4](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Starten eines automatisierten Proofing-Workflows von einem Adobe-CC-Dokument aus</strong> <p>Ohne Adobe CC verlassen zu müssen, können Sie einen automatisierten Proofing-Workflow für ein von Ihnen erstelltes Adobe CC-Dokument starten. Weitere Informationen finden Sie im Abschnitt <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Erstellen eines Korrekturabzugs von Illustrator oder InDesign</a> im Artikel <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">Verwenden der Workfront-Erweiterung für Illustrator und InDesign</a>.</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>Verhindern doppelter E-Mail-Adressen</strong> <p>Sie können dieselbe E-Mail-Adresse nicht mehr verwenden, wenn Sie mehrere Benutzende in Workfront erstellen, auch wenn diese E-Mail-Adressen von Fall zu Fall unterschiedlich sind. Sie können beispielsweise keinen Benutzer mit der E-Mail-Adresse JohnDoe@example.com und keinen anderen Benutzer mit der E-Mail-Adresse johndoe@example.com erstellen. </p> <p>Vor dieser Änderung wurde das Erstellen von Benutzern mit übereinstimmenden E-Mail-Adressen, die sich nur nach Groß-/Kleinschreibung unterschieden, unterstützt. </p> <p>Hinweis: Vorhandene Benutzer mit übereinstimmenden E-Mail-Adressen, die sich nur durch die Groß-/Kleinschreibung unterscheiden, müssen zu einem zukünftigen Datum aktualisiert werden. Wenn sich Benutzende in einer Workfront-Instanz mit übereinstimmenden E-Mail-Adressen befinden, die sich nur von Fall zu Fall unterscheiden, wird Workfront Sie mit zusätzlichen Informationen und einem Zeitplan kontaktieren, wenn diese aktualisiert werden müssen.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Zusätzliche Objekttypen für Typeahead-Felder in einem benutzerdefinierten Formular verfügbar</strong> 
     <p>Wenn Sie jetzt ein benutzerdefiniertes Feld mit automatischer Textvervollständigung erstellen, können Sie die folgenden Objekttypen mit dem Feld verknüpfen: Benutzer, Unternehmen, Gruppe, Aufgabengebiet, Portfolio, Programm, Projekt und Vorlage.</p> 
     <p>Zuvor konnten Sie nur den Benutzerobjekttyp mit einem benutzerdefinierten Feld mit automatischer Textvervollständigung verknüpfen.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>Dateiname der zuletzt angezeigten Version eines Dokuments</strong> <p>Wenn Sie jetzt eine Dokumentversion hochladen, deren Dateiname sich von dem der bestehenden Version unterscheidet, wird der neue Dateiname in Workfront angezeigt.</p> <p>Wenn Sie bisher eine neue Version mit einem anderen Dateinamen hinzugefügt haben, wird der Dateiname der vorherigen Version weiterhin in Workfront angezeigt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">Hochladen einer neuen Version eines Dokuments</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>Hinzufügen eines Filters zu einem Feld mit automatischer Textvervollständigung in einem benutzerdefinierten Formular</strong> <p>Wenn Sie nun einem benutzerdefinierten Formular ein Feld mit automatischer Textvervollständigung hinzufügen, können Sie einen Filter hinzufügen, um die Objekte zu begrenzen, die verfügbar sind, wenn jemand das Feld verwendet. Sie können beispielsweise das Feld so beschränken, dass der Benutzer nur Mitglieder des Marketing- und Verkaufsteams in Ihrer Organisation auswählen kann.</p> <p>Weitere Informationen finden Sie im Abschnitt Erstellen und Hinzufügen eines neuen Felds im Artikel Erstellen einer benutzerdefinierten Forms .</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Ändern des Anzeigetyps eines Felds in einem benutzerdefinierten Formular</strong> 
     <p>Jetzt können Sie den Anzeigetyp eines Felds in einem benutzerdefinierten Formular ändern.</p> 
     <p>Wenn Sie beispielsweise ein Kontrollkästchen erstellt haben, können Sie es in ein Dropdown-Feld oder ein Optionsfeld ändern. Diese drei Anzeigetypen für Felder sind austauschbar.</p> 
     <p>Wenn Sie ein einzeiliges Textfeld erstellt haben, können Sie es auch in ein Absatztextfeld ändern. Diese beiden Feldanzeigetypen sind austauschbar.</p> 
     <p>Um den Anzeigetyp eines benutzerdefinierten Felds zu ändern, mussten Sie zuvor ein neues Feld erstellen und das alte löschen. Dies erforderte die Übertragung von Daten, was häufig zeitaufwendig war.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Erstellen von Urlaubskalendern und -berichten</strong> 
     <p>Sie können jetzt die Ausfallzeiten der Benutzenden für eine bessere Planung und Ausführung sehen. Sie können Ihren Dashboards auch neue Berichte und Kalender hinzufügen, um eine Echtzeitansicht der Benutzerverfügbarkeit zu erhalten.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
