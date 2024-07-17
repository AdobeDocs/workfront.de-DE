---
title: Meilensteinpfad erstellen
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Als Adobe Workfront-Administrator können Sie Meilensteinpfade erstellen, die dann auf jedes Projekt im System angewendet werden können. Die Änderungen, die Sie an Meilensteinpfaden in diesem Bereich vornehmen, wirken sich auf das gesamte Workfront-System aus.
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%

---

# Meilensteinpfad erstellen

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Als Adobe Workfront-Administrator können Sie Meilensteinpfade erstellen, die dann auf jedes Projekt im System angewendet werden können. Die Änderungen, die Sie an Meilensteinpfaden in diesem Bereich vornehmen, wirken sich auf das gesamte Workfront-System aus.

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

## Meilensteine und Meilensteinpfade

Sie können die Schlüsselaufgaben in einem Projekt mit vordefinierten Meilensteinen verknüpfen. Diese Funktion bietet Managern und anderen Interessenträgern einen allgemeinen Überblick über den Fortschritt eines Projekts.

Die Summe aller vordefinierten Meilensteine wird als Meilensteinpfad bezeichnet.

Der erste Schritt beim Erstellen eines Meilensteinpfads besteht darin, zu ermitteln, was die Meilensteinschritte sind, und die Meilensteine festzulegen. Da Sie einen Meilensteinpfad mit mehreren Projekten verknüpfen können, müssen die Meilensteinschritte allgemeine Phasen oder Phasen eines Projekts sein.

Weitere Informationen dazu, wie Sie einen Meilensteinpfad mit einem Projekt und einem Meilenstein mit einer Aufgabe verknüpfen können, finden Sie unter [Meilensteine mit Aufgaben verknüpfen](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Meilensteinpfad erstellen

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **Prozesse** > **Milestone-Pfade**.
1. Klicken Sie auf **Neuer Meilensteinpfad.**
1. Geben Sie die folgenden Informationen im Bereich **Grundlegende Informationen** an:

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
      <td>Aktivieren Sie dieses Kontrollkästchen, wenn der Meilensteinpfad aktiv sein soll. Andere Benutzer können diesen Pfad finden und ihn bei der Erstellung oder Bearbeitung von Projekten an Projekte anhängen. Inaktive Meilensteinpfade können nicht an Projekte angehängt werden. Dies ist standardmäßig aktiviert.</td>
    </tr>
    <tr>
      <td>Gruppen</td>
      <td>Wählen Sie die aufgeführten Gruppen aus, damit Benutzer in diesen Gruppen diesen Meilensteinpfad anzeigen und auf ihre Projekte anwenden können. Die Startseite des Benutzers, der den Meilensteinpfad eingibt, ist standardmäßig ausgewählt.</td>
    </tr>
   </table>

1. Geben Sie die folgenden Informationen im Bereich **Milestones** an:

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
      <td> <p>Wählen Sie eine Farbe, die mit Ihrem Meilenstein verknüpft werden soll. </p> <p>Wenn Sie keine Farbe auswählen, wählt das System die letzte Farbe, die in einem Meilensteinpfad verwendet wird. Es wird empfohlen, für jeden Meilenstein eine eindeutige Farbe auszuwählen. Die Farbe wird für visuelle und Berichterstattungszwecke verwendet.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Milestone hinzufügen** und fügen Sie bei Bedarf weitere Meilensteine hinzu, bis der Pfad abgeschlossen ist.
1. Klicken Sie auf **Milestone-Pfad erstellen** , um Ihre Änderungen zu speichern.

   Ihr Meilensteinpfad kann mit einem Projekt verknüpft werden.

   Weitere Informationen zum Verknüpfen von Meilensteinpfaden mit Projekten und Meilensteinen mit Aufgaben finden Sie unter [Verknüpfen von Meilensteinen mit Aufgaben](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
