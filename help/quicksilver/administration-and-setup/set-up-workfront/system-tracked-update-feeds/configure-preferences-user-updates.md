---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Voreinstellungen für Benutzeraktualisierungen konfigurieren
description: Sie können Voreinstellungen konfigurieren, die auf bestimmte Funktionen zugreifen, wenn Benutzer Kommentare zu einem Objekt hinzufügen [!UICONTROL Updates] Bereich.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Voreinstellungen für Benutzeraktualisierungen konfigurieren

Sie können Voreinstellungen konfigurieren, über die Benutzer beim Hinzufügen von Kommentaren zu den [!UICONTROL Updates] Bereich.

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
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsstufe [!UICONTROL Systemadministrator].</p><p>Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Benutzer können Bilder in Updates hinzufügen

Standardmäßig können Benutzer keine Bilder in Aktualisierungen hinzufügen. Wenn Sie diese Voreinstellung aktivieren, können Benutzer Bilder in Aktualisierungen anhängen. Die Voreinstellung gilt für alle Aktualisierungen in allen Bereichen Ihrer [!DNL Workfront] -Instanz.

>[!NOTE]
>
>* In Updates gespeicherte Bilder werden für die maximale Anzahl an Dokumenten im Speicher gezählt. Weitere Informationen finden Sie unter [Dokumentenspeicherbeschränkungen überprüfen](../../../documents/managing-documents/check-document-storage.md).
>* Auf Bilder kann nur über das [!UICONTROL Updates] auf einem Objekt ein und ist nicht auf der Registerkarte [!UICONTROL Dokumente] Registerkarte.
>




1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).
1. Wählen Sie im linken Bereich die Option **[!UICONTROL Schnittstelle]** > **[!UICONTROL Feeds aktualisieren]**.
1. Wählen Sie die **[!UICONTROL Voreinstellungen]** Registerkarte.

   ![Benutzereinstellungen für Update-Feeds](assets/updatefeeds-preferences-350x137.png)

1. Wählen Sie die **[!UICONTROL Benutzer können Bilder in Updates hinzufügen]** aktivieren.
1. Auswählen **[!UICONTROL Speichern]**.

   Wenn diese Voreinstellung aktiviert ist, können Sie sie jederzeit deaktivieren. Alle Bilder, die bereits in den Aktualisierungen veröffentlicht wurden, verbleiben im [!UICONTROL Updates] -Bereich auf dem Objekt.
