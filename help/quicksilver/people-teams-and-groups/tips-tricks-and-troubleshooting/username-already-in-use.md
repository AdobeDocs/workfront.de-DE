---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Benutzername bereits in Verwendung
description: Lesen Sie diese Tipps, wenn Sie eine Fehlermeldung erhalten, dass der Benutzername bereits übernommen wurde.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 1%

---

# Benutzername bereits in Verwendung

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Systemadministrator]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Frage

Beim Erstellen eines neuen Benutzers wird ein Fehler vom Typ [!UICONTROL Upper] angezeigt, der angibt, dass der Benutzername bereits übernommen wurde. Diese E-Mail ist nicht mehr im System vorhanden. Warum wird dies angezeigt?

## Lösung

Dies kann auftreten, weil der Benutzername oder die E-Mail-Adresse in der aktuellen [!DNL Adobe Workfront]-Instanz nicht eindeutig ist. Benutzer können denselben Benutzernamen oder dieselbe E-Mail-Adresse in separaten Instanzen haben. Benutzer A könnte beispielsweise die folgenden E-Mail-Adressen mit einem [!DNL Workfront] -Konto verknüpfen: usera@company1.com und usera@company2.com.

>[!NOTE]
>
>Der primäre Administrator [!DNL Workfront] kann nicht denselben Benutzernamen oder dieselbe E-Mail-Adresse haben, wenn er sich in separaten Workfront-Instanzen im selben Cluster befindet.
>
>Wenn sich die Instanzen in verschiedenen Clustern befinden, kann der primäre Administrator denselben Benutzernamen oder dieselbe E-Mail-Adresse haben. Sie können den Cluster, in dem sich Ihre Instanz befindet, unter [!UICONTROL Setup] > [!UICONTROL System] > [!UICONTROL Kundeninformationen] anzeigen.

### Überprüfen Sie, ob Ihr Benutzername in Ihrer Instanz eindeutig ist.

Stellen Sie sicher, dass Benutzername und E-Mail-Adresse in der aktuellen [!DNL Workfront]-Instanz eindeutig sind:

1. Klicken Sie als [!DNL Workfront] -Administrator auf das Symbol **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Benutzer]**.
1. Sehen Sie sich die Spalte **[!UICONTROL E-Mail]** in der Personenliste an, um sicherzustellen, dass keine doppelten E-Mails gesendet werden.
1. Fügen Sie der Ansicht eine Spalte für den Benutzernamen hinzu.

   1. Klicken Sie im Dropdownmenü **[!UICONTROL Ansicht]** auf **[!UICONTROL Ansicht anpassen]**.
   1. Klicken Sie auf **[!UICONTROL Spalte hinzufügen]**.
   1. Geben Sie im Suchfeld *[!UICONTROL Benutzername]* ein.
   1. Wählen Sie **[!UICONTROL Benutzer]** > **[!UICONTROL Benutzername]** aus.
   1. Speichern Sie die Ansicht.\
      Dies führt zu einer Ansicht, in der die Benutzernamen angezeigt werden, unter denen Sie nach dem Duplikat suchen können.

1. Sehen Sie sich die Spalte **[!UICONTROL Benutzername]** in der Personenliste an, um sicherzustellen, dass keine doppelten Benutzernamen vorhanden sind.
