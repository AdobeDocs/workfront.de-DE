---
title: Anpassen der Startseite mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzenden angezeigt wird, wenn sie die Startseite in Adobe Workfront öffnen.
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

Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzenden angezeigt wird, wenn sie die Startseite zum ersten Mal öffnen.

Sie können Folgendes konfigurieren:

* Welche Widgets standardmäßig im Arbeitsbereich angezeigt werden
* Welcher Hintergrund ausgewählt ist
* Spezifische Widget-Einstellungen, einschließlich der verfügbaren Filter und Gruppen für die Widgets „Meine Projekte“, „Meine Aufgaben“ und „Meine Probleme“ sowie deren Standardeinstellungen

>[!IMPORTANT]
>
>Endbenutzer können ihre Hintergrund-Widgets ändern und auf der Seite neu anordnen, nachdem die Layout-Vorlage angewendet wurde. Sie können keine von einem Workfront-Administrator eingeschlossenen Widgets entfernen.
> 
>Administratoren haben die Möglichkeit, neue Widgets für Benutzer hinzuzufügen. Wenn ein Endbenutzer jedoch bereits die Widget-Reihenfolge oder die Hintergrundauswahl angepasst hat, werden diese spezifischen Anpassungen nicht geändert.

Weitere Informationen zur Startseite finden Sie unter [Erste Schritte mit der Startseite](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

Informationen zum Erstellen von Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layout-Vorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die von Ihnen vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layout-Vorlage an Benutzer finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.
Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassen der Startseite mithilfe einer Layout-Vorlage

So passen Sie die Startseite mithilfe einer Layout-Vorlage an:

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.

1. Klicken Sie auf den Abwärtspfeil ![](assets/dropdown-arrow.png) unter **Anpassen, was Benutzer sehen** und klicken Sie dann auf **Startseiten-Workspace**.

1. Klicken Sie auf der rechten Seite auf eine der folgenden Registerkarten:

   * **Design und Layout**: Auswählen, um Widgets und den Hintergrund auszuwählen und anzuordnen
   * **Widget-Einstellungen**: Wählen Sie diese Option aus, um Einstellungen für einzelne Widgets zu verwalten, z. B. für verfügbare Filter und Gruppen.

   Die folgende Tabelle enthält Details zu den einzelnen Registerkarten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Design und Layout</td> 
      <td>
      <p>Wählen Sie aus, welche Widgets in den Arbeitsbereichen der Benutzer angezeigt werden, sowie deren Position und wählen Sie einen Hintergrund aus.</p> 
      <p>Beachten Sie, dass Benutzende die ausgewählten Widgets zwar nicht entfernen können, sie jedoch frei verschieben und ihre Größe ändern können. Sie können auch weitere Widgets hinzufügen.</p>
      <p>Diese Registerkarte dient im Wesentlichen als Vorschau des tatsächlichen Startseiten-Arbeitsbereichs, den Benutzer mit dieser Layout-Vorlage erleben.</p> 
      <p> Führen Sie einen der folgenden Schritte aus: </p>
      <ul><li>Passen Sie diese Registerkarte entsprechend den Schritten an, die unter <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md" class="MCXref xref">Hinzufügen, Bearbeiten oder Entfernen von Widgets auf der Startseite“ beschrieben </a>. </li>
      <li>Wählen Sie Widgets aus und ordnen Sie den Arbeitsbereich so an, wie er den Benutzern angezeigt werden soll.</li>
      <li>Um den Hintergrund zu ändern, führen Sie die Schritte unter <b>Hintergrundanpassung</b> in <a href="/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md" class="MCXref xref">Erste Schritte mit der Startseite</a> aus.</li></p>
      <p>

   >[!NOTE]
   >
   >Nur durch Verschieben oder Ändern der Größe von Widgets in der Layout-Vorlage werden die Startseiten von Benutzenden nicht dazu Trigger, ihr Layout zu aktualisieren. Durch Hinzufügen oder Entfernen eines Widgets wird jedoch ein Trigger zu Benutzerseiten-Updates erstellt.

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
   >Diese Optionen erstrecken sich nicht auf das Bedienfeld Zusammenfassung . Sie müssen diesen Bereich auf der Registerkarte Zusammenfassung in der Layout-Vorlage konfigurieren.

   </p>
      <p> Wählen Sie aus der Liste links folgende Widgets aus:</p>
      <ul>
        <li>Meine Projekte</li>
        <li>Meine Aufgaben</li>
        <li>Meine Probleme</li>
      </ul>
      <p>Nachdem Sie das Widget ausgewählt haben, das Sie bearbeiten möchten, wählen Sie die <b>Filter</b>, <b>Spalten</b> und <b>Gruppen</b> aus, die Sie für die Startseite auf der rechten Seite verfügbar machen möchten.</p>
      <p> Sie können:</p>
      <ul>
      <li><p>Wählen Sie die für Benutzer verfügbaren Filter, Spalten oder Gruppen aus und ordnen Sie sie an, indem Sie das Kontrollkästchen neben den Optionen in der Liste aktivieren. Deaktivierte Optionen werden für Benutzende nicht angezeigt.</p></li>
      <li> <p>Optionen per Drag-and-Drop in die Liste ziehen, um eine Reihenfolge festzulegen.</p></li>
      <p>

   >[!IMPORTANT]
   >
   >* Die Filter-, Spalten- und Gruppenoptionen sind mit den Listenanpassungsoptionen in der Layout-Vorlage verknüpft. Hier vorgenommene Änderungen gelten auch für diese Einstellungen.
   >* Benutzer müssen mindestens Zugriff auf „Erstellen“ für Ansichten haben, damit die Spaltenkonfiguration des Administrators ordnungsgemäß auf ihre Startseiten angewendet werden kann.

   </p>
      <li><p>Legen Sie einen Standardfilter oder eine Standardgruppe für das Widget fest, indem Sie den Mauszeiger über eine Option bewegen und auf <b>Als Standard festlegen</b> klicken. Die aktuelle Standardeinstellung zeigt rechts neben der <b> ein blaues </b>.</p></li>
      <li><p>Fügen Sie einen vorhandenen Filter, eine vorhandene Spalte oder eine vorhandene Gruppe zur Liste der verfügbaren Optionen hinzu, indem Sie auf die Schaltfläche mit dem Pluszeichen unten in jeder Liste klicken, um dieser Liste eine Option hinzuzufügen. Beachten Sie, dass nur vorhandene Filter, Felder (für Spalten) oder Gruppen auf diese Weise hinzugefügt werden können.</p></li>
      </ul>
      <p>

   >[!NOTE]
   >
   >Wenn Sie einen Standardfilter oder eine Standardgruppierung für ein bestimmtes Widget mithilfe einer Layout-Vorlage festlegen, wird dieser möglicherweise aufgrund vorhandener Benutzereinstellungen nicht sofort wirksam. Um den neuen Filter oder die neue Gruppierung sofort anzuwenden, müssen Sie bzw. die Benutzenden möglicherweise ihre Benutzereinstellungen zurücksetzen, indem Sie &quot;/resetUser“ an das Ende der URL anhängen.

   </p>
      </td> 
      </tr>
      </tbody> 
      </table>

1. Passen Sie die Layout-Vorlage weiter an.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken **unten** links auf „Speichern“.

   >[!IMPORTANT]
   >
   >Benutzer müssen ihre Startseite aktualisieren, um Anpassungen aus der Layout-Vorlage sehen zu können.
