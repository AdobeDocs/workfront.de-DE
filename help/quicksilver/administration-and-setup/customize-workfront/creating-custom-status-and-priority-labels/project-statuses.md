---
title: Zugriff auf die Liste der Systemprojektstatus
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Benutzer können den Status eines Projekts angeben, damit andere Benutzer den aktuellen Entwicklungsstand des Projekts zu einem bestimmten Zeitpunkt sehen können.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Zugriff auf die Liste der Systemprojektstatus

Benutzer können den Status eines Projekts angeben, damit andere Benutzer den aktuellen Entwicklungsstand des Projekts zu einem bestimmten Zeitpunkt sehen können.

Workfront verfügt über neun Systemprojektstatus. Sie können den Namen dieser Status ändern, sie jedoch nicht löschen.

Sie können auch benutzerdefinierte Projektstatus entsprechend den Anforderungen in Ihrer Organisation hinzufügen.

Als Workfront-Administrator konfigurieren Sie den Standardstatus für alle neuen Projekte im System. Anweisungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

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
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zugriff auf Projektstatus

Als Workfront-Administrator können Sie auf die Liste der Projektstatus auf Systemebene zugreifen.

Informationen zum Bearbeiten eines Systemstatus und zum Erstellen benutzerdefinierter Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

{{step-1-to-setup}}

1. Klicken Sie **Projektvoreinstellungen** > **Status**.

1. Klicken Sie auf **Registerkarte** Projekt“.

   Auf dieser Registerkarte werden die in Workfront verfügbaren Projektstatus aufgeführt.

   ![Projektstatus](assets/project-status.png)

   Einzelheiten zu den einzelnen integrierten Systemprojektstatus finden Sie unter [Übersicht über Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Erstellen benutzerdefinierter Projektstatus und Anpassen der Systemstatus

Als Workfront-Administrator können Sie Workfront Systemprojektstatus hinzufügen. Als Gruppeneigentümer können Sie einen benutzerdefinierten Status hinzufügen, der für eine Gruppe spezifisch ist. Weitere Informationen zum Erstellen benutzerdefinierter Status oder zum Bearbeiten der Systemstatus finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Wenn Sie einen benutzerdefinierten Projektstatus erstellen, müssen Sie den neuen Status immer mit einem vorhandenen Systemstatus gleichsetzen. Sie müssen das Verhalten der Systemstatus verstehen, um herauszufinden, welcher Status für die Gleichsetzung Ihres benutzerdefinierten Status geeignet ist. Nachdem Sie den Status Gleichgestellt ausgewählt haben, kann diese Auswahl nicht mehr geändert werden. Weitere Informationen zum Systemprojektstatus finden Sie unter [Übersicht über den Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
