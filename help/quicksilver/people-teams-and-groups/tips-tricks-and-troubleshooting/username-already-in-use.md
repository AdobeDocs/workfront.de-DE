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
source-wordcount: '304'
ht-degree: 0%

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
   <td> <p>Beliebig</p> </td> 
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

Beim Erstellen eines neuen Benutzers muss ein [!UICONTROL Hopfen] -Fehler angezeigt, der besagt, dass der Benutzername bereits vergeben wurde. Diese E-Mail ist nicht mehr im System vorhanden. Warum wird dies angezeigt?

## Lösung

Dies kann daran liegen, dass Benutzername oder E-Mail-Adresse in der aktuellen [!DNL Adobe Workfront] -Instanz. Benutzer können denselben Benutzernamen oder dieselbe E-Mail-Adresse in separaten Instanzen haben. Beispielsweise könnten die folgenden E-Mail-Adressen von Benutzer A mit einem [!DNL Workfront] Konto: usera@company1.com und usera@company2.com.

>[!NOTE]
>
>Die primäre [!DNL Workfront] -Administrator kann nicht denselben Benutzernamen oder dieselbe E-Mail-Adresse haben, wenn sie sich in verschiedenen Workfront-Instanzen im selben Cluster befinden.
>
>Wenn sich die Instanzen in verschiedenen Clustern befinden, kann der primäre Administrator denselben Benutzernamen oder dieselbe E-Mail-Adresse haben. Sie können den Cluster anzeigen, in dem sich Ihre Instanz befindet [!UICONTROL Einrichtung] > [!UICONTROL System] > [!UICONTROL Kundeninformationen].

### Überprüfen Sie, ob Ihr Benutzername in Ihrer Instanz eindeutig ist.

Stellen Sie sicher, dass Benutzername und E-Mail-Adresse in der aktuellen [!DNL Workfront] instance:

1. Als [!DNL Workfront] Administrator klicken Sie auf die **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Benutzer]**.
1. Sehen Sie sich in der Liste der Personen die **[!UICONTROL Email]** um sicherzustellen, dass keine doppelten E-Mails vorhanden sind.
1. Fügen Sie der Ansicht eine Spalte für den Benutzernamen hinzu.

   1. Im **[!UICONTROL Ansicht]** Dropdown-Menü, klicken Sie auf **[!UICONTROL Ansicht anpassen]**.
   1. Klicken **[!UICONTROL Spalte hinzufügen]**.
   1. Geben Sie im Suchfeld *[!UICONTROL Benutzername]*.
   1. Auswählen **[!UICONTROL Benutzer]** > **[!UICONTROL Benutzername]**.
   1. Speichern Sie die Ansicht.\
      Dies führt zu einer Ansicht, in der die Benutzernamen angezeigt werden, unter denen Sie nach dem Duplikat suchen können.

1. Sehen Sie sich in der Liste der Personen die **[!UICONTROL Benutzername]** um sicherzustellen, dass keine doppelten Benutzernamen vorhanden sind.
