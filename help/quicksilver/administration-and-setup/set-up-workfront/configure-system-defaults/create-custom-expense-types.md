---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Benutzerdefinierte Ausgabentypen erstellen
description: Als [!DNL Adobe Workfront] Administrator können Sie benutzerdefinierte Ausgabentypen erstellen, um die mit Ihren Aufgaben und Projekten verbundenen Ausgaben zu definieren und zu verfolgen. Ausgaben sind Nicht-Arbeitskosten, die mit Aufgaben oder Projekten verknüpft werden können.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 1%

---

# Benutzerdefinierte Ausgabentypen erstellen

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] -Administrator können Sie benutzerdefinierte Ausgabentypen erstellen, um die mit Ihren Aufgaben und Projekten verbundenen Ausgaben zu definieren und zu verfolgen. Ausgaben sind Nicht-Arbeitskosten, die mit Aufgaben oder Projekten verknüpft werden können.

Sie können von Ihnen erstellte Ausgabetypen bearbeiten oder löschen. Sie können die integrierten [!DNL Workfront] Ausgabetypen nicht löschen oder bearbeiten.

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
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Standardausgabetypen

Die Ausgabentypen, die standardmäßig in &quot;[!DNL Workfront]&quot;enthalten sind, können nicht gelöscht oder bearbeitet werden. Dazu gehören:

* [!UICONTROL Advertising]
* [!UICONTROL Consulting]
* [!UICONTROL Unterhaltung]
* [!UICONTROL Allgemein]
* [!UICONTROL Materialien]
* [!UICONTROL Reise]

## Benutzerdefinierte Ausgabentypen erstellen

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront].
1. Klicken Sie auf **[!UICONTROL Ausgabetypen]**.
1. Klicken Sie auf **[!UICONTROL Neuer Ausgabentyp]**.
1. Geben Sie im angezeigten Feld **[!UICONTROL Neuer Ausgabentyp]** die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Geben Sie einen Namen für die Kosten an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung der Kosten an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Berechnete Einheit]</td> 
      <td> <p>Wählen Sie die Maßeinheit für Ihren Ausgabentyp aus der Dropdown-Liste aus.</p> <p>Folgende Maßeinheit ist verfügbar:</p> 
       <ul> 
        <li>Meile</li> 
        <li>Kilometer</li> 
        <li>Kilogramm</li> 
        <li>Dollar</li> 
        <li>Dollar</li> 
        <li>Tag</li> 
        <li>Andere - Wenn Sie diese Option auswählen, werden Sie aufgefordert, Ihre Maßeinheit zu benennen und die Maßeinheit als etwas zu definieren, das Ihrer Organisation bekannt ist.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Satz</td> 
      <td> <p>Geben Sie den Preis pro Einheit an. Dies ist ein Feld im Währungsformat und stellt die Kosten jeder Einheit dar, die im Feld <strong>[!UICONTROL Berechnete Einheit]</strong> ermittelt wurde. </p> <p>Die Rate kann einen numerischen Wert mit bis zu 4 Zahlen nach der Dezimalstelle enthalten. Beispiel: 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Ausgabentyp erstellen]**.\
   Der Ausgabentyp ist jetzt für Benutzer verfügbar, um ihn mit ihren Ausgaben für Projekte und Aufgaben zu verknüpfen.

## Ändern benutzerdefinierter Ausgabentypen

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront].
1. Klicken Sie auf **[!UICONTROL Ausgabetypen]**.
1. Wählen Sie den Ausgabentyp aus, den Sie ändern möchten, und klicken Sie dann auf **[!UICONTROL Bearbeiten]**.

   Das Dialogfeld **[!UICONTROL Ausgabentyp bearbeiten]** wird angezeigt.

1. Nehmen Sie die gewünschten Änderungen vor und klicken Sie dann auf **[!UICONTROL Änderungen speichern]**.\
   Der Ausgabentyp ist jetzt für Benutzer verfügbar, um ihn mit ihren Ausgaben für Projekte und Aufgaben zu verknüpfen.

Weitere Informationen zur Verwendung von Ausgaben und dazu, wie sie sich auf die Kosten eines Projekts auswirken können, finden Sie im Artikel [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).
