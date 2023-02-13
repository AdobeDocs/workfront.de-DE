---
title: Erstellen oder Bearbeiten eines Status
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: Als Adobe Workfront-Administrator können Sie benutzerdefinierte Status für Projekte, Aufgaben und Probleme erstellen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: f3785c66b979cc95bf1d2d2ccacbdeefe0ef0967
workflow-type: tm+mt
source-wordcount: '974'
ht-degree: 2%

---

# Erstellen oder Bearbeiten eines Status

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

Als Adobe Workfront-Administrator können Sie benutzerdefinierte Status für Projekte, Aufgaben und Probleme erstellen. Diese können für Benutzer im gesamten Workfront-System oder für bestimmte Gruppen oder Untergruppen verwendet werden. Weitere Informationen zu Status finden Sie unter [Statusübersicht](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Gruppenadministratoren können auch eigene Gruppenstatus erstellen, die nur von ihren Gruppen verwendet werden können. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzerdefinierten Status erstellen oder bearbeiten

Sie können einen benutzerdefinierten Status hinzufügen, der von Ihrer gesamten Organisation oder von einer einzelnen Gruppe verwendet werden kann.

Wenn Sie einen benutzerdefinierten Status für die gesamte Organisation erstellen, können Sie ihn so konfigurieren, dass alle Gruppen im System ihn verwenden können, ohne ihn zu bearbeiten. Sie können sie auch so konfigurieren, dass Gruppenadministratoren sie für ihre Gruppen ändern können, wie hier beschrieben: [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Projektvoreinstellungen** > **Status**.

1. (Bedingt) Wenn Sie einen Status für die Verwendung im gesamten System erstellen oder bearbeiten, stellen Sie sicher, dass **Systemstatus** wird in dem Feld oben rechts aktiviert.

   ![](assets/system-statuses-in-upper-rt-corner.jpg)

   Oder

   Wenn der Status für eine Gruppe oder Untergruppe bestimmt ist, geben Sie oben rechts den Gruppennamen ein und wählen Sie ihn aus, wenn er angezeigt wird.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Wählen Sie die Registerkarte des Objekttyps (**Projekt**, **Aufgaben** oder **Probleme**), die Sie mit dem Status verknüpfen möchten.

1. Wenn Sie einen neuen Status erstellen, klicken Sie auf **Neuen Status hinzufügen**.

   Oder

   Wenn Sie einen vorhandenen Status bearbeiten, halten Sie den Mauszeiger darüber und klicken Sie auf die Schaltfläche **Bearbeiten** -Symbol, das ganz rechts angezeigt wird.

   ![](assets/custom-status-edit.png)

1. Konfigurieren Sie den Status mit den folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Statusname</td> 
      <td> <p>Geben Sie einen Namen für den Status ein. Dies ist ein Pflichtfeld.</p> <p>Beachten Sie beim Erstellen eines Statusnamens, dass andere Benutzer im System einen Status mit demselben Namen erstellen können. Es wird empfohlen, einen eindeutigen Namen zu verwenden, um Verwirrung bei der Auswahl von Status in Workfront zu vermeiden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>(Optional) Geben Sie eine Beschreibung des Status ein. Dieser kommuniziert seinen Zweck mit denen, die ihn verwenden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Farbe</td> 
      <td> <p>Passen Sie die Farbe des Status an, indem Sie auf das Farbfeld klicken und eine Farbe aus dem Farbfeldbedienfeld auswählen. Sie können auch eine Hexadezimalzahl in das Feld eingeben.</p> <p>Die Statusfarbe wird oben rechts in Workfront angezeigt, wenn ein Benutzer das Objekt anzeigt.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entspricht</td> 
      <td> <p>Wählen Sie eine der Optionen aus der Liste aus, die die Funktion des Status am besten beschreibt. Wenn der Statusname beispielsweise Fertig lautet, sollte die Option, mit der er übereinstimmt, "Fertig"lauten.</p> <p>Jeder Status muss mit einer dieser Optionen übereinstimmen, da dies bestimmt, wie der Status funktioniert.</p> <p>Diese Option kann nach der Erstellung des Status nicht mehr geändert werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schlüssel</td> 
      <td> <p>Wenn Sie einen neuen Status erstellen, geben Sie einen Code oder eine Abkürzung für den Status ein oder verwenden Sie den für Sie generierten Status. Dieser Schlüssel muss in Workfront eindeutig sein, da er zu Berichtszwecken verwendet werden kann. Wenn Sie versuchen, einen Schlüssel anzugeben, der bereits im System verwendet wird, wird das Feld rot.</p> <p>Es kann nützlich sein, eine Abkürzung zu verwenden, die für diejenigen erkennbar ist, die sie verwenden werden.</p> <p>Diese Option kann nach der Erstellung des Status nicht mehr geändert werden.</p> <p>Sie können den Schlüsselcode für die Status Planung, Aktuell und Abgeschlossen nicht ändern. Dies ist wichtig, wenn Sie einen Bericht im Textmodus erstellen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status ausblenden</td> 
      <td> <p>(Nur Projekt- und Aufgabenstatus)</p> <p>Aktivieren Sie diese Option, wenn der Status für Benutzer ausgeblendet werden soll. Wenn sie deaktiviert ist (Standardeinstellung), können alle Benutzer im System den Status verwenden.</p> <p>Sie können den Status eines Problems ausblenden, indem Sie alle vier Ausgabetypen deaktivieren (Fehlerbericht, Reihenfolge ändern, Problem, Anforderung).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Für alle Gruppen sperren</td> 
      <td>
       <p>Wenn ein Status gesperrt ist, können Benutzer ihn im gesamten System sehen und verwenden und Gruppenadministratoren können ihn nicht für ihre Gruppen anpassen.</p> 
       <p>Wenn ein Status entsperrt ist, können Gruppenadministratoren ihn für ihre einzelnen Gruppen anpassen.</p>

   <div>
       <p>Sie können sowohl gesperrte als auch entsperrte Status in einem Systemgenehmigungsprozess verwenden. Wenn Sie einen Systemgenehmigungsprozess mit einem entsperrten Systemstatus erstellen, können Benutzer im gesamten System den Genehmigungsprozess an jedes Projekt, jede Aufgabe oder jedes Problem im System anhängen.</p>
       <p> In den folgenden Szenarien werden Warnmeldungen angezeigt, die Ihnen und Ihren Benutzern helfen, die Ergebnisse der Statusentsperrung zu verstehen:</p>
       <ul>
       <li>Ein Administrator entsperrt einen Systemstatus, der in einem Genehmigungsprozess verwendet wird. In einer Meldung wird gewarnt, dass der entsperrte Status für ihre Gruppen möglicherweise gelöscht wird, was verhindert, dass Gruppenmitglieder diesen Genehmigungsprozess ordnungsgemäß für Objekte verwenden, die ihrer Gruppe zugewiesen sind.</li>
       <li>Ein Benutzer beginnt mit der Bearbeitung eines Genehmigungsprozesses, der einen entsperrten Status verwendet. Eine Meldung informiert den Benutzer über den entsperrten Status, damit er beurteilen kann, ob es sinnvoll wäre, ihn erneut zu sperren oder zu ersetzen.</li>
       <li>Ein Genehmigungsprozess auf Systemebene mit einem entsperrten Status wird an ein Objekt angehängt und der Status wurde für die dem Objekt zugewiesene Gruppe gelöscht. Wenn ein Gruppenmitglied zum Bereich Validierungen für das Objekt wechselt, wird in einer Meldung erläutert, dass der Validierungsprozess für das Objekt nicht initiiert werden kann.</li>
       </ul>
       <p>Weitere Informationen zum Sperren von Status finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Status auf Systemebene gesperrt und entsperrt</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Anweisungen dazu, wie Sie diesen Status zu einem Standardstatus machen, finden Sie unter [Verwenden benutzerdefinierter Status als Standardstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Weitere Informationen zum Neuanordnen des Gruppenstatus finden Sie unter [Neuanordnen der Status auf Systemebene und Gruppe](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
