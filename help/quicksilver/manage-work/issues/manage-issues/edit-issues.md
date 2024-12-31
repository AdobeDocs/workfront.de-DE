---
product-area: projects
navigation-topic: manage-issues
title: Probleme bearbeiten
description: Sie können Informationen zu Problemen bearbeiten, die Sie erstellt haben oder die andere Benutzer erstellt haben, wenn sie die Probleme mit Ihnen geteilt haben. In diesem Artikel wird beschrieben, wie Sie nach einem Problem suchen, es suchen und bearbeiten können, wenn Sie dazu berechtigt sind.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 1449374a-ab0d-4c98-83cd-4e511467633a
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '2523'
ht-degree: 2%

---

# Probleme bearbeiten

Sie können Informationen zu Problemen bearbeiten, die Sie erstellt haben oder die andere Benutzer erstellt haben, wenn sie die Probleme mit Ihnen geteilt haben.

Sie können ein einzelnes Problem bearbeiten oder Probleme in einer Liste bearbeiten. Informationen zum Bearbeiten von Problemen in einer Liste finden Sie unter [Probleme in einer Liste bearbeiten](../../../manage-work/issues/manage-issues/edit-issues-in-a-list.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anfrage oder höher</p> <p>Prüfen Sie die Lizenz oder eine höhere Lizenz zur Bearbeitung von Anfragen im Abschnitt Probleme einer Aufgabe oder eines Projekts.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen zum Zugriff auf Probleme in Ihrer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Probleme gewähren</a>. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>. </p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute-Berechtigungen für ein Problem , um die folgenden Felder im Detailbereich zu bearbeiten: </p>
   <ul>
   <li>Beschreibung</li>
   <li>Status</li>
   <li>Schweregrad</li>
   </ul>
   <p>Verwalten Sie die Berechtigungen für ein Problem, um alle Felder im Detailbereich oder im Feld „Problem bearbeiten“ zu bearbeiten</p> <p> Informationen zum Gewähren von Berechtigungen für Probleme finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Freigeben eines Problems </a></p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriff auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Einschränkungen beim Bearbeiten von Problemen

Es gibt einige Einschränkungen, die Sie möglicherweise daran hindern, Probleme zu bearbeiten.

* Probleme, die sich in einem Genehmigungsprozess befinden, können nicht bearbeitet werden. Sie können nur die Zeit protokollieren oder den Status für ein Problem aktualisieren, das sich in der Phase „Ausstehende Genehmigung“ befindet.
* Sie können Probleme in einem Projekt mit dem Status „Abgeschlossen“, „Eingestellt“ oder „Genehmigung steht aus“ nur dann bearbeiten oder Dokumente zu Problemen hinzufügen, wenn diese Funktion von Ihrem Workfront-Administrator oder einem Gruppenadministrator im Bereich Projektvoreinstellungen aktiviert wurde. Informationen zum Festlegen von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Einzelnes Problem bearbeiten

Sie können ein Problem über die Bereiche „Problem bearbeiten“ oder „Problemdetails“ bearbeiten. Die folgenden Schritte beschreiben die Bearbeitung eines Problems im Feld „Problem bearbeiten“.

1. Navigieren Sie zum **Hauptmenü**.
1. Klicken Sie **Projekte** und anschließend auf den Namen eines Projekts, um das Projekt zu öffnen.
1. (Optional) Klicken Sie auf **Aufgaben** und dann auf den Namen einer Aufgabe, um die Aufgabe zu öffnen.
1. Klicken Sie **linken** auf „Probleme“.

   ![](assets/qs-issues-icon-highlighted-on-project-350x278.png)

1. (Optional) Um eingeschränkte Informationen zu einem Problem zu bearbeiten, klicken Sie **linken Bereich auf** Problemdetails“.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator oder Gruppenadministrator Ihre Layout-Vorlage geändert hat, werden die Felder im Bereich Problemdetails möglicherweise neu angeordnet oder nicht angezeigt. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   Gehen Sie wie folgt vor, um Informationen im Abschnitt Details zu bearbeiten:

   1. (Optional) Klicken Sie auf **Symbol „Alle** reduzieren“ in der oberen rechten Ecke, um alle Bereiche zu reduzieren.
   1. (Optional und bedingt) Wenn ein Bereich reduziert ist, klicken Sie auf den **Nach rechts zeigenden Pfeil** ![](assets/right-pointing-arrow.png) neben jedem Bereich, um den Bereich zu erweitern, den Sie bearbeiten möchten.
   1. (Optional) Um ein benutzerdefiniertes Formular anzuhängen, geben Sie zunächst den Namen eines Formulars in das Feld **Benutzerdefiniertes Formular hinzufügen** ein, wählen Sie es aus, wenn es in der Liste angezeigt wird, und klicken Sie dann auf **Änderungen speichern**.
   1. (Optional) Klicken Sie auf das **Exportieren**-Symbol ![](assets/export.png), um die Übersichts- und benutzerdefinierten Formularinformationen in eine PDF-Datei zu exportieren, und klicken Sie dann auf **Exportieren**. Wählen Sie aus den folgenden Optionen aus:

      * Alle auswählen (wird nur angezeigt, wenn mindestens ein benutzerdefiniertes Formular angehängt ist)
      * Übersicht
      * Der Name eines oder mehrerer benutzerdefinierter Formulare

      Die PDF-Datei wird auf Ihren Computer heruntergeladen.

      ![](assets/export-issue-details-selection-box-with-export-button-350x418.png)

      Weitere Informationen finden Sie unter [Exportieren benutzerdefinierter Formulare und Objektdetails](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

   Um Informationen zu den Feldern zu erhalten, die im Abschnitt „Anfragedetails“ sichtbar sind, fahren Sie wie unten beschrieben mit dem Bearbeiten des Problems im Feld „Problem bearbeiten“ fort.

1. Um alle Informationen zu einem Problem zu bearbeiten, wählen Sie ein Problem in einer Liste aus und klicken **oben in** Liste auf „Bearbeiten“

   Oder

   Klicken Sie auf den Namen eines Problems in einer Liste und dann auf das Menü **Mehr** neben dem Problemnamen und anschließend auf **Bearbeiten**

   Das **Problem bearbeiten** wird angezeigt.

   >[!IMPORTANT]
   >
   >Sie müssen über Verwaltungsberechtigungen für das Problem verfügen, um den Link Bearbeiten sehen zu können.

   Alle Problemfelder sind im Feld „Problem bearbeiten“ verfügbar und werden nach den im linken Bedienfeld aufgelisteten Bereichen gruppiert.

1. Erwägen Sie, Informationen in einem der folgenden Abschnitte anzugeben:

   * [Name des Problems](#issue-name)
   * [Übersicht](#overview)
   * [Arbeitsaufträge](#assignments)
   * [Benutzerdefinierte Formulare](#Custom%C2%A0F)
   * [Einstellungen](#settings)

   >[!NOTE]
   >
   >Je nachdem, wie Ihr Workfront-Administrator Ihre Layout-Vorlage einrichtet, können die Felder im Feld „Problem bearbeiten“ in Ihrer Umgebung unterschiedlich sein. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
   >
   >Die meisten der in den folgenden Abschnitten aufgelisteten Felder sind auch über das Feld „Neues Problem“ zugänglich, wenn Sie ein Problem erstellen. Die Abschnitte, unter denen sich die Felder befinden, stimmen nicht mit dem Feld „Neues Problem“ überein. Informationen zum Erstellen von Problemen finden Sie unter [Erstellen von Problemen](../../issues/manage-issues/create-issues.md).

### Name des Problems {#issue-name}

1. Beginnen Sie mit der Bearbeitung eines Problems, wie oben beschrieben.
1. Klicken Sie **Anfragename**.

   ![](assets/issue-name-section-edit-issue-box-nwe-350x127.png)

1. Aktualisieren Sie das Feld **Problemname**.
1. Klicken Sie **Speichern** oder fahren Sie mit der Bearbeitung der folgenden Abschnitte fort.

### Übersicht {#overview}

1. Beginnen Sie mit der Bearbeitung eines Problems, wie oben beschrieben.
1. Klicken Sie auf **Übersicht**.

   ![](assets/overview-section-edit-issue-box-nwe-350x284.png)

1. Aktualisieren oder überprüfen Sie eines der Felder in der folgenden Tabelle:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td> <p>Fügen Sie zusätzliche Informationen zum Problem hinzu.</p> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader">Abschnitt „Grundlegende Informationen“</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td> <p>Wählen Sie den Status des Problems aus. Weitere Informationen zum Problemstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md" class="MCXref xref">Zugriff auf die Liste der Systemanfragestatus</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Priorität</td> 
      <td> <p>Dies ist eine visuelle Markierung, mit der Sie Probleme priorisieren können.</p> <p>Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p><strong>Keine</strong> </p> </li> 
        <li> <p><strong>Niedrig</strong> </p> </li> 
        <li> <p><strong>normal</strong> </p> </li> 
        <li> <p><strong>Hoch</strong> </p> </li> 
        <li> <p><strong>Dringend</strong> </p> </li> 
       </ul> <p>Je nach den vom Workfront-Administrator ausgewählten Projektvoreinstellungen können die Namen der Prioritäten für Sie unterschiedlich sein. Weitere Informationen zum Bearbeiten von Prioritäten finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md" class="MCXref xref">Erstellen und Anpassen von Prioritäten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schweregrad</td> 
      <td> <p>Dies ist eine visuelle Markierung, die anzeigt, wie schwerwiegend das in dem Problem beschriebene Problem ist. Schweregrade beziehen sich ausschließlich auf Probleme. Wählen Sie aus den folgenden Optionen aus:</p> 
       <ul> 
        <li> <p style="font-weight: bold;">Kosmetisch</p> </li> 
        <li> <p style="font-weight: bold;">Verwirrend</p> </li> 
        <li> <p style="font-weight: bold;">Programmfehler mit Umgehungslösung</p> </li> 
        <li> <p style="font-weight: bold;">Programmfehler ohne Umgehungslösung</p> </li> 
        <li> <p style="font-weight: bold;">Schwerer Fehler</p> </li> 
       </ul> <p>Je nach den von Ihrem Workfront-Administrator ausgewählten Projektvoreinstellungen können die Namen der Schweregrade für Sie unterschiedlich sein. Weitere Informationen zum Bearbeiten von Schweregraden finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md" class="MCXref xref">Erstellen oder Anpassen von </a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL</td> 
      <td> <p>Geben Sie einen Weblink ein, der sich auf die Informationen zum Problem bezieht.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typ</td> 
      <td> <p>Je nach den Warteschlangeneigenschaften, die Ihr Projekt-Manager im Bereich „Warteschlangendetails“ des Projekts ausgewählt hat, können Sie möglicherweise den Typ des Problems angeben. Wählen Sie im Dropdown-Menü <b>Typ</b> eine der folgenden Optionen aus: </p> 
       <ul> 
        <li> <p><strong>Bug-Bericht</strong> </p> </li> 
        <li> <p><strong>Änderungsanforderung</strong> </p> </li> 
        <li> <p><strong>Probleme</strong> </p> </li> 
        <li> <p><strong>Anfrage</strong> </p> </li> 
       </ul> <p>Je nach den von Ihrem Workfront-Administrator ausgewählten Projektvoreinstellungen können die Namen der Problemtypen für Sie unterschiedlich sein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hauptansprechpartner</td> 
      <td>Standardmäßig ist der Primäre Kontakt der Ersteller des Problems. Um dies zu ändern, beginnen Sie, den Namen eines aktiven Benutzers in Workfront einzugeben, und wählen Sie ihn dann aus der Liste aus. Ein Problem kann nur einen Primären Kontakt haben.<br> Wenn Sie den Primären Kontakt ändern, hat der ursprüngliche primäre Kontakt weiterhin Verwaltungszugriff auf das Problem. Sie müssen diesen Zugriff manuell aus dem Zugriffsfeld für Probleme entfernen, wenn Sie ein Problem freigeben.

   <b>TIPP</b>

   <p>Beachten Sie beim Hinzufügen eines Benutzers des Typs "Primärer Kontakt“ den Avatar, die Primäre Rolle des Benutzers und seine E-Mail-Adresse, um zwischen Benutzern mit identischen Namen zu unterscheiden. Benutzende müssen mindestens einem Aufgabengebiet zugeordnet sein, damit sie es beim Hinzufügen anzeigen können.</p>
      <p> Die Einstellung Kontaktinformationen anzeigen muss in Ihrer Zugriffsebene aktiviert sein, damit Benutzer die E-Mails von Benutzern anzeigen können. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md">Gewähren des Benutzerzugriffs</a>.</p>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Commit-Datum und -Uhrzeit</td> 
      <td> <p>Dies ist das Datum, an dem der Bevollmächtigte der Anfrage schätzt, dass die Anfrage abgeschlossen wird. Nur Beauftragte können dieses Feld bearbeiten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplantes Startdatum</td> 
      <td>Standardmäßig ist das geplante Startdatum das Datum und die Uhrzeit, zu der das Problem erstellt wurde. Sie können das <strong>Geplantes Startdatum) </strong> Problems aktualisieren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geplantes Abschlussdatum und -zeit</td> 
      <td> Standardmäßig liegt das geplante Abschlussdatum 24 Stunden vor dem standardmäßigen geplanten Startdatum. Standardmäßig haben Probleme eine Dauer von 1 Tag. Sie können das <strong>geplante Abschlussdatum</strong> des Problems aktualisieren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliches Startdatum und Uhrzeit</td> 
      <td>Das tatsächliche Startdatum wird automatisch eingetragen, wenn Sie den Status des Problems in "<strong>" </strong>. Sie können das <strong>Tatsächliche Startdatum</strong> des Problems aktualisieren. Sie können das Datum bei Bedarf manuell aktualisieren. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tatsächliches Abschlussdatum und -uhrzeit</td> 
      <td>Das tatsächliche Abschlussdatum wird automatisch ausgefüllt, wenn Sie den Status des Problems in „Geschlossen<strong> </strong> oder <strong>" </strong>. Sie können das <strong>Tatsächliche Abschlussdatum</strong> für das Problem aktualisieren. Sie können das Datum bei Bedarf manuell aktualisieren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gelöst von</td> 
      <td> <p>Dies zeigt an, ob das Problem durch ein anderes Objekt behoben wurde. Sie können aus dem Dropdown-Menü auswählen, ob dieses Problem durch eine Aufgabe, ein Projekt oder ein anderes Problem gelöst werden soll, und dann beginnen, den Namen der Aufgabe, des Projekts oder des Problems einzugeben, die bzw. das das Problem lösen soll. Auswählen, wenn es in der Liste angezeigt wird.</p>

   <b>HINWEIS</b>

   Wenn Sie ein Objekt auswählen, um ein Problem zu beheben, wird der Problemstatus mit dem Status des Lösungsobjekts verknüpft und kann bei dem Problem nicht geändert werden. Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und das Auflösen von Objekten </a>.

   <b>TIPP</b>

   Wenn Ihr System- oder Gruppenadministrator das Feld „Gelöst von“ zu einer benutzerdefinierten Kopfzeile eines Problems hinzufügt, ändert sich das Feld in „Problem lösen“, „Aufgabe lösen“ oder „Projekt lösen“, wenn ein Lösungsobjekt mit dem Problem verknüpft ist.

   Dieses Feld kann nicht bearbeitet werden, wenn es in der Anfragekopfzeile angezeigt wird. Weitere Informationen zum Anpassen von Problem-Headern finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md">Anpassen von Objekt-Headern mithilfe einer Layout-Vorlage </a>
   </td> 
     </tr>

   <tr> 
      <td role="rowheader">Problem lösen, Aufgabe lösen oder Projekt lösen</td> 
      <td>Der verknüpfte Name des Problems, der Aufgabe oder des Problems, die bzw. das das Problem löst.  </td> 
     </tr> 
      <tr> 
      <td role="rowheader">Dies löst</td> 
      <td>Verknüpfter Name des Problems, das abgeschlossen wird, wenn das Problem, auf das Sie zugreifen, behoben ist.  </td> 
     </tr>


   </tbody> 
   </table>





1. Klicken Sie **Speichern** oder fahren Sie mit der Bearbeitung der folgenden Abschnitte fort.

#### Arbeitsaufträge {#assignments}

1. Beginnen Sie mit der Bearbeitung des Problems wie oben beschrieben.
1. Klicken Sie **linken** auf „Arbeitsaufträge“.

   ![](assets/assignments-section-edit-issue-box-nwe-350x230.png)

1. Klicken Sie auf **Personen, Rollen und Teams suchen** und geben Sie den Namen eines Benutzers, einer Rolle oder eines Teams ein, den/das Sie der Aufgabe zuweisen möchten. Klicken Sie dann auf den Namen oder drücken Sie die Eingabetaste, wenn er/sie in der Liste angezeigt wird.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this is still called this; asked Anna to change it to "roles" and add a comma)</p>
   -->

   >[!NOTE]
   >
   >Wenn der Name des Benutzers ein Sonderzeichen enthält, müssen Sie das Sonderzeichen in das Suchfeld einschließen.

   >[!TIP]
   >
   >Sie können mehrere Benutzer, Aufgabengebiete oder Teams zuweisen. Sie können nur aktive Benutzer, Aufgabengebiete und Teams zuweisen.
   >
   >
   >Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team zugewiesen wurde, bevor sie/er deaktiviert wurden, bleiben sie/sie dem Arbeitselement zugewiesen. In diesem Fall empfehlen wir Folgendes:
   >
   >* Weisen Sie das Arbeitselement den aktiven Ressourcen neu zu.
   >* Verknüpfen Sie die Benutzer in einem deaktivierten Team mit einem aktiven Team und weisen Sie das Arbeitselement dem aktiven Team zu.

1. (Optional) Geben Sie an, ob ein Bevollmächtigter der primäre Bevollmächtigte für das Problem ist, indem Sie den Mauszeiger über den Namen des Bevollmächtigten bewegen und auf **Primär machen** klicken. Ein Team kann nicht der primäre Zugewiesene eines Problems sein.
1. Aktualisieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Geplante Stunden</td> 
      <td> <p>Dies ist die tatsächliche Zeit, die die Verantwortlichen der Anfrage benötigen würden, um diese abzuschließen. Geben Sie die Anzahl der geplanten Stunden für das Problem ein.<br></p> <p>Hinweis: Durch eine Änderung der geplanten Stunden für die Anfrage wird das geplante Abschlussdatum der Anfrage nicht geändert. </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Rolle des Zugewiesenen</td> 
      <td> <p>Wählen Sie eine Rolle aus dem Dropdown<strong>Menü „Rolle des Verantwortlichen</strong> aus, wenn Sie eine Person als Verantwortlicher ausgewählt haben. Dies ist die Rolle, die der Beauftragte in dieser Anfrage erfüllen kann. </p> <p><b>TIPP</b>

   Im Dropdown-Menü werden nur die Aufgabengebiete angezeigt, die jedem Bearbeiter in seinem Profil zugeordnet sind.</p> </td>
   </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Speichern** oder fahren Sie mit der Bearbeitung der folgenden Abschnitte fort.

### Benutzerdefinierte Forms

1. Beginnen Sie mit der Bearbeitung eines Problems, wie oben beschrieben.
1. Klicken Sie **Benutzerdefinierte Forms**.

   ![](assets/custom-forms-section-edit-issue-box-nwe-350x132.png)

1. Wählen Sie im Feld **Benutzerdefiniertes Formular hinzufügen** das oder die benutzerdefinierten Formulare aus, die Sie mit dem Problem verknüpfen möchten. Sie müssen die benutzerdefinierten Formulare erstellen, bevor sie in diesem Feld ausgewählt werden können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Sie können bis zu zehn benutzerdefinierte Formulare zu einem Problem hinzufügen.

1. (Bedingt) Wenn Sie ein benutzerdefiniertes Formular an das Problem angehängt haben, bearbeiten Sie alle Felder im Formular. Sie müssen alle erforderlichen Felder angeben, bevor Sie das Problem speichern können.

   >[!NOTE]
   >
   >Je nachdem, wie der Workfront-Administrator die Berechtigungen für die Abschnitte in Ihrem benutzerdefinierten Formular festgelegt hat, können nicht alle dieselben Felder in einem bestimmten benutzerdefinierten Formular anzeigen oder bearbeiten. Die Berechtigungen zum Bearbeiten von Feldern innerhalb eines Abschnitts eines benutzerdefinierten Formulars hängen von den Berechtigungen ab, die Sie für das Problem selbst haben. Informationen zum Festlegen von Berechtigungen für Abschnitte eines benutzerdefinierten Formulars finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). Informationen zum Festlegen von Problemberechtigungen finden Sie unter [Freigeben eines Problems](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

1. Klicken Sie **Speichern** oder fahren Sie mit der Bearbeitung des folgenden Abschnitts fort.

### Einstellungen {#settings}

1. Beginnen Sie mit der Bearbeitung eines Problems, wie oben beschrieben.
1. Klicken Sie **Einstellungen**.

   ![](assets/settings-section-edit-issue-box-nwe-350x240.png)

   Aktualisieren Sie die folgenden Informationen:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Genehmigungsprozess</td> 
      <td> 
       <div> 
       <p>Wählen Sie einen Genehmigungsprozess aus, den Sie mit dem Problem verknüpfen möchten. Ihr Workfront-Administrator muss Genehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Problemen verknüpfen können. Benutzende mit administrativem Zugriff auf Genehmigungsprozesse <span> können auch gruppenspezifische Genehmigungsprozesse erstellen.</span>Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>. </p> 
       <p>Beachten Sie beim Hinzufügen von Genehmigungsprozessen Folgendes: </p> 
       <ul> 
       <li>In der Liste werden nur aktive Genehmigungsprozesse angezeigt. </li> 
       <li> <p>In der Liste werden systemweite und gruppenspezifische Genehmigungsprozesse angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt.</p> <p>Wichtig: Wenn sich die Gruppe des Projekts ändert, wird der gruppenspezifische Genehmigungsprozess zu einem einmaligen Genehmigungsprozess. Weitere Informationen darüber, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken</a>. </p> </li> 
       <li> <p>Sie können standardmäßige Genehmigungsprozesse definieren, die beim Erstellen von Anfrage-Warteschlangen oder Warteschlangenthemen automatisch an Probleme angehängt werden. Informationen zum Aktualisieren von Warteschlangendetails finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anfrage-Warteschlange</a>. Informationen zum Erstellen von Warteschlangenthemen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Warteschlangenthemen erstellen</a>. </p> </li> 
       <li>Bei Problemen mit der Massenbearbeitung gibt es die folgenden Szenarien: 
       <ul> 
       <li><p>Wenn Sie mehrere Probleme aus derselben Gruppe auswählen, werden in diesem Feld sowohl systemweite als auch gruppenspezifische Genehmigungsprozesse angezeigt.</p></li> 
       <li><p>Wenn Sie mehrere Probleme aus verschiedenen Gruppen auswählen, werden in diesem Feld nur Genehmigungsprozesse auf Systemebene angezeigt.</p></li> 
       <li><p>Wenn für eines der Probleme ein Genehmigungsprozess für den einmaligen Gebrauch angehängt ist, wird es durch den von Ihnen ausgewählten Genehmigungsprozess auf Systemebene oder Gruppenebene ersetzt. </p></li> 
       </ul></li> 
       </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td> <p>Aktivieren Sie das Kontrollkästchen, für das Sie Erinnerungsnachrichten an dieses Problem anhängen möchten. Alle Erinnerungsnachrichten für Probleme werden angezeigt. Ihr Workfront-Administrator muss Erinnerungsnachrichten konfigurieren, bevor Sie sie für ein Problem auswählen können. Weitere Informationen zum Konfigurieren von Erinnerungsnachrichten finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md" class="MCXref xref">Einrichten von Erinnerungsnachrichten</a></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern.**

## Problem in der Anfragekopfzeile bearbeiten (begrenzt)

Sie können eine begrenzte Menge an Informationen in der Anfrage-Kopfzeile bearbeiten.

Ihr System- oder Gruppenadministrator kann die Felder anpassen, die Sie im Problem-Header sehen. Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

![](assets/issue-header-350x19.png)

Die folgenden Felder sind standardmäßig in der Anfrage-Kopfzeile enthalten:

* Name des Problems
* Prozent abgeschlossen
* Arbeitsaufträge
* Geplantes Abschlussdatum und -zeit
* Status
* Treffen von Genehmigungsentscheidungen, wenn Sie in einem aktuellen Genehmigungsprozess als genehmigende Person festgelegt sind
