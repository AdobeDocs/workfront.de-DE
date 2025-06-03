---
product-area: templates
navigation-topic: templates-navigation-topic
title: Vorlage an ein Projekt anhängen
description: Sie können eine Vorlage entweder während der ersten Erstellungsphase des Projekts oder nach seiner Erstellung an ein Projekt anhängen.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: 0792651822fd85cb3bfbb754aaf949c4fc4038a1
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# Vorlage an ein Projekt anhängen

<!-- Audited: 5/2025 -->

Sie können eine Vorlage entweder während der ersten Erstellungsphase des Projekts oder nach seiner Erstellung an ein Projekt anhängen.

Weitere Informationen zum Erstellen eines Projekts mithilfe einer Vorlage finden Sie unter [Erstellen eines Projekts mithilfe einer Vorlage](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p>
   <p>Oder</p>
   <p>Aktuell: Plan</p>
    </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten </p> <p>Informationen zum Projektzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Zugriff auf Projekte gewähren</a>.</p> <p>Zugriff auf Vorlagen anzeigen</p> <p>Informationen zu Vorlagenberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Freigeben einer Vorlage</a>. </p> <p>Informationen zum Zugriff auf Vorlagen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Zugriff auf Vorlagen gewähren</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen und Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt</p> <p>Informationen zu Projektberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>. </p> <p>Anzeigen von Berechtigungen oder höher für die Vorlage</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

1. Klicken Sie auf **Mehr**-Symbol ![Mehr](assets/qs-more-icon-on-an-object.png) rechts neben dem Projektnamen.

   ![Dropdown „Mehr“](assets/more-dropdown.png)

   Oder

   Gehen Sie zu einer Projektliste oder einem Bericht und wählen Sie ein Projekt aus und klicken Sie dann oben in der Liste auf das **Mehr** Symbol ![Mehr](assets/qs-more-icon-on-an-object.png)Symbol Mehr).

   ![Mehr Menü erweitert](assets/more-menu-expanded.png)


1. Klicken Sie **Vorlage anhängen**. Das Feld **Vorlage anhängen** wird angezeigt.

1. Geben Sie zunächst den Namen der Vorlage, die Sie anhängen möchten, in das Feld **Suchvorlagen** ein und klicken Sie dann auf die Vorlage, wenn sie in der Liste angezeigt wird.

   Oder

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
      <td>Heben Sie die Markierung aller Aufgaben auf, die Sie aus der Vorlage ausschließen möchten, bevor Sie sie an das Projekt anhängen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wählen Sie die Projektaufgabe aus, die Sie als Vorgänger für die Aufgaben in dieser Vorlage haben möchten.</td> 
      <td> <p>Klicken Sie auf das Feld, um eine Liste der Projektaufgaben anzuzeigen, und wählen Sie dann aus, welche Aufgabe abgeschlossen sein muss, bevor die Vorlagenaufgaben beginnen können. Alternativ können Sie diesen Schritt überspringen und Beziehungen innerhalb des Projekts einrichten, nachdem die Vorlage angehängt wurde. </p> <p> Wählen Sie die Informationen <strong>Abhängigkeitstyp</strong>, <strong>Verzögerungszeit</strong> und , wenn Sie möchten, dass der Vorgänger erzwungen wird, indem Sie das Kontrollkästchen <strong>Vorgänger erzwingen</strong> aktivieren. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wählen Sie die Projektaufgabe aus, die Sie als übergeordnetes Element der Aufgaben in dieser Vorlage haben möchten.</td> 
      <td> Wählen Sie die Projektaufgabe aus, die Sie als übergeordnete Aufgabe für alle Vorlagenaufgaben festlegen möchten. Wenn Sie keine Auswahl treffen, werden alle Vorlagenaufgaben am Ende der aktuellen Projektaufgaben angezeigt. Sie können diesen Schritt überspringen und Aufgaben im Projekt verschieben, nachdem die Vorlage angehängt wurde.</td> 
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

   Oder

   Zulassen, dass der Anhang fertig gestellt wird, um die Vorlage zum Projekt hinzuzufügen.

   Nachdem Sie die Vorlage angehängt haben, können Sie das Projekt bearbeiten und alle Aufgaben, Informationen oder Einstellungen nach Bedarf anpassen.

1. (Optional) Klicken Sie im linken Bereich auf **Projektdetails** und dann auf **Übersicht**, um den Namen der Vorlage anzuzeigen, die Sie im Bereich **Projektbeziehungen** angehängt haben.

   >[!TIP]
   >
   >Wenn Sie mehr als eine Vorlage an das Projekt anhängen, wird nur die zuerst angehängte Vorlage in diesem Feld angezeigt. Weitere Informationen finden Sie [ Abschnitt „Anhängen mehrerer Vorlagen an ein vorhandenes Projekt und Anzeigen ](#attach-multiple-templates-to-an-existing-project-and-view-template-information) Vorlageninformationen“ in diesem Artikel.

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


