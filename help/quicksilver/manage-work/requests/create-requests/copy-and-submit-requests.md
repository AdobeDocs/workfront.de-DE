---
title: Anforderungen kopieren und senden
description: Wenn Sie ähnliche Anfragen häufig senden, können Sie eine vorhandene gesendete Anfrage kopieren. In diesem Fall können Sie eine vorhandene Anforderung kopieren, minimale Änderungen daran vornehmen und sie als neue Anforderung erneut senden.
author: Lisa
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 067a5bd54f794574f5f2d1ad98ad29b6e02ab297
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 1%

---

# Anforderungen kopieren und senden

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>-->

Wenn Sie ähnliche Anfragen häufig senden, können Sie eine vorhandene gesendete Anfrage kopieren. In diesem Fall können Sie eine vorhandene Anforderung kopieren, minimale Änderungen daran vornehmen und sie als neue Anforderung erneut senden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf das Hinzufügen von Anforderungen zu einer Anforderungswarteschlange</p> <p>Anzeigen von oder höheren Berechtigungen für die vorhandene Anforderung</p> <p>Informationen zum Einrichten einer Anforderungswarteschlange finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Mitarbeiter oder höher</p>
   Oder
   <p>Aktuell: Anforderung oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p>  </td> 
  </tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Zugriff auf das Hinzufügen von Anforderungen zu einer Anforderungswarteschlange</p> <p>Anzeigen von oder höheren Berechtigungen für die vorhandene Anforderung</p> <p>Informationen zum Einrichten einer Anforderungswarteschlange finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen über eine Anfrage verfügen, die Sie oder ein anderer Mitarbeiter Ihres Unternehmens zuvor gesendet haben, um sie kopieren und erneut senden zu können. Wenn die Anfrage einer anderen Person gehört, müssen Sie zumindest Zugriff auf View it haben, um sie kopieren und als neu senden zu können.

## Überlegungen zum Kopieren und Senden von Anforderungen als neue

* Sie können nur gesendete Anforderungen kopieren und senden. Entworfene Anforderungen können nicht kopiert werden.
* Sie können Anforderungen kopieren und senden, die Sie ursprünglich gesendet haben, oder Anforderungen, die von anderen gesendet wurden, und Sie haben Zugriff auf zumindest Ansicht.
* Sie haben immer Zugriff auf das Kopieren und Senden einer Kopie Ihrer eigenen Anfragen, es sei denn, jemand hat Ihre Berechtigungen für sie entfernt.
* Der Zugriff auf das Kopieren und Senden von Anforderungen, die ursprünglich von anderen gesendet wurden, wird möglicherweise automatisch Personen im selben Unternehmen gewährt, wenn der Ersteller der Anforderungswarteschlange die **Personen desselben Unternehmens aktiviert, die dieselben Berechtigungen für alle Anforderungen erben** in den Bereichen &quot;Warteschlangendetails&quot;oder &quot;Projekt bearbeiten&quot;. Wenn Sie diese Einstellung deaktivieren, kann nur der ursprüngliche Anfragende eigene Anforderungen anzeigen.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md)

* Sie können die Kopie der ursprünglichen Anforderung aktualisieren, bevor Sie sie als neue Anforderung erneut senden.
* Wenn die folgenden Änderungen nach dem Senden der ursprünglichen Anforderung auftreten, können Sie sie nicht mehr kopieren und erneut senden:

   * Die Anforderungswarteschlange wurde gelöscht.
   * Das Warteschlangenthema wurde gelöscht.

     >[!TIP]
     >
     >Wenn das Warteschlangenthema das einzige in der Anforderungswarteschlange war, können Sie die Anforderung dennoch kopieren und senden, und sie wird unter der Anforderungswarteschlange selbst gespeichert.

   * Die Anforderungswarteschlange wird nicht mehr als Warteschlange für Hilfeanfragen veröffentlicht. Weitere Informationen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
   * Wenn die Anforderungswarteschlange kein Warteschlangenthema enthält und die ursprüngliche Anforderung vor Januar 2022 eingereicht wurde.

   * Der Status des mit der Anforderungswarteschlange verknüpften Projekts ist nicht mehr aktuell.

