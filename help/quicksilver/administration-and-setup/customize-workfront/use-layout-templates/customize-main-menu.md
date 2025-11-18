---
title: Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layout-Vorlage verwenden, um die Optionen zu konfigurieren, die Benutzende sehen, wenn sie das Hauptmenü in Workfront öffnen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 6%

---

# Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage

{{preview-fast-release-general}}

<!--Audited: 01/2024-->

Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layout-Vorlage verwenden, um die Optionen zu konfigurieren, die Benutzende sehen, wenn sie das Hauptmenü in Workfront öffnen.

>[!NOTE]
>
>Die Optionen im Hauptmenü, die den Benutzern angezeigt werden, hängen von ihrem Lizenztyp und davon ab, welche Einstellungen in ihrer Zugriffsebene konfiguriert sind. Einige Benutzer, die diese Layoutvorlage verwenden werden, sehen möglicherweise nicht alle hier ausgewählten Optionen. Weitere Informationen finden Sie unter [Wie Zugriffsebenen und Berechtigungen zusammenarbeiten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) und [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>Möglicherweise werden im Hauptmenü unterschiedliche Optionen angezeigt, wenn Ihr Unternehmen das einheitliche Adobe Workfront-Erlebnis erhalten hat. Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

Informationen zum Erstellen von Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layout-Vorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die von Ihnen vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layout-Vorlage an Benutzer finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p>
       <p>Das Hinzufügen benutzerdefinierter Programme zum Hauptmenü ist nur für Organisationen verfügbar, die für Adobe App Builder lizenziert sind.</p></td> 
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

## Anpassen des Hauptmenü

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken **oben rechts** der Vorlage auf „Hauptmenü festlegen“.

   Das Feld Hauptmenü wird geöffnet. Dort werden die Bereiche angezeigt, die derzeit im Hauptmenü der Vorlage angezeigt werden, sowie die Elemente, die hinzugefügt werden können. Im Folgenden finden Sie alle möglichen Elemente, die Sie hinzufügen können:
   * Startseite

     >[!TIP]
     >
     >Standardmäßig wird das Startseiten -Symbol im Hauptmenü den Bereich Meine Aktualisierungen für Benutzer mit Überprüfungslizenz (im aktuellen Lizenzplan) anzeigen, es sei denn, ihnen ist eine Layoutvorlage mit ihrem Profil zugeordnet, die im Hauptmenü neben dem Bereich Startseite auch den Bereich Meine Aktualisierungen enthält.

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
     >Für den Szenario-Planer ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter [Szenarioplaner - Übersicht](../../../scenario-planner/scenario-planner-overview.md).

   * Teams
   * Benutzende

     >[!NOTE]
     >
     >Nur Benutzer mit einer Plan -Lizenz (im aktuellen Lizenzmodell) oder Benutzer mit einer Standard -Lizenz (im neuen Lizenzmodell) können den Bereich Benutzer ![Benutzersymbol](assets/users-icon-in-main-menu.png) im Hauptmenü sehen.

   * Anforderungen
   * Arbeitszeittabellen
   * Dokumente
   * Vorlagen
   * Ziele

     >[!NOTE]
     >
     >Für Ziele ist eine zusätzliche Lizenz erforderlich. Informationen zu Workfront-Zielen finden Sie unter [Adobe Workfront-Ziele - Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Meine Updates
   * Pinnwände
   * Blueprints
   * In Planung

     >[!NOTE]
     >
     >Für die Planung ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zur Workfront-Planung finden Sie [Erste Schritte mit Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

   * Benutzerdefinierte Anwendung

     >[!NOTE]
     >
     > Benutzerdefinierte Programme müssen separat erstellt werden, bevor sie als Hauptmenüoptionen verfügbar werden. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Programms für Workfront mit Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

1. Führen Sie einen der folgenden Schritte aus:

   * Ausblenden ![Symbol ausblenden](assets/remove-icon---x-in-circle.png) **Aktive Elemente** die nicht angezeigt werden sollen
   * &quot;![-Symbol](assets/add-icon-plus-in-circle.png) **Verfügbare Elemente** anzeigen, die nicht im Hauptmenü angezeigt werden sollen.
   * Ziehen Sie ![Symbol ziehen](assets/move-icon---dots.png) **Aktive Elemente**, um ihre Anzeigereihenfolge im Hauptmenü zu ändern.

1. Klicken Sie auf **Fertig**.

   Sie können auch jederzeit **Abbrechen** klicken, wenn Sie Ihre Änderungen verwerfen möchten.

1. <span class="preview">In der Vorschau-Umgebung: Passen Sie die Layout-Vorlage weiter an. Sie können jederzeit auf **Übernehmen** klicken, um Ihren Fortschritt zu speichern.</span>

   <span class="preview">ODER</span>

   <span class="preview">Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern und schließen**.</span>

1. In der Produktionsumgebung: Passen Sie die Layout-Vorlage weiter an.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf **Speichern** klicken, um Ihren Fortschritt zu speichern, und dann später mit dem Ändern der Vorlage fortfahren.

Weitere Informationen zu Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
