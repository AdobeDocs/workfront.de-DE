---
product-area: projects
navigation-topic: manage-tasks
title: Verschieben von Aufgaben
description: Sie können Aufgaben in verschiedene Projekte oder in verschiedene übergeordnete Aufgaben in Adobe Workfront verschieben.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '1479'
ht-degree: 2%

---

# Verschieben von Aufgaben

Sie können Aufgaben in Adobe Workfront zwischen den folgenden Objekten verschieben:

* Eine Ad-hoc-Aufgabe für ein Projekt.
* Eine Aufgabe von einem Projekt zu einem anderen Projekt.
* Eine Aufgabe aus einem Projekt unter einem anderen übergeordneten Element in einem anderen Projekt.
* Eine Aufgabe innerhalb desselben Projekts unter einem anderen übergeordneten Element.

Sie können eine Aufgabe auf Aufgabenebene verschieben oder eine Aufgabe aus einer Aufgabenliste verschieben.
Sie können eine einzelne Aufgabe verschieben oder mehrere Aufgaben gleichzeitig aus einer Liste von Aufgaben verschieben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Aktionen in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben verwalten</p> <p>Beitragen oder höhere Berechtigungen zum Projekt mit der Möglichkeit, Aufgaben hinzuzufügen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Verschieben von Aufgaben

Beachten Sie beim Verschieben einer Aufgabe Folgendes:

* Wenn Sie eine Aufgabe von einem Projekt in ein anderes verschieben, können die Aufgabendaten neu berechnet werden. Bei der Neuberechnung werden der Zeitplan, den das neue Projekt verwendet, und die Informationen zum Zeitplan des Projekts berücksichtigt.

* Sie haben die Möglichkeit, während des Verschiebevorgangs einige der Aufgabe zugeordnete Elemente in die verschobene Aufgabe zu verschieben. Die folgenden Objekte werden jedoch standardmäßig an die verschobene Aufgabe übertragen:

   * Probleme
   * Protokollierte Stunden
   * Benutzerkommentare
   * Benutzerdefinierte Formulare und benutzerdefinierte Feldinformationen
   * Teilaufgaben

Die folgenden Elemente werden standardmäßig nicht mit der Aufgabe verschoben:

* Meilensteine

## Verschieben von Aufgaben in eine Liste

1. Wechseln Sie zu dem Projekt, das die zu verschiebenden Aufgaben enthält.
1. Klicks **Aufgaben** im linken Bereich, um die Aufgabenliste anzuzeigen.
1. Klicken Sie auf **Planmodus** icon ![](assets/plan-mode-icon.png) und stellen sicher, dass **Automatische Speicherung** Umschalten aktiviert ist, wählen Sie dann die Aufgabe oder die Aufgaben aus, die Sie verschieben möchten.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Aufgaben können nicht verschoben werden, wenn die **Automatische Speicherung** Umschalter ist deaktiviert.

1. (Optional und bedingt) Wenn Sie die ausgewählten Aufgaben innerhalb desselben Projekts verschieben möchten, klicken Sie auf die ausgewählten Aufgaben, ziehen Sie sie und legen Sie sie dort ab, wo sie in das Projekt verschoben werden sollen.

   Nachdem Sie die Aufgaben an der richtigen Stelle im Projekt abgelegt haben, werden die Änderungen, die Sie an der Aufgabenhierarchie vorgenommen haben, sofort gespeichert. Alle mit der jeweiligen Aufgabe verknüpften Informationen werden mit den Aufgaben verschoben.

1. (Bedingt) Wählen Sie die zu verschiebenden Aufgaben aus und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Mehr** Menü ![](assets/qs-more-menu.png) Klicken Sie oben in der Aufgabenliste auf **Verschieben nach**.
   * Klicken Sie mit der rechten Maustaste auf die ausgewählten Aufgaben und klicken Sie dann auf **Verschieben nach**.
   * Klicken Sie bei der Auswahl einer Aufgabe auf die **Mehr** Menü ![](assets/more-icon-task-list.png) neben dem Aufgabennamen in der Liste und klicken Sie dann auf **Verschieben nach**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   Das Feld Aufgabe verschieben wird angezeigt

