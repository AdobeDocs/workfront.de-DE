---
title: Zugriff auf die Liste der Systemprojektstatus
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Benutzer können den Status eines Projekts angeben, damit andere Benutzer die aktuelle Entwicklungsphase des Projekts zu einem bestimmten Zeitpunkt sehen können.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1fc91438-1ead-40d2-b0aa-863c1125c2fb
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '392'
ht-degree: 0%

---

# Zugriff auf die Liste der Systemprojektstatus

Benutzer können den Status eines Projekts angeben, damit andere Benutzer die aktuelle Entwicklungsphase des Projekts zu einem bestimmten Zeitpunkt sehen können.

Workfront verfügt über neun Systemprojektstatus. Sie können den Namen dieser Status ändern, aber nicht löschen.

Sie können auch benutzerdefinierte Projektstatus hinzufügen, um den Anforderungen in Ihrer Organisation zu entsprechen.

Als Workfront-Administrator konfigurieren Sie den Standardstatus für alle neuen Projekte im System. Anweisungen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Zugriffsanforderungen

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

## Projektstatus aufrufen

Als Workfront-Administrator können Sie auf die Liste der Projektstatus auf Systemebene zugreifen.

Informationen zum Bearbeiten eines Systemstatus und zum Erstellen benutzerdefinierter Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie auf **Projekteinstellungen** > **Status**.

1. Klicken Sie auf die Registerkarte **Projekt** .

   Die in Workfront verfügbaren Projektstatus werden auf dieser Registerkarte aufgelistet.

   ![](assets/project-status.png)

   Weitere Informationen zu den einzelnen integrierten Systemprojektstatus finden Sie unter [Übersicht über den Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).

## Erstellen benutzerdefinierter Projektstatus und Anpassen des Systemstatus

Als Workfront-Administrator können Sie Workfront Systemprojektstatus hinzufügen. Als Gruppeninhaber können Sie einen benutzerspezifischen Status hinzufügen, der für eine Gruppe spezifisch ist. Weitere Informationen zum Erstellen benutzerdefinierter Status oder Bearbeiten der Systemstatus finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Wenn Sie einen benutzerdefinierten Projektstatus erstellen, müssen Sie immer den neuen Status mit einem vorhandenen Systemstatus gleichsetzen. Sie müssen das Verhalten der Systemstatus verstehen, um zu erfahren, welcher Status angemessen ist, um Ihren benutzerspezifischen Status mit anzugleichen. Nachdem Sie den Gleichheitsstatus ausgewählt haben, kann diese Auswahl nicht mehr geändert werden. Weitere Informationen zu den Systemprojektstatus finden Sie unter [Übersicht über den Systemprojektstatus](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/system-project-statuses.md).
