---
title: Neue Startseite mit einer Layoutvorlage anpassen
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer sehen, wenn sie die neue Startseite öffnen.
author: Nolan
feature: System Setup and Administration
role: Admin
source-git-commit: dad055b0901cfa8114f7f6b13b6f689d70b31205
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 1%

---

# Neue Startseite mit einer Layoutvorlage anpassen

Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer sehen, wenn sie die neue Startseite öffnen.

Sie können Folgendes konfigurieren:

* Welche Widgets werden standardmäßig im Arbeitsbereich und im Seitenlayout angezeigt
* Welche Hintergrundbilder werden ausgewählt?
* Spezifische Widget-Einstellungen, einschließlich der verfügbaren Filter und Gruppen für die Widgets Meine Projekte, My Tasks und My Issues sowie deren Standardeinstellungen

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebenen Vorlagenoptionen für das Administrator-Layout setzen die Anpassungsoptionen einzelner Benutzer außer Kraft.
>
>Wenn Änderungen an einer Layoutvorlage gespeichert werden, wird die neue Startseite für Benutzer dieser Layoutvorlage entsprechend der Layoutvorlage geändert und die vorhandenen Widget-Auswahlen werden an den unteren Rand der Seite verschoben. Widgets, die vom Administrator ausgewählt wurden, können von einem Benutzer neu positioniert und in der Größe angepasst werden. Sie können jedoch nicht entfernt werden.

Weitere Informationen zum neuen Home finden Sie unter [Erste Schritte mit der neuen Startseite](/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md).

Informationen zum Erstellen von Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Gruppenlayoutvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layoutvorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layoutvorlage zu Benutzern finden Sie unter [Benutzer einer Layoutvorlage zuweisen](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsstufe festgelegt hat. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Neue Startseite mit einer Layoutvorlage anpassen

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie beschrieben in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klicken Sie auf den Abwärtspfeil. ![](assets/dropdown-arrow.png) under **Anpassen der Ansicht von Benutzern** Klicken Sie auf **Startseite**.

1. Klicken Sie in den rechts angezeigten Registerkarten auf **Design und Layout** Widgets und den Hintergrund auszuwählen und anzuordnen oder **Widget-Einstellungen** um Einstellungen für einzelne Widgets zu verwalten, wie z. B. verfügbare Filter und Gruppen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design und Layout</td> 
      <td>
      <p>Wählen Sie aus, welche Widgets in den Arbeitsbereichen der Benutzer vorhanden sein sollen, geben Sie ihre Position an und wählen Sie einen Hintergrund aus. Beachten Sie, dass Benutzer zwar die ausgewählten Widgets nicht entfernen können, sie sich jedoch frei bewegen und ihre Größe ändern sowie zusätzliche Widgets hinzufügen können.</p>
      <p>Diese Registerkarte fungiert im Wesentlichen als kleiner neuer Home-Arbeitsbereich. Daher kann sie entsprechend den Schritten angepasst werden, die unter <a href="/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Hinzufügen, Bearbeiten oder Entfernen von Widgets auf der neuen Startseite</a>. Wählen Sie Widgets aus und ordnen Sie den Arbeitsbereich so an, wie er für Benutzer angezeigt werden soll.</p>
      <p>Gehen Sie wie folgt vor, um den Hintergrund zu ändern <b>Hintergrundanpassung</b> in <a href="/help/quicksilver/workfront-basics/using-home/new-home/get-started-with-new-home.md" class="MCXref xref">Erste Schritte mit der neuen Startseite</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Widget-Einstellungen</td> 
      <td>
      <p>Ändern Sie die Einstellungen für einzelne Widgets. Derzeit werden nur drei Widgets unterstützt:</p>
      <ul>
        <li>Meine Projekte</li>
        <li>Meine Aufgaben</li>
        <li>Meine Probleme</li>
      </ul>
      <p>Sobald Sie das Widget ausgewählt haben, das Sie bearbeiten möchten, werden die verfügbaren Optionen auf der rechten Seite angezeigt. Derzeit sind diese Optionen <b>Filter</b> und <b>Gruppen</b>. Sie können:</p>
      <ul>
        <li><b>Wählen Sie aus, welche Filter oder Gruppen Benutzern zur Verfügung stehen sollen:</b><p>Aktivieren Sie das Kontrollkästchen neben allen Optionen in der Liste, die Benutzer verwenden können sollen. Nicht aktivierte Optionen werden für Benutzer nicht angezeigt.</li></p>
        <li><b>Legen Sie einen Standardfilter oder eine Gruppe für das Widget fest:</b><p>Bewegen Sie den Mauszeiger über eine Option. Daraufhin wird eine Schaltfläche angezeigt, mit der Sie diese Option als Standard für Benutzer festlegen können. Die aktuelle Standardeinstellung weist rechts ein blaues Standardzeichen auf.</li></p>
        <li><b>Fügen Sie einen vorhandenen Filter oder eine bestehende Gruppe zur Liste der verfügbaren Optionen hinzu:</b><p>Klicken Sie auf die Schaltfläche mit dem Pluszeichen am unteren Rand jeder Liste, um der Liste eine Option hinzuzufügen. Beachten Sie, dass nur vorhandene Filter oder Gruppen auf diese Weise hinzugefügt werden können.</li></p>
      </ul>
      </td> 
     </tr>
    </tbody> 
   </table>

>[!IMPORTANT]
>
>Wenn Sie einen Standardfilter oder eine Gruppierung für ein bestimmtes Widget mithilfe einer Layoutvorlage festlegen, wird dieser möglicherweise aufgrund bestehender Benutzereinstellungen nicht sofort wirksam. Um den neuen Filter oder die Gruppierung sofort anzuwenden, müssen Sie oder der Benutzer möglicherweise seine Benutzereinstellungen zurücksetzen, indem Sie &quot;/resetUser&quot;an das Ende ihrer URL anhängen.

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern** in der unteren linken Ecke.

