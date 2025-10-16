---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Gelöschte Elemente wiederherstellen
description: Wenn Sie Workfront-Administrator sind, können Sie Projekte, Aufgaben, Probleme, Dokumente und Vorlagen in Adobe Workfront wiederherstellen, wenn sie in den letzten 30 Tagen gelöscht wurden. Nach 30 Tagen werden diese Elemente dauerhaft gelöscht und können nicht wiederhergestellt werden.
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: 156341072c291b5c03432da399a509d9772b73ea
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 2%

---

# Gelöschte Elemente wiederherstellen

<!--Audited: 12/2023-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Wenn Sie Workfront-Administrator sind, können Sie Projekte, Aufgaben, Probleme, Dokumente und Vorlagen in Adobe Workfront wiederherstellen, wenn sie in den letzten 30 Tagen gelöscht wurden. Nach 30 Tagen werden diese Elemente dauerhaft gelöscht und können nicht wiederhergestellt werden.

Wenn Sie ein -Objekt wiederherstellen, werden auch alle seine untergeordneten Objekte und Felder wiederhergestellt. Wenn Sie beispielsweise ein Projekt wiederherstellen, werden auch alle Aufgaben, Probleme, Dokumente, Stunden, Notizen, Zuweisungen und benutzerdefinierten Daten im Projekt wiederhergestellt.

Ein Gruppenadministrator bzw. eine Gruppenadministratorin kann diese Objekte auch für eine von ihm verwaltete Gruppe wiederherstellen.

>[!IMPORTANT]
>
>* Wenn Sie einen Bericht, ein Dashboard, einen Benutzer, eine Gruppe, ein Team oder eine Iteration löschen, kann dieser nicht wiederhergestellt werden.
>* Wenn in einer Gruppe eine andere Person als der Gruppenadministrator ein Dokument direkt in den Bereich Dokumente eines Objekts hochlädt, kann nur ein Workfront-Administrator das Dokument wiederherstellen.
>
>* Wenn Sie eine Aufgabe oder ein Problem verschieben und nicht auch die an die Aufgabe oder das Problem angehängten Dokumente verschieben, werden die Dokumente gelöscht und für 30 Tage in den Papierkorb gelegt. Ein Administrator kann sie wiederherstellen und sie werden erneut mit der verschobenen Aufgabe oder dem verschobenen Problem verbunden. Wenn die Aufgabe oder das Problem seit dem Verschieben gelöscht wurde, werden die Dokumente im Bereich Dokumente auf der Benutzerseite des Administrators wiederhergestellt, der sie wiederherstellt.

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
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Informationen, die beim Wiederherstellen eines Projekts, einer Aufgabe oder eines Problems wiederhergestellt werden

Beim Wiederherstellen eines Projekts, einer Aufgabe oder eines Problems werden die folgenden zugehörigen Informationen wiederhergestellt:

* Kommentare und Antworten im Bereich „Aktualisierungen“
* Genehmigungen
* Arbeitsaufträge
* Benutzerdefinierte Formulare
* Warteschlangen-Setup
* Business Cases, einschließlich Scorecards, Ziele und Risiken
* Projektteams
* Daten
* Probleme
* Aufgaben
* Teilaufgaben
* Statuswerte
* Finanzielle Informationen:

   * Abrechnungseinträge
   * Abrechnungssätze
   * Ausgaben

* Zeitleisteninformationen:

   * Vorgänger
   * Aufgabenbeschränkungen
   * Dauertyp

* Baselines

  Aufgaben-Baselines werden wiederhergestellt, wenn Sie ihr übergeordnetes Projekt oder ihre übergeordnete Aufgabe wiederherstellen, jedoch nicht, wenn Sie einzeln gelöschte Aufgaben wiederherstellen.

