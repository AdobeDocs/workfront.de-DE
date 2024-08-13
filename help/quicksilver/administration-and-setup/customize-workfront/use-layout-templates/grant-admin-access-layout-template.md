---
title: Administratorzugriff für eine Layout-Vorlage gewähren
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator können Sie den Gruppenadministratoren einer bestimmten Gruppe Administratorrechte für eine Layoutvorlage erteilen, damit sie die Vorlage bearbeiten können. Dadurch wird die Vorlage nicht den Benutzern in der Gruppe zugewiesen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 066a55ef-1904-4678-8866-c59428f78bc1
source-git-commit: a8214d9e10363881afbc2bd71f78f46cb6a25880
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# Administratorzugriff für eine Layoutvorlage gewähren

Als Adobe Workfront-Administrator können Sie den Gruppenadministratoren einer bestimmten Gruppe Administratorrechte für eine Layoutvorlage erteilen, damit sie die Vorlage bearbeiten können. Dadurch wird die Vorlage nicht den Benutzern in der Gruppe zugewiesen.

Weitere Informationen zum Zuweisen von Benutzern zu einer Layoutvorlage finden Sie unter [Zuweisen von Benutzern zu einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Layoutvorlagen für Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td><p>Systemadministratorzugriffsstufe</p><p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Administratorzugriff für eine Layoutvorlage gewähren

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie im oberen Abschnitt der Seite auf **Zugriff auf** gewähren.
1. Klicken Sie im angezeigten Feld auf **Gruppe hinzufügen**, geben Sie den Namen der Gruppe ein, klicken Sie auf den Namen, wenn er angezeigt wird, und klicken Sie dann auf **Fertig**.

   Alle Benutzer, die als Gruppenadministratoren für die von Ihnen festgelegte Gruppe bestimmt sind, können die Layoutvorlage verwalten. Die Vorlage wird jedoch nicht dem Gruppenmitglied für die Verwendung zugewiesen. Weitere Informationen zum Zuweisen einer Layoutvorlage zu einer Gruppe finden Sie unter [Zuweisen einer Layoutvorlage zu Benutzern](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md#assign) in diesem Artikel.

   >[!NOTE]
   >
   >* Wenn ein Gruppenadministrator eine Layoutvorlage erstellt, ist die Zuweisung des Administratorzugriffs obligatorisch. Die Layout-Vorlage ist für die angegebene Gruppe bestimmt und nur für diese sichtbar. Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). Informationen zu Gruppenadministratoren finden Sie unter [Gruppenadministratoren](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).
   >   
   >* Wenn Sie den Gruppenadministratoren einer bestimmten Gruppe keinen Administratorzugriff gewähren, haben alle Benutzer, die Benutzerkonten bearbeiten können, Administratorzugriff auf die Layoutvorlage. Einige Workfront-Administratoren haben die Absicht, keinen Administratorzugriff für eine Layoutvorlage zu gewähren, um sie zu einer Layoutvorlage auf Systemebene zu machen.

1. Sie können jederzeit auf Speichern klicken, um den Fortschritt zu speichern, und die Vorlage später weiter ändern.
