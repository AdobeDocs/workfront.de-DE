---
title: Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Workfront-Administrator können Sie mit einer Layout-Vorlage festlegen, welche Listenelemente in den Dropdown-Menüs Filter, Ansicht und Gruppierung angezeigt werden. Diese Menüs werden in Workfront über die oben genannten Listen angezeigt, z. B. die Aufgabenliste für ein Projekt.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: e9b61da8-2eca-4d88-969b-ae337e402540
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage

Als Adobe Workfront-Administrator können Sie mit einer Layout-Vorlage festlegen, welche Listenelemente in den Dropdown-Menüs Filter, Ansicht und Gruppierung angezeigt werden. Diese Menüs werden in Workfront über die folgenden Listen angezeigt, z. B. die Aufgabenliste für ein Projekt:

![](assets/filter-view-grouping-layout-templates.png)

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

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
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassen der Listensteuerelemente Filter, Ansicht und Gruppierung:

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie beschrieben in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Klicken Sie auf den Abwärtspfeil. ![](assets/down-arrow-blue.png) under **Anpassen der Ansicht von Benutzern** Klicken Sie auf **Listen** im Dropdown-Menü, das angezeigt wird.

   ![](assets/customize-what-users-see-dropdown-on-pg-adobe-branding.png)

1. Klicken Sie auf den Abwärtspfeil. ![](assets/down-arrow-blue.png) under **Liste zum Anpassen auswählen** und wählen Sie dann den Typ des Workfront-Objekts aus, für das Sie die Listensteuerelemente Filter, Ansicht und Gruppierung anpassen möchten.

   ![](assets/select-a-list-to-customize-menu-on-pg-adobe-branding.png)

   >[!NOTE]
   >
   >Wenn Sie Projekte als Liste auswählen, die angepasst werden soll, und dann Projekte deaktivieren, die ich im Bereich Filter besitze, sehen Benutzer diesen Filter nicht mehr oder können ihn nicht mehr verwenden:
   >
   >* In der Liste der Filter, die beim Klicken auf das Filtersymbol angezeigt werden ![](assets/filter-nwepng.png) über einer Liste:
   >   
   >  ![](assets/disable-filters-projects-im-on-or-own.png)
   >   
   >* In der Kopfzeile des Bereichs &quot;Projekte&quot;:
   >   
   >  ![](assets/disable-filter-pills.png)

1. (Optional) Wenn Sie den Standardfilter, die Standardansicht oder die Gruppierung für die Layoutvorlage ändern möchten, halten Sie den Mauszeiger über den Filter, die Ansicht oder die Gruppierung und klicken Sie auf **Als Standard festlegen**.

   Die Standardeinstellungen, die Sie auswählen, bestimmen, welche Filter-, Anzeigen- und Gruppierungsbenutzer in Workfront in Listen angezeigt werden, wenn ihnen die Layoutvorlage zugewiesen wird. Wenn Sie diese Standardwerte nicht ändern, sehen Benutzer alle Listen wie folgt:

   * **Filter**: Alle
   * **Ansicht**: Standard (sofern zutreffend) Einige Listen haben diese Ansicht nicht.)
   * **Gruppierung**: Nichts

   Sie können die Optionen &quot;Alle&quot;, &quot;Standard&quot;und &quot;Nichts&quot;ausblenden, nachdem Sie verschiedene Standardeinstellungen ausgewählt haben (siehe Schritt 5), diese jedoch nicht gelöscht werden können.

   Sie können jede andere als Standard verwendete Option löschen, müssen jedoch zuerst eine andere Standardeinstellung auswählen.

   Informationen zum Löschen von Filtern, Ansichten und Gruppierungen finden Sie unter [Standardfilter, Ansichten und Gruppierungen erstellen, bearbeiten und freigeben](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-and-share-default-fvgs.md).

1. Blenden Sie Listensteuerelemente wie folgt aus und fügen Sie sie hinzu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ausblenden von Listensteuerelementen</td> 
      <td> <p>Deaktivieren oder aktivieren Sie das Kontrollkästchen neben dem Listensteuerelement, das Sie ein- oder ausblenden möchten.</p> <p>Wenn ein Kontrollkästchen abgeblendet ist, können Sie dieses Listensteuerelement nicht ausblenden. Der Standard <img src="assets/default-pill.png"> -Einstellung für jedes Listensteuerelement ist abgeblendet, da Sie die derzeit als Standard konfigurierte Einstellung nicht ausblenden können.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefiniertes Listensteuerelement hinzufügen</td> 
      <td> <p> 
        <ol> 
         <li value="1"> Klicken <strong>Filter hinzufügen</strong>, <strong>Ansicht hinzufügen</strong>oder <strong>Gruppierung hinzufügen</strong> unten in der Liste "Filter", "Ansicht"oder "Gruppierung". Geben Sie in das daraufhin angezeigte Feld den Namen eines vorhandenen benutzerdefinierten Listenelements ein, das zuvor für Ihr Unternehmen erstellt wurde. Klicken Sie dann auf den Namen, wenn dieser angezeigt wird.</li> 
         <li value="2"> Wenn das neue benutzerdefinierte Listensteuerelement als Standardfilter, Ansicht oder Gruppierung für die Layoutvorlage festgelegt werden soll, klicken Sie auf <strong>Als Standard festlegen</strong>. </li> 
         <li value="3"> <p>Klicken <strong>Hinzufügen</strong> wenn Sie fertig sind.</p> <p><b>NOTIZ</b>: <p>Benutzer können benutzerdefinierte Listensteuerelemente zu ihren eigenen Listen hinzufügen. Wenn Sie benutzerdefinierte Listensteuerelemente in einer Layoutvorlage hinzufügen, werden Ihre Listensteuerelemente hinzugefügt und sie werden an den unteren Rand des Bedienfelds verschoben. Ihre ersetzen ihre nicht.</p> <p>Dies gilt auch, wenn Sie den Benutzer einer neuen Layoutvorlage zuweisen, die über benutzerdefinierte Listensteuerelemente verfügt. </p> <p>Informationen zum Anpassen von Listensteuerelementen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md" class="MCXref xref">Filterübersicht in Adobe Workfront</a>, <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Ansichten - Übersicht in Adobe Workfront</a>und <a href="../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md" class="MCXref xref">Gruppierungsübersicht in Adobe Workfront</a>.</p> </p> </li> 
        </ol> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

   >[!TIP]
   >
   >Sie können jederzeit auf Speichern klicken, um den Fortschritt zu speichern, und die Vorlage später weiter ändern.
