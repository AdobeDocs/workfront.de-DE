---
user-type: administrator
product-area: system-administration;user-management
keywords: manage,subgroup,edit
navigation-topic: create-and-manage-subgroups
title: Verwalten einer Untergruppe
description: Als Gruppenadministrator einer Untergruppe können Sie die Untergruppe erstellen, verschieben, anzeigen, bearbeiten, kopieren, umbenennen, exportieren und löschen. Sie können eine Untergruppe auch zu einer Gruppe der obersten Ebene machen, indem Sie sie aus ihrer übergeordneten Gruppe entfernen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 1%

---

# Verwalten einer Untergruppe

Als Gruppenadministrator einer Untergruppe können Sie die Untergruppe erstellen, verschieben, anzeigen, bearbeiten, kopieren, umbenennen, exportieren und löschen.

Sie können eine Untergruppe auch zu einer Gruppe der obersten Ebene machen, indem Sie sie aus ihrer übergeordneten Gruppe entfernen.

Wenn es Gruppen über Ihrer Gruppe gibt, können ihre Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Weitere Informationen zu Untergruppen finden Sie unter [Übersicht über Untergruppen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen, Verschieben, Anzeigen, Bearbeiten, Kopieren, Umbenennen, Exportieren oder Löschen einer Untergruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Klicken Sie auf den Namen der Gruppe, die die Untergruppe enthält, an der Sie arbeiten möchten.

   Oder

   Wenn Sie eine oder mehrere Untergruppen verschieben, klicken Sie auf den Namen der Zielgruppe (Sie geben an, welche Untergruppen Sie in einem späteren Schritt verschieben möchten).

1. Klicken Sie im linken Menü auf **Untergruppen**.

1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Neue Untergruppe erstellen</td> 
      <td> <p>Wenn Sie die neue Untergruppe eine Ebene weiter unten von der angezeigten Gruppe erstellen möchten, klicken Sie auf <strong>Untergruppe hinzufügen</strong>.</p> <p>Wenn Sie die neue Untergruppe auch unter einer anderen Untergruppe in der Liste erstellen möchten, wählen Sie diese Untergruppe aus und klicken Sie dann auf <strong>Hinzufügen von s</strong><strong>Untergruppe</strong>.</p> <p>Informationen zu den Optionen, die Sie zum Konfigurieren der Untergruppe verwenden können, finden Sie in der Tabelle unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Erstellen einer Untergruppe</a>.</p> <p>Eine Gruppierungshierarchie darf 15 Ebenen nicht überschreiten, eine einzelne Ebene kann jedoch eine unbegrenzte Anzahl paralleler Gruppen aufweisen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verschieben einer Untergruppe </td> 
      <td> <p>Sie können vorhandene Untergruppen unter eine andere Gruppe verschieben, die Sie verwalten.</p> <p>Eine Gruppierungshierarchie darf 15 Ebenen nicht überschreiten, eine einzelne Ebene kann jedoch eine unbegrenzte Anzahl paralleler Gruppen aufweisen.</p> 
       <ol> 
        <li value="1"> <p>(Optional) Wählen Sie eine Untergruppe aus, um sie zur Zielgruppe zu machen.</p> <p>Wenn Sie diesen Schritt überspringen, ist die in Schritt 3 ausgewählte Gruppe die Zielgruppe.</p> </li> 
        <li value="2">Klicken Sie auf <strong>Untergruppe hinzufügen</strong> &gt; <strong>Vorhandene Gruppe</strong>.</li> 
        <li value="3"> <p>Geben Sie im angezeigten Feld <strong>Vorhandene Gruppe</strong> den Namen der zu verschiebenden Untergruppe ein.</p> <p>Die angezeigten Ergebnisse enthalten keine Gruppen über der Zielgruppe.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe auswählen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol "<img src="assets/info-icon.png">"klicken, das neben der Gruppe angezeigt wird. Dadurch wird eine QuickInfo mit Informationen zur Gruppe angezeigt, z. B. die Hierarchie der Gruppen darüber und deren Administratoren.</p> </li> 
        <li value="4"> <p>Klicken Sie auf den Namen der Untergruppe, die verschoben werden soll, wenn sie in der Liste angezeigt wird.</p> </li> 
        <li value="5"> <p>Wiederholen Sie die Schritte c-d für alle anderen Untergruppen, die Sie in die Zielgruppe verschieben möchten</p> </li> 
        <li value="6">Klicken Sie auf <strong>Speichern</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bearbeiten einer Untergruppe</td> 
      <td> <p>Wählen Sie die zu bearbeitende Untergruppe aus und klicken Sie auf das Bearbeitungssymbol <img src="assets/edit-icon.png">.</p> <p>Informationen zu den Optionen, die Sie zum Konfigurieren der Untergruppe verwenden können, finden Sie in der Tabelle unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Erstellen einer Gruppe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine oder mehrere Untergruppen exportieren</td> 
      <td> 
       <ol> 
        <li value="1">Wählen Sie die zu exportierenden Untergruppen aus.</li> 
        <li value="2">Klicken Sie auf das Symbol Exportieren <img src="assets/export.png"> und wählen Sie dann das gewünschte Dateiformat aus.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine Untergruppe kopieren, um eine neue Gruppe der obersten Ebene zu erstellen</td> 
      <td> <p>(Nur für Workfront-Administratoren verfügbar.) Wenn Sie eine Untergruppe kopieren, wird sie zu einer übergeordneten Gruppe. Alle Gruppenmitglieder und Untergruppen werden damit kopiert. Die Gruppenmitglieder behalten alle Zuweisungen, die sie in der ursprünglichen Gruppe hatten.</p> <p>Weitere Informationen zum Kopieren einer Untergruppe finden Sie unter <a href="#about-copying-a-subgroup" class="MCXref xref">Über das Kopieren einer Untergruppe</a> in diesem Artikel.</p> 
       <ol> 
        <li value="1">Wählen Sie eine Untergruppe aus und klicken Sie dann auf das Symbol Kopieren <img src="assets/copy-icon.png"> , um eine neue Gruppe der obersten Ebene auf der Grundlage der ausgewählten Gruppe zu erstellen.</li> 
        <li value="2"> <p>Konfigurieren Sie die Einstellungen der neuen Gruppe.</p> <p>Hilfe zu diesen Einstellungen finden Sie in der Tabelle im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Erstellen einer Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe</a> im Artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Erstellen einer Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine Untergruppe löschen</td> 
      <td> <p><b>WICHTIG</b>: Wenn Sie eine Gruppe oder Untergruppe löschen, müssen Sie die Benutzer, Arbeitselemente und alle Untergruppen, die dieser Gruppe derzeit zugewiesen sind, beibehalten. Um sicherzustellen, dass die Objekte erhalten bleiben, müssen Sie die Objekte der Gruppe im folgenden Schritt einer anderen Gruppe zuweisen.</p> 
       <ol> 
        <li value="1">Wählen Sie die Untergruppe aus und klicken Sie dann auf das Löschsymbol <img src="assets/delete.png">.</li> 
        <li value="2">Geben Sie im angezeigten Feld <strong>Gruppe löschen</strong> mit der Eingabe den Namen der Gruppe ein, in die Sie die Mitglieder, Arbeitselemente und Untergruppen der Gruppe, die Sie löschen möchten, verschieben möchten.</li> 
        <li value="3">Klicken Sie auf <strong>Löschen Sie sie</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Wenn Sie eine Gruppe verwalten, die Untergruppen enthält, ist es hilfreich, Daten über die gesamte Gruppe und alle zugehörigen Untergruppen zu identifizieren und zu filtern. Verwenden Sie dazu das Feld Oberste übergeordnete ID in einem Bericht oder einer Liste.
>
>Angenommen, Sie verwalten eine große Marketing-Abteilung und möchten eine Liste aller Projekte, an denen die gesamte Abteilung arbeitet.
>
>In Workfront wird diese Marketingabteilung durch eine Gruppe namens Marketing mit drei Untergruppen namens Feldmarketing, Produktmarketing und digitalem Marketing vertreten. Um die Projekte aufzulisten, die zur gesamten Marketing-Abteilung gehören (alle vier Gruppen), können Sie einen Filter für den Bereich &quot;Projekte&quot;mit der folgenden Filterregel erstellen:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>Sie können auch das Feld &quot;Oberster übergeordneter Name&quot;verwenden, um Daten zu identifizieren, die einer Gruppe der obersten Ebene zugeordnet sind, jedoch nur in Ansichten, nicht in Filtern oder Gruppierungen.

## Entfernen Sie eine Untergruppe aus ihrer übergeordneten Gruppe und machen Sie sie zu einer Gruppe der obersten Ebene

Sie können eine Untergruppe zu einer Gruppe der obersten Ebene machen, indem Sie sie aus ihrer übergeordneten Gruppe entfernen.

>[!TIP]
>
>Wenn Sie eine Gruppe deaktivieren, der Untergruppen untergeordnet sind, werden diese Untergruppen ebenfalls inaktiv. Wenn Sie möchten, dass einer von ihnen aktiv ist, können Sie diese Anweisungen verwenden, um ihn aus der übergeordneten Gruppe zu entfernen und ihn dann erneut zu aktivieren.
>
>Anweisungen zum Deaktivieren und erneuten Aktivieren von Gruppen finden Sie in den Abschnitten [Details einer Gruppe anzeigen und verwalten](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) und [Details einer Gruppe anzeigen und verwalten](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) im Artikel [Details einer Gruppe anzeigen und verwalten](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md) .

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Wählen Sie die übergeordnete Gruppe der Gruppe aus, die Sie als Gruppe der obersten Ebene einrichten möchten, und klicken Sie dann auf das Bearbeitungssymbol ![](assets/edit-icon.png).
1. Geben Sie im angezeigten Feld **Gruppe bearbeiten** unter **Gruppenmitglieder und Gruppenadministratoren** den Namen der Untergruppe ein, aus der Sie eine Gruppe der obersten Ebene erstellen möchten, und klicken Sie dann auf das X rechts von ihrem Namen, sobald es angezeigt wird.
1. Klicken Sie auf **Speichern**.

## Mitglieder einer Gruppe anzeigen und verwalten

Wenn Sie die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen, können Sie alle Benutzer in den Untergruppen der Gruppe anzeigen und verwalten. Anweisungen finden Sie unter [Anzeigen und Verwalten von Untergruppenmitgliedern](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Über das Kopieren einer Untergruppe {#about-copying-a-subgroup}

Beachten Sie beim Kopieren einer Untergruppe Folgendes.

* Wenn eine von Ihnen kopierte Untergruppe über eigene Untergruppen verfügt, werden diese in die Kopie einbezogen und ihre Namen wie folgt formatiert:

  `Original subgroup name (Copy)`

* Jede Untergruppe, die zu einer öffentlichen Gruppe gehört, ist ebenfalls öffentlich, sodass jeder Benutzer mit Bearbeitungsbenutzerzugriff in oder aus der Gruppe Benutzer zur Untergruppe hinzufügen kann.
