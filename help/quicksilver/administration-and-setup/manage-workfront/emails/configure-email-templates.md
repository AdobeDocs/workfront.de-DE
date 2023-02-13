---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: E-Mail-Vorlagen konfigurieren
description: Als Adobe Workfront-Administrator können Sie E-Mail-Vorlagen konfigurieren, um Erinnerungsbenachrichtigungen zu unterstützen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '748'
ht-degree: 1%

---

# E-Mail-Vorlagen konfigurieren

Als Adobe Workfront-Administrator können Sie E-Mail-Vorlagen konfigurieren, um Erinnerungsbenachrichtigungen zu unterstützen.

E-Mail-Vorlagen enthalten die Nachricht, die Benutzern gesendet wird, wenn eine Erinnerungsbenachrichtigung initiiert wird.\
Ohne E-Mail-Vorlage wird die Erinnerungsbenachrichtigung als leerer Inhalt im Text der E-Mail gesendet.

E-Mail-Vorlagen können mit Erinnerungsbenachrichtigungen für Probleme, Aufgaben, Projekte und Timesheets verknüpft werden. Bei der Erstellung von E-Mail-Vorlagen kann Ihr Workfront-Administrator Inhalte für die E-Mail und eine Betreffzeile bereitstellen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Neue E-Mail-Vorlage erstellen {#create-a-new-email-template}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im Bedienfeld auf der linken Seite auf **Email** > **Benachrichtigungen**.

1. Klicken Sie auf **E-Mail-Vorlagen** Registerkarte und klicken Sie dann auf **Neue E-Mail-Vorlage**.

1. Im **Neue E-Mail-Vorlage** die folgenden Informationen angeben:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">E-Mail-Vorlage</td> 
      <td>Titel der E-Mail-Vorlage (erforderlich).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Beschreibung der Vorlage.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Objekttyp</td> 
      <td>Geben Sie den Objekttyp an, mit dem Sie die Vorlage verknüpfen möchten (Erforderlich, standardmäßig wird "Problem"festgelegt).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Betreff </td> 
      <td>Betreff, das beim Versand der E-Mail-Nachricht angezeigt wird (erforderlich).</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> <p>Inhalt, der beim Senden der E-Mail-Nachricht angezeigt wird</p> <p>Sie können die HTML-Formatierung für den E-Mail-Inhalt verwenden, wie unter <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">HTML-Formatierung zu einer E-Mail-Vorlage hinzufügen</a> in diesem Artikel.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

## HTML-Formatierung zu einer E-Mail-Vorlage hinzufügen {#add-html-formatting-to-an-email-template}

Sie können E-Mail-Vorlagen HTML-Tags hinzufügen, um benutzerdefinierte Benachrichtigungen zu erstellen.\
Erstellen Sie die E-Mail-Vorlage wie in [Neue E-Mail-Vorlage erstellen](#create-a-new-email-template).

Die HTML-Formatierung kann Ihre E-Mail-Vorlagen anreichern, wie in den folgenden Abschnitten dargestellt.

* [Verknüpfung zu Workfront-Objekten](#link-to-workfront-objects)
* [Verknüpfung zu benutzerdefinierten Feldern mit HTML](#link-to-custom-fields-with-html)
* [HTML-E-Mail-Beispiele](#html-email-examples)

### Verknüpfung zu Workfront-Objekten {#link-to-workfront-objects}

Sie können mithilfe der `$$` -Platzhalter, um den E-Mail-Generator anzuweisen, nach Werten aus der Datenbank zu suchen, die mit einem bestimmten Objekt verknüpft sind.

Der Hauptteil der E-Mail für eine Benachrichtigung, die den Verantwortlichen der Aufgabe über den Beginn benachrichtigt, kann beispielsweise folgende Struktur aufweisen:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b><strong>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td>
</tr>
<tr>
<td><b>HEADING</b></td>
<td>$$WILDCARD$$</td></tr>
</table>
</html>
```

Führen Sie einen der folgenden Schritte aus, um den Platzhalterwert für ein Objekt abzurufen:

<!-- Refer to the API Explorer and select the names of your objects from the Fields tab of any object. For more information about the API Explorer, see [Adobe Workfront API](../../../wf-api/workfront-api.md).-->

* Verwenden Sie den Wert &quot;valueField&quot;, den Sie in einer Textmodusansicht eines Berichts finden. Weitere Informationen zu Textmoduswerten finden Sie unter [Textmodus - Übersicht](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

   Der Wert &quot;heading&quot;kann der Name des Objekts sein, wie er im E-Mail-Textkörper angezeigt werden soll.

### Verknüpfung zu benutzerdefinierten Feldern mit HTML {#link-to-custom-fields-with-html}

Sie können mithilfe der Variablen **$$** -Platzhalter, um den E-Mail-Generator anzuweisen, nach Werten aus der mit dem Objekt verknüpften Datenbank zu suchen. Sie müssen auf beiden Seiten der Datenbankattributreferenz vorhanden sein.

Wenn Sie beispielsweise den folgenden Text als HTML hinzufügen, wird der Vorname des zugewiesenen Benutzers zur Erinnerungsbenachrichtigung hinzugefügt, die mit einer Aufgabe verknüpft ist:

`assignedTo:firstName`

Um benutzerdefinierte Felder mit derselben Formatierung hinzuzufügen, können Sie Folgendes zu Ihrer E-Mail-Benachrichtigung hinzufügen:

`DE:Custom Field As It Appears in Workfront`

Dies ist beispielsweise eine E-Mail-Vorlage, die einen Verweis auf ein benutzerdefiniertes Feld namens Versanddatum enthält und davon ausgeht, dass das Feld Versanddatum zu einer Aufgabe gehört.

Ersetzen `<your domain>` mit der Workfront-Domäne Ihres Unternehmens ohne die Klammern:

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><a href="https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which has a Delivery Date of $$DE:Task:Delivery Date$$.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
<tr>
<td><b>Description:</b></td>
<td>$$description$$</td>
<tr>
<td><b>Estimated Effort:</b></td>
<td>$$work$$ hours</td>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
<td><b>Delivery Date:</b></td>
<td>$$DE:Task:Delivery Date$$</td>
</tr>
</table>
</html>
```

>[!NOTE]
>
>Wenn das Feld zu einem Projekt gehört, ersetzen Sie Aufgabe durch Projekt:
>
>`DE:Project:Delivery Date`

### HTML-E-Mail-Beispiele {#html-email-examples}

* [Benachrichtigung zur verspäteten Erinnerung an ein Projekt (Beispiel)](#late-project-reminder-notification-example)
* [Aufgabe oder Problem Info zur Erinnerung starten (Beispiel)](#task-or-issue-about-to-start-reminder-example)

#### Benachrichtigung zur verspäteten Erinnerung an ein Projekt (Beispiel) {#late-project-reminder-notification-example}

Um eine E-Mail-Vorlage für eine verspätete Projekterinnerung zu bearbeiten, beachten Sie diese Informationen für die Felder Betreff und Inhalt .

Ersetzen `<your domain>` mit der Workfront-Domäne Ihres Unternehmens, ohne die Klammern.

**Betreff:**

Ein von Ihnen verwaltetes Projekt ist zu spät

**Inhalt:**

```html
<html>
<p>The <b><a href="https://<your domain>.my.workfront.com/project/view?ID=$$ID$$">$$name$$</a></b> project you are assigned as the owner of just became late.</p>
<table width="350" style="font-size:12px;">
<tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<tr>
<td><b>Planned Completion Date:</b></td>
<td>$$plannedCompletionDate$$</td>
</tr>
</table>
<p>Please review the task plan and bring it up to date to reflect the progress made so far. If it is necessary to update the plan to bring it reflect reality going forward, be sure to speak to $$sponsor:name$$ for approval before make these changes to the work breakdown structure.</p>
</html>
```

Dadurch wird eine E-Mail wie die folgende erzeugt:

![](assets/screen-shot-2016-09-16-at-3.52.54-pm-350x103.png)

#### Aufgabe oder Problem im Zusammenhang mit der Erinnerung {#task-or-issue-about-to-start-reminder-example}

Möglicherweise möchten Sie auch eine Erinnerungsbenachrichtigung für eine bevorstehende Aufgabe oder ein bevorstehendes Problem erstellen.

Der folgende Code kann in eine E-Mail-Vorlage eingefügt werden, die für Aufgaben- und Problemerinnerungsbenachrichtigungen verwendet werden kann, die eine beliebige Anzahl von Tagen vor dem geplanten Startdatum der Aufgabe oder des Problems gesendet werden.

Ersetzen `<your domain>` mit der Workfront-Domäne Ihres Unternehmens, ohne die Klammern.

Um dies für eine Problem-E-Mail zu verwenden, ändern Sie die `/task/view.` -Wert in der Verknüpfung zum Arbeitselement `/issue/view`.

**Betreff:**

`$$name$$ to start on $$plannedStartDate$$`

**Inhalt:**

```html
<html>
<p>$$assignedTo:firstName$$</p>
<p>You are assigned to work on <b><ahref=https://<your domain>.my.workfront.com/task/view?ID=$$ID$$">$$name$$</a></b>, which is due to start on $$plannedStartDate$$.</p>
<tablewidth=350"style=font-size:12px;">
<tr>
<td><b>Task Name:</b></td>
<td>$$name$$</td>
</tr>
<td><b>Project Name:</b></td>
<td>$$project:name$$</td>
</tr>
</tr>
<td><b>Created on:</b></td>
<td>$$entryDate$$</td>
</tr>
<tr>
<td><b>Project Manager:</b></td>
<td>$$project:owner:name$$</td>
<tr>
<td><b>Priority:</b></td>
<td>$$priority$$</td>
</tr>
<tr>
<td><b>Who is assigned to:</b></td>
<td>$$assignedTo:name$$</td>
</tr>
<tr>
<td><b>When it's due:</b></td>
<td>$$estCompletionDate$$</td>
</tr>
</table>
</html>
```

![email_template_delivered.png](assets/email-template-delivered.png)

Nachdem eine E-Mail-Vorlage erstellt wurde, können Benutzer sie mit Erinnerungsbenachrichtigungen verknüpfen, wie unter [Einrichten von Erinnerungsbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).
