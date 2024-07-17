---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Zugriff auf Blueprints konfigurieren
description: Als Systemadministrator können Sie den Zugriff für Benutzer aktivieren, um die Installation von Blueprints anzufordern, indem Sie eine Anforderungswarteschlange einrichten, in der die Anforderungen gespeichert werden. Dort können Sie Anforderungen an eine zentrale Stelle verfolgen und aktualisieren.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Zugriff auf Blueprints konfigurieren

Alle [!DNL Adobe Workfront] Benutzer können den Blueprint-Katalog durchsuchen.

Als Systemadministrator haben Sie folgende Möglichkeiten:

* Fügen Sie [!UICONTROL Blueprints] zum Hauptmenü in Layoutvorlagen hinzu und weisen Sie Benutzern oder Gruppen die Layoutvorlage zu. Weitere Informationen finden Sie unter [Anpassen des [!UICONTROL Hauptmenüs] mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) und [Zuweisen von Benutzern zu einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

  >[!NOTE]
  >
  >* Benutzern, denen keine Layoutvorlage zugewiesen ist, wird das Symbol [!UICONTROL Blueprints] im [!UICONTROL Hauptmenü] angezeigt.
  >* Wenn Sie eine neue Layoutvorlage erstellen, ist das Symbol [!UICONTROL Blueprints] standardmäßig in der Liste [!UICONTROL Aktive Elemente] für das Hauptmenü [!UICONTROL 5} enthalten.]


* Gewähren Sie Benutzern Zugriff, um die Installation von Blueprints anzufordern, indem Sie eine Anforderungswarteschlange zum Speichern der Anforderungen einrichten. Dort können Sie Anforderungen an eine zentrale Stelle verfolgen und aktualisieren. Gehen Sie für weitere Informationen wie folgt vor:
* Installieren Sie Blueprints. Weitere Informationen finden Sie unter [Installieren eines Blueprints](../../administration-and-setup/blueprints/blueprints-install.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p> Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] Lizenz</strong></td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Systemadministrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Voraussetzungen {#prerequisites}

* Sie müssen eine vorhandene Anforderungswarteschlange verwenden, um Blueprint-Anforderungen zu speichern. Das Projekt muss als Anforderungswarteschlange gespeichert werden und sich im Status [!UICONTROL Aktuell] befinden.
* Die Anforderungswarteschlange muss öffentlich sein. In den Details der Anforderungswarteschlange &quot;[!UICONTROL Wer kann dieser Warteschlange Anforderungen hinzufügen?]&quot; muss auf **[!UICONTROL Anyone]** gesetzt werden.

>[!TIP]
>
>Wenn Sie eine neue Anforderungswarteschlange für Blueprint-Anforderungen erstellen möchten, sollten Sie diese erstellen, bevor Sie den Blueprints-Zugriff konfigurieren. Informationen zum Erstellen einer Anforderungswarteschlange finden Sie unter [Erstellen einer Anforderungswarteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Auswählen der Anforderungswarteschlange zum Speichern von Blueprint-Anforderungen

Bevor Benutzer die Installation von Blueprints für sie anfordern können, müssen Sie eine Anforderungswarteschlange für diese Anforderungen auswählen. Bis die Anforderungswarteschlange definiert ist, können Benutzer nur den Blueprints-Katalog durchsuchen.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Blueprints]**.![](assets/main-menu-icon.png)
1. Klicken Sie oben rechts im Katalogbildschirm auf **[!UICONTROL Blueprint-Anforderungen konfigurieren]** .

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Geben Sie im Dialogfeld **[!UICONTROL Blueprints konfigurieren]** den Namen einer aktiven Anforderungswarteschlange ein und wählen Sie sie aus, wenn sie in den Suchergebnissen angezeigt wird.

   >[!IMPORTANT]
   >
   >In dieser Liste werden nur Warteschlangen für öffentliche Anforderungen angezeigt. Informationen zum Veröffentlichen Ihrer Anforderungswarteschlange finden Sie im Abschnitt [Voraussetzungen](#prerequisites) oben.

   Die Voreinstellung für die Anforderungswarteschlange ist festgelegt und Benutzer können jetzt die Blueprint-Installation anfordern.

   ![Anforderungswarteschlange konfigurieren](assets/Blueprints_access_setup_request_queue.png)

1. (Optional) Um Änderungen an der eigentlichen Anforderungswarteschlange vorzunehmen, klicken Sie auf **[!UICONTROL Diese Anforderungswarteschlange bearbeiten]**.

   Das Projekt für die Anforderungswarteschlange wird in einer neuen Browser-Registerkarte geöffnet und Sie können es nach Bedarf aktualisieren.

1. (Optional) Wenn die Anforderungswarteschlange Themengruppen oder Themen in der Warteschlange enthält, können Sie sie aus der Liste auswählen.
1. Um zum Blueprints-Katalog zurückzukehren, klicken Sie auf **[!UICONTROL Schließen]**.

>[!NOTE]
>
>Wenn Sie einen angeforderten Blueprint installieren, sollten Sie den Problemstatus in der Anforderungswarteschlange in **[!UICONTROL Geschlossen]** oder **[!UICONTROL Aufgelöst]** ändern, damit der Anforderer benachrichtigt wird. Weitere Informationen zum Installieren eines Blueprints finden Sie unter [Installieren eines Blueprints](../../administration-and-setup/blueprints/blueprints-install.md).
