---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: Weitere Verbesserungen in Version 2019.4
description: Auf dieser Seite werden verschiedene Verbesserungen beschrieben, die mit Version 2019.4 vorgenommen wurden. Sie wird in der Woche vom 11. November 2019 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 0%

---

# Weitere Verbesserungen in Version 2019.4

Auf dieser Seite werden verschiedene Verbesserungen beschrieben, die mit Version 2019.4 vorgenommen wurden. Sie wird in der Woche vom 11. November 2019 in der Produktionsumgebung zur Verfügung gestellt.

Eine Liste aller Änderungen, die in Version 2019.4 vorgenommen wurden, finden Sie unter [Versionsübersicht 2019.4](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Starten eines automatisierten Testversand-Workflows aus einem Adobe CC-Dokument</strong> <p>Ohne Adobe CC verlassen zu müssen, können Sie einen automatisierten Testversand-Workflow für ein von Ihnen erstelltes Adobe CC-Dokument starten. Weitere Informationen finden Sie im Abschnitt <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Erstellen eines Testversands von Illustrator oder InDesign</a> im Artikel <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">Verwenden der Workfront-Erweiterung für Illustrator und InDesign</a>.</p> </td> 
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
   <td> <strong>Duplizieren von E-Mail-Adressen verhindern</strong> <p>Sie können nicht mehr dieselbe E-Mail-Adresse verwenden, wenn Sie mehrere Benutzer in Workfront erstellen, auch wenn diese E-Mail-Adressen von Fall zu Fall variieren. Sie können beispielsweise keinen Benutzer mit der E-Mail-Adresse JohnDoe@example.com und einen anderen Benutzer mit der E-Mail-Adresse johndoe@example.com erstellen. </p> <p>Vor dieser Änderung wurde die Erstellung von Benutzern mit übereinstimmenden E-Mail-Adressen unterstützt, die sich nur von Fall zu Fall unterscheiden. </p> <p>Hinweis: Vorhandene Benutzer mit übereinstimmenden E-Mail-Adressen, die sich nur von Fall zu Fall unterscheiden, müssen an einem zukünftigen Datum aktualisiert werden. Wenn Sie Benutzer in einer Workfront-Instanz haben, deren E-Mail-Adressen nur von Fall zu Fall verschieden sind, kontaktiert Workfront Sie mit zusätzlichen Informationen und einer Zeitleiste, wenn diese aktualisiert werden müssen.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Zusätzliche Objekttypen, die für die Felder vom Typ voraus in einem benutzerdefinierten Formular verfügbar sind</strong> 
     <p>Wenn Sie jetzt ein benutzerdefiniertes "TypeAhead"-Feld erstellen, können Sie die folgenden Objekttypen mit dem Feld verknüpfen: Benutzer, Firma, Gruppe, Auftragsrolle, Portfolio, Programm, Projekt und Vorlage.</p> 
     <p>Zuvor konnten Sie nur den User-Objekttyp mit einem benutzerdefinierten Feld "TypeAhead"verknüpfen.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>Dateiname der neuesten Version eines angezeigten Dokuments</strong> <p>Wenn Sie jetzt eine Dokumentversion mit einem anderen Dateinamen als die vorhandene Version hochladen, wird der neue Dateiname in Workfront angezeigt.</p> <p>Wenn Sie zuvor eine neue Version mit einem anderen Dateinamen hinzugefügt haben, wurde der Dateiname der vorherigen Version weiterhin in Workfront angezeigt.</p> <p>Weitere Informationen finden Sie unter <a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">Hochladen einer neuen Version eines Dokuments</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>Fügen Sie einem Feld vom TypAhead in einem benutzerdefinierten Formular einen Filter hinzu</strong> <p>Wenn Sie jetzt ein Feld vom Typ "Vorwärts"zu einem benutzerdefinierten Formular hinzufügen, können Sie einen Filter hinzufügen, um die Objekte zu beschränken, die verfügbar sind, wenn jemand das Feld verwendet. Sie können beispielsweise das Feld so einschränken, dass der Benutzer nur Mitglieder der Marketing- und Verkaufsteams in Ihrer Organisation auswählen kann.</p> <p>Weitere Informationen finden Sie im Abschnitt Neues Feld erstellen und hinzufügen im Artikel Erstellen benutzerdefinierter Forms .</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Ändern des Anzeigetyps eines Felds in einem benutzerdefinierten Formular</strong> 
     <p>Jetzt können Sie den Anzeigetyp eines Felds in einem benutzerdefinierten Formular ändern.</p> 
     <p>Wenn Sie beispielsweise ein Kontrollkästchen-Feld erstellt haben, können Sie es in ein Dropdown-Feld oder ein Optionsfeld ändern. Diese drei Feldanzeigetypen sind austauschbar.</p> 
     <p>Wenn Sie ein einzeiliges Textfeld erstellt haben, können Sie es in ein Absatztext -Feld ändern. Diese beiden Feldanzeigetypen sind austauschbar.</p> 
     <p>Bisher mussten Sie zum Ändern des Anzeigetyps eines benutzerdefinierten Felds ein neues Feld erstellen und das alte löschen. Dies erforderte die Übertragung von Daten, die häufig zeitaufwendig waren.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Erstellen einer Zeitdauer für Kalender und Berichte</strong> 
     <p>Sie können nun die Zeitdauer des Benutzers für eine bessere Planung und Ausführung sehen. Sie können Ihren Dashboards auch neue Zeiträume für Berichte und Kalender hinzufügen, um einen Echtzeitüberblick über die Benutzerverfügbarkeit zu erhalten.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
