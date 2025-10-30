---
title: Gewähren von administrativem Zugriff für eine Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator können Sie Gruppenadministratoren einer bestimmten Gruppe administrativen Zugriff für eine Layout-Vorlage gewähren, damit sie die Vorlage bearbeiten können. Dadurch wird die Vorlage nicht den Benutzenden in der Gruppe zugewiesen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 0%

---

# Gewähren von administrativem Zugriff für eine Layout-Vorlage

{{preview-fast-release-general}}

Als Adobe Workfront-Administrator können Sie Gruppenadministratoren einer bestimmten Gruppe administrativen Zugriff für eine Layout-Vorlage gewähren, damit sie die Vorlage bearbeiten können. Dadurch wird die Vorlage nicht den Benutzenden in der Gruppe zugewiesen.

Informationen zum Zuweisen von Benutzern zu einer Layout-Vorlage finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Weitere Informationen zu Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.</p>
        <p>Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gewähren von administrativem Zugriff für eine Layout-Vorlage

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken **im oberen Bereich** Seite auf „Zugriff gewähren auf“.
1. Klicken Sie im angezeigten Feld auf **Gruppe hinzufügen**, geben Sie den Namen der Gruppe ein, klicken Sie auf den Namen, wenn er angezeigt wird, und klicken Sie dann auf **Fertig**.

   Alle Benutzer, die als Gruppenadministratoren für die von Ihnen angegebene Gruppe festgelegt wurden, können die Layout-Vorlage verwalten. Die Vorlage wird jedoch nicht den Mitgliedern der Gruppe für ihre Verwendung zugewiesen. Informationen zum Zuweisen einer Layout-Vorlage zu einer Gruppe finden Sie unter [Zuweisen einer Layout-Vorlage zu ](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) in diesem Artikel.

   >[!NOTE]
   >
   >* Wenn ein(e) Gruppen-Administrator(in) eine Layout-Vorlage erstellt, muss der Administratorzugriff zugewiesen werden. Die Layout-Vorlage ist für die angegebene Gruppe vorgesehen und nur für diese sichtbar. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). Informationen zu Gruppenadministratoren finden Sie unter [Gruppenadministratoren](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* Wenn Sie den Gruppenadministratoren in einer bestimmten Gruppe keinen administrativen Zugriff gewähren, haben alle Benutzer, die Benutzerkonten bearbeiten können, administrativen Zugriff auf die Layout-Vorlage. Einige Workfront-Administratoren entscheiden sich absichtlich dafür, keinen administrativen Zugriff auf eine Layout-Vorlage zu gewähren, um sie zu einer Layout-Vorlage auf Systemebene zu machen.

1. Sie können jederzeit auf <span class="preview">**Anwenden**</span> oder **Speichern** klicken, um Ihren Fortschritt zu speichern, und dann später mit dem Ändern der Vorlage fortfahren.
