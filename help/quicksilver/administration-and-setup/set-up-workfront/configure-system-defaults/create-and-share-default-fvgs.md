---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Standardfilter, Ansichten und Gruppierungen erstellen, bearbeiten und freigeben
description: Sie können Standardfilter, Ansichten und Gruppierungen erstellen und diese dann Benutzern in Ihrer Organisation zur Verfügung stellen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 75c4abfa9aebf1d07a851486391291cddc94f1a9
workflow-type: tm+mt
source-wordcount: '822'
ht-degree: 0%

---

# Standardfilter, Ansichten und Gruppierungen erstellen, bearbeiten und freigeben

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Sie können Standardfilter, Ansichten und Gruppierungen erstellen und diese dann Benutzern in Ihrer Organisation zur Verfügung stellen.

Wenn Sie Standardfilter, Ansichten und Gruppierungen erstellen, wie in diesem Artikel beschrieben, können Benutzer, für die Sie sie freigeben, diese beim Anzeigen ihrer Listen nutzen. Benutzer können ihre eigenen Filter, Ansichten und Gruppierungen basierend auf den von Ihnen erstellten erstellen, diese können jedoch nicht direkt ändern.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Standardfilter, Ansichten oder Gruppierungen erstellen

{{step-1-to-setup}}

1. Führen Sie je nachdem, ob Sie einen Filter, eine Ansicht oder eine Gruppierung erstellen oder bearbeiten, einen der folgenden Schritte aus:

   * Klicken **[!UICONTROL Schnittstelle]** > **[!UICONTROL Filter]**.

   * Klicken **[!UICONTROL Schnittstelle] >** **[!UICONTROL Ansichten]**.

   * Klicken **[!UICONTROL Schnittstelle]** > **[!UICONTROL Gruppierungen]**.

1. Wenn Sie einen Filter, eine Ansicht oder eine Gruppierung erstellen, klicken Sie auf **[!UICONTROL Filter hinzufügen]**, **[!UICONTROL Ansicht hinzufügen]** oder **[!UICONTROL Gruppierung hinzufügen]** und wählen Sie dann den Objekttyp aus, mit dem Sie den neuen Filter, die neue Ansicht oder die neue Gruppierung verbinden möchten.

   Oder

   Wenn Sie einen vorhandenen Filter, eine vorhandene Ansicht oder eine Gruppierung bearbeiten, wählen Sie ihn aus und klicken Sie auf die Schaltfläche **[!UICONTROL Bearbeiten]** icon ![Symbol Bearbeiten](assets/edit-icon.png).

