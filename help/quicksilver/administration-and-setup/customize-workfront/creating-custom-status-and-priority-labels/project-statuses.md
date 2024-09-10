---
title: Zugriff auf die Liste der Systemprojektstatus
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Benutzer können den Status eines Projekts angeben, damit andere Benutzer die aktuelle Entwicklungsphase des Projekts zu einem bestimmten Zeitpunkt sehen können.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# Zugriff auf die Liste der Systemprojektstatus

Benutzer können den Status eines Projekts angeben, damit andere Benutzer die aktuelle Entwicklungsphase des Projekts zu einem bestimmten Zeitpunkt sehen können.

Workfront verfügt über neun Systemprojektstatus. Sie können den Namen dieser Status ändern, aber nicht löschen.

Sie können auch benutzerdefinierte Projektstatus hinzufügen, um den Anforderungen in Ihrer Organisation zu entsprechen.

Als Workfront-Administrator konfigurieren Sie den Standardstatus für alle neuen Projekte im System. Anweisungen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Projektstatus aufrufen

Als Workfront-Administrator können Sie auf die Liste der Projektstatus auf Systemebene zugreifen.

Informationen zum Bearbeiten eines Systemstatus und zum Erstellen benutzerdefinierter Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

{{step-1-to-setup}}

1. Klicken Sie auf **Projekteinstellungen** > **Status**.

1. Klicken Sie auf die Registerkarte **Projekt** .

   Die in Workfront verfügbaren Projektstatus werden auf dieser Registerkarte aufgelistet.

   ![](assets/project-status.png)

   Weitere Informationen zu den einzelnen integrierten Systemprojektstatus finden Sie unter [Übersicht über den Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Erstellen benutzerdefinierter Projektstatus und Anpassen des Systemstatus

Als Workfront-Administrator können Sie Workfront Systemprojektstatus hinzufügen. Als Gruppeninhaber können Sie einen benutzerspezifischen Status hinzufügen, der für eine Gruppe spezifisch ist. Weitere Informationen zum Erstellen benutzerdefinierter Status oder Bearbeiten der Systemstatus finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Wenn Sie einen benutzerdefinierten Projektstatus erstellen, müssen Sie immer den neuen Status mit einem vorhandenen Systemstatus gleichsetzen. Sie müssen das Verhalten der Systemstatus verstehen, um zu erfahren, welcher Status angemessen ist, um Ihren benutzerspezifischen Status mit anzugleichen. Nachdem Sie den Gleichheitsstatus ausgewählt haben, kann diese Auswahl nicht mehr geändert werden. Weitere Informationen zu den Systemprojektstatus finden Sie unter [Übersicht über den Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
