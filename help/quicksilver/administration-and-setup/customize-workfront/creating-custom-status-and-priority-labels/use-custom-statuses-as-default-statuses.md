---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Verwenden benutzerdefinierter Status als Standardstatus
description: Wenn ein benutzerdefinierter Status als Standardstatus festgelegt wird, wird der neue Standardstatus im gesamten System auf verschiedene Weise verwendet. Die Art und Weise, wie sie verwendet wird, hängt davon ab, ob sie als Standardstatus auf Systemebene oder als Standardstatus auf Gruppenebene festgelegt ist.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 0%

---

# Verwenden benutzerdefinierter Status als Standardstatus

Wenn ein benutzerdefinierter Status als Standardstatus festgelegt wird, wird der neue Standardstatus im gesamten System auf verschiedene Weise verwendet. Die Art und Weise, wie sie verwendet wird, hängt davon ab, ob sie als Standardstatus auf Systemebene oder als Standardstatus auf Gruppenebene festgelegt ist.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Benutzerdefinierte Standardstatus auf Systemebene

Wenn Sie einen benutzerdefinierten Status als Standardsystemstatus festlegen, übernehmen alle im System erstellten neuen Gruppen diesen Status.

Gruppen, die bereits beim Festlegen des neuen Standardsystemstatus vorhanden waren, übernehmen diese nicht automatisch.

Angenommen, in Ihrer Adobe Workfront-Umgebung wurden bereits zwei Gruppen erstellt (Marketing und Vertrieb). Sie erstellen einen neuen benutzerdefinierten Status, der mit &quot;Aktuell&quot;übereinstimmt, und rufen den Status In Prozess auf. Jetzt erstellen Sie eine neue Gruppe namens Engineering. In diesem Szenario erbt die Engineering-Gruppe den neuen Standardstatus, die Marketing- und Vertriebsgruppen nicht.

## Benutzerdefinierte Standardstatus auf Gruppenebene

Ein benutzerdefinierter Status, den Sie als standardmäßigen Gruppenstatus festlegen, wird unter folgenden Umständen verwendet:

* **Wenn das Workfront-System automatisch einen Status auswählt, wird der standardmäßige Gruppenstatus verwendet:** Der benutzerdefinierte Status, den Sie als Standardgruppenstatus festlegen, wird verwendet, wenn das Workfront-System einem Objekt automatisch einen Status zuweist.

  Beispielsweise kann eine Aufgabe so konfiguriert werden, dass sie automatisch in den Status Abgeschlossen wechselt, wenn der Prozentsatz der Abschlüsse 100 % erreicht. Wenn Sie einen benutzerdefinierten Status erstellen, der dem Status Abgeschlossen entspricht, und diesen benutzerdefinierten Status als Standardstatus festlegen, ändert Workfront den Status der Aufgabe in den neuen Standardstatus.

  Benutzerdefinierte Status werden auf diese Weise nur mit Gruppenstatus verwendet, die mit einer Aufgabe oder einem Problem verknüpft sind. Benutzerdefinierte Status können auf diese Weise nicht für Status verwendet werden, die mit einem Projekt verknüpft sind.

* Der **Status eines Projekts wird von der mit dem Projekt verknüpften Gruppe bestimmt**: Wenn sich die mit einem bestimmten Projekt verknüpfte Gruppe ändert, ändert sich der Status des Projekts in Abhängigkeit von den für die Gruppe definierten Standardstatus. (Eine Gruppe kann beim Bearbeiten des Projekts über das Feld Gruppen mit einem Projekt verknüpft werden.)

  Wenn sich diese Gruppe ändert, ändert sich der Status des Projekts, wenn für die neue Gruppe ein anderer Standardstatus definiert ist, der dem aktuellen Status des Projekts entspricht.

  Beispielsweise kann ein Projekt mit der Marketing-Gruppe verknüpft werden und der Status des Projekts ist auf Planung eingestellt. Das Projekt wird so bearbeitet, dass es nun mit der Vertriebsgruppe verknüpft ist. Die Gruppe &quot;Verkauf&quot;verfügt über einen benutzerdefinierten standardmäßigen Gruppenstatus namens &quot;Thinking&quot;(dieser Status entspricht der der Planung). Da die Gruppe für das Projekt geändert wurde, ändert sich der Status des Projekts jetzt in Denken.

Wenn Sie Gruppenadministrator sind, lesen Sie [Festlegen eines Status als Standardstatus für eine Gruppe](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Problemstatus

Wenn der benutzerdefinierte Status ein Problemstatus ist, müssen alle vier Ausgabetypen dafür aktiviert sein (Fehlerbericht, Änderungsreihenfolge, Problem und Anfrage). Beispielsweise kann der Status Neu geöffnet im unten gezeigten Problemstatus nicht als Standardstatus verwendet werden, da der Problemtyp Reihenfolge ändern nicht ausgewählt ist:

![](assets/all-4-issue-types-enabled.png)

## Benutzerdefinierten Status als Standardstatus festlegen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Projekteinstellungen** > **Status**.
1. (Bedingt) Wenn Sie einen Standardstatus für eine Gruppe festlegen, geben Sie im Menü oben rechts den Namen der Gruppe ein und wählen Sie diese dann aus, wenn sie angezeigt wird.
1. Öffnen Sie je nach dem Statustyp, den Sie als Standardstatus festlegen möchten, die Registerkarte **Projekt**, **Aufgaben** oder **Probleme**.
1. Klicken Sie auf das Dropdown-Menü **Standardstatus festlegen** .
1. Wählen Sie im angezeigten Dropdown-Bereich neben dem Status, für den Sie den Standardstatus festlegen möchten, den gewünschten Standardstatus aus.
1. Klicken Sie auf **Speichern**.
1. Verknüpfen Sie das Projekt mit der Gruppe, in der sich der Status befindet.

   >[!NOTE]
   >
   >Wenn Sie den benutzerdefinierten Status für eine Gruppe festlegen und das Projekt später einer anderen Gruppe zuweisen, wird der Projektstatus neu geladen und kann sich ändern.

   1. Wechseln Sie zu dem Projekt, in dem Sie den benutzerdefinierten Status verwenden möchten.
   1. Klicken Sie auf das Menü Mehr ![](assets/more-icon.png) und dann auf **Bearbeiten**.
   1. Wählen Sie im Feld **Projekt bearbeiten** , das im Feld **Gruppe** unter **Projektverknüpfung** angezeigt wird, die Gruppe aus, in der sich der Status befindet.
   1. Klicken Sie auf **Änderungen speichern**.
