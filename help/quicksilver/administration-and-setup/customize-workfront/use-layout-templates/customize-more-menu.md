---
title: Anpassen des Menüs Mehr mithilfe einer Layout-Vorlage
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: 'Sie können eine Layout-Vorlage verwenden, um die Optionen zu bestimmen, die angezeigt werden, wenn Benutzende auf das Menü Mehr (das Dreipunkt-Menü) klicken, während sie die folgenden Objekte in Adobe Workfront anzeigen: Projekte, Aufgaben, Probleme, Portfolios und Programme.'
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 2faeea4f8128b7858232048d687c270a1e3709f5
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 10%

---

# Anpassen des Menüs Mehr mithilfe einer Layout-Vorlage

{{highlighted-preview-article-level}}

Sie können eine Layout-Vorlage verwenden, um die Optionen zu bestimmen, die angezeigt werden, wenn Benutzende auf das Menü Mehr (das Dreipunkt-Menü) klicken, während sie die folgenden Objekte in Adobe Workfront anzeigen: Projekte, Aufgaben, Probleme, Portfolios und Programme.

![Beispielmenü „Mehr“ für ein Projekt](assets/more-menu-display-for-project.png)

Informationen zum Erstellen von Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [&#x200B; unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layout-Vorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die von Ihnen vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layout-Vorlage an Benutzer finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.</p>
        <p>Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Anpassen des Menüs Mehr für einen Bereich in Workfront

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie **Dropdown-Menü Anpassen, was Benutzer sehen** auf den Namen eines Objekttyps oder eines Workfront-Bereichs, dessen Menü „Mehr“ Sie anpassen möchten.
1. Klicken Sie **Menüoptionen auswählen**.
1. Führen Sie im Feld **Menüoptionen auswählen** einen der folgenden Schritte aus, um zu bestimmen, was Benutzende im Menü Mehr für den ausgewählten Workfront-Bereich oder -Objekttyp sehen werden:

   * Klicken Sie auf **Anzeigen** ![Symbol anzeigen](assets/add-secondary-nav-item.png) oder **Ausblenden** ![Symbol ausblenden](assets/delete-secondary-nav-item.png), um Abschnitte im linken Bereich ein- oder auszublenden. Sie können keine Elemente ausblenden, die kein Symbol **Anzeigen** oder **Ausblenden** aufweisen.

   * Ziehen Sie Elemente ![Symbol Verschieben](assets/move-icon---dots.png), um ihre Reihenfolge im linken Bedienfeld zu ändern.

1. Klicken Sie auf **Fertig**.