* Sie können eine Kopie einer konvertierten Anforderung kopieren und senden, wenn die Anforderung im Konvertierungsprozess beibehalten wurde. Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

  >[!TIP]
  >
  >Die kopierte Anforderung ist nicht mit einem aufgelösten Objekt verknüpft.

## Anforderungen kopieren und senden

{{step1-to-requests}}

1. (Bedingt) Wenn der Abschnitt &quot;Gesendet&quot;nicht standardmäßig angezeigt wird, klicken Sie im linken Bereich auf **Gesendet** .

   >[!TIP]
   >
   >   Ihr Workfront- oder Gruppenadministrator kann Ihre Layoutvorlage anpassen und Bereiche aus dem Hauptmenü oder aus dem linken Bereich in Ihrer Umgebung entfernen. In diesem Fall sind sie möglicherweise nicht für Sie verfügbar.

1. Suchen Sie die Anforderung, die Sie kopieren und als neu senden möchten, und führen Sie einen der folgenden Schritte aus:

   * Wählen Sie sie aus und klicken Sie dann oben links in der Liste &quot;Gesendete Anforderungen&quot;auf **Kopieren** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) .

   >[!TIP]
   >
   > Wenn Sie zuvor keine Anforderung ausgewählt haben, ist das Symbol Kopieren abgeblendet.

   * Klicken Sie auf das Menü **Mehr** rechts neben dem Anforderungsnamen, klicken Sie dann auf **Kopieren und als neu senden** .![](assets/more-icon.png)

     Oder

     Klicken Sie mit der rechten Maustaste auf die ausgewählte Anforderung und klicken Sie dann auf **Kopieren und als neu senden**.

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >Wenn Sie keinen Zugriff auf das Erstellen von Problemen haben, erhalten Sie eine Warnung, dass Ihr Administrator Sie daran gehindert hat, Anforderungen zu erstellen.

1. (Optional) Aktualisieren Sie bei Bedarf die folgenden Informationen:

   * **Anforderungstyp**: die Anforderungswarteschlange, in der die kopierte Anforderung gespeichert wird. Standardmäßig wird die kopierte Anforderung in der Anforderungswarteschlange der ursprünglichen Anforderung gespeichert.
   * **Themengruppen** und **Themen in der Warteschlange**, sofern ausgewählt. Die Namen oder Themengruppen und Themen der Warteschlange werden für Ihre Umgebung angepasst. Standardmäßig wird die kopierte Anforderung in den Themengruppen und den Warteschlangenthemen der ursprünglichen Anforderung gespeichert.

     >[!TIP]
     >
     >Wenn sich der Pfad vom Pfad der ursprünglichen Anforderung ändert, hat der Ersteller der Anforderungswarteschlange die Warteschlange geändert.

