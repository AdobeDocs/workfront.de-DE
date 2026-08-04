---
user-type: administrator
product-area: system-administration;setup
title: Zu verfolgende Felder im Änderungsverlauf konfigurieren
description: Als Workfront-Administrator können Sie konfigurieren, welche Objektfelder und Aktionen Workfront verfolgt.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 71bd341da0b506429ab25726ae3be82829034f9f
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 9%

---

# Felder konfigurieren, die im Änderungsverlauf verfolgt werden sollen

{{highlighted-preview-article-level}}

Adobe Workfront generiert automatische Systemaktualisierungen, um die folgenden Ereignisse aufzuzeichnen:

* Änderungen, die Benutzer in einem Objektfeld vornehmen
* Aktionen, die Benutzer für ein Objekt ausführen

Diese Systemaktualisierungen enthalten die folgenden Informationen:

* Die vorgenommene Änderung
* Der Name des Benutzers, der die Änderung vorgenommen hat
* Uhrzeit und Datum der Änderung

Als Workfront-Administrator können Sie konfigurieren, welche Objektfelder und Aktionen Workfront verfolgt.

Sie können beispielsweise Workfront alle Änderungen nachverfolgen lassen, die Benutzer an den Namen von Problemen im gesamten System vornehmen. Jede Änderung des Problemnamens wird dann als Eintrag im Änderungsprotokoll angezeigt. Weitere Informationen finden Sie unter [Anzeigen und Verwalten des &#x200B;](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-manage-change-history.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Beschränkungen beim Feld-Tracking

Die Beschränkungen für die Anzahl der Felder, die Sie verfolgen können, werden durch Ihr Workfront-Paket definiert.

| Workfront-Paket | Maximale Anzahl an getrackten Feldern |
|---------|----------|
| Auswählen | 700 |
| Prime | 3000 |
| Ultimate | 5000 |
| Workflow Select | 1000 |
| Workflow Prime | 5000 |
| Workflow Ultimate | Unbegrenzt |

## Felder hinzufügen, die verfolgt werden sollen

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Tracking ändern > Konfiguration**.
1. Klicken Sie im Konfigurationsbildschirm auf **Feld hinzufügen**.
1. Wählen **im Feld „Felder**&quot; ein Objekt aus. Sie können mit der Eingabe des Objektnamens beginnen und ihn dann auswählen, wenn er in der Liste angezeigt wird.
1. Wählen Sie als Nächstes die Feldnamen aus, die Sie für dieses Objekt verfolgen möchten. Sie können mit der Eingabe des Feldnamens beginnen und ihn dann auswählen, wenn er in der Liste angezeigt wird.

   Für das Objekt sind sowohl benutzerdefinierte Felder als auch native Felder verfügbar.
   Bereits getrackte Felder werden wie in der Liste ausgewählt angezeigt.

   ![Felder für die Änderungsnachverfolgung hinzufügen](assets/change-history-config-add-fields.png)

1. Nachdem Sie alle Felder ausgewählt haben, die Sie nachverfolgen möchten, klicken Sie auf **Hinzufügen**.

   Die Felder werden der Liste Getrackte Felder hinzugefügt.

## Felder entfernen, die nicht mehr verfolgt werden sollen

Sie können Felder entfernen, die das System nicht für einen bestimmten Objekttyp über die Workfront-Benutzeroberfläche verfolgen soll.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Tracking ändern > Konfiguration**.
1. Wählen Sie im Konfigurationsbildschirm das Feld bzw. die Felder aus, die Sie nicht mehr verfolgen möchten.

   Möglicherweise wird derselbe Feldname mehrmals angezeigt. Die Felder werden nach Objekt gruppiert, sodass Sie das richtige Feld finden können. Sie können auch das Suchfeld oben auf dem Bildschirm verwenden.

1. Wählen **Löschen** in der Aktionsleiste am unteren Bildschirmrand aus.
1. Klicken Sie **der Bestätigungsmeldung** Entfernen“.

   Die Felder werden aus der Liste Getrackte Felder entfernt.


