---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Benutzername wird bereits verwendet
description: Lesen Sie diese Tipps, wenn Sie eine Fehlermeldung erhalten, dass der Benutzername bereits vergeben ist.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 1%

---

# Bereits verwendeter Benutzername

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Systemadministrator</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
