---
title: Anforderungen kopieren und senden
description: Wenn Sie ähnliche Anfragen häufig senden, können Sie eine vorhandene gesendete Anfrage kopieren. In diesem Fall können Sie eine vorhandene Anfrage kopieren, minimal ändern und als neue Anfrage erneut senden.
author: Alina
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 1%

---

# Anforderungen kopieren und senden

Wenn Sie ähnliche Anfragen häufig senden, können Sie eine vorhandene gesendete Anfrage kopieren. In diesem Fall können Sie eine vorhandene Anfrage kopieren, minimal ändern und als neue Anfrage erneut senden.

<!--Old?? 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td> <p>Neu: Mitwirkender oder höher</p>
   Oder
   <p>Aktuell: Anforderung oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p>  </td> 
  </tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Zugriff zum Hinzufügen von Anfragen zu einer Anfragewarteschlange</p> <p>Anzeigen von oder höheren Berechtigungen für die vorhandene Anfrage</p> <p>Informationen zum Einrichten einer Anfrage-Warteschlange finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anfrage-Warteschlange</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen über eine Anfrage verfügen, die Sie oder eine andere Person in Ihrem Unternehmen zuvor gesendet haben, um sie kopieren und erneut senden zu können. Wenn die Anfrage zu einer anderen Person gehört, müssen Sie mindestens über Zugriff auf die Option Anzeigen verfügen, um sie als neu kopieren und senden zu können.

## Überlegungen zum Kopieren und Senden von Anfragen als neu

* Sie können nur gesendete Anfragen kopieren und senden. Entworfene Anfragen können nicht kopiert werden.
* Sie können ursprünglich gesendete Anfragen oder Anfragen, die von anderen gesendet wurden, kopieren und senden, wobei Sie zumindest Zugriff auf „Anzeigen“ haben.
* Sie haben immer Zugriff auf das Kopieren und Senden einer Kopie Ihrer eigenen Anfragen, es sei denn, jemand hat Ihre Berechtigungen für diese entfernt.
* Der Zugriff auf Anfragen zum Kopieren und Senden, die ursprünglich von anderen Benutzern gesendet wurden, kann automatisch Personen in derselben Firma gewährt werden, wenn der Ersteller der Anfrage-Warteschlange die **Personen aus derselben Firma erben dieselben Berechtigungen für alle Anfragen** in den Bereichen Warteschlangendetails oder Projekt bearbeiten aktiviert. Wenn Sie diese Einstellung deaktivieren, kann nur der ursprüngliche Anfragende seine eigenen Anfragen anzeigen.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Anfrage-Warteschlange erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md)

* Sie können die Kopie der ursprünglichen Anfrage aktualisieren, bevor Sie sie als neue Anfrage erneut senden.
* Wenn die folgenden Änderungen nach dem Senden der ursprünglichen Anfrage auftreten, können Sie diese nicht mehr kopieren und erneut senden:

   * Die Anfrage-Warteschlange wurde gelöscht.
   * Das Warteschlangenthema wurde gelöscht.

     >[!TIP]
     >
     >Wenn das Warteschlangenthema das einzige in der Anfragewarteschlange war, können Sie die Anfrage dennoch kopieren und senden und sie wird in der Anfragewarteschlange selbst gespeichert.

   * Die Anfrage-Warteschlange wird nicht mehr als Hilfe-Anfrage-Warteschlange veröffentlicht. Weitere Informationen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Wenn die Anfrage-Warteschlange kein Warteschlangenthema enthält und die ursprüngliche Anfrage vor Januar 2022 gesendet wurde.

   * Der Status des Projekts, das mit der Anfrage-Warteschlange verknüpft ist, ist nicht mehr aktuell.

* Sie können eine Kopie einer konvertierten Anfrage kopieren und senden, wenn die Anfrage im Konvertierungsprozess beibehalten wurde. Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >Die kopierte Anfrage ist nicht mit einem anfragelösenden Objekt verknüpft.

## Anforderungen kopieren und senden

{{step1-to-requests}}

