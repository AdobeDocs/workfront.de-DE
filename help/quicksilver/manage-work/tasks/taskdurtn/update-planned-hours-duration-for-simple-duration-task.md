---
product-area: projects
navigation-topic: task-duration
title: Aktualisieren der geplanten Stunden und Dauer einer Aufgabe mit dem einfachen Typ Dauer
description: Standardmäßig berechnet Adobe Workfront die Dauer einer Aufgabe mit dem Typ Einfache Dauer basierend auf der geplanten Dauer. In bestimmten Bereichen von Workfront können Sie jedoch auch die geplante Stundenzeit und die Dauer einer einfachen Dauer manuell bearbeiten.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 1%

---

# Aktualisieren der geplanten Stunden und Dauer einer Aufgabe mit dem einfachen Typ Dauer

Standardmäßig berechnet Adobe Workfront die Dauer einer Aufgabe mit dem Typ Einfache Dauer basierend auf der geplanten Dauer. In bestimmten Bereichen von Workfront können Sie jedoch auch die geplante Stundenzeit und die Dauer einer einfachen Dauer manuell bearbeiten.

Sie können entweder die geplante Stunde und Dauer einer Aufgabe mit einem einfachen Dauer-Typ inline oder auf Aufgabenebene im Bereich &quot;Zuweisungen&quot;bearbeiten.

Weitere Informationen zum Bearbeiten von Informationen inline finden Sie unter [Inline-Bearbeitung von Elementen in einer Liste in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

In diesem Artikel wird beschrieben, wie Sie die geplante Stunde und Dauer für eine Aufgabe mit dem einfachen Typ Dauer auf Aufgabenebene im Bereich Zuweisungen aktualisieren können.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgabe verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aktualisieren der geplanten Stunden und Dauer einer Aufgabe mit dem einfachen Typ Dauer

>[!IMPORTANT]
>
>Nachdem Sie die Dauer einer Aufgabe mit einfacher Dauer manuell aktualisiert haben, stoppt Workfront die Berechnung anhand der geplanten Stunden.

So bearbeiten Sie im Feld &quot;Erweiterte Zuweisungen&quot;die geplante Stunde und Dauer einer Aufgabe mit einem einfachen Typ für die Dauer:

1. Klicken Sie in einer Aufgabenliste auf den Namen der Aufgabe, deren Dauer Sie ändern möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das Symbol **Mehr** ![](assets/qs-more-icon-on-an-object.png) neben dem Namen der Aufgabe, klicken Sie auf **Bearbeiten** und dann auf **Zuweisungen**.
   * Klicken Sie auf &quot;**Zugeordnet zu**&quot;oder auf den Namen der Zuweisungen im Bereich &quot;Zuweisungen&quot;der Aufgabenkopfzeile und klicken Sie dann auf &quot;**Erweitert**&quot;.

1. Geben Sie einen Gesamtwert für die **geplanten Stunden** für alle Zuweisungen ein, z. B. 10 Stunden. Die Gesamtzahl der geplanten Stunden wird gleichmäßig auf alle Ressourcen verteilt, die der Aufgabe zugewiesen sind.
1. (Optional) Passen Sie die geplanten Stunden jeder Ressource, die der Aufgabe zugewiesen ist, manuell an. Die Gesamtzahl der geplanten Stunden für die Aufgabe wird entsprechend den neuen Stunden aktualisiert, die Ihren Ressourcen zugewiesen sind.
1. Geben Sie einen Wert für die Aufgabe **Dauer** ein, z. B. 2 Tage.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Klicken Sie auf **Speichern**.
