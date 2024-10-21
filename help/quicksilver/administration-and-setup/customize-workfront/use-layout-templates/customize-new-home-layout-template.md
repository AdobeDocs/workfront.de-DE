---
title: Anpassen der neuen Startseite mithilfe einer Layoutvorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer sehen, wenn sie die Startseite öffnen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 0a19683e2311b1acc57423f5cb5a7dd141c8b79c
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 1%

---

# Anpassen der Startseite mithilfe einer Layout-Vorlage

Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer sehen, wenn sie die Startseite zum ersten Mal öffnen.

Sie können Folgendes konfigurieren:

* Welche Widgets werden standardmäßig im Arbeitsbereich angezeigt?
* Welche Hintergrundbilder werden ausgewählt?
* Spezifische Widget-Einstellungen, einschließlich der verfügbaren Filter und Gruppen für die Widgets Meine Projekte, My Tasks und My Issues sowie deren Standardeinstellungen

>[!IMPORTANT]
>
>Endbenutzer können ihren Hintergrund ändern und Widgets auf der Seite neu anordnen, nachdem die Layoutvorlage angewendet wurde. Sie können Widgets, die von einem Workfront-Administrator enthalten sind, nicht entfernen.
> <br>
>Administratoren haben die Möglichkeit, neue Widgets für Benutzer hinzuzufügen. Wenn ein Endbenutzer jedoch bereits seine Widget-Reihenfolge oder Hintergrundauswahl angepasst hat, werden diese spezifischen Anpassungen nicht geändert.



Weitere Informationen zur Startseite finden Sie unter [Erste Schritte mit der Startseite](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

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
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Startseite mit einer Layoutvorlage anpassen

So passen Sie die Startseite mithilfe einer Layoutvorlage an:

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.

1. Klicken Sie auf den Abwärtspfeil ![](assets/dropdown-arrow.png) unter **Anpassen, was Benutzer sehen**, und klicken Sie dann auf **Home Workspace**.

1. Klicken Sie auf den Registerkarten rechts entweder auf **Design &amp; Layout** , um Widgets und den Hintergrund auszuwählen und anzuordnen, oder auf **Widget-Einstellungen** , um Einstellungen für einzelne Widgets wie verfügbare Filter und Gruppen zu verwalten.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design und Layout</td> 
      <td>
      <p>Wählen Sie aus, welche Widgets in den Arbeitsbereichen der Benutzer vorhanden sein sollen, geben Sie ihre Position an und wählen Sie einen Hintergrund aus. Beachten Sie, dass Benutzer zwar die ausgewählten Widgets nicht entfernen können, sie sich jedoch frei bewegen und ihre Größe ändern sowie zusätzliche Widgets hinzufügen können.</p>
      <p>Diese Registerkarte funktioniert im Wesentlichen als kleiner Home-Arbeitsbereich. Daher kann sie entsprechend den Schritten angepasst werden, die unter <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Widgets in Home</a> hinzufügen, bearbeiten oder entfernen beschrieben werden. Wählen Sie Widgets aus und ordnen Sie den Arbeitsbereich so an, wie er für Benutzer angezeigt werden soll.</p>
      <p>Um den Hintergrund zu ändern, führen Sie die Schritte unter <b>Hintergrundanpassung</b> in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Erste Schritte mit Startseite</a> aus.</p>
      <p>

>[!NOTE]
>
>Durch das Verschieben oder Ändern der Größe von Widgets in der Layout-Vorlage werden die Startseiten von Benutzern nicht zur Aktualisierung ihres Layouts Trigger. Das Hinzufügen oder Entfernen eines Widgets Trigger jedoch eine Aktualisierung der Benutzerseiten.

</p>
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
      <p>Sobald Sie das Widget ausgewählt haben, das Sie bearbeiten möchten, werden die verfügbaren Optionen auf der rechten Seite angezeigt. Zu diesen Optionen gehören <b>Filter</b>, <b>Spalten</b> und <b>Gruppen</b>. Sie können:</p>
      <ul>
      <li><p><b>Wählen Sie Filter, Spalten oder Gruppen aus, die Benutzern zur Verfügung stehen, und ordnen Sie sie an:</b></p>
      <p>Aktivieren Sie das Kontrollkästchen neben allen Optionen in der Liste, die Benutzer verwenden können sollen. Diese Optionen werden nicht auf das Bedienfeld "Zusammenfassung"erweitert. Sie müssen diesen Bereich auf der Registerkarte "Zusammenfassung"in der Layout-Vorlage konfigurieren. Nicht aktivierte Optionen werden für Benutzer nicht angezeigt. Ziehen Sie Optionen per Drag-and-Drop in die Liste, um eine Reihenfolge festzulegen.</li></p>
      <p>

>[!IMPORTANT]
>
>* Die Optionen Filter, Spalten und Gruppe sind mit den Optionen zur Listenanpassung in der Layout-Vorlage verknüpft. Die hier vorgenommenen Änderungen gelten auch für diese Einstellungen.
>* Benutzer müssen mindestens Zugriff auf Ansichten erstellen haben, damit die Konfiguration der Administrator-Spalte ordnungsgemäß auf ihre Startseiten angewendet werden kann.

</p>
      <li><p><b>Legen Sie einen Standardfilter oder eine Gruppe für das Widget fest:</b></p>
      <p>Bewegen Sie den Mauszeiger über eine Option. Daraufhin wird eine Schaltfläche angezeigt, mit der Sie diese Option als Standard für Benutzer festlegen können. Die aktuelle Standardeinstellung weist rechts ein blaues Standardzeichen auf.</li></p>
      <li><p><b>Fügen Sie einen vorhandenen Filter, eine Spalte oder eine Gruppe zur Liste der verfügbaren Optionen hinzu:</b></p>
      <p>Klicken Sie auf die Schaltfläche mit dem Pluszeichen am unteren Rand jeder Liste, um der Liste eine Option hinzuzufügen. Beachten Sie, dass nur vorhandene Filter, Felder (für Spalten) oder Gruppen auf diese Weise hinzugefügt werden können.</p></li>
      </ul>
      <p>

>[!NOTE]
>
>Wenn Sie einen Standardfilter oder eine Gruppierung für ein bestimmtes Widget mithilfe einer Layoutvorlage festlegen, wird dieser möglicherweise aufgrund bestehender Benutzereinstellungen nicht sofort wirksam. Um den neuen Filter oder die Gruppierung sofort anzuwenden, müssen Sie oder der Benutzer möglicherweise seine Benutzereinstellungen zurücksetzen, indem Sie &quot;/resetUser&quot;an das Ende ihrer URL anhängen.

</p>
  </td> 
  </tr>
  </tbody> 
  </table>

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie unten links auf **Speichern** .

>[!IMPORTANT]
>
>Sie müssen die Startseite aktualisieren, um Anpassungen aus der Layoutvorlage anzuzeigen.
