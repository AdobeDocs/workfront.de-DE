---
title: Erstellen von Workfront-Objekten mit der Workfront-Planungs-Datensatzautomatisierung
description: Sie können Automatisierungen in der Workfront-Planung konfigurieren, die bei Aktivierung Objekte in Workfront erstellen.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
source-git-commit: bac3ed2a169e070b541192ab312d4fc1a1b467d1
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# Erstellen von Workfront-Objekten mit der Workfront-Planungs-Datensatzautomatisierung

Sie können Automatisierungen in der Workfront-Planung konfigurieren, die bei Aktivierung Objekte in Workfront erstellen.

Sie aktivieren die Automatisierung in Datensätzen. Das Objekt in Workfront ist mit dem Planungsdatensatz verbunden, in dem Sie die Automatisierung aktiviert haben.

Sie können beispielsweise eine Automatisierung erstellen, die eine Workfront-Planungs-Kampagne durchführt und in Workfront ein Projekt erstellt, um den Fortschritt dieser Kampagne zu verfolgen. Das Projekt würde mit der Workfront-Planungskampagne verbunden sein.

Weitere Informationen zu verbundenen Datensätzen finden Sie unter [Übersicht über verbundene Datensätze](/help/quicksilver/planning/records/connected-records-overview.md).


## Automatisierung in der Workfront-Planung konfigurieren

Sie müssen eine Automatisierung in der Workfront-Planung konfigurieren, bevor Sie sie zum Erstellen von Workfront-Objekten verwenden können.

1. Klicken Sie auf das Menü **Mehr** ![](assets/more-menu.png) und wählen Sie **Automatisierungen** aus.

   Die Liste der verfügbaren Automatisierungen wird geöffnet.

1. Klicken Sie oben rechts im Bildschirm auf **Neue Automatisierung erstellen** .
1. Geben Sie im Feld **Schaltflächentext** den Text ein, der auf der Schaltfläche angezeigt werden soll. Benutzer klicken auf diese Schaltfläche, wenn sie die Automatisierung zum Erstellen eines Workfront-Objekts verwenden.
1. (Optional) Um der Schaltfläche ein Symbol hinzuzufügen, wählen Sie ein Symbol aus den verfügbaren Optionen aus.
1. Wählen Sie im Feld **Einen Typ von** erstellen das Objekt aus, das durch die Automatisierung erstellt werden soll.

   Verfügbare Objekte sind:

   * Projekt
   * Portfolio
   * Programm
   * Gruppe

1. Wählen Sie im Feld **Wählen Sie das Feld aus, das im Feld &quot;Projektname&quot;** verwendet werden soll, ein Datensatzfeld aus. Für das neue Projekt in Workfront werden die Inhalte dieses Felds als Name verwendet.
1. Wählen Sie im Feld **Wählen Sie das Feld aus, mit dem das erstellte Projekt verknüpft werden soll**, ein Datensatzfeld aus. Das neue Projekt in Workfront wird in diesem Feld angezeigt, wenn der Datensatz in der Workfront-Planung angezeigt wird.
1. Wählen Sie für den Typ des zu erstellenden Objekts andere Optionen aus.
1. Klicken Sie auf **Erstellen**

Die Automatisierung wird in der Liste der Automatisierungen angezeigt und kann in Datensätzen verwendet werden.

## Verwenden einer Workfront-Planungs-Automatisierung zum Erstellen eines Workfront-Objekts

1. Öffnen Sie in der Workfront-Planung die Seite &quot;Record Type&quot;, die die Datensätze enthält, die Sie zum Erstellen von Workfront-Objekten verwenden möchten.
1. Wählen Sie mindestens einen Datensatz aus.
1. Klicken Sie unten rechts im Bildschirm auf die Schaltfläche Automatisierung .

   In diesem Beispiel handelt es sich um die Schaltfläche Projekt erstellen .

   ![Automatisierungsschaltfläche](assets/automation-custom-button.png)

>[!NOTE]
>
>Es wird empfohlen, zu überprüfen, ob das Objekt erwartungsgemäß erstellt und verbunden wurde.