1. Fahren Sie mit dem Verschieben der Aufgabe fort, wie im Abschnitt beschrieben [Verschieben einer Aufgabe auf Aufgabenebene](#move-a-task-at-the-task-level) in diesem Artikel, beginnend mit Schritt 4.

   <!--
   is this still accurate?!
   -->

## Verschieben einer Aufgabe auf Aufgabenebene {#move-a-task-at-the-task-level}

Sie können Aufgaben nicht nur aus einer Aufgabenliste verschieben, sondern auch auf Aufgabenebene verschieben, nachdem Sie sie geöffnet haben.

1. Suchen Sie eine Aufgabe in Ihrem Workfront-System, indem Sie danach suchen.
1. Klicken Sie auf den Namen der Aufgabe, um sie zu öffnen.
1. Klicken Sie auf **Mehr** Dropdown-Menü ![](assets/qs-more-menu.png) neben dem Namen der Aufgabe klicken Sie auf **Verschieben nach**. Das Feld Aufgabe verschieben wird angezeigt.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Optional) Aktualisieren Sie die **Aufgabenname**. Die Aufgabe wechselt mit dem neuen Namen am neuen Speicherort. Workfront zeichnet den ursprünglichen Namen der Aufgabe nicht auf.

   >[!TIP]
   >
   >Das Feld &quot;Aufgabenname&quot;ist abgeblendet und kann nicht bearbeitet werden, wenn ausgewählt wird, um mehrere Aufgaben in einer Liste zu verschieben. Sie können den Mauszeiger über das Feld &quot;Aufgabenname&quot;bewegen und eine Liste aller ausgewählten Aufgaben wird angezeigt.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Geben Sie den Namen der **Zielprojekt** wo die Aufgabe verschoben werden soll **Zielprojekt auswählen** -Feld.

   Wenn Sie die Aufgabe innerhalb desselben Projekts verschieben möchten, geben Sie den Namen des aktuellen Projekts ein.

   >[!TIP]
   >
   >* Beim Namen des Projekts wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können auch mit der Eingabe der Referenznummer beginnen oder die Kennung des Projekts eingeben. Auf diese Weise können Sie zwischen Projekten mit identischen Namen unterscheiden.
   >* In der Liste werden nur 100 Projekte angezeigt.

