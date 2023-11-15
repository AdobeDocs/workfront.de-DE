---
title: Zugriff auf Adobe Maestro gewähren
description: Erfahren Sie, wie Sie Zugriff gewähren und Informationen in Adobe Maestro freigeben.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: 90c730bbab2e62bcc60bee37272edb1219b2afb4
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Zugriff auf Adobe Maestro gewähren

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Zugriff auf Maestro zu erhalten
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

Derzeit können alle Benutzer in Ihrer Organisation Zugriff auf Maestro haben, wenn die folgende Voraussetzung erfüllt ist:

* Ihr Unternehmen ist am Adobe Maestro Closed-Beta-Programm angemeldet.

  Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren.


Informationen darüber, welchen Zugriff Sie benötigen, finden Sie unter [Adobe Maestro-Zugriffsübersicht](../access/access-overview.md).

>[!NOTE]
>
>Es gibt keine Zugriffsebenen oder Berechtigungen, die mit Benutzern oder den Informationen in Maestro verknüpft sind. Alle Benutzer, für die Maestro in ihrer Umgebung aktiviert ist, können alle Informationen, die andere Benutzer Maestro hinzufügen, anzeigen, bearbeiten und löschen.

## Maestro für Benutzer in Ihrer Workfront-Instanz aktivieren

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.-->

Nachdem sich Ihr Unternehmen für das Betaprogramm Maestro angemeldet hat, können Sie den Maestro-Bereich für andere Benutzer mithilfe einer Layoutvorlage hinzufügen.

So geben Sie den Maestro-Bereich mithilfe einer Layoutvorlage frei:

1. Anmelden bei **Workfront** als Workfront-Administrator.

1. Fügen Sie die **Maestro** icon ![](assets/maestro-icon.png) der **Hauptmenü** mithilfe einer **Layout-Vorlage**.

   Weitere Informationen finden Sie unter [Hauptmenü mithilfe einer Layoutvorlage anpassen](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Weisen Sie die Layoutvorlage den Benutzern zu, die Zugriff auf Maestro erhalten sollen.

   Weitere Informationen finden Sie unter [Benutzer einer Layoutvorlage zuweisen](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Alle Benutzer, die der Vorlage zugewiesen sind, können jetzt im Hauptmenü auf Maestro zugreifen.

   Benutzer können damit beginnen, Arbeitsbereiche, Datensatztypen, Datensätze und Felder zu erstellen.

<!--
## Share permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group, then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (********) add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu at the right of a user or group name, then click **Remove**. 
    
    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 
1. Click **Save**.

-->