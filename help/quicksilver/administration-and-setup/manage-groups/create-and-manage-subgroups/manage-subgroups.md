---
user-type: administrator
product-area: system-administration;user-management
keywords: verwalten,Untergruppe,bearbeiten
navigation-topic: create-and-manage-subgroups
title: Verwalten einer Untergruppe
description: Als Gruppenadministrator einer Untergruppe können Sie die Untergruppe erstellen, verschieben, anzeigen, bearbeiten, kopieren, umbenennen, exportieren und löschen. Sie können eine Untergruppe auch zu einer Gruppe der obersten Ebene machen, indem Sie sie aus der übergeordneten Gruppe entfernen.
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

Sie können eine Untergruppe auch zu einer Gruppe der obersten Ebene machen, indem Sie sie aus der übergeordneten Gruppe entfernen.

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Weitere Informationen zu Untergruppen finden Sie unter [Untergruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen, Verschieben, Anzeigen, Bearbeiten, Kopieren, Umbenennen, Exportieren oder Löschen einer Untergruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![](assets/groups-icon.png).

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, die die Untergruppe enthält, an der Sie arbeiten möchten.

   Oder

   Wenn Sie eine oder mehrere Untergruppen verschieben, klicken Sie auf den Namen der Zielgruppe (Sie geben in einem späteren Schritt an, welche Untergruppen verschoben werden sollen).

1. Klicken Sie im linken Menü auf **Untergruppen**.

1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Erstellen einer neuen Untergruppe</td> 
      <td> <p>Wenn Sie die neue Untergruppe eine Ebene unterhalb der angezeigten Gruppe erstellen möchten, klicken Sie auf "<strong> hinzufügen</strong>.</p> <p>Wenn Sie die neue Untergruppe unter einer anderen Untergruppe in der Liste erstellen möchten, wählen Sie diese Untergruppe aus und klicken Sie dann auf <strong>Hinzufügen s</strong><strong>subgroup</strong>.</p> <p>Informationen zu den Optionen, mit denen Sie die Untergruppe konfigurieren können, finden Sie in der Tabelle unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md" class="MCXref xref">Erstellen einer Untergruppe</a>.</p> <p>Eine Gruppenhierarchie kann nicht mehr als 15 Ebenen umfassen, aber eine einzelne Ebene kann eine unbegrenzte Anzahl paralleler Gruppen aufweisen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verschieben einer Untergruppe </td> 
      <td> <p>Sie können bestehende Untergruppen unter eine andere Gruppe verschieben, die Sie verwalten.</p> <p>Eine Gruppenhierarchie kann nicht mehr als 15 Ebenen umfassen, aber eine einzelne Ebene kann eine unbegrenzte Anzahl paralleler Gruppen aufweisen.</p> 
       <ol> 
        <li value="1"> <p>(Optional) Wählen Sie eine Untergruppe aus, um sie zur Zielgruppe zu machen.</p> <p>Wenn Sie diesen Schritt überspringen, ist die in Schritt 3 ausgewählte Gruppe die Zielgruppe.</p> </li> 
        <li value="2">Klicken Sie <strong>Untergruppe hinzufügen</strong> &gt; <strong>Vorhandene Gruppe</strong>.</li> 
        <li value="3"> <p>Geben <strong> im angezeigten </strong> „Vorhandene Gruppe“ den Namen einer Untergruppe ein, die Sie verschieben möchten.</p> <p>Die angezeigten Ergebnisse enthalten keine Gruppen oberhalb der Zielgruppe.</p> <p>Sie können sicherstellen, dass Sie die richtige Gruppe auswählen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol <img src="assets/info-icon.png"> neben der Gruppe klicken. Dadurch wird eine QuickInfo angezeigt, die Informationen über die Gruppe auflistet, wie z. B. die Hierarchie der darüber liegenden Gruppen und deren Administratoren.</p> </li> 
        <li value="4"> <p>Klicken Sie auf den Namen der Untergruppe, die Sie verschieben möchten, wenn sie in der Liste angezeigt wird.</p> </li> 
        <li value="5"> <p>Wiederholen Sie die Schritte c-d für alle anderen Untergruppen, die Sie in die Zielgruppe verschieben möchten</p> </li> 
        <li value="6">Klicken Sie auf <strong>Speichern</strong>.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bearbeiten einer Untergruppe</td> 
      <td> <p>Wählen Sie die zu bearbeitende Untergruppe aus und klicken Sie dann auf das Symbol „Bearbeiten“ <img src="assets/edit-icon.png">.</p> <p>Informationen zu den Optionen, mit denen Sie die Untergruppe konfigurieren können, finden Sie in der Tabelle unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Erstellen einer Gruppe</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine oder mehrere Untergruppen exportieren</td> 
      <td> 
       <ol> 
        <li value="1">Wählen Sie die zu exportierende Untergruppe bzw. die zu exportierenden Untergruppen aus.</li> 
        <li value="2">Klicken Sie auf das Symbol Exportieren <img src="assets/export.png"> wählen Sie dann das gewünschte Dateiformat aus.</li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopieren einer Untergruppe, um eine neue Gruppe der obersten Ebene zu erstellen</td> 
      <td> <p>(Nur für Workfront-Administratoren verfügbar.) Wenn Sie eine Untergruppe kopieren, wird sie zu einer übergeordneten Gruppe. Alle Gruppenmitglieder und Untergruppen werden damit kopiert. Die Gruppenmitglieder behalten alle Arbeitsaufträge bei, die sie in der ursprünglichen Gruppe hatten.</p> <p>Weitere Informationen zum Kopieren einer Untergruppe finden Sie unter <a href="#about-copying-a-subgroup" class="MCXref xref">Informationen zum Kopieren einer </a>) in diesem Artikel.</p> 
       <ol> 
        <li value="1">Wählen Sie eine Untergruppe aus und klicken Sie dann auf das Symbol Kopieren <img src="assets/copy-icon.png"> , um eine neue Gruppe der obersten Ebene basierend auf der ausgewählten Gruppe zu erstellen.</li> 
        <li value="2"> <p>Konfigurieren Sie die Einstellungen der neuen Gruppe.</p> <p>Hilfe zu diesen Einstellungen finden Sie in der Tabelle im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Erstellen einer Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder </a>) im Artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group" class="MCXref xref">Erstellen einer Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Löschen einer Untergruppe</td> 
      <td> <p><b>WICHTIG</b>: Wenn Sie eine Gruppe oder Untergruppe löschen, müssen Sie die Benutzenden, Arbeitselemente und alle Untergruppen beibehalten, die ihr derzeit zugewiesen sind. Um sicherzustellen, dass sie erhalten bleiben, müssen Sie bei einer Eingabeaufforderung die Objekte der Gruppe im folgenden Schritt einer anderen Gruppe zuweisen.</p> 
       <ol> 
        <li value="1">Wählen Sie die Untergruppe aus und klicken Sie dann auf das Symbol Löschen <img src="assets/delete.png">.</li> 
        <li value="2">Beginnen Sie mit der Eingabe in das <strong>Gruppe löschen</strong> angezeigte Feld und wählen Sie dann den Namen der Gruppe aus, in die Sie die Mitglieder, Arbeitselemente und Untergruppen der zu löschenden Gruppe verschieben möchten.</li> 
        <li value="3">Klicken Sie <strong>Löschen</strong>.</li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

