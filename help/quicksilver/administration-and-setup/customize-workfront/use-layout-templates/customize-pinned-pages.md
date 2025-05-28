---
title: Anpassen von fixierten Seiten mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: In einer Layout-Vorlage können Sie oben in Adobe Workfront die Seiten anheften, für die Benutzerinnen und Benutzer immer verfügbar sein sollen. Dabei kann es sich entweder um Seiten handeln, auf die über das Hauptmenü oder über Dashboards zugegriffen wird.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 55cc75c5-8b8c-48e7-b114-b41fe3d545d8
source-git-commit: 76797ce2afb6a6a929531f02ed3a3b3f75240602
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 4%

---

# Anpassen von fixierten Seiten mithilfe einer Layout-Vorlage

In einer Layout-Vorlage können Sie oben in Adobe Workfront die Seiten anheften, für die Benutzerinnen und Benutzer immer verfügbar sein sollen. Dabei kann es sich entweder um Seiten handeln, auf die über das Hauptmenü ![Hauptmenüsymbol](assets/main-menu-icon.png) oder das Hauptmenü ![Hauptmenüsymbol) zugegriffen ](assets/main-menu-icon.png), falls verfügbar, oder um Dashboards.

Alle Pins, die von Ihren Benutzerinnen und Benutzern eigenständig hinzugefügt wurden, werden rechts neben den Pins angezeigt, die Sie der Layout-Vorlage hinzufügen.

Weitere Informationen zum Anheften von Seiten finden Sie unter [Seiten anheften, um Ihren Arbeitsbereich anzupassen](../../../workfront-basics/the-new-workfront-experience/pin-pages.md).

Weitere Informationen zu Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layout-Vorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die von Ihnen vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layout-Vorlage an Benutzer finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

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
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.
Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Seiten mithilfe einer Layout-Vorlage anheften

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken **unter &quot;** Navigationsbereich“ auf **Neuen Pin hinzufügen**.

1. Führen Sie im angezeigten Dropdown-Menü einen der folgenden Schritte aus:

   * Wählen Sie aus den folgenden Bereichen:

      * Kalender
      * Dashboards
      * Dokumente
      * Ziele
      * Startseite
      * Meine Updates
      * Portfolios
      * Programme
      * Projekte
      * Berichte
      * Anforderungen
      * Ressourcen- zuordnung
      * Szenarios
      * Teams
      * Vorlagen
      * Arbeitszeittabellen
      * Benutzende
      * Blueprints
      * In Planung

     >[!IMPORTANT]
     >
     >Für die Ansicht der Ziele, Szenarien und Planungsbereiche sind zusätzliche Lizenzen erforderlich.
     >
     >* Informationen zu Workfront-Zielen finden Sie unter [Adobe Workfront-Ziele - Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).
     >
     >* Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter [Szenarioplaner - Übersicht](../../../scenario-planner/scenario-planner-overview.md).
     >
     >* Weitere Informationen zu Workfront Planning finden Sie unter [Adobe Workfront Planning Overview](/help/quicksilver/planning/general/planning-overview.md).

   * Klicken Sie **Dashboard hinzufügen**
      * Geben Sie einen beschreibenden Namen in das Feld <!--**Quick link name**-->**Benutzerdefinierter Name** ein
      * Wählen Sie ein Dashboard im <!-- dropdown for existing or canvas dashboard, called "Choose a dashboard" now --> **Dashboard hinzufügen** aus
      * Klicken Sie **Hinzufügen**.

1. Wiederholen Sie diesen Schritt, um alle weiteren Seiten anzuheften.

1. (Optional) Um eine Nadel zu verschieben, bewegen Sie den Mauszeiger über die Nadel und klicken Sie auf das Menüsymbol „Mehr“ ![](assets/more-icon.png) neben dem Namen der Nadel. Klicken Sie dann auf **Nach links** oder **Nach rechts verschieben**, um die Nadel in die ausgewählte Richtung zu verschieben, oder klicken Sie auf **Nach vorne verschieben**, um die Nadel in die ganz linke Position zu verschieben.

1. (Optional) Um eine Nadel umzubenennen, bewegen Sie den Mauszeiger über die Nadel und klicken Sie auf das Menüsymbol ![Mehr](assets/more-icon.png) neben dem Namen der Nadel. Klicken Sie dann auf **Nadel umbenennen**. Geben Sie einen neuen Namen ein und klicken Sie dann auf **Speichern**.

1. (Optional) Um eine Nadel zu löschen, bewegen Sie den Mauszeiger über die Nadel und klicken Sie auf das Menüsymbol ![Mehr](assets/more-icon.png) neben dem Namen der Nadel. Klicken Sie dann auf **Nadel entfernen**.

1. Passen Sie die Layout-Vorlage weiter an.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf **Speichern** klicken, um Ihren Fortschritt zu speichern, und dann später mit dem Ändern der Vorlage fortfahren.
