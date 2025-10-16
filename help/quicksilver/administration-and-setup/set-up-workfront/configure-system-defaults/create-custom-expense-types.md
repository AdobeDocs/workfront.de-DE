---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Erstellen benutzerdefinierter Ausgabentypen
description: Als  [!DNL Adobe Workfront]  können Sie benutzerdefinierte Ausgabentypen erstellen, um die mit Ihren Aufgaben und Projekten verbundenen Ausgaben zu definieren und zu verfolgen. Kosten sind sonstige Kosten, die mit Aufgaben oder Projekten verbunden werden können.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 4%

---

# Benutzerdefinierte Ausgabentypen erstellen

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] können Sie benutzerdefinierte Ausgabentypen erstellen, um die mit Ihren Aufgaben und Projekten verbundenen Ausgaben zu definieren und zu verfolgen. Kosten sind sonstige Kosten, die mit Aufgaben oder Projekten verbunden werden können.

Sie können alle von Ihnen erstellten Ausgabentypen bearbeiten oder löschen. Die integrierten Ausgabentypen [!DNL Workfront] können nicht gelöscht oder bearbeitet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL -Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Standardausgabentypen

Zu den standardmäßigen Ausgabentypen in [!DNL Workfront], die nicht gelöscht oder bearbeitet werden können, gehören die folgenden:

* [!UICONTROL Werbung]
* [!UICONTROL Beratung]
* [!UICONTROL Unterhaltung]
* [!UICONTROL Allgemein]
* [!UICONTROL Materialien]
* [!UICONTROL Reise]

## Benutzerdefinierte Ausgabentypen erstellen

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Ausgabentypen]**.
1. Klicken Sie **[!UICONTROL Neuer Ausgabentyp]**.
1. Geben Sie **[!UICONTROL Dialogfeld „Neuer]**&quot; die folgenden Informationen ein:

   * **Name** - Ein Name für die Ausgabe.
   * **Beschreibung** - Eine Beschreibung der Ausgabe.
   * **Berechnete Einheit** - Wählen Sie in der Dropdown-Liste die Maßeinheit für Ihren Ausgabentyp aus. Die folgenden Maßeinheiten sind verfügbar:

      * Meile
      * Kilometer
      * Kilogramm
      * Dollar
      * Hour
      * Day
      * Sonstiges - Wenn Sie diese Option wählen, werden Sie aufgefordert, die Maßeinheit zu benennen und diese als eine Ihrer Organisation vertraute Einheit zu definieren.

   * **Rate** - Der Preis pro Einheit. Dies ist ein währungsformatiertes Feld, das die Kosten für jede Einheit darstellt, die im Feld **Berechnete Einheit** festgelegt wird. Die Rate kann einen numerischen Wert mit bis zu 4 Zahlen nach dem Dezimaltrennzeichen enthalten. Beispiel: 1.0375.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Der Ausgabentyp steht jetzt Benutzenden zur Verfügung, um ihn mit ihren Ausgaben für Projekte und Aufgaben zu verknüpfen.

## Benutzerdefinierte Ausgabentypen ändern

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Ausgabentypen]**.
1. Wählen Sie den zu ändernden Ausgabentyp aus und klicken Sie dann auf das Symbol **[!UICONTROL Bearbeiten]** ![Symbol Bearbeiten](assets/edit-icon.png).

   Das **[!UICONTROL Ausgabentyp bearbeiten]** wird angezeigt.

1. Nehmen Sie die gewünschten Änderungen vor und klicken Sie dann auf **[!UICONTROL Speichern]**.

   Der Ausgabentyp steht jetzt Benutzenden zur Verfügung, um ihn mit ihren Ausgaben für Projekte und Aufgaben zu verknüpfen.

Weitere Informationen zur Verwendung von Ausgaben und dazu, wie sich diese auf die Kosten eines Projekts auswirken können, finden Sie im Artikel [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).
