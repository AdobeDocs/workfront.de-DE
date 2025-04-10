---
title: Meilensteinpfad erstellen
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Als Adobe Workfront-Administrator können Sie Meilensteinpfade erstellen, die dann auf jedes Projekt im System angewendet werden können. Die Änderungen an Meilensteinpfaden in diesem Bereich wirken sich auf das gesamte Workfront-System aus.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 7f96cddc18e70dff34beb33ef2785af69a55c36f
workflow-type: tm+mt
source-wordcount: '815'
ht-degree: 3%

---

# Meilensteinpfad erstellen

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Als Adobe Workfront-Administrator können Sie Meilensteinpfade erstellen, die dann auf jedes Projekt im System angewendet werden können. Die Änderungen an Meilensteinpfaden in diesem Bereich wirken sich auf das gesamte Workfront-System aus.

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Meilensteine und Meilensteinpfade

Sie können die wichtigsten Aufgaben in einem Projekt mit vordefinierten Meilensteinen verknüpfen. Diese Funktion bietet Managern und anderen Stakeholdern einen Überblick über den Fortschritt eines Projekts.

Die Summe aller vordefinierten Meilensteine wird als Meilensteinpfad bezeichnet.

Der erste Schritt beim Erstellen eines Meilensteinpfads besteht darin, zu ermitteln, was die Meilensteinschritte sind, und die Meilensteine festzulegen. Da Sie einen Meilensteinpfad mit mehreren Projekten verknüpfen können, müssen die Meilensteinschritte allgemeine Phasen oder Phasen eines Projekts sein.

Weitere Informationen dazu, wie Sie einen Meilensteinpfad mit einem Projekt und einen Meilenstein mit einer Aufgabe verknüpfen können, finden Sie unter [Zuordnen von Meilensteinen zu Aufgaben](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Meilensteinpfad erstellen

{{step-1-to-setup}}

1. Klicken Sie **Prozesse** > **Meilensteinpfade**.
1. Klicken Sie auf **Neuer Meilensteinpfad.**
1. Geben Sie folgende Informationen im Bereich **Basisinformationen** an:

   <table style="table-layout:auto">
    <tr>
      <td>Meilensteinpfadname</td>
       <td>Geben Sie einen Namen für den Meilensteinpfad ein.</td>
    </tr>
    <tr>
      <td>Beschreibung</td>
      <td>Geben Sie eine Beschreibung ein, um den Meilensteinpfad zu definieren.</td>
    </tr>
    <tr>
       <td>Ist aktiv</td>
      <td>Aktivieren Sie dieses Kontrollkästchen, wenn der Meilensteinpfad aktiv sein soll. Andere Benutzer können diesen Pfad suchen und ihn beim Erstellen oder Bearbeiten von Projekten an Projekte anhängen. Inaktive Meilensteinpfade können nicht an Projekte angehängt werden. Dies ist standardmäßig aktiviert.</td>
    </tr>
    <tr>
      <td>Gruppen</td>
      <td>Wählen Sie die aufgelisteten Gruppen aus, damit die Benutzer in diesen Gruppen diesen Meilensteinpfad sehen und auf ihre Projekte anwenden können. Die Hauptgruppe des Benutzers, der den Meilensteinpfad eingibt, ist standardmäßig ausgewählt.</td>
    </tr>
   </table>

1. Geben Sie die folgenden Informationen im Bereich **Meilensteine** an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Geben Sie für jeden Meilenstein beschreibende Namen ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie eine Beschreibung für den Meilenstein ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Farbe</td> 
      <td> <p>Farbe auswählen, die mit Ihrem Meilenstein verknüpft werden soll. </p> <p>Wenn Sie keine Farbe auswählen, wählt das System die letzte Farbe aus, die in einem Meilensteinpfad verwendet wird. Es wird empfohlen, für jeden Meilenstein eine eigene Farbe zu wählen. Die Farbe wird für visuelle und Reporting-Zwecke verwendet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Meilenstein hinzufügen** und fügen Sie weitere Meilensteine nach Bedarf hinzu, bis der Pfad abgeschlossen ist.

1. Klicken Sie **Meilensteinpfad erstellen** um Ihre Änderungen zu speichern.

   Ihr Meilensteinpfad kann jetzt mit einem Projekt verknüpft werden.

   Weitere Informationen zum Verknüpfen von Meilensteinpfaden mit Projekten und Meilensteinen mit Aufgaben finden Sie unter [Verknüpfen von Meilensteinen mit Aufgaben](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).


1. (Optional) Klicken Sie auf **Export**-Symbol ![Export-Symbol](assets/export-icon.png) und wählen Sie dann eines der folgenden Formate aus, um die Liste der Meilensteinpfade in eine Datei zu exportieren:

   * PDF
   * Excel
   * Excel (xlsx)
   * Durch Tabulatoren getrennt

1. (Optional) Wählen Sie einen Meilenstein in der Meilensteinliste aus und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png), um Meilensteininformationen zu bearbeiten.
1. (Optional) Wählen Sie in der Meilenstein-Liste einen Meilenstein aus und klicken Sie dann auf das **Löschen**-Symbol ![Löschen](assets/delete-icon.png), um ihn zu löschen.
1. Klicken Sie **Ja, löschen**.
Der Meilenstein wurde gelöscht und kann nicht wiederhergestellt werden. Alle mit dem Meilenstein verknüpften Projektinformationen und alle mit den Meilensteinpfaden verknüpften Aufgabeninformationen werden ebenfalls gelöscht.


## Anzeigen von Meilensteinpfaddetails in einem Bericht

Sie können die Details eines Meilensteinpfads in einem Projektbericht anzeigen.

Sie müssen einem Projekt einen Meilensteinpfad zuordnen, bevor Sie dessen Details in einem Projektbericht anzeigen können.

Informationen zum Verknüpfen von Meilensteinpfaden mit Projekten finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

{{step1-to-reports}}

1. Klicken Sie **Neuer Bericht** und dann auf **Projekt**.
1. Klicken Sie auf **Spalte hinzufügen**.
1. Beginnen Sie im Bereich **In dieser Spalte anzeigen** mit der Eingabe **Meilensteinpfad** und klicken Sie dann auf **Meilensteinpfadname**, wenn er angezeigt wird.
1. (Optional) Klicken Sie **Filter** und fügen Sie dem Bericht den folgenden Filter hinzu: **Projektmeilensteinpfad-ID ist nicht leer**.

   Der Filter stellt sicher, dass Sie im Bericht nur Projekte anzeigen, die mit einem Meilensteinpfad verknüpft sind.

1. Klicken Sie auf **Speichern + schließen**.
1. Fügen Sie einen Namen für Ihren Bericht hinzu und klicken Sie dann auf **Übernehmen**.

   Der Projektbericht wird angezeigt. Die mit jedem Projekt verknüpften Meilensteinpfade werden in der letzten Spalte des Berichts angezeigt.
1. Klicken Sie auf den Namen eines Meilensteinpfads in der letzten Spalte des Berichts.

   Die Details des Meilensteinpfads werden angezeigt.

   ![Meilensteinpfaddetails aus dem Projektbericht](assets/milestone-details-from-project-report.png)

   Auf der Seite mit den Meilensteinpfaddetails werden die folgenden Informationen angezeigt:

   * Meilensteinpfad - Name, ID und Beschreibung
   * Meilensteinpfadgruppen
   * Meilensteinnamen, Beschreibungen, Farben und Farbsymbole

1. (Optional) Klicken Sie auf **Zurück**, um zum Projektbericht zurückzukehren.



