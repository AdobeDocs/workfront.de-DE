---
title: Anpassen der Landingpage mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Workfront-Administrator können Sie mithilfe einer Layout-Vorlage festlegen, welchen Bereich Benutzerinnen und Benutzern bei jeder Anmeldung bei Workfront angezeigt werden soll.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 57a1046a-434a-4453-a101-c5f0a16e079e
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '432'
ht-degree: 5%

---

# Anpassen der Landingpage mithilfe einer Layout-Vorlage

{{preview-fast-release-general}}

Als Adobe Workfront-Administrator können Sie mithilfe einer Layout-Vorlage festlegen, welchen Bereich Benutzerinnen und Benutzer bei jeder Anmeldung bei Workfront sehen sollen.

Benutzer können eine der folgenden Aktionen öffnen:

* Ein ausgewiesenes Workfront-Gebiet
* Ein benutzerdefiniertes Dashboard.

Informationen zum Erstellen von Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layout-Vorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die von Ihnen vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layout-Vorlage an Benutzer finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../use-layout-templates/assign-users-to-layout-template.md).

>[!NOTE]
>
>Wenn Anfragen als Landingpage festgelegt ist, sehen Mitwirkende oder Antragstellende, die der Layout-Vorlage zugewiesen sind, stattdessen die Startseite als Landingpage. Es wird empfohlen, eine andere Landingpage als Anfragen für Layout-Vorlagen für Mitwirkende oder Antragsteller zu wählen.

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
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.</p>
        <p>Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassen der Landingpage

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie im **oberen Navigationsbereich** auf **Landingpage auswählen** und wählen Sie dann den Bereich aus, der Benutzern bei der Anmeldung angezeigt werden soll.

   Wählen Sie aus den folgenden Bereichen aus oder fügen Sie ein benutzerdefiniertes Dashboard hinzu:

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
   >Für die Anzeige der Szenarien, Ziele und Planungsbereiche sind zusätzliche Lizenzen erforderlich.
   >
   >* Informationen zu Workfront-Zielen finden Sie unter [Adobe Workfront-Ziele - Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).
   >
   >* Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter [Szenarioplaner - Übersicht](../../../scenario-planner/scenario-planner-overview.md).
   >
   >* Weitere Informationen zu Workfront Planning finden Sie unter [Adobe Workfront Planning Overview](/help/quicksilver/planning/general/planning-overview.md).

1. <span class="preview">In der Vorschau-Umgebung: Passen Sie die Layout-Vorlage weiter an. Sie können jederzeit auf **Übernehmen** klicken, um Ihren Fortschritt zu speichern.</span>

   <span class="preview">ODER</span>

   <span class="preview">Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern und schließen**.</span>

1. In der Produktionsumgebung: Passen Sie die Layout-Vorlage weiter an.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf **Speichern** klicken, um Ihren Fortschritt zu speichern, und dann später mit dem Ändern der Vorlage fortfahren.
