---
product-area: projects
navigation-topic: manage-tasks
title: Aufgaben verschieben
description: In Adobe Workfront können Sie Aufgaben in verschiedene Projekte oder übergeordnete Aufgaben verschieben.
author: Alina
feature: Work Management
exl-id: 93295d70-a6cf-46ca-b621-228fa6c983f5
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '1487'
ht-degree: 2%

---

# Verschieben von Aufgaben

<!--Audited: 12/2024-->


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Sie können Aufgaben in Adobe Workfront zwischen den folgenden Objekten verschieben:

* Eine Ad-hoc-Aufgabe für ein Projekt.
* Eine Aufgabe von einem Projekt in ein anderes Projekt.
* Eine Aufgabe aus einem Projekt unter einem anderen übergeordneten Element in einem anderen Projekt.
* Eine Aufgabe innerhalb desselben Projekts unter einem anderen übergeordneten Element.

Sie können eine Aufgabe auf Aufgabenebene verschieben oder eine Aufgabe aus einer Liste von Aufgaben verschieben.
Aus einer Aufgabenliste können Sie eine einzelne Aufgabe oder mehrere Aufgaben gleichzeitig verschieben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Aktionen in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neuer Plan: Standard </p> 
 <p>oder</p>  
<p>Aktueller Plan: Arbeit oder höher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgaben</p> <p>Contribute oder höhere Berechtigungen für das Projekt mit der Möglichkeit, Aufgaben hinzuzufügen</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Verschieben von Aufgaben

Beachten Sie beim Verschieben einer Aufgabe Folgendes:

* Ihr System- oder Gruppenadministrator kann verhindern, dass Aufgaben, für die Stunden protokolliert wurden, verschoben werden, je nachdem, wie er die Einstellung Benutzern das Verschieben von Aufgaben erlauben konfiguriert hat, und welche Probleme mit protokollierten Stunden im Bereich Setup auftreten. Weitere Informationen finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Wenn Sie eine Aufgabe von einem Projekt in ein anderes verschieben, werden die Aufgabentermine möglicherweise neu berechnet. Bei der Neuberechnung werden der Zeitplan, den das neue Projekt verwendet, und die Zeitplaninformationen des Projekts aus berücksichtigt.

* Sie haben während des Verschiebungsvorgangs die Möglichkeit, einige mit der Aufgabe verknüpfte Elemente auszuwählen und in die verschobene Aufgabe zu verschieben. Standardmäßig werden die folgenden Objekte jedoch an die verschobene Aufgabe übertragen:

   * Probleme
   * Protokollierte Stunden
   * Benutzerkommentare
   * Benutzerdefinierte Formulare und Informationen zu benutzerdefinierten Feldern
   * Teilaufgaben

* Die folgenden Elemente werden standardmäßig nicht mit der Aufgabe verschoben:

   * Meilensteine

## Verschieben von Aufgaben in einer Liste

1. Wechseln Sie zu dem Projekt, das die Aufgabe(n) enthält, die Sie verschieben möchten.
1. Klicken Sie **linken** auf „Aufgaben“, um die Aufgabenliste anzuzeigen.
1. Klicken Sie auf das **Planmodus**-Symbol ![](assets/plan-mode-icon.png) und stellen Sie sicher, dass der Umschalter **Automatisches Speichern** aktiviert ist, und wählen Sie dann die Aufgabe(n) aus, die Sie verschieben möchten.

   ![](assets/autosave-icon-on-highlighted-350x202.png)

   >[!IMPORTANT]
   >
   >Aufgaben können nicht verschoben werden, wenn der Umschalter **Automatisches Speichern** deaktiviert ist.

1. (Optional und bedingt) Wenn Sie die ausgewählten Aufgaben innerhalb desselben Projekts verschieben möchten, klicken Sie auf die ausgewählten Aufgaben, ziehen Sie sie und legen Sie sie an der gewünschten Stelle im Projekt ab.

   Nachdem Sie die Aufgaben an der richtigen Stelle im Projekt abgelegt haben, werden die von Ihnen an der Aufgabenhierarchie vorgenommenen Änderungen sofort gespeichert. Alle mit jeder Aufgabe verknüpften Informationen werden mit den Aufgaben verschoben.

1. (Bedingt) Wählen Sie die Aufgabe(n) aus, die Sie verschieben möchten, und führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf **Mehr**-![](assets/qs-more-menu.png) oben in der Aufgabenliste und dann auf **Verschieben nach**.
   * Klicken Sie mit der rechten Maustaste auf die ausgewählten Aufgaben und dann auf **Verschieben nach**.
   * Klicken Sie bei der Auswahl einer Aufgabe auf das **Mehr**-Menü ![](assets/more-icon-task-list.png) neben dem Aufgabennamen in der Liste und dann auf **Verschieben nach**.

   ![](assets/move-task-in-list-nwe-350x119.png)

   Das **Aufgabe verschieben** wird angezeigt

