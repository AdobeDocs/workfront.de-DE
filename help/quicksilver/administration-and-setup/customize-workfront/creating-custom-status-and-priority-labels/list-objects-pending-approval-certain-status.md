---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Listen Sie Objekte mit ausstehenden Genehmigungsprozessen mit einem bestimmten Status auf
description: Wenn Sie versuchen, einen Status zu löschen, wird in einer Fehlermeldung möglicherweise darauf hingewiesen, dass er nicht gelöscht werden kann, da er in ausstehenden Genehmigungsprozessen für Objekte in Ihrem System verwendet wird. Wenn Sie diese Objekte suchen und überprüfen möchten, um zu entscheiden, was Sie tun müssen, können Sie einen Bericht ausführen, in dem sie aufgelistet werden.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Listen Sie Objekte mit ausstehendem Genehmigungsprozess mit einem bestimmten Status auf

Wenn Sie versuchen, einen Status zu löschen, wird in einer Fehlermeldung möglicherweise darauf hingewiesen, dass er nicht gelöscht werden kann, da er sich in mindestens einem ausstehenden Genehmigungsprozess in Ihrem System befindet. Sie können einen Bericht ausführen, um die Objekte aufzulisten, bei denen sich der Bericht in einem ausstehenden Genehmigungsprozess befindet, und dann entscheiden, was Sie für jedes Objekt tun müssen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
     <p>Standard</p>
     <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p><p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td>
  </tr>
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Sie erhalten Verwaltungsberechtigungen für die von Ihnen erstellten Berichte.</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Im Standardmodus

{{step1-to-reports}}

1. Klicken Sie **Neuer Bericht** und wählen Sie **Projektbericht**, **Aufgabenbericht** oder **Problembericht**.
1. Öffnen Sie die **Filter**.
1. Klicken Sie **Filterregel hinzufügen** und gehen Sie dann wie folgt vor, um die Regel einzurichten:
   1. Beginnen Sie mit der Eingabe von `status` und wählen Sie **Status** aus, wenn es angezeigt wird.
   1. Belassen **Gleich** im zweiten Feld.
   1. Wählen Sie den Namen des Status im dritten Feld aus.
1. Klicken **erneut auf „Filterregel hinzufügen** und gehen Sie dann wie folgt vor, um die Regel einzurichten
   1. Beginnen Sie mit der Eingabe von `pending status` und wählen Sie dann dieses Element aus, wenn es unter dem Objekttyp angezeigt wird, in dem Sie suchen **Projekt**, **Aufgabe** oder **Problem**.
   1. Belassen **Gleich** im zweiten Feld.
   1. Geben Sie `in` in das dritte Feld ein.
1. Klicken **erneut auf „Filterregel hinzufügen** und gehen Sie dann wie folgt vor, um die Regel einzurichten
   1. Beginnen Sie mit der Eingabe des Genehmigungsprozesses und wählen Sie **Gruppen-ID** aus, wenn er unter &quot;**&quot;**.
   1. Wählen Sie **zweite Feld** Ist leer“ aus.
1. Klicken Sie auf **Speichern + Schließen**, um den Bericht auszuführen und alle Objekte des Typs, den Sie für Genehmigungsprozesse im Status „Ausstehend“ angegeben haben, basierend auf dem von Ihnen angegebenen Status (**Projekt**, **Aufgabe** oder **Problem**) aufzulisten.
1. Wiederholen Sie diese Schritte, um dieselben Informationen für die beiden anderen Objekttypen zu finden.


## Im Textmodus

{{step1-to-reports}}

1. Klicken Sie **Neuer Bericht** und wählen Sie **Projektbericht**, **Aufgabenbericht** oder **Problembericht**.
1. Öffnen Sie die **Filter**.
1. Wählen Sie **In Textmodus wechseln** aus.
1. Kopieren Sie Folgendes und fügen Sie es in das Bearbeitungsfenster ein. Ersetzen Sie dabei XXX durch die aus drei Buchstaben bestehende Taste für den Status :

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Sie können den Schlüssel in der Liste der Status anzeigen, wie in den folgenden Artikeln gezeigt:
   * [Zugriff auf die Liste der Systemprojektstatus](project-statuses.md)
   * [Zugriff auf die Liste der Status von Systemaufgaben](task-statuses.md)
   * [Zugriff auf die Liste der Systemanfragestatus](issue-statuses.md)

1. Klicken Sie auf **Speichern + Schließen**, um den Bericht auszuführen und alle Objekte des Typs, den Sie für Genehmigungsprozesse im Status „Ausstehend“ angegeben haben, basierend auf dem von Ihnen angegebenen Status (**Projekt**, **Aufgabe** oder **Problem**) aufzulisten.
1. Wiederholen Sie diese Schritte, um dieselben Informationen für die beiden anderen Objekttypen zu finden.