1. Konfigurieren Sie den Filter, die Ansicht oder die Gruppierung.

   Informationen zu den verfügbaren Optionen finden Sie in einem der folgenden Artikel:

   * [Filterübersicht in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Ansichten - Übersicht in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Gruppierungsübersicht in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Klicken **[!UICONTROL Speichern]** in der Nähe der unteren linken Ecke.

Sie können den Filter, die Ansicht oder die Gruppierung Benutzern in Ihrem System zur Verfügung stellen. Weitere Informationen zum Freigeben von Filtern, Ansichten oder Gruppierungen für andere Benutzer finden Sie im Abschnitt [Bereitstellen von Filtern, Ansichten oder Gruppierungen für Benutzer](#make-filters-views-or-groupings-available-to-users) in diesem Artikel.


## Anzeigen oder Ausblenden von Filtern, Ansichten oder Gruppierungen, die in der Layout-Vorlage verfügbar sind

Sie können Filter, Ansichten oder Gruppierungen in der Layout-Vorlage ein- oder ausblenden. Sichtbare Filter sind systemweit für alle Benutzer verfügbar. Sie können eine Layout-Vorlage verwenden, um sichtbare Filter für bestimmte Benutzer oder Gruppen auszublenden.

>[!NOTE]
>
>Wenn ein Benutzer einen Filter, eine Ansicht oder eine Gruppierung aktiv verwendet und dann von einem Administrator deaktiviert wird, hat der Benutzer weiterhin Zugriff, bis er einen neuen Filter, eine neue Ansicht oder eine neue Gruppierung auswählt. Nachdem sie einen neuen Filter, eine neue Ansicht oder eine neue Gruppierung ausgewählt haben, können sie nicht mehr zum ausgeblendeten Filter, zur ausgeblendeten Ansicht oder zur ausgeblendeten Gruppierung zurückkehren.

So blenden Sie in der Layout-Vorlage verfügbare Filter, Ansichten oder Gruppierungen ein oder aus:

1. Klicken **[!UICONTROL Schnittstelle]** und klicken Sie dann auf einen der folgenden Punkte: **[!UICONTROL Filter]**, **[!UICONTROL Ansichten]** oder **[!UICONTROL Gruppierungen]**.

1. (Bedingt) Wählen Sie den Filter, die Ansicht oder die Gruppierung aus, die Sie Benutzern zur Verfügung stellen möchten, und klicken Sie auf **[!UICONTROL Systemweit aktivieren]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Wenn Sie den Filter, die Ansicht oder die Gruppierung für die meisten Benutzer verfügbar halten, ihn aber vor anderen ausblenden möchten, können Sie die Layout-Vorlage verwenden. Weitere Informationen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Bedingt) Wählen Sie den Filter, die Ansicht oder die Gruppierung aus, die Sie für Benutzer ausblenden möchten, und klicken Sie auf **[!UICONTROL Systemweit deaktivieren]**. Nach der Deaktivierung werden der Filter, die Ansicht oder die Gruppierung aus der Layoutvorlage sowie Benutzer im gesamten System ausgeblendet.


## Verfügbar machen von Filtern, Ansichten oder Gruppierungen für alle Benutzer {#make-filters-views-or-groupings-available-to-users}

In diesen Schritten wird beschrieben, wie Sie Filter, Ansichten und Gruppierungen über die [!UICONTROL Freigeben] im Dialogfeld [!UICONTROL Schnittstelle] Gebiet in [!UICONTROL Einrichtung]. Diese Einstellung funktioniert wie ein Ein-/Ausschalten-Schalter für das gesamte System, einschließlich der Layout-Vorlage.

{{step-1-to-setup}}

1. Klicken **[!UICONTROL Schnittstelle]** und klicken Sie dann auf einen der folgenden Punkte: **[!UICONTROL Filter]**, **[!UICONTROL Ansichten]** oder **[!UICONTROL Gruppierungen]**.

1. Wählen Sie den Filter, die Ansicht oder die Gruppierung aus, die Sie Benutzern zur Verfügung stellen möchten, und klicken Sie dann auf die Schaltfläche **[!UICONTROL Freigeben]** icon ![Freigabesymbol](assets/share-icon.png) , um [!UICONTROL Filterzugriff], [!UICONTROL Zugriff anzeigen]oder [!UICONTROL Gruppierungszugriff] Formular.
1. (Bedingt) Um den Filter, die Ansicht oder die Gruppierung für alle Benutzer im System verfügbar zu machen, klicken Sie auf die Schaltfläche **[!UICONTROL Fanggerät]** Dropdown-Menü ![](assets/gear-menu-for-sharing-items.png)Klicken Sie auf **[!UICONTROL Diese Funktion systemweit sichtbar machen]**. Alle Benutzer im System können jetzt den Filter, die Ansicht oder die Gruppierung sehen.

   Oder

   Beginnen Sie mit der Eingabe des Namens bestimmter Benutzer, Teams, Rollen, Gruppen oder Unternehmen, für die der Filter, die Ansicht oder die Gruppierung freigegeben werden soll, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   Weitere Informationen zur Freigabe finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Benutzer, die Sie angegeben haben, können jetzt den Standardfilter, die Standardansicht oder die Gruppierung sehen, wenn Sie den Objekttyp anzeigen, mit dem Sie ihn verknüpft haben.

## Filter, Ansichten und Gruppierungen löschen

{{step-1-to-setup}}

1. Führen Sie je nachdem, ob Sie einen Filter, eine Ansicht oder eine Gruppierung löschen, einen der folgenden Schritte aus:

   * Klicken **[!UICONTROL Schnittstelle]** > **[!UICONTROL Filter]**

   * Klicken **[!UICONTROL Schnittstelle]** > **[!UICONTROL Ansichten]**

   * Klicken **[!UICONTROL Schnittstelle]** > **[!UICONTROL Gruppierungen]**

1. Wählen Sie ein oder mehrere Elemente in der Liste aus und klicken Sie auf die Schaltfläche **[!UICONTROL Löschen]** icon ![Löschsymbol](assets/delete.png).
1. Detaillierte Informationen zum Konfigurieren von Filtern, Ansichten oder Gruppierungen finden Sie in einem der folgenden Artikel.

   * [Filterübersicht in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Ansichten - Übersicht in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Gruppierungsübersicht in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
