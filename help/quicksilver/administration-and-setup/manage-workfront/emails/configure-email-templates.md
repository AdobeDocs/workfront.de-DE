---
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: emails-administration
title: Konfigurieren von E-Mail-Vorlagen
description: Als Adobe Workfront-Administrator können Sie E-Mail-Vorlagen konfigurieren, um Erinnerungsbenachrichtigungen zu unterstützen.
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 2ebc3be5-2734-4012-9277-86176c070137
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 3%

---


# E-Mail-Vorlagen konfigurieren

<!--Audited: 10/2024-->


Als Adobe Workfront-Administrator können Sie E-Mail-Vorlagen konfigurieren, um Erinnerungsbenachrichtigungen zu unterstützen.

E-Mail-Vorlagen enthalten die Nachricht, die an Benutzer gesendet wird, wenn eine Erinnerungsbenachrichtigung initiiert wird.\
Ohne E-Mail-Vorlage wird die Erinnerungsbenachrichtigung als leerer Inhalt im Textkörper der E-Mail gesendet.

E-Mail-Vorlagen können mit Erinnerungsbenachrichtigungen für Probleme, Aufgaben, Projekte und Arbeitszeittabellen verknüpft werden. Beim Erstellen von E-Mail-Vorlagen kann Ihr Workfront-Administrator Inhalte für die E-Mail und eine Betreffzeile bereitstellen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## E-Mail-Vorlage erstellen {#create-an-email-template}

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **E-Mail** > **Benachrichtigungen** > **E-Mail-Vorlagen**.

   ![Registerkarte E-Mail-Vorlagen](assets/email-templates-tab-under-setup-email-notifications-area.png)

1. Klicken Sie auf **Neue E-Mail-Vorlage**.

1. Geben Sie im Feld **Neue E** Mail-Vorlage) die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Fügen Sie der E-Mail-Vorlage einen Titel hinzu. Dies ist ein Pflichtfeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Objekttyp</td> 
      <td>Geben Sie den Objekttyp an, mit dem Sie die Vorlage verknüpfen möchten. Wählen Sie aus den folgenden Objekten:
      <ul>
      <li>Projekt</li>
      <li>Aufgabe</li>
      <li>Problem</li>
      <li>Arbeitszeittabelle</li> </ul>

   Dies ist ein erforderliches Feld, das standardmäßig auf Projekt eingestellt ist.</td>
   </tr>
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Fügen Sie weitere Informationen über die E-Mail-Vorlage, ihren Zweck und die vorgesehene Zielgruppe hinzu.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Betreff </td> 
      <td>Fügen Sie den Text hinzu, der in der Betreffzeile der E-Mail angezeigt wird, wenn die von der Vorlage generierte E-Mail-Nachricht gesendet wird. Dies ist ein Pflichtfeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Textkörper </td> 
      <td> <p>Fügen Sie den Text für den Inhalt der E-Mail-Nachricht hinzu.</p> <p>Sie können die HTML-Formatierung für den E-Mail-Inhalt verwenden, wie im Abschnitt <a href="#add-html-formatting-to-an-email-template" class="MCXref xref">Hinzufügen der HTML-Formatierung zu einer E-Mail-Vorlage</a> in diesem Artikel beschrieben.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

## Hinzufügen einer HTML-Formatierung zu einer E-Mail-Vorlage {#add-html-formatting-to-an-email-template}