1. Fahren Sie mit dem Verschieben der Aufgabe fort, wie im Abschnitt [Verschieben einer Aufgabe auf Aufgabenebene](#move-a-task-at-the-task-level) in diesem Artikel beschrieben, beginnend mit Schritt 4.

   <!--
   is this still accurate?!
   -->

## Verschieben einer Aufgabe auf Aufgabenebene {#move-a-task-at-the-task-level}

Sie können eine Aufgabe nicht nur aus einer Aufgabenliste verschieben, sondern auch auf Aufgabenebene verschieben, nachdem Sie sie geöffnet haben.

1. Suchen Sie nach einer Aufgabe in Ihrem Workfront-System.
1. Klicken Sie auf den Namen der Aufgabe, um sie zu öffnen.
1. Klicken Sie auf **Mehr** Dropdown-Menü ![](assets/qs-more-menu.png) neben dem Namen der Aufgabe und dann auf **Verschieben nach**. Das Feld Aufgabe verschieben wird angezeigt.

   ![](assets/move-task-at-task-level-nwe-350x222.png)

1. (Optional) Aktualisieren Sie den **Aufgabennamen**. Die Aufgabe wird mit dem neuen Namen an den neuen Speicherort verschoben. Workfront zeichnet den Originalnamen der Aufgabe nicht auf.

   >[!TIP]
   >
   >Das Feld Aufgabenname ist abgeblendet und kann nicht bearbeitet werden, wenn Sie auswählen, ob mehrere Aufgaben in einer Liste verschoben werden sollen. Sie können den Mauszeiger über das Feld Aufgabenname bewegen, und eine Liste aller ausgewählten Aufgaben wird angezeigt.
   >
   >
   >![](assets/move-task-multiple-tasks-box-with-list-of-task-names-nwe-350x142.png)

1. Geben Sie den Namen des **Zielprojekts** in das Feld **Zielprojekt auswählen** ein, in das die Aufgabe verschoben werden soll.

   Wenn Sie die Aufgabe innerhalb desselben Projekts verschieben möchten, geben Sie den Namen des aktuellen Projekts ein.

   >[!TIP]
   >
   >* Beim Namen des Projekts wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können auch mit der Eingabe der Referenznummer beginnen oder die ID des Projekts eingeben. Auf diese Weise können Sie zwischen Projekten mit identischen Namen unterscheiden.
   >* In der Liste werden nur 100 Projekte angezeigt.

1. (Bedingt) Klicken Sie auf **Zugriff anfordern** um Zugriff auf das Projekt anzufordern, wenn Sie keinen Zugriff auf das ausgewählte Projekt haben.
1. (Bedingt) Verschiebt die Aufgabe in das ausgewählte Zielprojekt, ohne Zugriff anzufordern, wenn Sie Zugriff zum Hinzufügen von Aufgaben zu einer der Aufgaben im Zielprojekt haben.

   ![](assets/move-task-request-access-from-project-nwe-350x120.png)

   >[!TIP]
   >
   >Ähnliche Meldungen werden angezeigt, wenn das ausgewählte Projekt ausstehend, genehmigt, abgeschlossen oder eingestellt ist und der Workfront-Administrator das Hinzufügen von Aufgaben zu diesen Projekten verhindert. Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optional) Klicken Sie **linken** auf „Optionen“

   Oder

   Scrollen Sie im Feld Aufgabe verschieben nach unten zum Abschnitt **Optionen** und heben Sie dann die Auswahl der in der folgenden Tabelle aufgeführten Elemente auf, um sie aus den verschobenen Aufgaben zu entfernen . Alle Optionen sind standardmäßig ausgewählt.

   >[!IMPORTANT]
   >
   >Wenn Sie Elemente in der Optionsliste deaktivieren, gehen Daten verloren. Informationen aus der vorhandenen Aufgabe werden entfernt und können nicht wiederhergestellt werden.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td>Deaktivieren Sie diese Option, um alle Informationen aus der Aufgabe zu entfernen, wenn Sie sie an die neue Position verschieben. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einschränkung</td> 
      <td> <p>Die Aufgabenbeschränkung wird auf So bald wie möglich oder So spät wie möglich basierend auf der Einstellung des Projektzeitplanmodus festgelegt.</p> <p> Wenn diese Option aktiviert ist, wird die aktuelle Einschränkung der Aufgabe mit der Aufgabe übertragen. </p> 
      <p><b>NOTIZ</b>

   Wenn ein Vorgang mit datumsspezifischen Einschränkungen in ein anderes Projekt verschoben oder kopiert wird und die Einschränkungstermine des Vorgangs außerhalb der Termine des neuen Projekts liegen, wird entweder die Aufgabenbeschränkung auf „So bald wie möglich“ oder „So spät wie möglich“ geändert oder die geplanten Start- oder Abschlussdaten der Projekte werden angepasst.

   Im Folgenden finden Sie Beispiele für datumsspezifische Einschränkungen:
   <ul>
      <li> Starten am</li>
      <li> Muss beendet werden am</li>
      <li> Nicht früher anfangen als</li>
      <li> Nicht später anfangen als</li>
      </ul>

   Informationen zu Aufgabenbeschränkungen und dazu, wie sich Vorgangseinschränkungen oder Projekttermine auswirken können, finden Sie unter <a href="../../../manage-work/tasks/task-constraints/task-constraint-overview.md" class="MCXref xref">Übersicht über </a> Aufgabenbeschränkung“. Suchen Sie nach einer bestimmten Einschränkung.</p> </td>
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
      <td>Der Aufgabenstatus ist Neu. Andernfalls wird der vorhandene Aufgabenstatus beibehalten. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td>Die Finanzinformationen für die Aufgabe werden entfernt und Workfront aktualisiert den Kostentyp der Aufgabe auf „Keine Kosten“ und den Umsatztyp der Aufgabe als „Nicht fakturierbar“. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Alle Vorgänger</td> 
      <td> <p>Wenn diese Option ausgewählt ist, wird die Abhängigkeit zu einem projektübergreifenden Vorgänger, wenn Sie die Aufgabe in ein anderes Projekt verschieben. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Die an die Aufgabe angehängten Dokumente werden nicht an die verschobene Aufgabe übertragen. Dazu gehören Versionen, Testsendungen und verknüpfte Dokumente.</p> <p>Dies umfasst keine Dokumentengenehmigungen. Dokumentgenehmigungen können beim Verschieben einer Aufgabe nicht verschoben werden.</p> 
      <b>HINWEIS</b>

   Wenn Sie sich dafür entscheiden, die Dokumente nicht mit der Aufgabe verschieben zu lassen, werden die Dokumente gelöscht und für 30 Tage in den Papierkorb gelegt. Ein Administrator kann sie wiederherstellen und sie werden bei der verschobenen Aufgabe wiederhergestellt.

   Wenn die Aufgabe nach dem Verschieben gelöscht wird, werden die wiederhergestellten Dokumente im Bereich Dokumente der Benutzerseite des Administrators platziert, der sie wiederherstellt.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td>Die Aufgabenerinnerungen werden nicht an die verschobene Aufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Die für die Aufgabe protokollierten Ausgaben werden nicht auf die verschobene Aufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Berechtigungen</td> 
      <td> <p>Workfront entfernt die Namen aller Entitäten, die in der Freigabeliste der Aufgabe angezeigt werden. </p> </td> 
     </tr> 
    </tbody> 
   </table>



