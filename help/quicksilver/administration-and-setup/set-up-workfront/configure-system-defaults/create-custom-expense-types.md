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
source-git-commit: ff4a9b317bd75b298a7a39814b4ae265c92c6d2a
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

---

# Benutzerdefinierte Ausgabentypen erstellen

{{highlighted-preview}}

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] können Sie benutzerdefinierte Ausgabentypen erstellen, um die mit Ihren Aufgaben und Projekten verbundenen Ausgaben zu definieren und zu verfolgen. Kosten sind sonstige Kosten, die mit Aufgaben oder Projekten verbunden werden können.

Sie können alle von Ihnen erstellten Ausgabentypen bearbeiten oder löschen. Die integrierten Ausgabentypen [!DNL Workfront] können nicht gelöscht oder bearbeitet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td><p>Neu: [!UICONTROL Standard]</p>
   Oder
   <p>Aktuell: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Standardausgabentypen

Zu den standardmäßigen Ausgabentypen in [!DNL Workfront], die nicht gelöscht oder bearbeitet werden können, gehören die folgenden:

* [!UICONTROL Advertising]
* [!UICONTROL Beratung]
* [!UICONTROL Unterhaltung]
* [!UICONTROL Allgemein]
* [!UICONTROL Materialien]
* [!UICONTROL Reise]

## Benutzerdefinierte Ausgabentypen erstellen

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Ausgabentypen]**.
1. Klicken Sie **[!UICONTROL Neuer Ausgabentyp]**.
1. Geben **[!UICONTROL im Dialogfeld „Neuer]**&quot; die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Geben Sie einen Namen für die Ausgabe an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beschreibung]</td> 
      <td>Geben Sie eine Beschreibung für die Ausgabe an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Berechnete Einheit]</td> 
      <td> <p>Wählen Sie die Maßeinheit für Ihren Ausgabentyp aus der Dropdown-Liste aus.</p> <p>Folgende Maßeinheiten sind verfügbar:</p> 
       <ul> 
        <li>Meile</li> 
        <li>Kilometer</li> 
        <li>Kilogramm</li> 
        <li>Dollar</li> 
        <li>Dollar</li> 
        <li>Tag</li> 
        <li>Sonstiges - Wenn Sie diese Option wählen, werden Sie aufgefordert, die Maßeinheit zu benennen und diese als eine Ihrer Organisation vertraute Einheit zu definieren.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rate</td> 
      <td> <p>Geben Sie den Preis pro Einheit an. Dies ist ein währungsformatiertes Feld, das die Kosten für jede Einheit darstellt, die im Feld <strong>[!UICONTROL Berechnete Einheit]</strong> festgelegt wird. </p> <p>Die Rate kann einen numerischen Wert mit bis zu 4 Zahlen nach dem Dezimaltrennzeichen enthalten. Beispiel: 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Ausgabentyp erstellen** <span class="preview">oder **[!UICONTROL Speichern]**.</span>

   Der Ausgabentyp steht jetzt Benutzenden zur Verfügung, um ihn mit ihren Ausgaben für Projekte und Aufgaben zu verknüpfen.

## Benutzerdefinierte Ausgabentypen ändern

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Ausgabentypen]**.
1. Wählen Sie den zu ändernden Ausgabentyp aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

   Das **[!UICONTROL Ausgabentyp bearbeiten]** wird angezeigt.

1. Nehmen Sie die gewünschten Änderungen vor und klicken Sie dann auf **Änderungen speichern** <span class="preview">oder **[!UICONTROL Speichern]**.</span>

   Der Ausgabentyp steht jetzt Benutzenden zur Verfügung, um ihn mit ihren Ausgaben für Projekte und Aufgaben zu verknüpfen.

Weitere Informationen zur Verwendung von Ausgaben und dazu, wie sich diese auf die Kosten eines Projekts auswirken können, finden Sie im Artikel [Verwalten von Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md).
