---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Erstellen und Ändern der Projektvorlagen einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit der Gruppe und ihren Untergruppen verknüpfte Projektvorlagen anzeigen und mit ihnen arbeiten.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f97a12eb-9002-4f11-908a-c68c1e6dc9c9
source-git-commit: 10780ff51d5b1d9d73cb0a6fb0982abc320b0313
workflow-type: tm+mt
source-wordcount: '1241'
ht-degree: 1%

---

# Erstellen und Ändern der Projektvorlagen einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit der Gruppe und ihren Untergruppen verknüpfte Projektvorlagen anzeigen und mit ihnen arbeiten.

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

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
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr>
  <tr> 
   <td>Objektberechtigungen</td>
   <td>Zugriff auf die Vorlagen, die angezeigt werden sollen und mit denen Sie arbeiten möchten, anzeigen oder höher</td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Im Bereich Gruppen können Sie Vorlagen für Ihre Gruppe anzeigen, damit arbeiten und erstellen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie Vorlagen erstellen oder ändern möchten.
1. Klicken Sie im linken Bereich auf **Vorlagen**, um die Vorlagen aufzulisten, die mit der Gruppe und etwaigen Untergruppen, die sie möglicherweise hat, verknüpft sind.

   Sie müssen Ansichtszugriff auf eine Vorlage haben, um sie in dieser Liste zu sehen. Weitere Informationen zu diesem Zugriff finden Sie unter [Zugriff auf Vorlagen gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vorlage hinzufügen</td> 
      <td> <p>Klicken Sie <strong>Neue Vorlage</strong> und konfigurieren Sie sie dann mithilfe der verfügbaren Optionen. Weitere Informationen zu diesen Optionen finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/create-template.md" class="MCXref xref">Erstellen einer Projektvorlage</a>.</p> <p>Die Vorlage wird automatisch mit der Gruppe verknüpft.</p> <p>Informationen dazu, wie Gruppenvoreinstellungen auf neue Vorlagen angewendet werden, finden Sie unter <a href="#how-preferences-apply-to-templates-and-template-tasks" class="MCXref xref">Wie Voreinstellungen auf Vorlagen und Vorlagenaufgaben angewendet werden</a> in diesem Artikel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine oder mehrere Vorlagen bearbeiten</td> 
      <td> <p>Wählen Sie mindestens eine Vorlage aus, klicken Sie auf das Symbol Bearbeiten <img src="assets/edit-icon.png"> verwenden Sie dann eine der verfügbaren Optionen, um sie zu konfigurieren. Weitere Informationen zu diesen Optionen finden Sie unter <a href="../../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Projektvorlagen bearbeiten</a>.</p> <p>Das Symbol Bearbeiten ist nur verfügbar, wenn Sie Bearbeitungszugriff auf alle ausgewählten Vorlagen haben. Weitere Informationen zu diesem Zugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Zugriff auf Vorlagen gewähren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine oder mehrere Vorlagen löschen</td> 
      <td> <p>Wählen Sie mindestens eine Vorlage aus und klicken Sie dann auf das Symbol Löschen <img src="assets/delete.png">.</p> <p>Dieses Symbol ist nur verfügbar, wenn Sie Bearbeitungszugriff auf alle ausgewählten Vorlagen haben. Weitere Informationen zu diesem Zugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Zugriff auf Vorlagen gewähren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Freigeben einer oder mehrerer Vorlagen</td> 
      <td> <p>Wählen Sie mindestens eine Vorlage aus, klicken Sie auf das Symbol Freigeben <img src="assets/share-icon.png"> dann auf eine der folgenden Optionen im Dropdown-Menü:</p> 
       <ul> 
        <li> <p><strong>Vorlage</strong>: Fügen Sie im <strong> „Zugriff auf </strong>" Namen hinzu, um anzugeben, wer Zugriff auf die Vorlage selbst haben möchte.</p> <p>Weitere Informationen finden Sie im Abschnitt <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md#share" class="MCXref xref">Freigeben einer Vorlage</a> im Artikel <a href="../../../manage-work/projects/create-and-manage-templates/share-project-template.md" class="MCXref xref">Freigeben von Projektvorlagen</a>.</p> </li> 
        <li><strong>Projekt</strong> <strong>: Fügen Sie im </strong> „Projektzugriff“ Namen hinzu, um anzugeben, wem Sie Zugriff auf die aus der Vorlage erstellten Projekte gewähren möchten</li> 
       </ul> <p>Das Symbol Freigeben ist nur verfügbar, wenn Sie Freigabezugriff auf alle ausgewählten Vorlagen haben. Weitere Informationen zu diesem Zugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md" class="MCXref xref">Zugriff auf Vorlagen gewähren</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Liste der Vorlagen exportieren</td> 
      <td>Klicken <strong> auf </strong>Exportieren<img src="assets/export.png"> und wählen Sie dann das Dateiformat für die exportierte Liste aus.</td> 
     </tr> 
    </tbody> 
   </table>

## So werden Voreinstellungen auf Vorlagen und Vorlagenaufgaben angewendet {#how-preferences-apply-to-templates-and-template-tasks}

Wenn Sie eine Projektvorlage erstellen, werden die in den folgenden Tabellen aufgelisteten Einstellungen automatisch durch eine entsprechende Projekt- oder Aufgabenvoreinstellung konfiguriert.

>[!NOTE]
>
>Die Voreinstellung eines Projekts oder einer Aufgabe auf Gruppenebene bzw. Systemebene wirkt sich auf eine Projektvorlage aus, je nachdem, ob Sie die Vorlage zum Zeitpunkt ihrer Erstellung einer Gruppe zugeordnet haben.
>
>Wenn Sie sie mit einer Gruppe verknüpft haben, wird die Einstellung auf Gruppenebene wirksam. Dies geschieht in den folgenden Szenarien:
>
>* Sie erstellen die Vorlage aus dem Bereich Gruppen , wie in diesem Artikel erläutert
>* Beim Erstellen der Vorlage mithilfe einer Kickstart-Datei legen Sie eine Gruppe fest
>* Beim Erstellen der Vorlage mit der API geben Sie eine Gruppe an
>
>Wenn Sie die neue Vorlage nicht mit einer Gruppe verknüpft haben, wird die Voreinstellung auf Systemebene wirksam. Dies tritt in den folgenden Szenarien auf. (Wenn Sie der Vorlage oder Vorlagenaufgabe später eine Gruppe zuweisen, wirken sich die Einstellungen der Gruppe nicht auf sie aus.)
>
>* Die Vorlage wird im Bereich Vorlagen erstellt
>* Beim Erstellen der Vorlage mit einer Kickstart-Datei geben Sie keine Gruppe an
>* Beim Erstellen der Vorlage mit der API geben Sie keine Gruppe an
>

* [Projektvorlageneinstellungen werden durch Projekt- und Aufgabenvoreinstellungen konfiguriert](#project-template-settings-configured-by-project-and-task-preferences)
* [Einstellungen der Vorlagenaufgabe nach Aufgabenvoreinstellungen konfiguriert](#template-task-settings-configured-by-task-preferences)

### Einstellungen für Projektvorlagen, die durch Projekt- und Aufgabenvoreinstellungen konfiguriert sind {#project-template-settings-configured-by-project-and-task-preferences}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Performance-Index-Methode</p> </td> 
   <td> <p>Wird von der Gruppenprojektvoreinstellung „Leistungsindexmethode“ konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder dieselbe Projektvoreinstellung auf Systemebene, wenn nicht.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bedingungstyp</p> </td> 
   <td> <p>Wird über die Voreinstellung des Projekts auf Gruppenebene konfiguriert „Die Projektbedingung wird automatisch anhand des Fortschrittsstatus festgelegt“, wenn die neue Vorlage mit einer Gruppe verknüpft wird, oder dieselbe Voreinstellung des Projekts auf Systemebene, wenn dies nicht der Fall ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zeitplan ab</p> </td> 
   <td> <p>Wird durch die Voreinstellung „Zeitplan ab“ auf Gruppenebene konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder dieselbe Voreinstellung auf Systemebene, wenn dies nicht der Fall ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Benutzer-Ausfallzeit</p> </td> 
   <td> <p>Wird über die Voreinstellung „Benutzer-Ausfallzeit“ auf Gruppenebene konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder über dieselbe Voreinstellung auf Systemebene, wenn dies nicht der Fall ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Art der Aktualisierung</p> </td> 
   <td> <p>Konfiguriert durch die Voreinstellung des Projekts auf Gruppenebene „Projektzeitleisten werden automatisch neu berechnet“, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder dieselbe Voreinstellung des Projekts auf Systemebene, wenn dies nicht der Fall ist.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Zugriff auf Abschnittseinstellungen</p> </td> 
   <td> <p>Wird durch die Voreinstellungen für Aufgaben auf Gruppenebene im Abschnitt „Zugriff“ konfiguriert, wenn Sie die neue Vorlage mit einer Gruppe verknüpfen, oder durch die Voreinstellung für Projekte auf Systemebene, wenn dies nicht der Fall ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

Informationen zu den in dieser Tabelle aufgeführten Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Informationen zu den Aufgaben- und Problemvoreinstellungen finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!NOTE]
>
>* Wenn Sie die Gruppe ändern, die einer vorhandenen Projektvorlage zugeordnet ist, bleiben die Vorlageneinstellungen unverändert.
>* Wenn Sie eine vorhandene Vorlagenaufgabe in eine andere Vorlage verschieben, bleiben die folgenden Einstellungen in der Vorlagenaufgabe unverändert, unabhängig von der mit der neuen Vorlage verknüpften Gruppe:>
>   * Dauertyp
>   * Umsatztyp
>   * Kostenart
>
>  Die Vorlagenaufgabe ist jedoch von der Einstellung „Wenn jemand einer Aufgabe zugewiesen wird“ in der neuen Vorlage betroffen. Weitere Informationen finden Sie im Abschnitt [Zugriff](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) im Artikel [Projektvorlagen bearbeiten](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).
>
>* Wenn ein(e) Administrator(in) ein Projekt als Vorlage speichert, werden alle Einstellungen für die Vorlage vom Projekt übernommen, einschließlich der Gruppe .
>
>  Wenn ein(e) Administrator(in) eine Aufgabe oder ein Problem mithilfe einer Vorlage in ein Projekt konvertiert, werden alle Einstellungen für die Vorlage durch das bestimmt, was bereits in der Vorlage gespeichert ist.
>

### Einstellungen der Vorlagenaufgabe nach Aufgabenvoreinstellungen konfiguriert {#template-task-settings-configured-by-task-preferences}

Wenn Sie eine Vorlagenaufgabe erstellen, werden einige ihrer Einstellungen automatisch durch eine entsprechende Aufgabenvoreinstellung konfiguriert. Diese Einstellungen sind in der folgenden Tabelle aufgeführt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Dauertyp </p> </td> 
   <td> <p>Wird durch die Voreinstellung für Aufgaben auf Gruppenebene „Dauertyp“ konfiguriert, wenn Sie die Vorlage mit einer Gruppe verknüpfen, oder dieselbe Voreinstellung für Aufgaben und Probleme auf Systemebene, wenn Sie dies nicht tun.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Umsatztyp</p> </td> 
   <td> <p>Wird von der Aufgabenvoreinstellung auf Gruppenebene „Umsatztyp“ konfiguriert, wenn Sie die Vorlage mit einer Gruppe verknüpfen, oder dieselbe Voreinstellung für Aufgaben und Probleme auf Systemebene, wenn Sie dies nicht tun.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Kostenart </p> </td> 
   <td> <p> Wird über die Voreinstellung „Kostentyp“ auf Gruppenebene konfiguriert, wenn Sie die Vorlage mit einer Gruppe verknüpfen, oder dieselbe Voreinstellung für Aufgaben und Probleme auf Systemebene, wenn dies nicht der Fall ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

Informationen zu den in dieser Tabelle aufgeführten Aufgabenvoreinstellungen finden Sie unter [Systemweite Aufgaben- und Problemvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