1. (Optional) Klicken Sie **linken Bedienfeld auf**&#x200B;Übergeordnetes Element auswählen“

   Oder

   Scrollen Sie zum Abschnitt **Übergeordnetes Element auswählen** und wählen Sie dann im Zielprojekt die Aufgabe aus, die Sie zum übergeordneten Element der verschobenen Aufgabe werden möchten.

   >[!TIP]
   >
   >Wenn Sie auswählen, dass mehrere Aufgaben in einer Liste verschoben werden sollen, werden alle ausgewählten Aufgaben zu untergeordneten Aufgaben des ausgewählten übergeordneten Elements.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste eines der übergeordneten Elemente im Projektplan aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie nach einer übergeordneten Aufgabe anhand des Namens.

   Die Aufgabe wird in der Liste angezeigt.

   ![Übergeordnete Aufgabe beim Verschieben einer Aufgabe mit Suchfunktion auswählen](assets/select-parent-when-moving-tasks-with-search-functionality-nwe-350x110.png)

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Aufgabe auswählen, werden die Aufgaben nicht als Teilaufgaben, sondern als Hauptaufgaben verschoben und am Ende der Aufgabenliste im Zielprojekt platziert.

1. Klicken Sie **Aufgabe verschieben**

   Oder

   Klicken Sie **Aufgaben verschieben** wenn Sie mehrere Aufgaben in einer Liste auswählen.

   Die verschobenen Aufgaben befinden sich nun im angegebenen Projekt und sind entweder Teilaufgaben einer übergeordneten Aufgabe oder die letzten Aufgaben im Projekt.
