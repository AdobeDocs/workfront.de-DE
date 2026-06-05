---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Zugriff auf Blueprints konfigurieren
description: Als Systemadministrator können Sie den Zugriff für Benutzer aktivieren, um die Installation von Blueprints anzufordern, indem Sie eine Anfrage-Warteschlange zum Speichern der Anfragen einrichten. Dort haben Sie einen einzigen Ort, um Anfragen zu verfolgen und zu aktualisieren.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ssQ-zj5Hn4ZalKVm1ERlR3NIpqNJlwJjDqQoSFzJHMw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 512
ht-degree: 8%

---

# Konfigurieren des Zugriffs auf Blueprints

Alle [!DNL Adobe Workfront] können den Blueprint-Katalog durchsuchen.

Als Systemadministrator haben Sie folgende Möglichkeiten:

* Fügen Sie [!UICONTROL Blueprints] zum Hauptmenü in Layout-Vorlagen hinzu und weisen Sie die Layout-Vorlage Benutzern oder Gruppen zu. Weitere Informationen finden Sie unter [Anpassen des [!UICONTROL Hauptmenüs] Verwenden einer Layout-](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) und [Zuweisen von Benutzern zu einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

  >[!NOTE]
  >
  >* Benutzern, denen keine Layoutvorlage zugewiesen ist, wird das [!UICONTROL Blueprints] im [!UICONTROL Hauptmenü] angezeigt.
  >* Wenn Sie eine neue Layout-Vorlage erstellen[!UICONTROL &#x200B; wird das Symbol &#x200B;]Blueprints“ standardmäßig in die Liste [!UICONTROL Aktive Elemente] für das [!UICONTROL Hauptmenü] aufgenommen.


* Aktivieren Sie den Zugriff für Benutzer, um die Installation von Blueprints anzufordern, indem Sie eine Anfrage-Warteschlange zum Speichern der Anfragen einrichten. Dort haben Sie einen einzigen Ort, um Anfragen zu verfolgen und zu aktualisieren. Weitere Informationen finden Sie im folgenden Verfahren.
* Blueprints installieren. Weitere Informationen finden Sie unter [Blueprint installieren](../../administration-and-setup/blueprints/blueprints-install.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Workfront-Administrator </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen {#prerequisites}

* Zum Speichern von Blueprint-Anfragen muss eine vorhandene Anfrage-Warteschlange verwendet werden. Das Projekt muss als Anfrage-Warteschlange gespeichert werden und den Status [!UICONTROL aktuell] aufweisen.
* Die Anfrage-Warteschlange muss öffentlich sein. In den Details der Anfrage-Warteschlange [!UICONTROL Wer kann dieser Warteschlange Anforderungen hinzufügen?]&quot; muss auf &quot;**[!UICONTROL &quot;]** sein.

>[!TIP]
>
>Wenn Sie eine neue Anfragewarteschlange für Blueprint-Anfragen erstellen möchten, sollten Sie sie vor dem Konfigurieren des Blueprint-Zugriffs erstellen. Informationen zum Erstellen einer Anfrage-Warteschlange finden Sie [Erstellen einer Anfrage-Warteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Wählen Sie die Anfrage-Warteschlange aus, um Blueprint-Anfragen zu speichern

Bevor Benutzer die Installation von Blueprints für sie anfordern können, müssen Sie eine Anfrage-Warteschlange für diese Anfragen auswählen. Bis die Anfrage-Warteschlange definiert ist, können Benutzer nur den Blueprint-Katalog durchsuchen.

{{step1-to-blueprints}}

1. Klicken **[!UICONTROL oben rechts]** Katalogbildschirm auf „Blueprint-Anfragen konfigurieren“.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Geben **[!UICONTROL im Dialogfeld „Blueprints konfigurieren]** den Namen einer aktiven Anfrage-Warteschlange ein und wählen Sie diese aus, wenn sie in den Suchergebnissen angezeigt wird.

   >[!IMPORTANT]
   >
   >In dieser Liste werden nur öffentliche Anfrage-Warteschlangen angezeigt. Um Ihre Anfrage-Warteschlange öffentlich zu machen, lesen Sie [&#x200B; Abschnitt „Voraussetzungen](#prerequisites) weiter oben.

   Die Einstellung für die Anfrage-Warteschlange ist festgelegt, und Benutzer können jetzt die Blueprint-Installation anfordern.

   ![Anfrage-Warteschlange konfigurieren](assets/Blueprints_access_setup_request_queue.png)

1. (Optional) Um Änderungen an der eigentlichen Anfrage-Warteschlange vorzunehmen, klicken Sie auf **[!UICONTROL Diese Anfrage-Warteschlange bearbeiten]**.

   Das Projekt „Anfrage-Warteschlange“ wird in einer neuen Browser-Registerkarte geöffnet und kann bei Bedarf aktualisiert werden.

1. (Optional) Wenn die Anfrage-Warteschlange Themengruppen oder Warteschlangenthemen enthält, können Sie diese aus der Liste auswählen.
1. Um zum Blueprint-Katalog zurückzukehren, klicken Sie auf **[!UICONTROL Schließen]**.

>[!NOTE]
>
>Wenn Sie eine angeforderte Blueprint installieren, sollten Sie in der Anfrage-Warteschlange den Problemstatus in **[!UICONTROL Geschlossen]** oder **[!UICONTROL Gelöst]** ändern, damit der Antragsteller benachrichtigt wird. Informationen zum Installieren eines Blueprints finden Sie unter [Installieren eines Blueprints](../../administration-and-setup/blueprints/blueprints-install.md).
