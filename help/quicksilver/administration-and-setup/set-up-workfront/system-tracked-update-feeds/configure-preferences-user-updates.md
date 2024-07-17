---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Voreinstellungen für Benutzeraktualisierungen konfigurieren
description: Sie können Voreinstellungen konfigurieren, die auf bestimmte Funktionen zugreifen, wenn Benutzer Kommentare im Bereich [!UICONTROL Aktualisierungen] eines Objekts hinzufügen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d6d18423-d13c-42e8-b8ee-43e6842b6481
source-git-commit: fd876089c964d57224452023b4656cd6df40b5a3
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 1%

---

# Voreinstellungen für Benutzeraktualisierungen konfigurieren

Sie können Voreinstellungen konfigurieren, die Benutzern Zugriff auf bestimmte Funktionen gewähren, wenn sie Kommentare zum Bereich [!UICONTROL Aktualisierungen] eines Objekts hinzufügen.

## Zugriffsanforderungen

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
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsstufe [!UICONTROL Systemadministrator].</p><p>Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

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