1. (Bedingt) Klicken Sie auf **Zugriff anfordern** , um Zugriff auf das Projekt anzufordern, wenn Sie keinen Zugriff auf das ausgewählte Projekt haben.
1. (Bedingt) Verschieben Sie die Aufgabe weiterhin in das ausgewählte Zielprojekt, ohne Zugriff anzufordern, wenn Sie Zugriff haben, um Aufgaben zu einer der Aufgaben im Zielprojekt hinzuzufügen.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Ähnliche Meldungen werden angezeigt, wenn das ausgewählte Projekt noch nicht genehmigt, abgeschlossen oder deaktiviert ist, wenn der Workfront-Administrator verhindert, dass diesen Projekten Aufgaben hinzugefügt werden. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optional) Klicken Sie auf **Optionen** im linken Bereich

   Oder

   Scrollen Sie nach unten zum **Optionen** im Feld Aufgabe verschieben die Auswahl eines Elements aufheben, das in der unten stehenden Tabelle aufgeführt ist, um es aus den verschobenen Aufgaben zu entfernen. Alle Optionen sind standardmäßig ausgewählt.

   >[!IMPORTANT]
   >
   >Wenn Sie Elemente in der Optionsliste deaktivieren, gehen Daten verloren. Informationen aus der bestehenden Aufgabe werden entfernt und können nicht wiederhergestellt werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td>Deaktivieren Sie diese Option, um alle Informationen aus der Aufgabe zu entfernen, wenn sie an die neue Position verschoben wird. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einschränkung</td> 
      <td> <p>Die Aufgabenbegrenzung wird auf "Sofort wie möglich"oder "So spät wie möglich"festgelegt, basierend auf der Einstellung "Projektplanmodus".</p> <p> Wenn diese Option aktiviert ist, wird die aktuelle Beschränkung der Aufgabe mit der Aufgabe übertragen. </p> 
      <p><b>NOTIZ</b>

   Wenn beim Verschieben oder Kopieren einer Aufgabe mit datumsspezifischen Begrenzungen in ein anderes Projekt die Beschränkungsdaten der Aufgabe außerhalb der Daten des neuen Projekts liegen, wird entweder die Aufgabenbegrenzung so bald wie möglich oder so spät wie möglich geändert oder die geplanten Start- oder Abschlussdaten der Projekte werden angepasst.

   Im Folgenden finden Sie Beispiele für datumsspezifische Einschränkungen:
   <ul>
      <li> Starten am</li>
      <li> Muss beendet werden am</li>
      <li> Nicht früher anfangen als</li>
      <li> Nicht später anfangen als</li>
      </ul>

   Informationen zu Aufgabenbegrenzungen und dazu, wie Aufgabenbegrenzungen oder Projektdaten betroffen sein können, finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Übersicht über Aufgabenbegrenzungen</a> und suchen Sie nach einer bestimmten Einschränkung.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td> <p>Alle Zuweisungen werden aus der Aufgabe entfernt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsprozess</td> 
      <td>Alle Genehmigungsprozesse werden aus der Aufgabe entfernt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fortschritt</td> 
      <td>Der Aufgabenstatus ist "Neu". Andernfalls wird der Status der vorhandenen Aufgabe beibehalten. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td>Die Finanzinformationen der Aufgabe werden entfernt und die Workfront aktualisiert den Aufgabenkatalog auf "Keine Kosten"und die Aufgabe "Umsatz"auf "Nicht abrechenbar". </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle Vorgänger</td> 
      <td> <p>Wenn diese Option aktiviert ist, wird die Abhängigkeit zum projektübergreifenden Vorgänger, wenn Sie die Aufgabe in ein anderes Projekt verschieben. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Die mit der Aufgabe verknüpften Dokumente werden nicht an die verschobene Aufgabe übertragen. Dazu gehören Versionen, Testsendungen und verknüpfte Dokumente.</p> <p>Dokumentgenehmigungen sind nicht enthalten. Dokumentgenehmigungen können beim Verschieben einer Aufgabe nie verschoben werden.</p> 
      <b>NOTIZ</b>

   Wenn Sie sich dafür entscheiden, die Dokumente nicht mit der Aufgabe verschieben zu lassen, werden die Dokumente gelöscht und 30 Tage lang in den Papierkorb gelegt. Ein Administrator kann sie wiederherstellen und wird für die verschobene Aufgabe wiederhergestellt.

   Wenn die Aufgabe gelöscht wird, nachdem sie verschoben wurde, werden die wiederhergestellten Dokumente im Bereich &quot;Dokumente&quot;der Benutzerseite des Administrators platziert, der sie wiederherstellt.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td>Die Aufgabenerinnerungen werden nicht an die verschobene Aufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Die bei der Aufgabe protokollierten Ausgaben werden nicht auf die verschobene Aufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Berechtigungen</td> 
      <td> <p>Workfront entfernt die Namen aller Entitäten, die in der Liste "Freigeben"der Aufgabe angezeigt werden. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Optional) Klicken Sie auf **Übergeordnetes Element auswählen** im linken Bereich

   Oder

   Scrollen Sie zum **Übergeordnetes Element auswählen** und wählen Sie dann die Aufgabe im Zielprojekt aus, die Sie der verschobenen Aufgabe übergeordnet werden möchten.

   >[!TIP]
   >
   >Bei der Auswahl, mehrere Aufgaben in einer Liste zu verschieben, werden alle ausgewählten Aufgaben zu den untergeordneten Elementen des ausgewählten übergeordneten Elements.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste einen der übergeordneten Elemente des Projektplans aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie anhand des Namens nach einer übergeordneten Aufgabe.

   Die Aufgabe wird in der Liste angezeigt.

   ![Auswählen einer übergeordneten Aufgabe beim Verschieben einer Aufgabe mit Suchfunktion ](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Aufgabe auswählen, werden die Aufgaben als Hauptaufgaben und nicht als Unteraufgaben verschoben und am Ende der Aufgabenliste im Zielprojekt platziert.

1. Klicks **Aufgabe verschieben**

   Oder

   Klicks **Aufgaben verschieben** wenn Sie mehrere Aufgaben in einer Liste auswählen.

   Die verschobenen Aufgaben befinden sich jetzt im angegebenen Projekt und sind entweder Unteraufgaben einer übergeordneten Aufgabe oder die letzten Aufgaben im Projekt.