1. (Bedingt) Wenn der Abschnitt „Gesendet“ nicht standardmäßig angezeigt wird, klicken **im linken** auf „Gesendet“.

   >[!TIP]
   >
   >   Der Workfront- oder Gruppenadministrator bzw. die Gruppenadministratorin kann Ihre Layout-Vorlage anpassen und Bereiche aus dem Hauptmenü oder aus dem linken Bedienfeld in Ihrer Umgebung entfernen. In diesem Fall sind sie möglicherweise nicht für Sie verfügbar.

1. Suchen Sie die Anfrage, die Sie als neu kopieren und senden möchten, und führen Sie einen der folgenden Schritte aus:

   * Wählen Sie diese aus **klicken Sie dann** Kopieren![](assets/copy-and-submit-as-new-requests-area-nwe.png) oben links in der Liste „Gesendete Anfragen“.

   >[!TIP]
   >
   > Wenn Sie nicht zuerst eine Anfrage ausgewählt haben, wird das Kopiersymbol abgeblendet.

   * Klicken Sie auf das **Mehr**-Menü ![](assets/more-icon.png) rechts neben dem Anfragenamen und dann auf **Kopieren und als neu übermitteln**

     Oder

     Klicken Sie mit der rechten Maustaste auf die ausgewählte Anfrage und klicken Sie dann auf **Kopieren und als neu übermitteln**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Wenn Sie keinen Zugriff haben, um Probleme zu erstellen, erhalten Sie eine Warnung, dass Ihr Administrator Sie daran gehindert hat, Anfragen zu erstellen.

1. (Optional) Aktualisieren Sie bei Bedarf die folgenden Informationen:

   * **Anfrage-**: Die Anfrage-Warteschlange, in der die kopierte Anfrage gespeichert wird. Standardmäßig wird die kopierte Anfrage in der Anfragewarteschlange der ursprünglichen Anfrage gespeichert.
   * **Themengruppen** und **Warteschlangenthemen**, wenn sie ausgewählt sind. Die Namen von Themengruppen und Warteschlangenthemen werden für Ihre Umgebung angepasst. Standardmäßig wird die kopierte Anfrage in den Themengruppen und Warteschlangenthemen der ursprünglichen Anfrage gespeichert.

     >[!TIP]
     >
     >Wenn sich der Pfad vom Pfad der ursprünglichen Anfrage ändert, hat der Ersteller der Anfrage-Warteschlange die Warteschlange geändert.