>[!TIP]
>
>Wenn Sie eine Gruppe verwalten, die Untergruppen enthält, ist es hilfreich, Daten über die gesamte Gruppe und alle zugehörigen Untergruppen identifizieren und filtern zu können. Verwenden Sie dazu das Feld ID des obersten übergeordneten Elements in einem Bericht oder einer Liste.
>
>Angenommen, Sie verwalten eine große Marketing-Abteilung und möchten eine Liste aller Projekte anzeigen, an denen die gesamte Abteilung arbeitet.
>
>In Workfront wird diese Marketing-Abteilung durch eine Gruppe namens Marketing mit drei Untergruppen namens Field Marketing, Product Marketing und Digital Marketing repräsentiert. Um die Projekte aufzulisten, die zur gesamten Marketing-Abteilung gehören (alle 4 Gruppen), können Sie mit der folgenden Filterregel einen Filter für den Bereich „Projekte“ erstellen:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>Sie können auch das Feld Name des obersten übergeordneten Elements verwenden, um Daten zu identifizieren, die mit einer Gruppe der obersten Ebene verknüpft sind, jedoch nur in Ansichten, nicht in Filtern oder Gruppierungen.

## Entfernen Sie eine Untergruppe aus der übergeordneten Gruppe und machen Sie sie zu einer Gruppe der obersten Ebene.

Sie können eine Untergruppe zu einer Gruppe der obersten Ebene machen, indem Sie sie aus der übergeordneten Gruppe entfernen.

>[!TIP]
>
>Wenn Sie eine Gruppe deaktivieren, die Untergruppen enthält, werden diese Untergruppen ebenfalls inaktiv. Wenn Sie möchten, dass eine der Gruppen aktiv ist, können Sie sie mithilfe dieser Anweisungen aus der übergeordneten Gruppe entfernen und dann reaktivieren.
>
>Anweisungen zum Deaktivieren und Reaktivieren von Gruppen finden Sie in den Abschnitten [Anzeigen und Verwalten der Details einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#view) und [Anzeigen und Verwalten ](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md#inactive) Details einer Gruppe im Artikel [Anzeigen und Verwalten der Details einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![](assets/groups-icon.png).

1. Wählen Sie die übergeordnete Gruppe der Gruppe aus, die Sie zu einer Gruppe der obersten Ebene machen möchten, und klicken Sie dann auf das Symbol Bearbeiten ![](assets/edit-icon.png).
1. Beginnen Sie im angezeigten **Gruppe bearbeiten** unter **Gruppenmitglieder und Gruppenadministratoren** mit der Eingabe des Namens der Untergruppe, die Sie zu einer Gruppe der obersten Ebene machen möchten, und klicken Sie dann rechts neben ihrem Namen auf das X, wenn sie angezeigt wird.
1. Klicken Sie auf **Speichern**.

## Anzeigen und Verwalten der Untergruppenmitglieder einer Gruppe

Wenn Sie die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen, können Sie alle Benutzenden in den Untergruppen der Gruppe anzeigen und verwalten. Anweisungen finden Sie unter [Anzeigen und Verwalten von Untergruppenmitgliedern](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Informationen zum Kopieren einer Untergruppe {#about-copying-a-subgroup}

Beachten Sie beim Kopieren einer Untergruppe Folgendes.

* Wenn eine kopierte Untergruppe über eigene Untergruppen verfügt, sind diese in der Kopie enthalten und ihre Namen sind wie folgt formatiert:

  `Original subgroup name (Copy)`

* Jede Untergruppe, die zu einer öffentlichen Gruppe gehört, ist ebenfalls öffentlich, sodass jeder Benutzer mit edit-user-Zugriff, unabhängig davon, ob er in der Gruppe ist oder nicht, Benutzer zur Untergruppe hinzufügen kann.
