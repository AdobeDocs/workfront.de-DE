---
title: Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Optionen zu konfigurieren, die Benutzern beim Öffnen des Hauptmenüs in Workfront angezeigt werden.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 3%

---

# Hauptmenü mithilfe einer Layoutvorlage anpassen

<!--Audited: 01/2024-->

Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Optionen zu konfigurieren, die Benutzern beim Öffnen des Hauptmenüs in Workfront angezeigt werden.

![Hauptmenüoptionen](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>Die Optionen des Hauptmenüs, die den Benutzern angezeigt werden, hängen vom Lizenztyp und den Einstellungen der jeweiligen Zugriffsstufe ab. Einige Benutzer, die diese Layoutvorlage verwenden werden, sehen möglicherweise nicht alle Optionen, die Sie hier auswählen. Weitere Informationen finden Sie unter [Wie Zugriffsebenen und Berechtigungen zusammenarbeiten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) und [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>Möglicherweise werden im Hauptmenü verschiedene Optionen angezeigt, wenn Ihr Unternehmen mit dem einheitlichen Adobe Workfront-Erlebnis integriert wurde. Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

Informationen zum Erstellen von Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Layoutvorlagen für Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layoutvorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layoutvorlage zu Benutzern finden Sie unter [Zuweisen von Benutzern zu einer Layoutvorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Abo</strong></td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td><p>Aktuell: Plan</p>
   Oder
   <p>Neu: Standard</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfiguration der Zugriffsebene</strong></td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.</p>
    <p>Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> 
     </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hauptmenü anpassen

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie oben rechts in der Vorlage auf **Hauptmenü festlegen** .

   Das Feld Hauptmenü wird geöffnet. Es werden die Bereiche angezeigt, die derzeit im Hauptmenü der Vorlage angezeigt werden, sowie die Elemente, die hinzugefügt werden können. Im Folgenden finden Sie alle möglichen Elemente, die Sie hinzufügen können:
   * Startseite

     >[!TIP]
     >
     >Standardmäßig zeigt das Startseiten-Symbol im Hauptmenü den Bereich Meine Updates für Benutzer von Review-Lizenzierungen (im aktuellen Lizenzplan) an, es sei denn, ihnen ist eine Layoutvorlage zugeordnet, die neben dem Startbereich auch den Bereich Meine Updates im Hauptmenü enthält.

   * Portfolios
   * Programme
   * Projekte
   * Berichte
   * Dashboards
   * Kalender
   * Ressourcen- zuordnung
   * Szenarios

     >[!NOTE]
     >
     >Für den Szenario-Planer ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Überblick über den Szenario-Planer](../../../scenario-planner/scenario-planner-overview.md).

   * Teams
   * Benutzende

     >[!NOTE]
     >
     >Nur Benutzer mit einer Planungslizenz (im aktuellen Lizenzmodell) oder Benutzer mit einer Standardlizenz (im neuen Lizenzmodell) können den Bereich Benutzer ![](assets/users-icon-in-main-menu.png) im Hauptmenü sehen.

   * Anforde- rungen
   * Arbeitszeit- tabellen
   * Dokumente
   * Vorlagen
   * Analytik
   * Proofing
   * Ziele

     >[!NOTE]
     >
     >Ziele erfordern eine zusätzliche Lizenz. Weitere Informationen zu Workfront-Zielen finden Sie unter [Übersicht über Adobe Workfront-Ziele](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Meine Updates
   * Pinnwände
   * Blueprints
   * In Planung

     >[!NOTE]
     >
     >Für die Planung ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zur Workfront-Planung finden Sie unter [Übersicht über die Adobe Workfront-Planung](/help/quicksilver/planning/general/planning-overview.md)

1. Führen Sie einen der folgenden Schritte aus:

   * Ausblenden von ![](assets/remove-icon---x-in-circle.png) **aktiven Elementen**, die Sie nicht anzeigen möchten
   * Anzeigen von ![](assets/add-icon-plus-in-circle.png) **Verfügbaren Elementen** , die Sie im Hauptmenü anzeigen möchten.
   * Ziehen Sie ![](assets/move-icon---dots.png) **Aktive Elemente** , um ihre Anzeigereihenfolge im Hauptmenü zu ändern.

1. Klicken Sie auf **Fertig**.

   Sie können auch jederzeit auf **Abbrechen** klicken, wenn Sie Ihre Änderungen verwerfen möchten.

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit dem Anpassen fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf Speichern klicken, um den Fortschritt zu speichern, und die Vorlage später weiter ändern.

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
