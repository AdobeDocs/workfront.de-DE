---
title: Übersicht über Projektbedingung und Bedingungstyp
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Die Projektbedingung ist eine visuelle Darstellung des Projektfortschritts. Es handelt sich um eine berichtspflichtige Variable, die durch die Beziehung zwischen dem geplanten, geplanten und geschätzten Projektdatum bestimmt wird.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Übersicht über Projektbedingung und Bedingungstyp

Die Projektbedingung ist eine visuelle Darstellung des Projektfortschritts. Es handelt sich um eine berichtspflichtige Variable, die durch die Beziehung zwischen dem geplanten, geplanten und geschätzten Projektdatum bestimmt wird.

## Übersicht über Projektbedingungen

Beachten Sie Folgendes, um die Bedingung eines Projekts zu verstehen:

* Als Projekteigentümer können Sie entscheiden, ob die Bedingung eines Projekts manuell oder automatisch festgelegt wird. Die Bedingung eines Projekts kann wie folgt festgelegt werden:

   * Manuell durch Benutzer, die Zugriff auf &quot;Projekt verwalten&quot;haben und wenn der Bedingungstyp des Projekts auf &quot;Manuell&quot;festgelegt ist.
   * Automatisch von Adobe Workfront, wenn der Bedingungstyp des Projekts auf Fortschrittsstatus festgelegt ist. Der Fortschritt des Projekts wird durch den Fortschritt der Aufgaben im Projekt bestimmt. Weitere Informationen zum Fortschrittsstatus des Projekts finden Sie unter [Übersicht über den Projektstatus](../../../manage-work/projects/planning-a-project/project-progress-status.md).

   Informationen zum Aktualisieren des Bedingungstyps des Projekts finden Sie unter [Bedingungstyp eines Projekts festlegen](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Wenn Sie es Workfront ermöglichen, den Projektzustand automatisch abzuschätzen, empfehlen wir, Vorgänger für Ihre Aufgaben zu verwenden, damit der Aufgabenfortschritt den tatsächlichen Fortschritt und den Fortschrittsstatus des Projekts widerspiegelt.
* Als Projekteigentümer können Sie das Projekt so ändern, dass es einen manuellen Bedingungstyp verwendet, anstatt den Fortschrittsstatus zu verwenden, indem Sie den Bedingungstyp von Fortschrittsstatus in Manuell ändern.

   >[!NOTE]
   >
   >Projekte mit einem der folgenden Status werden immer als On Target markiert, unabhängig vom Datum der Aufgaben und ihrem Fortschritt:
   >
   >* Idee
   >* Angefordert
   >* Genehmigt
   >* Abgelehnt


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## So aktualisiert Workfront die Projektbedingung auf Grundlage des Fortschrittsstatus

Wenn der Bedingungstyp des Projekts auf &quot;Manuell&quot;festgelegt ist, können Sie festlegen, welche Bedingung des Projekts unabhängig vom Fortschrittsstatus des Projekts ist.

Es wird jedoch empfohlen, den Bedingungstyp des Projekts auf den Fortschrittsstatus festzulegen, damit Sie anhand des Fortschritts Ihrer Aufgaben einen klaren Hinweis darauf erhalten, welcher wahre Fortschritt des Projekts erzielt wird. Informationen zur Berechnung des Fortschrittsstatus von Projekten durch Workfront finden Sie unter [Übersicht über den Projektstatus](../../../manage-work/projects/planning-a-project/project-progress-status.md).

In diesem Fall können die Werte für die Projektbedingung wie folgt lauten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Projektbedingung</td> 
   <td>Projektfortstatus</td> 
   <td>Workfront-Bedingungsindikator</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Im Zielbereich</td> 
   <td> <li>Wenn der Fortschrittsstatus des Projekts "Einschaltzeit"lautet, lautet die Bedingung des Projekts <strong>In Target</strong>.</li> </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gefährdet</td> 
   <td>Wenn der Fortschrittsstatus des Projekts <strong>Hinter</strong> oder <strong>Risiko</strong>festgelegt ist, lautet die Bedingung des Projekts <strong>Risiko</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>In Schwierigkeiten</td> 
   <td>Wenn der Fortschrittsstatus des Projekts <strong>Verspätet</strong>festgelegt ist, lautet die Bedingung des Projekts <strong>In Schwierigkeiten</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Bedingungen können für Ihre Umgebung angepasst werden, sodass Sie in Ihrer Umgebung mehr als drei Optionen für Bedingungen finden können. Die Namen der Bedingungen können sich von den oben aufgeführten unterscheiden. Informationen zum Anpassen von Bedingungen in finden Sie im Artikel [Benutzerdefinierte Bedingung erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Bericht zu Projektbedingungen, Aktualisierung der Projektbedingungen und Hinweis zur letzten Bedingung

In der Ansicht eines Projektberichts können Sie die folgenden Felder bezüglich der Projektbedingung anzeigen:

* **Projektbedingung:** Zeigt die aktuelle Projektbedingung an.
* **Aktualisierung der Projektbedingungen**: Zeigt die neueste Aktualisierung, die der Projekteigentümer im Aktualisierungsstream des Projekts bereitgestellt hat, zusammen mit der neuen Bedingung an.\
   Kommentare zu Bedingungsaktualisierungen werden nicht im **Bedingungsaktualisierung** Spalte; nur die Hauptaktualisierung angezeigt wird.

* **Hinweis zu letzter Bedingung**: Zeigt die Aktualisierung an, die der Eigentümer des Objekts zuletzt in einem Objekt eingegeben hat. Dieses Feld ist hilfreich, um die aktuellste Aktivität oder Interaktion des Eigentümers auf einem Objekt anzuzeigen.\
   Die **Hinweis zu letzter Bedingung** leer ist, wenn der Hinweistext der letzten Anmerkung eines Objekts gelöscht wurde. Wenn eine neue Anmerkung auf dem Objekt eingegeben wird, wird sie zur letzten Anmerkung und wird erneut in der Spalte angezeigt.

Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
