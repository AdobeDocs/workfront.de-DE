---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Benutzername wird bereits verwendet
description: Lesen Sie diese Tipps, wenn Sie eine Fehlermeldung erhalten, dass der Benutzername bereits vergeben ist.
author: Becky
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
TQID: https://experienceleague.adobe.com/uGrOaZZzbE6CkodhE1TlCtW4rRJkfqljWGJbNSzxODc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 300
ht-degree: 14%

---

# Benutzername wird bereits verwendet

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Frage

Beim Erstellen eines neuen Benutzers wird ein [!UICONTROL Hoppla]-Fehler angezeigt, der angibt, dass der Benutzername bereits verwendet wird. Es gibt keine anderen Vorkommen dieser E-Mail im System. Warum wird dies angezeigt?

## Lösung

Dies kann entweder auftreten, weil der Benutzername oder die E-Mail-Adresse in der aktuellen [!DNL Adobe Workfront]-Instanz nicht eindeutig ist. Benutzer können denselben Benutzernamen oder dieselbe E-Mail-Adresse in separaten Instanzen haben. Beispielsweise könnten Benutzer A über die folgenden E-Mail-Adressen verfügen, die mit einem [!DNL Workfront]-Konto verknüpft sind: usera@company1.com und usera@company2.com.

>[!NOTE]
>
>Der primäre [!DNL Workfront]-Administrator kann nicht denselben Benutzernamen oder dieselbe E-Mail-Adresse haben, wenn er sich in separaten Workfront-Instanzen im selben Cluster befindet.
>
>Wenn sich die Instanzen auf verschiedenen Clustern befinden, kann der primäre Administrator bzw. die primäre Administratorin denselben Benutzernamen oder dieselbe E-Mail-Adresse haben. Sie können den Cluster, auf dem sich Ihre Instanz befindet, unter [!UICONTROL Setup] > [!UICONTROL System] > [!UICONTROL Kundeninformationen] anzeigen.

### Überprüfen Sie, ob Ihr Benutzername in Ihrer Instanz eindeutig ist

Stellen Sie sicher, dass der Benutzername und die E-Mail-Adresse in der aktuellen [!DNL Workfront]-Instanz eindeutig sind:

{{step-1-to-users}}

1. Überprüfen Sie in der Personenliste die Spalte **[!UICONTROL E-Mail]**, um sicherzustellen, dass keine doppelten E-Mails vorhanden sind.
1. Fügen Sie der Ansicht eine Spalte für den Benutzernamen hinzu.

   1. Klicken Sie **[!UICONTROL Dropdown]** Menü Ansicht auf **[!UICONTROL Ansicht anpassen]**.
   1. Klicken Sie auf **[!UICONTROL Spalte hinzufügen]**.
   1. Geben Sie im Suchfeld &quot;*[!UICONTROL &quot;]*.
   1. Wählen Sie **[!UICONTROL Benutzer]** > **[!UICONTROL Benutzername]** aus.
   1. Speichern Sie die Ansicht.\
      Dies führt zu einer Ansicht, in der die Benutzernamen angezeigt werden, in denen Sie nach dem Duplikat suchen können.

1. Suchen Sie in der Personenliste in der Spalte **[!UICONTROL Benutzername]**, um sicherzustellen, dass es keine doppelten Benutzernamen gibt.
