---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Gelöschte Elemente wiederherstellen
description: Wenn Sie Workfront-Administrator sind, können Sie Projekte, Aufgaben, Probleme, Dokumente und Vorlagen in Adobe Workfront wiederherstellen, wenn sie in den letzten 30 Tagen gelöscht wurden. Nach 30 Tagen werden diese Elemente dauerhaft gelöscht und können nicht wiederhergestellt werden. Beim Wiederherstellen eines Objekts werden auch alle untergeordneten Objekte und Felder wiederhergestellt. Wenn Sie beispielsweise ein Projekt wiederherstellen, werden alle Aufgaben, Probleme, Dokumente, Stunden, Anmerkungen, Zuweisungen und benutzerdefinierten Daten im Projekt ebenfalls wiederhergestellt.items
feature: System Setup and Administration
author: Lisa
role: Admin
exl-id: e5b63652-ce16-44a9-a806-a41f19970ee1
source-git-commit: dfd8dd07e1a88da872550163051e703f6aea5f74
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 1%

---

# Gelöschte Elemente wiederherstellen

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Wenn Sie Workfront-Administrator sind, können Sie Projekte, Aufgaben, Probleme, Dokumente und Vorlagen in Adobe Workfront wiederherstellen, wenn sie in den letzten 30 Tagen gelöscht wurden. Nach 30 Tagen werden diese Elemente dauerhaft gelöscht und können nicht wiederhergestellt werden.

Beim Wiederherstellen eines Objekts werden auch alle untergeordneten Objekte und Felder wiederhergestellt. Wenn Sie beispielsweise ein Projekt wiederherstellen, werden alle Aufgaben, Probleme, Dokumente, Stunden, Anmerkungen, Zuweisungen und benutzerdefinierten Daten im Projekt ebenfalls wiederhergestellt.

Ein Gruppenadministrator kann diese Objekte auch für eine von ihm verwaltete Gruppe wiederherstellen.

>[!IMPORTANT]
>
>* Wenn Sie einen Bericht, ein Dashboard, einen Benutzer, eine Gruppe, ein Team oder eine Iteration löschen, kann dieser nicht wiederhergestellt werden.
>* Wenn in einer Gruppe ein anderer Benutzer als der Gruppenadministrator ein Dokument direkt in den Dokumentbereich eines Objekts hochlädt, kann nur ein Workfront-Administrator das Dokument wiederherstellen.
>
>* Wenn Sie eine Aufgabe oder ein Problem verschieben und die an die Aufgabe oder das Problem angehängten Dokumente nicht verschieben, werden die Dokumente gelöscht und 30 Tage lang im Papierkorb abgelegt. Ein Administrator kann sie wiederherstellen und wird erneut an die verschobene Aufgabe oder das Problem angehängt. Wenn die Aufgabe oder das Problem seit dem Verschieben gelöscht wurde, werden die Dokumente im Bereich &quot;Dokumente&quot;der Benutzerseite des Administrators wiederhergestellt, der sie wiederherstellt.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
   oder
   <p>Aktuell: Plan</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben.

## Informationen, die beim Wiederherstellen eines Projekts, einer Aufgabe oder eines Problems abgerufen werden

Wenn Sie ein Projekt, eine Aufgabe oder ein Problem wiederherstellen, werden die folgenden zugehörigen Informationen zusammen mit diesem wiederhergestellt:

* Kommentare und Antworten im Bereich &quot;Updates&quot;
* Genehmigungen
* Arbeitsaufträge
* Benutzerdefinierte Formulare
* Warteschlangeneinrichtung
* Geschäftsfälle, einschließlich Scorecards, Ziele und Risiken
* Projektteams
* Daten
* Probleme
* Aufgaben
* Teilaufgaben
* Statuswerte
* Finanzinformationen:

   * Rechnungsdatensätze
   * Abrechnungssätze
   * Ausgaben

* Informationen zur Zeitleiste:

   * Vorgänger
   * Aufgabenbegrenzungen
   * Art der Dauer

* Baselines

  Grundlinien von Aufgaben werden beim Wiederherstellen des übergeordneten Projekts oder der übergeordneten Aufgabe wiederhergestellt, jedoch nicht beim Wiederherstellen einzeln gelöschter Aufgaben.

* Stunden (und Stunden-IDs)

  Ob Stunden für das gelöschte Element wiederhergestellt werden, hängt von den Einstellungen ab, die Sie beim Konfigurieren der Voreinstellungen für Zeitpläne und Stunden ausgewählt haben. Weitere Informationen finden Sie unter [Konfigurieren der Auswirkungen auf die Stunden, in denen ein Objekt gelöscht und wiederhergestellt wird](../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md).

* Die URL des Elements

  Nach der Wiederherstellung bleibt die URL des Elements unverändert. Wenn Benutzer Lesezeichen für den Artikel erstellt haben, bleiben diese gültig.

* Zugriff und Berechtigungen

  Benutzer, die Zugriff auf das Element hatten, bevor es gelöscht wurde, erhalten nach der Wiederherstellung wieder Zugriff.

