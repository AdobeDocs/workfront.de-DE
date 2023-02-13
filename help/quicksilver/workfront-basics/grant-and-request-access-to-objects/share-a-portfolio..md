---
title: Portfolio freigeben
description: Sie können ein Portfolio für andere Benutzer freigeben, wenn Sie über Zugriffsberechtigungen verfügen.
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: e608cf5bdb0227ea5b8d3109db411e98145aaa38
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 1%

---

# Portfolio freigeben

Ihr Adobe Workfront-Administrator kann Ihnen beim Zuweisen Ihrer Zugriffsebene Zugriff auf das Anzeigen oder Bearbeiten von Portfolios gewähren. Sie müssen über eine Planungslizenz verfügen, um Zugriff auf die Bearbeitung eines Portfolios zu erhalten. Weitere Informationen finden Sie unter [Zugriff auf Portfolios gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

Neben der Ihnen zugewiesenen Zugriffsebene können Sie auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Portfolios von Benutzern erhalten, die diese für Sie freigeben können. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Wie Zugriffsebenen und Berechtigungen zusammenarbeiten](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Berechtigungen beziehen sich auf ein Element in Workfront und definieren, welche Aktionen Benutzer für dieses Element ausführen können.

## Überlegungen zur Freigabe von Portfolios

Zusätzlich zu den unten stehenden Überlegungen siehe [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann allen Elementen im System Berechtigungen hinzufügen oder entfernen, ohne Eigentümer dieser Elemente zu sein.

* Der Ersteller eines Portfolios hat standardmäßig die Berechtigung &quot;Verwalten&quot;.
* Sie können ein Portfolio einzeln oder mehrere Portfolios gleichzeitig freigeben. Die Freigabe eines Portfolios entspricht der Freigabe anderer Objekte in Workfront. Weitere Informationen finden Sie unter [Objekt freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Sie können nur Ansichts- oder Verwaltungsberechtigungen für Portfolio erteilen.

   ![](assets/screen-shot-2014-01-23-at-12.45.15-pm.png)    ![](assets/screen-shot-2014-01-22-at-10.03.43-am-190x167.png)

* Wenn Sie ein Portfolio freigeben, erben Benutzer standardmäßig dieselben Berechtigungen für alle untergeordneten Objekte, die mit dem Portfolio verknüpft sind.

   Weitere Informationen zur Hierarchie von Objekten in Workfront finden Sie unter [Objekte in Adobe Workfront verstehen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Sie können geerbte Berechtigungen aus dem Portfolio entfernen. Weitere Informationen zum Entfernen von Berechtigungen von Objekten finden Sie unter [Berechtigungen aus Objekten entfernen](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Portfolio-Berechtigungen

Die folgende Tabelle zeigt, welche Berechtigungen Sie Benutzern gewähren können, wenn sie ein Portfolio anzeigen oder verwalten können:

| **Aktionen** | **Verwalten** | **Anzeigen** |
|---|---|---|
| Bearbeiten von Portfolio-Details | ✓ |   |
| Portfolio anzeigen | ✓ | ✓ |
| Portfolio löschen | ✓ |   |
| Anhängen eines benutzerdefinierten Formulars | ✓ |   |
| Benutzerdefiniertes Feld bearbeiten | ✓ |   |
| Programm hinzufügen oder entfernen&#42; | ✓ |   |
| Projekt hinzufügen oder entfernen&#42; | ✓ |   |
| Projekt genehmigen | ✓ |   |
| Portfolio-Optimierung&#42; | ✓ |   |
| Dokumentordner hinzufügen&#42; | ✓ | ✓ |
| Dokument hinzufügen | ✓ | ✓ |
| Aktualisierungen/Kommentare | ✓ | ✓ |
| Freigeben | ✓ | ✓ |
| Systemweit freigeben |   | ✓ |

*Diese Berechtigungen werden durch die Zugriffsebene und Berechtigungen für andere Objekte wie Projekte, Programme und Dokumente gesteuert.
