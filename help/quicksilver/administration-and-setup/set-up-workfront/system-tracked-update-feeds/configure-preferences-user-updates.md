---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Konfigurieren von Voreinstellungen für Benutzeraktualisierungen
description: Sie können Voreinstellungen konfigurieren, die auf bestimmte Funktionen zugreifen, wenn Benutzer Kommentare im Bereich [!UICONTROL Aktualisierungen] eines Objekts hinzufügen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/67OfYPIrN7Tzciapa37YHviFI4uptaGgkWkMMREgw-k
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 271
ht-degree: 12%

---

# Konfigurieren von Voreinstellungen für Benutzeraktualisierungen

<!--Audited: 08/2025-->

Sie können Voreinstellungen konfigurieren, die Benutzern Zugriff auf bestimmte Funktionen gewähren, wenn sie Kommentare im Bereich [!UICONTROL Aktualisierungen] eines Objekts hinzufügen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td><p>Systemadministrator, um diese Schritte auf Systemebene auszuführen. </p>
   <p>Planer, um diese Schritte für eine Gruppe auszuführen, zusätzlich zum Manager dieser Gruppe.</p></td>
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td><p>To perform these steps at the system level, you need the [!UICONTROL System Administrator] access level.</p><p>To perform them for a group, you must be a manager of that group.</p></td>
  </tr> 
 </tbody> 
</table>
-->

## Benutzern das Bearbeiten von Bildern in Aktualisierungen erlauben

Standardmäßig können Benutzende in Aktualisierungen keine Bilder hinzufügen. Wenn Sie diese Einstellung aktivieren, können Benutzer Bilder in Aktualisierungen anhängen. Die Voreinstellung gilt für alle Aktualisierungen in allen Bereichen Ihrer [!DNL Workfront].

>[!NOTE]
>
>* In Aktualisierungen gespeicherte Bilder werden in Richtung des Speicherlimits für Dokumente gezählt. Weitere Informationen finden Sie [Überprüfen von Dokumentspeicherbeschränkungen](../../../documents/managing-documents/check-document-storage.md).
>* Auf Bilder kann über die Registerkarte [!UICONTROL Aktualisierungen] eines Objekts zugegriffen werden. Sie sind auch im Bereich [!UICONTROL Dokumente] unter dem [!UICONTROL Hauptmenü] verfügbar.
>

1. Klicken Sie auf **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Setup]** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).
1. Wählen Sie im linken Bedienfeld **[!UICONTROL Schnittstelle]** > **[!UICONTROL Aktualisierungs-Feeds]**.
1. Wählen Sie die **[!UICONTROL Voreinstellungen]** aus.

   ![Benutzervoreinstellungen für Aktualisierungs-Feeds](assets/updatefeeds-preferences-350x137.png)

1. Aktivieren Sie **[!UICONTROL Kontrollkästchen (Benutzern erlauben, Bilder in Aktualisierungen hinzuzufügen]**.
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Wenn diese Einstellung aktiviert ist, können Sie sie jederzeit deaktivieren. Alle Bilder, die bereits in Aktualisierungen veröffentlicht wurden, verbleiben im Bereich [!UICONTROL Aktualisierungen] des Objekts.
