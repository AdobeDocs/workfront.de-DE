---
product-area: templates
navigation-topic: templates-navigation-topic
title: Vorlage an ein Projekt anhängen
description: Sie können eine Vorlage entweder während der ersten Erstellungsphase des Projekts oder nach seiner Erstellung an ein Projekt anhängen.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '1126'
ht-degree: 2%

---

# Vorlage an ein Projekt anhängen

<!-- Audited: 10/2025 -->

Sie können eine Vorlage entweder während der ersten Erstellungsphase des Projekts oder nach seiner Erstellung an ein Projekt anhängen.

Weitere Informationen zum Erstellen eines Projekts mithilfe einer Vorlage finden Sie unter [Erstellen eines Projekts mithilfe einer Vorlage](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
    <p>Plan</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten </p> <p>Zugriff auf Vorlagen anzeigen</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt</p> <p>Anzeigen von Berechtigungen oder höher für die Vorlage</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard</p>
   <p>Or</p>
   <p>Current: Plan</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects </p> <p>For information about project access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> <p>View access to&nbsp;Templates</p> <p>For information about template permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Share a template</a>. </p> <p>For information about template access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Grant access to templates</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create and modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>. </p> <p>View permissions or higher to the template</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Considerations when adding templates to projects</h2>
<p>(NOTE: moved this to an Overview article of its own) </p>
<p>Consider the following when adding templates to projects:</p>
<ul>
<li> <p>You can attach only active templates to projects. </p> </li>
<li> <p>You can attach a template to a project when the project is in a status of Complete, Dead, or in Pending Approval, only when your Adobe Workfront administrator <span>or a group administrator</span> has enabled this functionality in the Project&nbsp;Preferences area. For information about setting project preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configure system-wide project preferences</a>. </p> </li>
<li> <p>Unless you exclude specific template tasks from being added in the attachment process, all template tasks are added to the existing project. </p> </li>
<li> <p>Most template settings are added to the project. </p> </li>
<li> <p>Some settings from the template automatically transfer to the project, unless you specifically mark them to be excluded. </p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<span class="autonumber"><span><b>Example: </b></span></span>
<p>For example, these settings are added to the project:</p>
<ul>
<li>Start&nbsp;From field</li>
<li>Custom forms and the information on them</li>
<li>Queue Details </li>
<li>Financial settings </li>
</ul>
</div> </li>
</ul>
</div>
-->

## Vorlage an ein vorhandenes Projekt anhängen {#attach-a-template-to-an-existing-project}

Sie können eine Vorlage über die Projektseite oder eine Projektliste oder einen Bericht an ein Projekt anhängen.

{{step1-to-projects}}

1. Wählen Sie auf **Seite** das Projekt aus, dem Sie eine Vorlage anhängen möchten.

1. Klicken Sie auf **Mehr**-Symbol ![Mehr Dropdown](assets/more-dropdown.png) rechts neben dem Projektnamen.

   ![Symbol „Mehr“](assets/qs-more-icon-on-an-object.png)

   ODER

   Gehen Sie zu einer Projektliste oder einem Bericht, wählen Sie ein Projekt aus und klicken Sie dann oben in der Liste auf das **Mehr** Symbol ![Mehr](assets/more-dropdown.png)Dropdown-Liste.

   ![Mehr Menü erweitert](assets/more-menu-expanded.png)

1. Klicken Sie **Vorlage anhängen**. Das Feld **Vorlage anhängen** wird angezeigt.

1. Geben Sie zunächst den Namen der Vorlage, die Sie anhängen möchten, in das Feld **Suchvorlagen** ein und klicken Sie dann auf die Vorlage, wenn sie in der Liste angezeigt wird.

   ODER

   Klicken Sie auf den Namen einer Vorlage im Bereich **Sonstige Vorlagen**.

   Rechts wird eine Vorschau der Vorlage angezeigt, die die folgenden Informationen zur Vorlage enthält:

   * Dauer
   * Besitzerin bzw. Besitzer
   * Die Anzahl der Aufgaben der obersten Ebene (enthält eine Liste der ersten drei Aufgaben der obersten Ebene)
   * Gesamtzahl der Aufgaben
   * Namen der benutzerdefinierten Formulare in Anhängen

   ![Vorlagenfeld anhängen](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Optional) Klicken Sie auf das Symbol **Favoriten** ![Favoritensymbol](assets/favorites-icon-small.png) rechts neben dem Vorlagennamen, um die Vorlage als Favorit zu markieren und in die Liste **Favoriten** zu verschieben.

1. (Optional) Klicken Sie erneut auf das **Favoriten**-Symbol ![Favoriten](assets/favorites-icon-selected.png), um es aus der Liste **Favoriten** zu entfernen.
1. Klicken Sie **Anpassen und anhängen**. Das Seitenbedienfeld **Vorlage anhängen** wird geöffnet.

1. (Optional) Aktualisieren Sie die Informationen in den folgenden Abschnitten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Abschnitt „Aufgaben“</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Die unten ausgewählten Vorlagenaufgaben werden in das Projekt importiert. Deaktivieren Sie die Auswahl der Einträge, die Sie ausschließen möchten. </td> 
      <td><p>Heben Sie die Markierung aller Aufgaben auf, die Sie aus der Vorlage ausschließen möchten, bevor Sie sie an das Projekt anhängen.</p>
      <p><b>TIPP</b></p>
      <p>Sie können nur eine Aufgabe auswählen.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wählen Sie die Projektaufgabe aus, die Sie als Vorgänger für die Aufgaben in dieser Vorlage haben möchten.</td> 
      <td> <p>Klicken Sie in das Feld Feld, um eine Liste der Projektaufgaben anzuzeigen, und wählen Sie dann aus, welche Aufgabe abgeschlossen sein muss, bevor die Vorlagenaufgaben beginnen können. Alternativ können Sie diesen Schritt überspringen und Beziehungen innerhalb des Projekts einrichten, nachdem die Vorlage angehängt wurde. </p> <p> Wählen Sie die Informationen <strong>Abhängigkeitstyp</strong>, <strong>Verzögerungszeit</strong> und , wenn Sie möchten, dass der Vorgänger erzwungen wird, indem Sie das Kontrollkästchen <strong>Vorgänger erzwingen</strong> aktivieren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wählen Sie die Projektaufgabe aus, die Sie als übergeordnetes Element der Aufgaben in dieser Vorlage haben möchten.</td> 
      <td> <p>Wählen Sie die Projektaufgabe aus, die Sie als übergeordnete Aufgabe für alle Vorlagenaufgaben festlegen möchten. Wenn Sie keine Auswahl treffen, werden alle Vorlagenaufgaben am Ende der aktuellen Projektaufgaben angezeigt. Sie können diesen Schritt überspringen und Aufgaben im Projekt verschieben, nachdem die Vorlage angehängt wurde.</p>
      <p><b>NOTIZ</b></p>
      <p>Wenn Sie eine übergeordnete Vorlagenaufgabe mit zusätzlichen untergeordneten Elementen ausgewählt haben, zeigt nur das übergeordnete Element die Projektaufgabe als Vorgänger an, nachdem sie dem Projekt hinzugefügt wurde. Für die untergeordneten Vorlagenaufgaben wird kein Vorgänger angezeigt.</p>
      <p>Wenn Sie nur eine untergeordnete Vorlagenaufgabe ausgewählt haben, wird die Projektaufgabe nach dem Hinzufügen zum Projekt als Vorgänger angezeigt. </p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Abschnitt Optionen</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Die ausgewählten Elemente unten werden in das Projekt übertragen. Deaktivieren Sie die Auswahl der Einträge, die Sie ausschließen möchten.</td> 
      <td> <p>Deaktivieren Sie die Kontrollkästchen für alle Informationen, die Sie aus der Vorlage ausschließen möchten, bevor Sie sie an das Projekt anhängen. Weitere Informationen zu den einzelnen Feldern finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Übersicht über das Anhängen einer Vorlage an ein Projekt</a>. </p> <p>Wichtig: Wenn Sie das Kontrollkästchen <strong>Warteschlangeneigenschaften und Problem-Setup</strong> aktivieren, überschreiben die Warteschlangendetails der Vorlage die des Projekts. In diesem Fall werden die Routing-Regeln, Warteschlangenthemen und Themengruppen der Vorlage zu denen des Projekts hinzugefügt. <br>Wenn das Projekt als Anforderungswarteschlange eingerichtet ist und die dem Projekt angehängte Vorlage nicht als Anforderungswarteschlange eingerichtet ist, werden die Warteschlangeninformationen des Projekts entfernt, wenn Sie das Kontrollkästchen <strong>Warteschlangeneigenschaften und Problem-Setup</strong> aktiviert lassen. <br>Wenn Sie das Kontrollkästchen <strong>Warteschlangeneigenschaften und Problem-Setup</strong> deaktivieren, bleiben alle Warteschlangeneinstellungen des Projekts erhalten und es werden keine Warteschlangeneinstellungen aus der Vorlage angehängt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Benutzerdefinierter Forms-Abschnitt</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Forms</td> 
      <td> <p>Wenn benutzerdefinierte Formulare an die Vorlage angehängt werden, werden ihre Namen im linken Bereich angezeigt. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Aktualisieren Sie die Informationen in den benutzerdefinierten Formularen. Diese Informationen werden an das Projekt übertragen.

   >[!TIP]
   >
   >* Dieser Schritt ist obligatorisch, wenn die benutzerdefinierten Formulare in der Vorlage erforderliche Felder enthalten, die leer sind.
   >* Wenn die Felder aus den benutzerdefinierten Vorlagenformularen bereits im Projekt vorhanden sind und Informationen enthalten, werden die bereits im Projekt enthaltenen Informationen beibehalten. Sie können sie beim Anhängen der Vorlage nicht bearbeiten.

1. Klicken Sie **Vorlage anhängen.**
1. Klicken Sie auf **Anlage abbrechen**, um das Anhängen der Vorlage abzubrechen.

   ODER

   Zulassen, dass der Anhang fertig gestellt wird, um die Vorlage zum Projekt hinzuzufügen.

   Nachdem Sie die Vorlage angehängt haben, können Sie das Projekt bearbeiten und alle Aufgaben, Informationen oder Einstellungen nach Bedarf anpassen.

1. (Optional) Klicken Sie im linken Bereich auf **Projektdetails** und dann auf **Übersicht**, um den Namen der Vorlage anzuzeigen, die Sie im Bereich **Projektbeziehungen** angehängt haben.

   >[!TIP]
   >
   >Wenn Sie mehr als eine Vorlage an das Projekt anhängen, wird nur die zuerst angehängte Vorlage in diesem Feld angezeigt. Weitere Informationen finden Sie [&#x200B; Abschnitt „Anhängen mehrerer Vorlagen an ein vorhandenes Projekt und Anzeigen &#x200B;](#attach-multiple-templates-to-an-existing-project-and-view-template-information) Vorlageninformationen“ in diesem Artikel.

1. (Optional) Entfernen Sie Vorlageninformationen aus dem Projekt, an das Sie die Vorlage angehängt haben. Weitere Informationen finden Sie unter [Entfernen von Vorlageninformationen aus einem Projekt](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Mehrere Vorlagen an ein vorhandenes Projekt anhängen und Vorlageninformationen anzeigen {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

Sie können mehrere Vorlagen (jeweils eine) an dasselbe Projekt anhängen, indem Sie die Schritte ausführen, die im Abschnitt [Anhängen einer Vorlage an ein vorhandenes Projekt](#attach-a-template-to-an-existing-project) in diesem Artikel beschrieben werden. Dadurch werden die Aufgaben und andere Informationen aus jeder Vorlage zum Projekt hinzugefügt.

>[!TIP]
>
>Wenn Sie mehrere Vorlagen an ein Projekt anhängen, wird nur die zuerst angehängte Vorlage im Bereich Projektdetails angezeigt.

So zeigen Sie an, welche Vorlage auf ein Projekt angewendet wird:

{{step1-to-projects}}

1. Wählen Sie auf **Seite** das Projekt aus, an das eine Vorlage angehängt ist.

1. Klicken Sie **linken** auf „Projektdetails“.

1. Suchen Sie den Namen der an das Projekt angehängten Vorlage im Feld **Vorlage** unten im Abschnitt **Übersicht** unter **Projektbeziehungen**.

   ![Vorlageninformationen zu einem Projekt](assets/nwe-template-info-on-project-350x356.png)