Sie können E-Mail-Vorlagen HTML-Tags hinzufügen, um benutzerdefinierte Benachrichtigungen zu erstellen.\
Erstellen Sie die E-Mail-Vorlage wie in [Erstellen einer neuen E-Mail-Vorlage](#create-a-new-email-template) beschrieben.

HTML-Formatierung kann Ihre E-Mail-Vorlagen anreichern, wie in den folgenden Abschnitten gezeigt.

* [Verknüpfung zu Workfront-Objekten](#link-to-workfront-objects)
* [Verknüpfen mit benutzerdefinierten Feldern mit HTML](#link-to-custom-fields-with-html)
* [HTML-E-Mail-Beispiele](#html-email-examples)

### Link zu Workfront-Objekten {#link-to-workfront-objects}

Sie können Links zu Workfront-Feldern hinzufügen, indem Sie den `$$`-Platzhalter verwenden, um den E-Mail-Generator anzuweisen, nach Werten aus der mit einem bestimmten Objekt verknüpften Datenbank zu suchen.

Beispielsweise kann der Textkörper der E-Mail für eine Benachrichtigung, die den Verantwortlichen über die Aufgabe benachrichtigt, die in Kürze beginnen soll, dieser Struktur folgen:

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

Um den Wert „Platzhalter“ für ein Objekt abzurufen, führen Sie einen der folgenden Schritte aus:

* Konsultieren Sie den API Explorer und wählen Sie die Namen Ihrer Objekte auf der Registerkarte Felder eines beliebigen Objekts aus. Weitere Informationen zum API Explorer finden Sie unter [API Explorer](/help/quicksilver/wf-api/general/api-explorer.md).

* Verwenden Sie den `valuefield`, den Sie in einer Textmodusansicht eines Berichts finden. Weitere Informationen zu Textmoduswerten finden Sie unter [Übersicht über den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

Der `heading` kann der Name des Objekts sein, so wie er im E-Mail-Textkörper angezeigt werden soll.

### Verknüpfen mit benutzerdefinierten Feldern mit HTML {#link-to-custom-fields-with-html}

Sie können Links zu Benutzern und benutzerdefinierten Feldern einfügen, indem Sie den `$$`-Platzhalter verwenden, um den E-Mail-Generator anzuweisen, nach Werten aus der mit dem Objekt verknüpften Datenbank zu suchen. Sie müssen auf beiden Seiten der Datenbankattributreferenz vorhanden sein.

Wenn Sie beispielsweise den folgenden Text als HTML hinzufügen, wird der Vorname des zugewiesenen Benutzers zu der mit einer Aufgabe verknüpften Erinnerungsbenachrichtigung hinzugefügt:

`assignedTo:firstName`

Um benutzerdefinierte Felder mit derselben Formatierung hinzuzufügen, können Sie Folgendes in Ihrer E-Mail-Benachrichtigung hinzufügen:

`DE:Custom Field As It Appears in Workfront`

Dies ist beispielsweise eine E-Mail-Vorlage mit einem Verweis auf ein benutzerdefiniertes Feld namens Versanddatum. Dabei wird davon ausgegangen, dass das Feld Versanddatum zu einer Aufgabe gehört.

Ersetzen Sie `<your domain>` durch die Workfront-Domain Ihres Unternehmens, ohne die Klammern:

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
>Wenn das Feld zu einem Projekt gehört, ersetzen Sie die Aufgabe durch ein Projekt:
>
>`DE:Project:Delivery Date`

### HTML-E-Mail-Beispiele {#html-email-examples}

* [Benachrichtigung zur verspäteten Projekterinnerung (Beispiel)](#late-project-reminder-notification-example)
* [Aufgabe oder Problem bezüglich des Starts einer Erinnerung (Beispiel)](#task-or-issue-about-to-start-reminder-example)

#### Benachrichtigung zur verspäteten Projekterinnerung (Beispiel) {#late-project-reminder-notification-example}

Beachten Sie beim Bearbeiten einer E-Mail-Vorlage für eine verspätete Projekterinnerung diese Informationen für die Felder Betreff und Inhalt .

Ersetzen Sie `<your domain>` durch die Workfront-Domain Ihres Unternehmens, ohne die Klammern.

**Betreff:**

Ein Projekt, das Sie verwalten, ist zu spät gekommen

**content:**

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

Dadurch wird eine E-Mail ähnlich der folgenden erzeugt:

![Projekt wurde zu einer verspäteten E-Mail](assets/project-became-late-email.png)

#### Aufgabe oder Problem bezüglich des Starts der Erinnerung {#task-or-issue-about-to-start-reminder-example}

Möglicherweise möchten Sie auch eine Erinnerungsnachricht für eine bevorstehende Aufgabe oder ein bevorstehendes Problem erstellen.

Der folgende Code kann in eine E-Mail-Vorlage eingefügt werden, um ihn für Aufgaben- und Problem-Erinnerungsbenachrichtigungen zu verwenden, die beliebig viele Tage vor dem geplanten Startdatum der Aufgabe oder des Problems gesendet werden.

Ersetzen Sie `<your domain>` durch die Workfront-Domain Ihres Unternehmens, ohne die Klammern.

Um diese Option für eine Anfrage-E-Mail zu verwenden, ändern Sie den `/task/view.` im Link zum Arbeitselement in `/issue/view`.

**Betreff:**

`$$name$$ to start on $$plannedStartDate$$`

**content:**

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

![email_template_deliverated.png](assets/email-template-delivered.png)

Nachdem eine E-Mail-Vorlage erstellt wurde, können Benutzer sie mit Erinnerungsbenachrichtigungen verknüpfen, wie in [Einrichten von Erinnerungsbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md) beschrieben.
