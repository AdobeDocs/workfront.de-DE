---
title: Status erstellen oder bearbeiten
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: Als Adobe Workfront-Administrator können Sie benutzerdefinierte Status für Projekte, Aufgaben und Probleme erstellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 2%

---

# Status erstellen oder bearbeiten

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

Als Adobe Workfront-Administrator können Sie benutzerdefinierte Status für Projekte, Aufgaben und Probleme erstellen. Diese können für Benutzende im gesamten Workfront-System oder für bestimmte Gruppen oder Untergruppen sein. Weitere Informationen zu Status finden Sie unter [Status - Übersicht](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Gruppenadministratoren können auch eigene Gruppenstatus erstellen, die nur von ihren Gruppen verwendet werden können. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
     <p>Neu: Standard</p>
     <p>oder</p>
     <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen oder Bearbeiten eines benutzerdefinierten Status

Sie können einen benutzerdefinierten Status hinzufügen, der von Ihrer gesamten Organisation oder einer einzelnen Gruppe verwendet werden kann.

Wenn Sie einen benutzerdefinierten Status für die gesamte Organisation erstellen, können Sie ihn so konfigurieren, dass alle Gruppen im System ihn verwenden können, ohne ihn zu bearbeiten. Oder Sie können ihn so konfigurieren, dass Gruppenadministratoren ihn für ihre Gruppen ändern können, wie in [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md) beschrieben.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Projektvoreinstellungen** > **Status**.

1. (Bedingt) Wenn Sie einen Status zur systemweiten Verwendung erstellen oder bearbeiten, stellen Sie sicher, dass **Systemstatus** im Feld oben rechts ausgewählt ist.

   ![Systemstatus](assets/system-statuses-in-upper-rt-corner-new.jpg)

   Oder

   Wenn der Status für eine Gruppe oder Untergruppe lautet, beginnen Sie, den Namen der Gruppe in der oberen rechten Ecke einzugeben, und wählen Sie sie aus, wenn sie angezeigt wird.

   ![Systemstatus für Gruppe](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Wählen Sie die Registerkarte des Objekttyps (**Projekt**, **Aufgaben** oder **Probleme**) aus, den Sie mit dem Status verknüpfen möchten.

1. Wenn Sie einen neuen Status erstellen, klicken Sie auf &quot;**Status hinzufügen**.

   Oder

   Wenn Sie einen vorhandenen Status bearbeiten, halten Sie den Mauszeiger darüber und klicken Sie dann auf das **Bearbeiten**-Symbol, das ganz rechts angezeigt wird.

   ![Benutzerdefinierten Status bearbeiten](assets/custom-status-edit.png)

1. Konfigurieren Sie den Status mithilfe der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Statusname</td> 
      <td> <p>Geben Sie einen Namen für den Status ein. Dies ist ein Pflichtfeld.</p> <p>Beachten Sie beim Erstellen eines Statusnamens, dass andere Benutzer im System einen Status mit demselben Namen erstellen können. Es wird empfohlen, einen eindeutigen Namen zu verwenden, um Verwirrungen bei der Auswahl von Status in Workfront zu vermeiden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>(Optional) Geben Sie eine Beschreibung des Status ein. Dies kommuniziert seinen Zweck an diejenigen, die es verwenden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Farbe</td> 
      <td> <p>Passen Sie die Farbe des Status an, indem Sie auf das Farbfeld klicken und eine Farbe aus dem Farbfeld auswählen. Sie können auch eine Hexadezimalzahl in das Feld eingeben.</p> <p>Die Statusfarbe wird in der rechten oberen Ecke von Workfront angezeigt, wenn ein(e) Benutzende(r) das Objekt aufruft.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entspricht</td> 
      <td> <p>Wählen Sie eine der Optionen aus der Liste aus, die die Funktion des Status am besten beschreibt. Wenn der Statusname beispielsweise „Fertig“ lautet, sollte die entsprechende Option „Fertig“ sein.</p> <p>Jeder Status muss mit einer dieser Optionen übereinstimmen, da dies bestimmt, wie der Status funktioniert.</p> <p>Diese Option kann nach der Erstellung des Status nicht mehr geändert werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schlüssel</td> 
      <td> <p>Wenn Sie einen neuen Status erstellen, geben Sie einen Code oder eine Abkürzung für den Status ein oder verwenden Sie die für Sie generierte Abkürzung. Dieser Schlüssel muss in Workfront eindeutig sein, da er zu Berichtszwecken verwendet werden kann. Wenn Sie versuchen, einen Schlüssel anzugeben, der bereits im System verwendet wird, wird das Feld rot.</p> <p>Es kann nützlich sein, eine Abkürzung zu verwenden, die für diejenigen erkennbar ist, die sie verwenden werden.</p> <p>Diese Option kann nach der Erstellung des Status nicht mehr geändert werden.</p> <p>Sie können den Schlüssel-Code für die Status „Planung“, „Aktuell“ und „Abgeschlossen“ nicht ändern. Dies ist wichtig, wenn Sie einen Bericht im Textmodus erstellen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Status ausblenden</td> 
      <td> <p>(Nur Projekt- und Aufgabenstatus)</p> <p>Aktivieren Sie diese Option, wenn der Status vor Benutzern ausgeblendet werden soll. Wenn diese Option deaktiviert ist (Standardeinstellung), können alle Benutzenden im System den Status verwenden.</p> <p>Sie können den Problemstatus ausblenden, indem Sie diese Option für alle vier Problemtypen (Fehlerbericht, Änderungsauftrag, Problem, Anfrage) deaktivieren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Für alle Gruppen sperren</td> 
      <td>
       <p>Wenn ein Status gesperrt ist, können Benutzende im gesamten System ihn sehen und verwenden, und Gruppenadministratoren können ihn nicht für ihre Gruppen anpassen.</p> 
       <p>Wenn ein Status entsperrt wird, können Gruppenadministratoren ihn für ihre individuellen Gruppen anpassen.</p>

   <div>
       <p>Sie können in einem Systemgenehmigungsprozess sowohl den Status „Gesperrt“ als auch den Status „Entsperrt“ verwenden. Wenn Sie einen Systemgenehmigungsprozess mit einem entsperrten Systemstatus erstellen, können Benutzer im gesamten System den Genehmigungsprozess an jedes Projekt, jede Aufgabe oder jedes Problem im System anhängen.</p>
       <p> In den folgenden Szenarien werden Warnmeldungen angezeigt, die Ihnen und Ihren Benutzern helfen, die Ergebnisse der Entsperrung eines Status zu verstehen:</p>
       <ul>
       <li>Ein Administrator entsperrt einen Status auf Systemebene, der in einem Genehmigungsprozess verwendet wird. Eine Meldung warnt davor, dass der entsperrte Status für die Gruppen gelöscht werden könnte, was verhindern würde, dass Gruppenmitglieder diesen Genehmigungsprozess ordnungsgemäß für Objekte verwenden, die ihrer Gruppe zugewiesen sind.</li>
       <li>Ein Benutzer beginnt mit der Bearbeitung eines Genehmigungsprozesses, der einen entsperrten Status verwendet. Eine Meldung informiert den Benutzer über den entsperrten Status, damit er beurteilen kann, ob es sinnvoll wäre, ihn erneut zu sperren oder zu ersetzen.</li>
       <li>Ein Genehmigungsprozess auf Systemebene mit einem entsperrten Status wird an ein Objekt angehängt und der Status wurde für die dem Objekt zugewiesene Gruppe gelöscht. Wenn ein Gruppenmitglied zum Abschnitt Genehmigungen für das Objekt wechselt, wird in einer Meldung erklärt, dass der Genehmigungsprozess für das Objekt nicht gestartet werden kann.</li>
       </ul>
       <p>Weitere Informationen zum Sperrstatus finden Sie unter <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Gesperrte und entsperrte Status auf Systemebene</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

   Anweisungen, wie Sie diesen Status als Standardstatus festlegen, finden Sie unter [Verwenden benutzerdefinierter Status als Standardstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Weitere Informationen zur Neuanordnung von Gruppenstatus finden Sie unter [Neuanordnung von Systemstatus und Gruppenstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
