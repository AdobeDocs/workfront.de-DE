---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Voreinstellungen für Benutzeraktualisierungen konfigurieren
description: Sie können Voreinstellungen konfigurieren, die auf bestimmte Funktionen zugreifen, wenn Benutzer Kommentare im Bereich [!UICONTROL Aktualisierungen] eines Objekts hinzufügen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 1%

---

# Voreinstellungen für Benutzeraktualisierungen konfigurieren

Sie können Voreinstellungen konfigurieren, die Benutzern Zugriff auf bestimmte Funktionen gewähren, wenn sie Kommentare zum Bereich [!UICONTROL Aktualisierungen] eines Objekts hinzufügen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td><p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsstufe [!UICONTROL Systemadministrator].</p><p>Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzer können Bilder in Updates hinzufügen

Standardmäßig können Benutzer keine Bilder in Aktualisierungen hinzufügen. Wenn Sie diese Voreinstellung aktivieren, können Benutzer Bilder in Aktualisierungen anhängen. Die Voreinstellung gilt für alle Aktualisierungen in allen Bereichen Ihrer [!DNL Workfront] -Instanz.

>[!NOTE]
>
>* In Updates gespeicherte Bilder werden für die maximale Anzahl an Dokumenten im Speicher gezählt. Weitere Informationen finden Sie unter [Überprüfen der Speicherbeschränkungen für Dokumente](../../../documents/managing-documents/check-document-storage.md).
>* Auf Bilder kann über die Registerkarte [!UICONTROL Aktualisierungen] in einem Objekt zugegriffen werden. Sie sind auch im Bereich [!UICONTROL Dokumente] unter dem Hauptmenü [!UICONTROL  verfügbar.]
>

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)
1. Wählen Sie im linken Bereich **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]** aus.
1. Wählen Sie die Registerkarte **[!UICONTROL Voreinstellungen]** aus.

   ![Benutzereinstellungen für Update-Feeds](assets/updatefeeds-preferences-350x137.png)

1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Benutzern erlauben, in Aktualisierungen Bilder hinzuzufügen]** .
1. Wählen Sie **[!UICONTROL Speichern]** aus.

   Wenn diese Voreinstellung aktiviert ist, können Sie sie jederzeit deaktivieren. Alle Bilder, die bereits in Updates veröffentlicht wurden, verbleiben im Bereich [!UICONTROL Updates] des Objekts.
