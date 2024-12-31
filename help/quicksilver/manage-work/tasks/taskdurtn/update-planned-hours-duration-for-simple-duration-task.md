---
product-area: projects
navigation-topic: task-duration
title: Geplante Stunden und Dauer einer Aufgabe mit einem einfachen Dauertyp aktualisieren
description: Standardmäßig berechnet Adobe Workfront die Dauer einer Aufgabe mit einem einfachen Dauertyp auf der Grundlage der geplanten Stunden. Sie können jedoch in bestimmten Bereichen von Workfront auch manuell die Anzahl der geplanten Stunden und die Dauer einer Aufgabe vom Typ Einfache Dauer bearbeiten.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 1%

---

# Geplante Stunden und Dauer einer Aufgabe mit einem einfachen Dauertyp aktualisieren

Standardmäßig berechnet Adobe Workfront die Dauer einer Aufgabe mit einem einfachen Dauertyp auf der Grundlage der geplanten Stunden. Sie können jedoch in bestimmten Bereichen von Workfront auch manuell die Anzahl der geplanten Stunden und die Dauer einer Aufgabe vom Typ Einfache Dauer bearbeiten.

Sie können „Geplante Stunden“ und „Dauer“ einer Aufgabe mit einem einfachen Dauertyp entweder inline oder auf Aufgabenebene im Bereich „Zuweisungen“ bearbeiten.

Weitere Informationen zur Inline-Bearbeitung von Informationen finden Sie unter [Inline-Bearbeitung von Elementen in einer Liste in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

In diesem Artikel wird beschrieben, wie Sie die geplanten Stunden und die Dauer für eine Aufgabe mit einem einfachen Dauertyp auf Aufgabenebene im Bereich Zuweisungen aktualisieren können.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgabe</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Geplante Stunden und Dauer einer Aufgabe mit einem einfachen Dauertyp aktualisieren

>[!IMPORTANT]
>
>Nachdem Sie die Dauer für eine Aufgabe vom Typ Einfache Dauer manuell aktualisiert haben, berechnet Workfront sie nicht mehr anhand der geplanten Stunden.

So bearbeiten Sie die geplanten Stunden und die Dauer einer Aufgabe mit einem einfachen Dauertyp im Feld Erweiterte Zuweisungen:

1. Klicken Sie in einer Aufgabenliste auf den Namen der Aufgabe, für die Sie den Dauertyp ändern möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das **Mehr**-Symbol ![](assets/qs-more-icon-on-an-object.png) neben dem Namen der Aufgabe, klicken Sie auf **Bearbeiten** und dann auf **Arbeitsaufträge**.
   * Klicken Sie auf **Zugewiesen an** oder den Namen der Zuweisungen im Bereich „Zuweisungen“ der Aufgabenkopfzeile und dann auf **Erweitert**.

1. Geben Sie einen Gesamtwert für die **geplanten Stunden** für alle Zuweisungen ein, z. B. 10 Stunden. Die Gesamtzahl der geplanten Stunden wird gleichmäßig auf alle Ressourcen aufgeteilt, die der Aufgabe zugewiesen sind.
1. (Optional) Passen Sie die geplanten Stunden für jede Ressource, die der Aufgabe zugewiesen wurde, manuell an. Die Gesamtzahl der geplanten Stunden für die Aufgabe wird aktualisiert, um die neuen Stunden widerzuspiegeln, die Ihren Ressourcen einzeln zugewiesen wurden.
1. Geben Sie einen Wert für die Aufgabe **Dauer** ein, z. B. 2 Tage.

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Klicken Sie auf **Speichern**.