1. (Optional) Aktualisieren Sie alle Informationen aus der kopierten Anfrage. Je nachdem, welche Felder der Ersteller der Anfrage-Warteschlange im Abschnitt **Neue Problemfelder** der Unterregisterkarte **Warteschlangendetails** im Projekt aktiviert hat, finden Sie möglicherweise eines der folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Betreff</strong> </td> 
      <td>Zeigt den Namen der ursprünglichen Anfrage an. Aktualisieren Sie sie, falls erforderlich. Andernfalls benennt Workfront die kopierte Anfrage <b>Kopie von &lt;Name der ursprünglichen Anfrage&gt;</b>. Dies ist ein Pflichtfeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Zeigt die Beschreibung der ursprünglichen Anfrage an. Aktualisieren Sie sie, falls erforderlich.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Zeigt die URL der ursprünglichen Anfrage an. Aktualisieren Sie sie, falls erforderlich.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorität</strong> </td> 
      <td> <p>Geben Sie die Priorität Ihrer Anfrage an. Die Priorität sollte definieren, wie schnell diese Anfrage Ihrer Meinung nach gelöst werden sollte. Die Standardoptionen sind:</p> 
       <ul> 
        <li>Keine</li> 
        <li>Niedrig</li> 
        <li>Normal</li> 
        <li>Hoch</li> 
        <li>Dringend</li> 
       </ul> <p>Ihr Workfront-Administrator kann die Namen von Prioritäten ändern.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schweregrad</strong> </td> 
      <td> <p>Geben Sie den Schweregrad für Ihre Anfrage an. Der Schweregrad sollte die Auswirkungen dieser Anfrage auf Ihre Arbeit definieren, falls sie nicht rechtzeitig behoben wird. Die Standardoptionen sind:</p> 
       <ul> 
        <li>Kosmetisch</li> 
        <li>Verwirrend</li> 
        <li>Programmfehler mit Umgehungslösung</li> 
        <li>Programmfehler ohne Umgehungslösung</li> 
        <li>Schwerer Fehler</li> 
       </ul> <p>Ihr Workfront-Administrator kann die Namen der Schweregrade ändern.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Primärer Kontakt</strong> </td> 
      <td>Der Primäre Ansprechpartner einer Anfrage ist standardmäßig bei Ihnen, da Sie die Ansprechperson für alle Fragen im Zusammenhang mit der Anfrage sind. Sie können dies jedoch für jeden anderen Workfront-Benutzer ändern.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Arbeitsaufträge</strong></span> </td> 
      <td> <p>Geben Sie den Namen eines aktiven Benutzers, Aufgabengebiets oder Teams an, dem die Anfrage zugewiesen werden soll. </p> <p> Sie können mehr als einen Benutzer, ein Aufgabengebiet oder ein Team angeben. </p> <p>Je nachdem, wie die Anfrage-Warteschlange eingerichtet wurde, können Sie die Anfrage möglicherweise nur einem oder zwei Ressourcentypen zuweisen statt allen drei. </p> <p>Es wird empfohlen, Routing-Regeln für die Anfrage-Warteschlangen zu verwenden, damit sie automatisch an die entsprechenden Ressourcen weitergeleitet werden können. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Je nachdem, wie die Anfrage-Warteschlange eingerichtet wurde, können Sie der Anfrage möglicherweise nur einen Ressourcentyp zuweisen (z. B. Benutzer). Wenn der Anfrage-Warteschlange auch eine Routing-Regel zugeordnet ist, die die Anfrage automatisch an einen anderen Ressourcentyp weiterleitet (z. B. ein Team), wird Ihre Anfrage sowohl der Entität, die Sie beim Senden der Anfrage manuell angeben (Benutzer), als auch der in der Routing-Regel angegebenen Ressource (dem Team) zugewiesen.</p> <p style="font-weight: normal;">Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Anfrage-Warteschlange erstellen</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Routing-Regeln erstellen</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplante Stunden</strong> </td> 
      <td> <p>Schätzen Sie, wie viele Stunden es dauern würde, bis diese Anfrage abgeschlossen ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplantes Startdatum</strong> </td> 
      <td> <p>Das Datum, an dem die Bearbeitung dieser Anfrage beginnen soll.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplantes Abschlussdatum</strong> </td> 
      <td>Das Datum, an dem diese Anfrage aufgelöst werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>Der Standardstatus einer neuen Anfrage lautet „Neu“. Ihr Workfront-Administrator hat möglicherweise den Namen dieses Status geändert. Sie können den Status in diesem Dropdown-Menü auch in etwas Anderes ändern.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dokumente</strong> </td> 
      <td> <p>Dokumente zu Ihrer Anfrage hinzufügen. Die dem ursprünglichen Antrag beigefügten Dokumente werden nicht auf den kopierten Antrag übertragen.</p> <p><b>TIPP</b>

   Je nachdem, wie die Anfrage-Warteschlange eingerichtet wurde, wird der Abschnitt Dokumente möglicherweise vor oder nach den benutzerdefinierten Feldern angezeigt.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Optional) Aktualisieren Sie bei Bedarf alle Informationen in den angehängten benutzerdefinierten Formularen.

   >[!TIP]
   >
   >* Alle benutzerdefinierten Formulare, die an die ursprüngliche Anfrage angehängt sind, sowie die in den benutzerdefinierten Feldern enthaltenen Werte werden auf die kopierte Anfrage übertragen. Dazu gehören Felder, die Logik enthalten.
   >* Benutzerdefinierte Formulare können nicht aus der kopierten Anfrage entfernt werden.

1. Klicken Sie **Senden**.

   Die kopierte Anfrage wird als neue Anfrage in der von Ihnen angegebenen Anfrage-Warteschlange gesendet.