* Stunden (und Stunden-IDs)

  Ob Stunden im gelöschten Element wiederhergestellt werden, hängt von den Einstellungen ab, die Sie beim Konfigurieren der Voreinstellungen für Arbeitszeittabellen und Stunden ausgewählt haben. Weitere Informationen finden Sie unter [Auswirkungen auf Stunden konfigurieren, in denen ein Objekt gelöscht und wiederhergestellt wird](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* Die URL des Elements

  Nach der Wiederherstellung bleibt die URL des Elements unverändert. Wenn Personen Browser-Lesezeichen für das Element erstellt haben, bleiben diese gültig.

* Zugriff und Berechtigungen

  Benutzende, die vor dem Löschen Zugriff auf das Element hatten, erhalten nach der Wiederherstellung Zugriff.

* Dokumente (einschließlich geprüfter Dokumente)

  Beachten Sie beim Wiederherstellen von Dokumenten und Dokumentversionen Folgendes:

   * Dokumente, die einzeln gelöscht wurden, können einzeln wiederhergestellt werden.

     Dokumente, die zusammen mit dem übergeordneten Projekt, der übergeordneten Aufgabe oder dem übergeordneten Problem gelöscht wurden, werden beim Wiederherstellen des übergeordneten Elements wiederhergestellt. Sie können sie jedoch nicht einzeln wiederherstellen.

   * Alle Versionen eines Dokuments oder eines Korrekturabzugs werden wiederhergestellt, wenn das Dokument wiederhergestellt wird.\
     Einzelne Versionen eines Dokuments oder eines Korrekturabzugs, die einzeln gelöscht wurden, können nicht wiederhergestellt werden.

## Informationen, die beim Wiederherstellen eines Projekts, einer Aufgabe oder eines Problems nicht wiederhergestellt werden

Wenn Sie ein Projekt, eine Aufgabe oder ein Problem wiederherstellen, werden die folgenden zugehörigen Informationen nicht zusammen mit diesen wiederhergestellt:

* Likes
* Empfehlungen
* E-Mail-Adresse in Anfrage-Warteschlange aufnehmen
* Favoriten

  Ein Projekt, eine Aufgabe oder ein Problem, das bzw. das Sie vor dem Löschen zum Favoritenmenü hinzugefügt haben, wird nach dem Wiederherstellen nicht wieder im Favoritenmenü angezeigt.

* Auflösen von Objekten

  Ein Lösungsobjekt ist ein konvertiertes Problem, das mit der Option **Ursprüngliches Problem beibehalten und seine Lösung hiermit verknüpfen** &lt;**(Projekt** oder **Aufgabe)**> konfiguriert wurde. Wenn Sie das übergeordnete Projekt oder die übergeordnete Aufgabe löschen, wird das Problem nicht mehr als Lösungsobjekt identifiziert, da keine Verbindung mehr zum Projekt oder zur Aufgabe besteht. Wenn Sie das übergeordnete Element wiederherstellen, wird die Verknüpfung nicht wiederhergestellt.

  Weitere Informationen dazu, wie Workfront-Admins oder Gruppenadmins Probleme so konfigurieren, dass sie beim Konvertieren dem Lösungsobjekt entsprechen, finden Sie unter [Konfigurieren von systemweiten Aufgaben- und &#x200B;](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) und [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  Weitere Informationen zum Konvertieren von Problemen finden Sie unter [Übersicht über das Konvertieren von Problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Elemente wiederherstellen

{{step-1-to-setup}}

1. Klicken Sie **Papierkorb** > **Zuletzt gelöscht**.
1. Klicken Sie auf **Registerkarte**, **Aufgaben**, **Probleme**, **Vorlagen** oder **Dokumente** je nach dem Typ des Elements, das Sie wiederherstellen möchten.

   Elemente werden standardmäßig nach der Spalte **Löschdatum** sortiert.

1. Wählen Sie bis zu 10 Elemente aus, die Sie wiederherstellen möchten.

   Wenn Sie eine untergeordnete Aufgabe löschen, wird diese in der Liste angezeigt.

   Wenn Sie eine übergeordnete Aufgabe löschen, wird in der Liste nur die übergeordnete Aufgabe angezeigt. Alle untergeordneten Aufgaben werden jedoch wiederhergestellt, wenn Sie eine übergeordnete Aufgabe wiederherstellen.

1. Klicken Sie **Wiederherstellen**, um die ausgewählten Elemente an ihrem ursprünglichen Speicherort wiederherzustellen.
1. (Optional) Um das wiederhergestellte Element schnell anzuzeigen, führen Sie die Schritte unter [Wiederhergestelltes Element anzeigen](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md) aus.

   Weitere Informationen dazu, was nach der Wiederherstellung eines Elements geschieht, finden Sie im Abschnitt [Was passiert nach der Wiederherstellung von Elementen](#what-happens-after-you-restore-items) in diesem Artikel.

## Was passiert nach der Wiederherstellung von Elementen? {#what-happens-after-you-restore-items}

* Wenn Sie Aufgaben und Teilaufgaben wiederherstellen, werden diese in der Reihenfolge angezeigt, in der sie vor dem Löschen waren.

  Wenn sich die Reihenfolge der anderen Aufgaben jedoch ändert, während die Aufgabe gelöscht wird, kann die Aufgabe am Ende der Liste der Aufgaben oder Teilaufgaben wiederhergestellt werden.

* Nach dem Wiederherstellen eines Elements:

   * Es wird eine Meldung angezeigt, die Sie darüber informiert, ob Sie erfolgreich waren.

     Sie erhalten auch eine E-Mail-Benachrichtigung. Wenn Sie mehrere Elemente wiederhergestellt haben, werden sie in der E-Mail aufgelistet.

   * Ein Kommentar wird im Bereich Aktualisierungen des Projekts, der Aufgabe oder des Problems und im Bereich des übergeordneten Objekts angezeigt.

     Dies geschieht nicht, wenn Sie ein Dokument oder eine Vorlage wiederherstellen.

## Wiederhergestellte Korrekturabzüge

Wenn jemand ein Dokument wiederherstellt, das einen Korrekturabzug enthält, wird auf der Seite mit den Proofing-Aktivitäten für den Korrekturabzug möglicherweise der Name des ersten Workfront-Administrators angezeigt, der für die Instanz Ihres Unternehmens aufgelistet ist (in der Reihenfolge der Profilkennung), anstatt der tatsächlichen Person, die den Korrekturabzug wiederhergestellt hat.
