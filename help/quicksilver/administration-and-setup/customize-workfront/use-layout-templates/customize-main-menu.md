---
title: Hauptmenü mithilfe einer Layoutvorlage anpassen
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Optionen zu konfigurieren, die Benutzern beim Öffnen des Hauptmenüs in Workfront angezeigt werden.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 9c78d8e08e62c86a4e1340644ed76c61ce7f2674
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# Hauptmenü mithilfe einer Layoutvorlage anpassen

Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie eine Layoutvorlage verwenden, um die Optionen zu konfigurieren, die Benutzern beim Öffnen des Hauptmenüs in Workfront angezeigt werden:

![Optionen des Hauptmenüs](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>Die Optionen des Hauptmenüs, die den Benutzern angezeigt werden, hängen vom Lizenztyp und den Einstellungen der jeweiligen Zugriffsstufe ab. Einige Benutzer, die diese Layoutvorlage verwenden werden, sehen möglicherweise nicht alle Optionen, die Sie hier auswählen. Weitere Informationen finden Sie unter [Wie Zugriffsebenen und Berechtigungen zusammenarbeiten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) und [Konfigurierbarer Zugriff auf Funktionen für jeden Objekttyp](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Gruppenlayoutvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Abo</strong></td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz</strong></td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassen des Hauptmenüs

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie beschrieben in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicken **Hauptmenü festlegen** in der Nähe der oberen rechten Ecke.

   Im angezeigten Feld Hauptmenü können Sie die Elemente sehen, die derzeit im Hauptmenü der Vorlage aktiv sind, sowie die Elemente, die hinzugefügt werden können. Im Folgenden finden Sie alle möglichen Elemente, die hinzugefügt werden können:

   * Startseite

      >[!TIP]
      >
      >Standardmäßig wird &quot;Home&quot;als &quot;Meine Updates für Benutzer von Review-Lizenzen&quot;angezeigt, es sei denn, ihnen ist eine Layoutvorlage zugeordnet, die den Bereich Meine Updates im Hauptmenü enthält.

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
      >Der Szenario-Planer ist nur im neuen Adobe Workfront-Erlebnis verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Übersicht über den Szenario-Planer](../../../scenario-planner/scenario-planner-overview.md).

   * Teams
   * Benutzer

      >[!NOTE]
      >
      >Nur Benutzer mit einer Planungslizenz können Benutzer sehen ![](assets/users-icon-in-main-menu.png) im Hauptmenü.

   * Anforde- rungen
   * Arbeitszeittabellen
   * Dokumente
   * Vorlagen
   * Analytik
   * Proofing
   * Ziele

      >[!NOTE]
      >
      >Dies erfordert eine zusätzliche Lizenz. Weitere Informationen zu Workfront-Zielen finden Sie unter [Übersicht über Adobe Workfront-Ziele](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Meine Updates
   * Pinnwände
   * Blueprints

1. Führen Sie einen der folgenden Schritte aus:

   * Ausblenden ![](assets/remove-icon---x-in-circle.png) **Aktive Elemente** dass Sie
   * Anzeigen ![](assets/add-icon-plus-in-circle.png) **Verfügbare Elemente** die Sie im Hauptmenü anzeigen möchten.
   * Ziehen ![](assets/move-icon---dots.png) **Aktive Elemente** , um die Anzeigereihenfolge im Hauptmenü zu ändern.

1. Klicken **Fertig**.

   Sie können auch auf **Abbrechen** Sie können Ihre Änderungen jederzeit verwerfen.

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf Speichern klicken, um den Fortschritt zu speichern, und die Vorlage später weiter ändern.

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
