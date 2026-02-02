---
product-area: projects
navigation-topic: task-duration
title: Geplante Stunden und Dauer einer Aufgabe mit einem einfachen Dauertyp aktualisieren
description: Standardmäßig berechnet Adobe Workfront die Dauer einer Aufgabe mit einem einfachen Dauertyp auf der Grundlage der geplanten Stunden. Sie können jedoch in bestimmten Bereichen von Workfront auch manuell die Anzahl der geplanten Stunden und die Dauer einer Aufgabe vom Typ Einfache Dauer bearbeiten.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '450'
ht-degree: 6%

---

# Geplante Stunden und Dauer einer Aufgabe mit einem einfachen Dauertyp aktualisieren

Standardmäßig berechnet Adobe Workfront die Dauer einer Aufgabe mit einem einfachen Dauertyp auf der Grundlage der geplanten Stunden. Sie können jedoch in bestimmten Bereichen von Workfront auch manuell die Anzahl der geplanten Stunden und die Dauer einer Aufgabe vom Typ Einfache Dauer bearbeiten.

Sie können „Geplante Stunden“ und „Dauer“ einer Aufgabe mit einem einfachen Dauertyp entweder inline oder auf Aufgabenebene im Bereich „Zuweisungen“ bearbeiten.

Weitere Informationen zur Inline-Bearbeitung von Informationen finden Sie unter [Inline-Bearbeitung von Elementen in einer Liste in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

In diesem Artikel wird beschrieben, wie Sie die geplanten Stunden und die Dauer für eine Aufgabe mit einem einfachen Dauertyp auf Aufgabenebene im Bereich Zuweisungen aktualisieren können.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard oder höher</p> 
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p> <p>Zugriff auf Aufgaben bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf die Aufgabe verwalten </p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Geplante Stunden und Dauer einer Aufgabe mit einem einfachen Dauertyp aktualisieren

>[!IMPORTANT]
>
>Nachdem Sie die Dauer für eine Aufgabe vom Typ Einfache Dauer manuell aktualisiert haben, berechnet Workfront sie nicht mehr anhand der geplanten Stunden.

So bearbeiten Sie die geplanten Stunden und die Dauer einer Aufgabe mit einem einfachen Dauertyp im Feld Erweiterte Zuweisungen:

1. Klicken Sie in einer Aufgabenliste auf den Namen der Aufgabe, für die Sie den Dauertyp ändern möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das **Mehr**-Symbol ![Mehr-Symbol auf einem Objekt](assets/qs-more-icon-on-an-object.png) neben dem Namen der Aufgabe, klicken Sie auf **Bearbeiten** dann auf **Zuweisungen**.
   * Klicken Sie auf **Zugewiesen an** oder den Namen der Zuweisungen im Bereich „Zuweisungen“ der Aufgabenkopfzeile und dann auf **Erweitert**.

1. Geben Sie einen Gesamtwert für die **geplanten Stunden** für alle Zuweisungen ein, z. B. 10 Stunden. Die Gesamtzahl der geplanten Stunden wird gleichmäßig auf alle Ressourcen aufgeteilt, die der Aufgabe zugewiesen sind.
1. (Optional) Passen Sie die geplanten Stunden für jede Ressource, die der Aufgabe zugewiesen wurde, manuell an. Die Gesamtzahl der geplanten Stunden für die Aufgabe wird aktualisiert, um die neuen Stunden widerzuspiegeln, die Ihren Ressourcen einzeln zugewiesen wurden.
1. Geben Sie einen Wert für die Aufgabe **Dauer** ein, z. B. 2 Tage.

   ![Erweiterte Zuweisungen Einfache Dauer Mehrere Ressourcen](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Klicken Sie auf **Speichern**.
