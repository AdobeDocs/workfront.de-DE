---
title: Anpassen der Startseite mithilfe einer Layoutvorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer sehen, wenn sie die Startseite in Adobe Workfront öffnen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b9997e79-a893-49dd-8c90-290399b2d2f7
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '853'
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
> 
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

1. Klicken Sie auf den Registerkarten rechts auf eine der folgenden Optionen:

   * **Design und Layout**: Wählen Sie diese Option aus, um Widgets und den Hintergrund auszuwählen und anzuordnen
   * **Widget-Einstellungen**: Wählen Sie diese Option, um Einstellungen für einzelne Widgets zu verwalten, z. B. verfügbare Filter und Gruppen.

   Die folgende Tabelle enthält Details zu den einzelnen Registerkarten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design und Layout</td> 
      <td>
      <p>Wählen Sie aus, welche Widgets in den Arbeitsbereichen der Benutzer angezeigt werden sollen, geben Sie ihre Position an und wählen Sie einen Hintergrund aus.</p> 
      <p>Beachten Sie, dass Benutzer zwar die ausgewählten Widgets nicht entfernen können, sie sich jedoch frei bewegen und ihre Größe ändern können. Sie können auch weitere Widgets hinzufügen.</p>
      <p>Dieser Tab dient im Wesentlichen als Vorschau des tatsächlichen Home-Arbeitsbereichs, den Benutzer mit dieser Layoutvorlage erleben.</p> 
      <p> Führen Sie einen der folgenden Schritte aus: </p>
      <ul><li>Passen Sie diese Registerkarte entsprechend den Schritten an, die unter "<a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Widgets in Home</a> hinzufügen, bearbeiten oder entfernen"beschrieben sind. </li>
      <li>Wählen Sie Widgets aus und ordnen Sie den Arbeitsbereich so an, wie er für Benutzer angezeigt werden soll.</li>
      <li>Um den Hintergrund zu ändern, führen Sie die Schritte unter <b>Hintergrundanpassung</b> in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Erste Schritte mit Startseite</a> aus.</li></p>
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
      <p>Ändern Sie die Einstellungen für einzelne Widgets.</p> 
      <p>

   >[!NOTE]
   >
   >Diese Optionen werden nicht auf das Bedienfeld &quot;Zusammenfassung&quot;erweitert. Sie müssen diesen Bereich auf der Registerkarte &quot;Zusammenfassung&quot;in der Layout-Vorlage konfigurieren.

   </p>
      <p> Wählen Sie aus den folgenden Widgets aus der Liste links aus:</p>
      <ul>
        <li>Meine Projekte</li>
        <li>Meine Aufgaben</li>
        <li>Meine Probleme</li>
      </ul>
      <p>Nachdem Sie das Widget ausgewählt haben, das Sie bearbeiten möchten, wählen Sie die <b>Filter</b>, <b>Spalten</b> und <b>Gruppen</b> aus, die Sie für die Startseite auf der rechten Seite verfügbar machen möchten.</p>
      <p> Sie können:</p>
      <ul>
      <li><p>Wählen Sie die für Benutzer verfügbaren Filter, Spalten oder Gruppen aus und ordnen Sie sie an, indem Sie das Kontrollkästchen neben den Optionen in der Liste aktivieren. Nicht aktivierte Optionen werden für Benutzer nicht angezeigt.</p></li>
      <li> <p>Ziehen Sie Optionen per Drag-and-Drop in die Liste, um eine Reihenfolge festzulegen.</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* Die Optionen Filter, Spalten und Gruppe sind mit den Optionen zur Listenanpassung in der Layout-Vorlage verknüpft. Die hier vorgenommenen Änderungen gelten auch für diese Einstellungen.
   >* Benutzer müssen mindestens Zugriff auf Ansichten erstellen haben, damit die Konfiguration der Administrator-Spalte ordnungsgemäß auf ihre Startseiten angewendet werden kann.

   </p>
      <li><p>Legen Sie einen Standardfilter oder eine Gruppe für das Widget fest, indem Sie den Mauszeiger über eine Option bewegen und auf <b>Als Standard festlegen</b> klicken. Der aktuelle Standard zeigt rechts ein blaues <b>Standard</b> -Zeichen an.</p></li>
      <li><p>Fügen Sie einen vorhandenen Filter, eine Spalte oder eine Gruppe zur Liste der verfügbaren Optionen hinzu, indem Sie unten in jeder Liste auf die Schaltfläche mit dem Pluszeichen klicken, um dieser Liste eine Option hinzuzufügen. Beachten Sie, dass nur vorhandene Filter, Felder (für Spalten) oder Gruppen auf diese Weise hinzugefügt werden können.</p></li>
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
   >Benutzer müssen ihre Startseite aktualisieren, um die Anpassungen aus der Layoutvorlage anzuzeigen.