* Dokumente (einschließlich beglaubigter Dokumente)

  Beachten Sie beim Wiederherstellen von Dokumenten und Dokumentversionen Folgendes:

   * Einzelne gelöschte Dokumente können einzeln wiederhergestellt werden.

     Dokumente, die zusammen mit dem übergeordneten Projekt, der Aufgabe oder dem Problem gelöscht wurden, werden beim Wiederherstellen des übergeordneten Projekts wiederhergestellt, können jedoch nicht einzeln wiederhergestellt werden.

   * Alle Versionen eines Dokuments oder Dokumentversands werden bei der Wiederherstellung des Dokuments wiederhergestellt.\
     Einzelne Versionen eines Dokuments oder Dokumentennachweises, die einzeln gelöscht wurden, können nicht wiederhergestellt werden.

## Informationen, die beim Wiederherstellen eines Projekts, einer Aufgabe oder eines Problems nicht wiederhergestellt werden

Wenn Sie ein Projekt, eine Aufgabe oder ein Problem wiederherstellen, werden die folgenden zugehörigen Informationen nicht zusammen mit diesem wiederhergestellt:

* Gefällt mir
* Empfehlungen
* E-Mail-Adresse in die Anforderungswarteschlange aufnehmen
* Favoriten

  Ein Projekt, eine Aufgabe oder ein Problem, das bzw. die/das Sie vor dem Löschen zum Menü &quot;Favoriten&quot;hinzugefügt haben, wird nach der Wiederherstellung nicht mehr im Menü &quot;Favoriten&quot;angezeigt.

* Objekte auflösen

  Ein aufgelöstes Objekt ist ein konvertiertes Problem, das mit der Option konfiguriert wurde **Behalten Sie das ursprüngliche Problem bei und binden Sie seine Lösung an dieses Problem** &lt;**Projekt** oder **task)**>. Wenn Sie das übergeordnete Projekt oder die übergeordnete Aufgabe löschen, wird das Problem nicht mehr als aufgelöstes Objekt identifiziert, da keine Verknüpfung mehr mit dem Projekt oder der Aufgabe besteht. Wenn Sie das übergeordnete Element wiederherstellen, wird der Link nicht wiederhergestellt.

  Weitere Informationen dazu, wie ein Workfront-Administrator oder Gruppenadministrator Probleme so konfiguriert, dass sie bei der Konvertierung mit dem aufgelösten Objekt übereinstimmen, finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) und [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

  Weitere Informationen zu Konvertierungsproblemen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Elemente wiederherstellen

{{step-1-to-setup}}

1. Klicks **Papierkorb** > **Kürzlich gelöscht**.
1. Klicken Sie auf **Projekte**, **Aufgaben**, **Probleme**, **Vorlagen** oder **Dokumente** -Tab, abhängig vom Elementtyp, den Sie wiederherstellen möchten.

   Elemente werden nach **Löschdatum** -Spalte standardmäßig aus.

1. Wählen Sie bis zu 10 Elemente aus, die Sie wiederherstellen möchten.

   Wenn Sie eine untergeordnete Aufgabe löschen, wird sie in der Liste angezeigt.

   Wenn Sie eine übergeordnete Aufgabe löschen, wird nur die übergeordnete Aufgabe in der Liste angezeigt. Alle untergeordneten Aufgaben werden jedoch wiederhergestellt, wenn Sie eine übergeordnete Aufgabe wiederherstellen.

1. Klicks **Wiederherstellen** , um die ausgewählten Elemente an ihrem ursprünglichen Speicherort wiederherzustellen.
1. (Optional) Um das wiederhergestellte Element schnell anzuzeigen, führen Sie die Schritte unter [Wiederhergestelltes Element anzeigen](../../../administration-and-setup/manage-workfront/manage-deleted-items/view-restored-items.md).

   Weitere Informationen dazu, was nach dem Wiederherstellen eines Elements geschieht, finden Sie im Abschnitt [Was passiert nach dem Wiederherstellen von Elementen?](#what-happens-after-you-restore-items) in diesem Artikel.

## Was passiert nach dem Wiederherstellen von Elementen? {#what-happens-after-you-restore-items}

* Wenn Sie Aufgaben und Unteraufgaben wiederherstellen, werden sie in der Reihenfolge angezeigt, in der sie vor dem Löschen waren.

  Wenn sich die Reihenfolge anderer Aufgaben ändert, während die Aufgabe gelöscht wird, kann die Aufgabe jedoch am Ende der Liste der Aufgaben oder Unteraufgaben wiederhergestellt werden.

* Nachdem Sie ein Element wiederhergestellt haben:

   * Es wird eine Meldung angezeigt, die Sie darüber informiert, ob Sie erfolgreich waren.

     Sie erhalten auch eine E-Mail-Benachrichtigung. Wenn Sie mehrere Elemente wiederhergestellt haben, werden diese in der E-Mail aufgelistet.

   * Ein Kommentar wird im Bereich Updates des Projekts, der Aufgabe oder des Problems sowie im Bereich des übergeordneten Objekts angezeigt.

     Dies geschieht nicht, wenn Sie ein Dokument oder eine Vorlage wiederherstellen.

## Wiederhergestellte Testsendungen

Wenn ein Benutzer ein Dokument wiederherstellt, das über einen Testversand verfügt, zeigt die Seite &quot;Testversandaktivitäten&quot;für den Testversand möglicherweise den Namen des ersten aktiven Workfront-Administrators an, der für die Instanz Ihres Unternehmens aufgelistet ist (in der Reihenfolge der Profil-ID), und nicht den tatsächlichen Benutzer, der den Testversand wiederhergestellt hat.
