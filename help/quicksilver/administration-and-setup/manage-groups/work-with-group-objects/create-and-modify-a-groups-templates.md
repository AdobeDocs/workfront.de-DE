---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Erstellen und Ändern von Gruppenprojektvorlagen
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich "Gruppen"verwalten, können Sie Projektvorlagen anzeigen und verwenden, die mit der Gruppe und ihren Untergruppen verknüpft sind.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '1280'
ht-degree: 1%

---

# Erstellen und Ändern von Gruppenprojektvorlagen

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich &quot;Gruppen&quot;verwalten, können Sie Projektvorlagen anzeigen und verwenden, die mit der Gruppe und ihren Untergruppen verknüpft sind.

Wenn es Gruppen über Ihrer Gruppe gibt, können ihre Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff oder höher auf die Vorlagen anzeigen, die Sie anzeigen und verwenden möchten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben.

+++

## Anzeigen, Arbeiten mit und Erstellen von Vorlagen für Ihre Gruppe über den Bereich Gruppen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie Vorlagen erstellen oder ändern möchten.
1. Klicken Sie im linken Bereich auf **Vorlagen** , um die Vorlagen aufzulisten, die der Gruppe und etwaigen Untergruppen zugeordnet sind.

   Sie müssen Zugriff auf eine Vorlage haben, um sie in dieser Liste sehen zu können. Weitere Informationen zu diesem Zugriff finden Sie unter [Gewähren des Zugriffs auf Vorlagen](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vorlage hinzufügen</td> 
      <td> <p>Klicken Sie auf <strong>Neue Vorlage</strong> und konfigurieren Sie sie dann mithilfe der verfügbaren Optionen. Weitere Informationen zu diesen Optionen finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Erstellen einer Projektvorlage</a>.</p> <p>Die Vorlage wird automatisch mit der Gruppe verknüpft.</p> <p>Informationen dazu, wie Gruppenvoreinstellungen auf neue Vorlagen angewendet werden, finden Sie unter <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Wie Voreinstellungen auf Vorlagen und Vorlagenaufgaben angewendet werden</a> in diesem Artikel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine oder mehrere Vorlagen bearbeiten</td> 
      <td> <p>Wählen Sie mindestens eine Vorlage aus, klicken Sie auf das Bearbeitungssymbol <img src="assets/edit-icon.png"> und verwenden Sie dann eine der verfügbaren Optionen, um sie zu konfigurieren. Weitere Informationen zu diesen Optionen finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Bearbeiten von Projektvorlagen</a>.</p> <p>Das Symbol Bearbeiten ist nur verfügbar, wenn Sie Zugriff auf alle ausgewählten Vorlagen haben. Weitere Informationen zu diesem Zugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Gewähren des Zugriffs auf Vorlagen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine oder mehrere Vorlagen löschen</td> 
      <td> <p>Wählen Sie mindestens eine Vorlage aus und klicken Sie dann auf das Löschsymbol <img src="assets/delete.png">.</p> <p>Dieses Symbol ist nur verfügbar, wenn Sie Zugriff auf alle ausgewählten Vorlagen haben. Weitere Informationen zu diesem Zugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Gewähren des Zugriffs auf Vorlagen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorlagen freigeben</td> 
      <td> <p>Wählen Sie mindestens eine Vorlage aus, klicken Sie auf das Freigabesymbol <img src="assets/share-icon.png"> und anschließend auf eine der folgenden Optionen im Dropdown-Menü:</p> 
       <ul> 
        <li> <p><strong>Vorlage</strong>: Fügen Sie im angezeigten Feld <strong>Vorlagenzugriff</strong> Namen hinzu, um anzugeben, wer auf die Vorlage selbst zugreifen soll.</p> <p>Weitere Informationen finden Sie im Abschnitt <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Vorlage freigeben</a> im Artikel <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Projektvorlagen freigeben</a>.</p> </li> 
        <li><strong>Projekt</strong>: Fügen Sie im angezeigten Feld <strong>Projektzugriff</strong> Namen hinzu, um anzugeben, wer auf die Projekte zugreifen soll, die aus der Vorlage erstellt wurden.</li> 
       </ul> <p>Das Symbol Freigabe ist nur verfügbar, wenn Sie Zugriff auf alle ausgewählten Vorlagen haben. Weitere Informationen zu diesem Zugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Gewähren des Zugriffs auf Vorlagen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Liste von Vorlagen exportieren</td> 
      <td>Klicken Sie auf <strong>Export</strong> <img src="assets/export.png"> und wählen Sie dann das Dateiformat aus, das Sie für die exportierte Liste verwenden möchten.</td> 
     </tr> 
    </tbody> 
   </table>

## Wie werden Voreinstellungen auf Vorlagen und Vorlagenaufgaben angewendet? {#how-preferences-apply-to-templates-and-template-tasks}

Wenn Sie eine Projektvorlage erstellen, werden die in den Tabellen unten aufgeführten Einstellungen automatisch durch eine Korrelationsprojekt- oder Aufgabenvoreinstellung konfiguriert.

>[!NOTE]
>
>Eine Projekt- oder Aufgabenvoreinstellung auf Gruppen- oder Systemebene wirkt sich auf eine Projektvorlage aus, je nachdem, ob Sie die Vorlage bei ihrer Erstellung mit einer Gruppe verknüpft haben.
>
>Wenn Sie es mit einer Gruppe verknüpft haben, wird die Voreinstellung auf Gruppenebene wirksam. Dies geschieht in den folgenden Szenarien:
>
>* Sie erstellen die Vorlage aus dem Bereich Gruppen , wie in diesem Artikel beschrieben
>* Sie geben eine Gruppe an, wenn Sie die Vorlage mit einer Schnellstartdatei erstellen
>* Sie geben eine Gruppe an, wenn Sie die Vorlage mithilfe der API erstellen
>
>Wenn Sie die neue Vorlage nicht mit einer Gruppe verknüpft haben, wird die Voreinstellung auf Systemebene wirksam. Dies tritt in den unten stehenden Szenarien auf. (Wenn Sie der Vorlage oder Vorlagenaufgabe später eine Gruppe zuweisen, wirken sich die Voreinstellungen der Gruppe nicht darauf aus.)
>
>* Sie erstellen die Vorlage aus dem Bereich Vorlagen .
>* Sie geben keine Gruppe an, wenn Sie die Vorlage mit einer Schnellstartdatei erstellen
>* Sie geben keine Gruppe an, wenn Sie die Vorlage mit der API erstellen
>

* [Durch Projekt- und Aufgabenvoreinstellungen konfigurierte Projektvorlageneinstellungen](#project-template-settings-configured-by-project-and-task-preferences)
* [VorlagenAufgabeneinstellungen, die von Aufgabenvoreinstellungen konfiguriert wurden](#template-task-settings-configured-by-task-preferences)

### Von Projekt- und Aufgabenvoreinstellungen konfigurierte Projektvorlageneinstellungen {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Performance-Index-Methode</p> </td> 
   <td> <p>Wird durch die Gruppenebenenpräferenz "Leistungsindex-Methode"konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder wenn nicht mit einer Projektreferenz auf Systemebene.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bedingungstyp</p> </td> 
   <td> <p>Wird durch die Projektanvoreinstellung auf Gruppenebene konfiguriert: "Legen Sie die Projektbedingung automatisch auf Grundlage des Fortschrittsstatus fest", wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder andernfalls mit der Projektoption auf Systemebene.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Planen aus</p> </td> 
   <td> <p>Wird durch die Gruppenebenenpräferenz "Planen von"konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder durch dieselbe Projektanvoreinstellung auf Systemebene, wenn nicht.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Benutzerzeit</p> </td> 
   <td> <p>Wird durch die Gruppenvorgabe "Benutzerzeit ab"für das Projekt konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder durch die Projektoption auf Systemebene, wenn dies nicht der Fall ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Aktualisierungstyp</p> </td> 
   <td> <p>Wird durch die Gruppenpräferenz "Projektzeitpläne werden automatisch neu berechnet"konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder wenn nicht mit der Projektoption auf Systemebene.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zugriffsparteneinstellungen</p> </td> 
   <td> <p>Wird durch die Aufgabenvoreinstellungen auf Gruppenebene im Abschnitt "Zugriff"konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder wenn nicht mit der Projektreferenz auf Systemebene.</p> </td> 
  </tr> 
 </tbody> 
</table>

Informationen zu den in dieser Tabelle aufgeführten Projektvoreinstellungen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Weitere Informationen zu den Aufgaben- und Problemeinstellungen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Wenn Sie die Gruppe ändern, die mit einer vorhandenen Projektvorlage verknüpft ist, bleiben die Einstellungen der Vorlage unverändert.
>* Wenn Sie eine vorhandene Vorlagenaufgabe in eine andere Vorlage verschieben, bleiben die folgenden Einstellungen in der Vorlagenaufgabe unverändert, unabhängig von der mit der neuen Vorlage verknüpften Gruppe:>
>   * Dauertyp
>   * Umsatztyp
>   * Kostenart
>
>  Die Vorlagenaufgabe wird jedoch durch die Einstellung &quot;Wenn einer Aufgabe eine Person zugewiesen ist&quot;in der neuen Vorlage beeinflusst. Weitere Informationen finden Sie im Abschnitt [Zugriff](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) im Artikel [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Wenn ein Administrator ein Projekt als Vorlage speichert, werden alle Einstellungen für die Vorlage vom Projekt übernommen, einschließlich der Gruppe.
>
>  Wenn ein Administrator eine Aufgabe oder ein Problem mithilfe einer Vorlage in ein Projekt konvertiert, werden alle Einstellungen für die Vorlage durch die bereits in der Vorlage gespeicherten Einstellungen bestimmt.
>

### VorlagenAufgabeneinstellungen, die von Aufgabenvoreinstellungen konfiguriert wurden {#template-task-settings-configured-by-task-preferences}

Wenn Sie eine Vorlagenaufgabe erstellen, werden einige ihrer Einstellungen automatisch durch eine Voreinstellung für die korrelierende Aufgabe konfiguriert. Diese Einstellungen sind in der folgenden Tabelle aufgeführt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Dauertyp </p> </td> 
   <td> <p>Wird durch die Aufgabenvoreinstellung auf Gruppenebene "Dauer-Typ"konfiguriert, wenn Sie die Vorlage mit einer Gruppe verknüpfen, oder durch dieselbe Aufgabe auf Systemebene und die Ausgabevorgabe, wenn nicht anders.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Umsatztyp</p> </td> 
   <td> <p>Wird durch die Aufgabenvoreinstellung auf Gruppenebene "Umsatztyp"konfiguriert, wenn Sie die Vorlage mit einer Gruppe verknüpfen, oder durch dieselbe Aufgabe auf Systemebene und Ausgabevorgabe, wenn nicht.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Kostenart </p> </td> 
   <td> <p> Wird durch die Aufgabenvoreinstellung auf Gruppenebene "Kostentyp"konfiguriert, wenn Sie die Vorlage mit einer Gruppe verknüpfen, oder durch die gleiche Aufgabe auf Systemebene und die Ausgabevorgabe, wenn nicht anders.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den in dieser Tabelle aufgeführten Aufgabenvoreinstellungen finden Sie unter [Systemweite Aufgaben konfigurieren und Voreinstellungen für Aufgaben festlegen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
