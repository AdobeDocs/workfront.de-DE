---
product-area: templates
navigation-topic: templates-navigation-topic
title: Eine Vorlage an ein Projekt anhängen
description: Sie können eine Vorlage entweder während der ersten Erstellungsphase des Projekts oder nach seiner Erstellung an ein Projekt anhängen.
author: Alina
feature: Work Management
exl-id: bce9af59-5467-4458-b923-01bfa469e2d8
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 0%

---

# Eine Vorlage an ein Projekt anhängen

Sie können eine Vorlage entweder während der ersten Erstellungsphase des Projekts oder nach seiner Erstellung an ein Projekt anhängen.

Weitere Informationen zum Erstellen eines Projekts mit einer Vorlage finden Sie unter [Erstellen eines Projekts mit einer Vorlage](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die in diesem Artikel beschriebenen Schritte durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten </p> <p>Weitere Informationen zum Projektzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Gewähren des Zugriffs auf Projekte</a>.</p> <p>Zugriff auf Vorlagen anzeigen</p> <p>Weitere Informationen zu Vorlagenberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md" class="MCXref xref">Vorlagenfreigabe</a>. </p> <p>Informationen zum Vorlagenzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Gewähren des Zugriffs auf Vorlagen</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt verwalten</p> <p>Weitere Informationen zu Projektberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>. </p> <p>Berechtigungen für die Vorlage anzeigen oder höher</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

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

## Eine Vorlage an ein vorhandenes Projekt anhängen {#attach-a-template-to-an-existing-project}

Sie können eine Vorlage an ein Projekt in Workfront von der Projektseite aus oder von einer Projektliste oder einem Bericht aus anhängen.

1. Wechseln Sie zu dem Projekt, an das Sie eine Vorlage anhängen möchten, und klicken Sie auf das Symbol **Mehr** ![](assets/qs-more-icon-on-an-object.png) rechts neben dem Projektnamen

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   Oder

   Wechseln Sie zu einer Projektliste oder einem Bericht, wählen Sie ein Projekt aus und klicken Sie dann oben in der Liste auf das Symbol **Mehr** ![](assets/qs-more-icon-on-an-object.png) .

   ![](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)


1. Klicken Sie auf **Vorlage anhängen**.

   Das Feld Vorlage anhängen wird angezeigt.

1. Beginnen Sie mit der Eingabe des Namens der Vorlage, die Sie anhängen möchten, im Feld **Suchvorlagen** und klicken Sie dann darauf, wenn sie angezeigt wird.in der Liste

   Oder

   Klicken Sie im Bereich **Andere Vorlagen** auf den Namen einer Vorlage.

   Rechts wird eine Vorschau der Vorlage mit den folgenden Informationen zur Vorlage angezeigt:

   * Dauer
   * Besitzerin bzw. Besitzer
   * Die Anzahl der Aufgaben auf oberster Ebene (einschließlich einer Liste der ersten drei Aufgaben auf oberster Ebene)
   * Gesamtzahl der Aufgaben
   * Namen angehängter benutzerdefinierter Formulare

   ![](assets/attach-template-box-template-preview-area-nwe-350x282.png)

1. (Optional) Klicken Sie auf das Symbol **Favoriten** links neben dem Vorlagennamen, um ihn als Favoriten zu kennzeichnen. ![](assets/favorites-icon-small.png) Dadurch wird die Vorlage in die Favoritenliste verschoben.

   ![](assets/favorites-icon-on-template-list-in-attach-template-box-nwe-350x79.png)

1. (Optional) Klicken Sie erneut auf das Symbol **Favoriten** ![](assets/favorites-icon-selected.png) , um es aus der Favoritenliste zu entfernen.
1. Klicken Sie auf **Anpassen und anhängen**.

   ![](assets/attach-template-large-box-nwe-350x262.png)

1. Aktualisieren Sie die Informationen in den folgenden Abschnitten, bevor Sie die Vorlage anhängen (oder klicken Sie jederzeit auf **Vorlage anhängen** ):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Aufgabenbereich</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-tasks-section-nwe-350x289.png" style="width: 350;height: 289;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Die folgenden Vorlagenaufgaben werden in das Projekt importiert. Heben Sie die Auswahl der Personen auf, die Sie ausschließen möchten. </td> 
      <td>Heben Sie die Auswahl aller Aufgaben auf, die Sie aus der Vorlage ausschließen möchten, bevor Sie sie an das Projekt anhängen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wählen Sie die Projektaufgabe aus, die Sie als Vorgänger für die Aufgaben in dieser Vorlage benötigen.</td> 
      <td> <p>Klicken Sie auf das Feld, um eine Liste der Projektaufgaben anzuzeigen. Wählen Sie die Projektaufgabe aus, die beendet werden soll, bevor die Vorlagenaufgaben beginnen können. Alternativ können Sie diesen Schritt überspringen und Beziehungen innerhalb des Projekts einrichten, nachdem die Vorlage angehängt wurde. </p> <p> Wählen Sie die Informationen <strong>Abhängigkeitstyp</strong>, <strong>Lag</strong> und ob der Vorgänger <strong>erzwungen</strong> sein soll oder nicht. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Wählen Sie die Projektaufgabe aus, die Sie als übergeordnetes Element der Aufgaben in dieser Vorlage verwenden möchten.</td> 
      <td> Wählen Sie die Projektaufgabe aus, die Sie als übergeordnete Aufgabe für alle Vorlagenaufgaben festlegen möchten. Wenn Sie keine Auswahl treffen, werden alle Vorlagenaufgaben am Ende Ihrer aktuellen Projektaufgaben angezeigt. Sie können diesen Schritt überspringen und Aufgaben im Projekt verschieben, nachdem die Vorlage angehängt wurde.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Optionsabschnitt</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-options-section-nwe-350x78.png" style="width: 350;height: 78;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Die unten ausgewählten Elemente werden in das Projekt übertragen. Heben Sie die Auswahl der Personen auf, die Sie ausschließen möchten.</td> 
      <td> <p>Deaktivieren Sie die Kontrollkästchen neben allen Informationen, die Sie aus der Vorlage löschen möchten, bevor Sie sie an das Projekt anhängen. Diese Informationen werden nicht von der Vorlage an das Projekt übertragen. Weitere Informationen zu den einzelnen Feldern finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/attach-template-to-project-overview.md" class="MCXref xref">Übersicht über das Anhängen einer Vorlage an ein Projekt</a>. </p> <p>Wichtig: Wenn Sie das Kontrollkästchen <strong>Eigenschaften der Warteschlange und Problemeinrichtung</strong> aktivieren, werden die Details der Warteschlange der Vorlage überschrieben. In diesem Fall werden die Routing-Regeln, Warteschlangenthemen und Themengruppen der Vorlage zu denen des Projekts hinzugefügt. <br>Wenn das Projekt als Anforderungswarteschlange eingerichtet ist und die Vorlage, die Sie an das Projekt anhängen, nicht als Anforderungswarteschlange eingerichtet ist, werden die Warteschlangeninformationen des Projekts entfernt, wenn Sie das Kontrollkästchen <strong>Eigenschaften der Warteschlange und Einrichtung der Probleme</strong> aktiviert lassen. <br>Wenn Sie das Feld <strong>Eigenschaften der Warteschlange und Problemeinrichtung</strong> deaktivieren, werden alle Einstellungen für die Warteschlangeneinrichtung des Projekts beibehalten und es werden keine Einstellungen für die Warteschlangeneinrichtung aus der Vorlage angehängt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p role="rowheader" colspan="2">Benutzerspezifischer Forms-Abschnitt</p> <p role="rowheader" colspan="2"> <img src="assets/attach-template-large-box-custom-forms-section-nwe-350x274.png" style="width: 350;height: 274;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefinierte Forms</td> 
      <td> <p>Wenn benutzerdefinierte Formulare an die Vorlage angehängt werden, werden ihre Namen im linken Bereich angezeigt. </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Aktualisieren Sie die Informationen in den benutzerdefinierten Formularen. Diese Informationen werden an das Projekt übermittelt.

   >[!TIP]
   >
   >* Dieser Schritt ist obligatorisch, wenn die benutzerdefinierten Formulare in der Vorlage leere erforderliche Felder enthalten.
   >* Wenn die Felder aus der Vorlage bereits im Projekt vorhanden sind und Informationen enthalten, bleiben die bereits im Projekt enthaltenen Informationen erhalten. Sie können sie beim Anhängen der Vorlage nicht bearbeiten.

1. Klicken Sie auf **Vorlage anhängen.**
1. Klicken Sie auf **Anlage abbrechen** , um die Vorlage nicht mehr anzuhängen.

   Oder

   Lassen Sie die Fertigstellung der Anlage zu, um die Vorlage zum Projekt hinzuzufügen.

   Nachdem Sie die Vorlage angehängt haben, können Sie das Projekt bearbeiten und alle Aufgaben, Informationen oder Einstellungen nach Bedarf anpassen.

1. (Optional) Klicken Sie auf **Projektdetails** und dann auf **Überblick** , um den Namen der Vorlage anzuzeigen, die Sie im Bereich **Projektbeziehungen** angehängt haben.

   >[!TIP]
   >
   >Wenn Sie dem Projekt mehr als eine Vorlage anhängen, wird nur die zuvor angehängte Vorlage in diesem Feld angezeigt. Weitere Informationen finden Sie im Abschnitt [Mehrere Vorlagen an ein vorhandenes Projekt anhängen und Vorlageninformationen anzeigen](#attach-multiple-templates-to-an-existing-project-and-view-template-information) in diesem Artikel.

1. (Optional) Entfernen Sie Vorlageninformationen aus dem Projekt, an das Sie die Vorlage angehängt haben. Weitere Informationen finden Sie unter [Vorlageninformationen aus einem Projekt entfernen](../../../manage-work/projects/create-and-manage-templates/remove-template-from-project.md).

## Mehrere Vorlagen an ein vorhandenes Projekt anhängen und Vorlageninformationen anzeigen {#attach-multiple-templates-to-an-existing-project-and-view-template-information}

Sie können mehrere Vorlagen (einzeln) an dasselbe Projekt anhängen, indem Sie die im Abschnitt [Anhängen einer Vorlage an ein vorhandenes Projekt](#attach-a-template-to-an-existing-project) in diesem Artikel beschriebenen Schritte befolgen. Dadurch werden die Aufgaben und andere Informationen aus den einzelnen Vorlagen zum Projekt hinzugefügt.

>[!TIP]
>
>Wenn Sie einem Projekt mehrere Vorlagen anhängen, wird nur die Vorlage, die Sie zuerst angehängt haben, im Bereich Projektdetails angezeigt.

So erfahren Sie, welche Vorlage auf ein Projekt angewendet wird:

1. Navigieren Sie zu einem Projekt, an das eine Vorlage angehängt ist.
1. Klicken Sie im linken Bereich auf **Projektdetails** .
1. Suchen Sie den Namen der mit dem Projekt verknüpften Vorlage im Feld **Vorlage** unten im Abschnitt **Überblick** unter **Projektbeziehungen** .

   ![](assets/nwe-template-info-on-project-350x356.png)


