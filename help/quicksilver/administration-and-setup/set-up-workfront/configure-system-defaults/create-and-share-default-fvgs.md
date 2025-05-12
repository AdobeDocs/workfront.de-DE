---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Systemweite Filter, Ansichten und Gruppierungen erstellen, bearbeiten und freigeben
description: Sie können Standardfilter, Ansichten und Gruppierungen erstellen und sie dann für Benutzer in Ihrer Organisation verfügbar machen.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: ad6d983524e19e60e0c884faed2990d9fa6549d7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# Systemweite Filter, Ansichten und Gruppierungen erstellen, bearbeiten und freigeben

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Sie können Filter, Ansichten und Gruppierungen erstellen und sie für Benutzer in Ihrer Organisation systemweit verfügbar machen.

Wenn Sie systemweite Filter, Ansichten und Gruppierungen erstellen, wie in diesem Artikel beschrieben, können Benutzer, für die Sie sie freigeben, diese beim Anzeigen ihrer Listen nutzen. Benutzer können basierend auf den von Ihnen erstellten Filtern, Ansichten und Gruppierungen eigene Filter, Ansichten und Gruppierungen erstellen, diese jedoch nicht direkt ändern.

Beachten Sie, dass sich die von Ihnen erstellten systemweiten Filter, Ansichten und Gruppierungen von den Standardfiltern, die Adobe Workfront automatisch für Sie im System erstellt, unterscheiden. Diese Standardfilter, -ansichten und -gruppierungen können nicht bearbeitet oder gelöscht werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter, Ansichten oder Gruppierungen erstellen

{{step-1-to-setup}}


1. Klicken Sie **[!UICONTROL Schnittstelle]** und klicken Sie dann auf eine der folgenden Optionen: **[!UICONTROL Filter]**, **[!UICONTROL Ansichten]** oder **[!UICONTROL Gruppierungen]**.

1. Wenn Sie einen Filter, eine Ansicht oder eine Gruppierung erstellen, klicken Sie auf **[!UICONTROL Filter hinzufügen]**, **[!UICONTROL Ansicht hinzufügen]** oder **[!UICONTROL Gruppierung hinzufügen]** und wählen Sie dann den Objekttyp aus, mit dem Sie den neuen Filter, die neue Ansicht oder die neue Gruppierung verknüpfen möchten.

   Oder

   Wenn Sie einen vorhandenen Filter, eine vorhandene Ansicht oder eine vorhandene Gruppierung bearbeiten, wählen Sie ihn aus und klicken Sie dann auf das Symbol **[!UICONTROL Bearbeiten]** ![Symbol Bearbeiten](assets/edit-icon.png).

1. Filter, Ansicht oder Gruppierung konfigurieren.

   Informationen zu den verfügbaren Optionen finden Sie in einem der folgenden Artikel:

   * [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Ansichten - Übersicht in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Gruppierungen - Übersicht in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Klicken **[!UICONTROL unten links]** „Speichern“.

Sie können den Filter, die Ansicht oder die Gruppierung für Benutzer in Ihrem System verfügbar machen. Weitere Informationen zum Freigeben von Filtern, Ansichten oder Gruppierungen für andere Benutzer finden Sie im Abschnitt [Erstellen von Filtern, Ansichten oder Gruppierungen für Benutzer](#make-filters-views-or-groupings-available-to-users) in diesem Artikel.


## In der Layout-Vorlage verfügbare Filter, Ansichten oder Gruppierungen ein- oder ausblenden

Sie können Filter, Ansichten oder Gruppierungen aus der Layout-Vorlage ein- oder ausblenden. Sichtbare Filter sind systemweit für alle Benutzer verfügbar. Sie können eine Layout-Vorlage verwenden, um sichtbare Filter für bestimmte Benutzende oder Gruppen auszublenden.

>[!NOTE]
>
>Wenn ein(e) Benutzende(r) aktiv einen Filter, eine Ansicht oder eine Gruppierung verwendet und dieser dann von einem Administrator deaktiviert wird, hat der/die Benutzende weiterhin Zugriff, bis er/sie einen neuen Filter, eine neue Ansicht oder eine neue Gruppierung auswählt. Nachdem sie einen neuen ausgewählt haben, können sie nicht mehr zum verborgenen zurückkehren.

So blenden Sie die in der Layout-Vorlage verfügbaren Filter, Ansichten oder Gruppierungen ein oder aus:

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Schnittstelle]** und klicken Sie dann auf eine der folgenden Optionen: **[!UICONTROL Filter]**, **[!UICONTROL Ansichten]** oder **[!UICONTROL Gruppierungen]**.

1. (Bedingt) Wählen Sie den Filter, die Ansicht oder die Gruppierung aus, die Sie den Benutzern zur Verfügung stellen möchten, und klicken Sie dann auf **[!UICONTROL Systemweit aktivieren]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Wenn Sie möchten, dass der Filter, die Ansicht oder die Gruppierung für die meisten Benutzer verfügbar bleibt, sie jedoch vor anderen ausblenden, können Sie die Layout-Vorlage verwenden. Weitere Informationen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Bedingt) Wählen Sie den Filter, die Ansicht oder die Gruppierung aus, die Sie vor Benutzern ausblenden möchten, und klicken Sie dann auf **[!UICONTROL Systemweit deaktivieren]**. Der Filter, die Ansicht oder die Gruppierung ist jetzt in der Layout-Vorlage und für Benutzende im System ausgeblendet.


## Filter, Ansichten oder Gruppierungen für alle Benutzer verfügbar machen {#make-filters-views-or-groupings-available-to-users}

In diesen Schritten wird erläutert, wie Sie Filter, Ansichten und Gruppierungen über das Dialogfeld [!UICONTROL Freigeben] im Bereich [!UICONTROL Schnittstelle] in [!UICONTROL Setup] verfügbar machen. Diese Einstellung wirkt wie ein Ein-/Aus-Schalter für das gesamte System, einschließlich der Layout-Vorlage.

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Schnittstelle]** und klicken Sie dann auf eine der folgenden Optionen: **[!UICONTROL Filter]**, **[!UICONTROL Ansichten]** oder **[!UICONTROL Gruppierungen]**.

1. Wählen Sie den Filter, die Ansicht oder die Gruppierung aus, die Sie den Benutzern zur Verfügung stellen möchten, und klicken Sie dann auf das **[!UICONTROL Freigabe]**-Symbol ![Freigeben](assets/share-icon.png).
1. Geben Sie den Namen bestimmter Benutzer, Teams, Rollen, Gruppen oder Unternehmen ein, für die Sie den Filter, die Ansicht oder die Gruppierung freigeben möchten, und klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.

   Weitere Informationen zur Freigabe finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klicken Sie auf **[!UICONTROL Speichern]**. Benutzer, die Sie angegeben haben, können jetzt den Filter, die Ansicht oder die Gruppierung sehen, wenn Sie den Objekttyp anzeigen, mit dem Sie ihn verknüpft haben.

## Filter, Ansichten und Gruppierungen löschen

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Schnittstelle]** und klicken Sie dann auf eine der folgenden Optionen: **[!UICONTROL Filter]**, **[!UICONTROL Ansichten]** oder **[!UICONTROL Gruppierungen]**.

1. Wählen Sie ein oder mehrere Elemente in der Liste aus und klicken Sie dann auf das **[!UICONTROL Löschen]**-Symbol ![Löschen](assets/delete.png).

1. Klicken Sie im **Löschen**-Dialogfeld auf **Ja, Löschen**.