1. (Optional) Aktualisieren Sie alle Informationen aus der kopierten Anforderung. Je nachdem, welche Felder der Ersteller der Anforderungswarteschlange im Abschnitt **Neue Problemfelder** der Unterregisterkarte **Warteschlangendetails** des Projekts aktiviert hat, können Sie eines der folgenden Felder finden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Betreff</strong> </td> 
      <td>Zeigt den Namen der ursprünglichen Anforderung an. Aktualisieren Sie es bei Bedarf. Andernfalls benennt Workfront die kopierte Anforderung <b>Kopie von &lt;Name der ursprünglichen Anforderung&gt;</b>. Dies ist ein Pflichtfeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Zeigt die Beschreibung der ursprünglichen Anforderung an. Aktualisieren Sie es bei Bedarf.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>Zeigt die URL der ursprünglichen Anforderung an. Aktualisieren Sie es bei Bedarf.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priorität</strong> </td> 
      <td> <p>Geben Sie die Priorität Ihrer Anfrage an. Mit der Priorität sollte definiert werden, wie schnell diese Anfrage Ihrer Meinung nach gelöst werden sollte. Die Standardoptionen sind:</p> 
       <ul> 
        <li>Keine</li> 
        <li>Niedrig</li> 
        <li>Normal</li> 
        <li>Hoch</li> 
        <li>Dringend</li> 
       </ul> <p>Ihr Workfront-Administrator kann die Prioritätsnamen ändern.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Schweregrad</strong> </td> 
      <td> <p>Geben Sie den Schweregrad für Ihre Anfrage an. Der Schweregrad sollte die Auswirkungen dieser Anfrage auf Ihre Arbeit definieren, sollte sie nicht rechtzeitig gelöst werden. Die Standardoptionen sind:</p> 
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
      <td>Der Primäre Kontakt einer Anfrage ist standardmäßig auf Sie festgelegt, da Sie als Ansprechpartner für alle Fragen im Zusammenhang mit der Anfrage fungieren. Sie können dies jedoch in einen anderen Workfront-Benutzer ändern.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>Arbeitsaufträge</strong></span> </td> 
      <td> <p>Geben Sie den Namen eines aktiven Benutzers, einer aktiven Rolle oder eines Teams an, dem die Anforderung zugewiesen werden soll. </p> <p> Sie können mehr als einen Benutzer, eine Jobrolle oder ein Team angeben. </p> <p>Je nachdem, wie die Anforderungswarteschlange eingerichtet wurde, können Sie die Anforderung möglicherweise nur einem oder zwei Ressourcentypen zuweisen, nicht allen drei. </p> <p>Es wird empfohlen, Routing-Regeln für Ihre Anforderungswarteschlangen zu verwenden, damit sie automatisch an die entsprechenden Ressourcen weitergeleitet werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">Je nachdem, wie die Anforderungswarteschlange eingerichtet wurde, können Sie der Anforderung möglicherweise nur einen Ressourcentyp zuweisen (z. B. Benutzer). Wenn eine Routing-Regel auch mit der Anforderungswarteschlange verknüpft ist und die Anforderung automatisch an einen anderen Ressourcentyp weitergeleitet wird (z. B. ein Team), wird Ihre Anforderung sowohl der Entität zugewiesen, die Sie beim Senden der Anforderung manuell angeben (Benutzer), als auch der in der Routing-Regel angegebenen Ressource (Team).</p> <p style="font-weight: normal;">Weitere Informationen finden Sie in den folgenden Artikeln:</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Routing-Regeln erstellen</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplante Stunden</strong> </td> 
      <td> <p>Schätzen Sie, wie viele Stunden es dauern würde, bis diese Anfrage abgeschlossen ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplantes Startdatum</strong> </td> 
      <td> <p>Das Datum, an dem die Arbeit an dieser Anfrage beginnen soll.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Geplantes Abschlussdatum</strong> </td> 
      <td>Das Datum, an dem diese Anfrage behoben werden soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Status</strong> </td> 
      <td>Der Standardstatus einer neuen Anforderung lautet "Neu". Möglicherweise hat der Workfront-Administrator den Namen dieses Status geändert. Sie können den Status auch in etwas Anderes über dieses Dropdown-Menü ändern.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dokumente</strong> </td> 
      <td> <p>Fügen Sie Ihrer Anforderung Dokumente hinzu. Die der ursprünglichen Anfrage beigefügten Dokumente werden nicht an die kopierte Anforderung übertragen.</p> <p><b>TIPP</b>

   Je nachdem, wie die Anforderungswarteschlange eingerichtet wurde, wird der Abschnitt Dokumente möglicherweise vor oder nach den benutzerdefinierten Feldern angezeigt.</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. (Optional) Aktualisieren Sie bei Bedarf alle Informationen in den angehängten benutzerdefinierten Formularen.

   >[!TIP]
   >
   >* Alle benutzerdefinierten Formulare, die an die ursprüngliche Anforderung angehängt sind, und die Werte in den benutzerdefinierten Feldern werden an die kopierte Anforderung übertragen. Dazu gehören Felder, die Logik enthalten.
   >* Sie können keine benutzerdefinierten Formulare aus der kopierten Anforderung entfernen.

1. Klicken Sie auf **Senden**.

   Die kopierte Anforderung wird als neue Anforderung in der von Ihnen angegebenen Anforderungswarteschlange gesendet.
