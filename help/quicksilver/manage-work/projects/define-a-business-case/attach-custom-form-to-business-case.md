---
navigation-topic: business-case-and-scorecards
title: Anhängen eines benutzerdefinierten Formulars an einen Business Case
description: Benutzerdefinierte Forms werden verwendet, um Informationen zu erfassen, die in bestehenden Adobe Workfront-Feldern nicht angezeigt werden.
author: Alina
feature: Work Management
exl-id: f781fd00-968c-4e5d-b82c-a74acedb2734
source-git-commit: f21fd0761d942916039f6364e62f489a07217bfe
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# Anhängen eines benutzerdefinierten Formulars an einen Business Case

Benutzerdefinierte Forms werden verwendet, um Informationen zu erfassen, die in bestehenden Adobe Workfront-Feldern nicht angezeigt werden. 

Weitere Informationen zum Erstellen benutzerdefinierter Forms finden Sie im Artikel [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen oder höher für das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Benutzerdefinierte Forms an Projekte anhängen

Sie können benutzerdefinierte Forms in den folgenden Bereichen an ein Projekt anhängen:

* Beim Bearbeiten eines Projekts im Abschnitt Projektdetails .
* Beim Bearbeiten eines Projekts im Feld Projekt bearbeiten .
* Beim Massenbearbeiten mehrerer Projekte aus einer Liste von Projekten.

  Informationen zum Anhängen benutzerdefinierter Formulare an Projekte während der Bearbeitung eines oder mehrerer Projekte finden Sie im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

* Beim Erstellen des Business Case eines Projekts, im Business Case, wie in diesem Artikel beschrieben.

Informationen zum Anhängen benutzerdefinierter Formulare an Objekte finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Benutzerdefinierte Forms an den Business Case anhängen

Um ein benutzerdefiniertes Formular zu einem Business Case hinzuzufügen, muss der Workfront-Administrator diese Option in „Setup“ auswählen. Weitere Informationen zur Aktivierung benutzerdefinierter Formulare im Setup finden Sie im Abschnitt [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) im Artikel [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

So fügen Sie ein benutzerdefiniertes Formular hinzu:

1. Gehen Sie zu dem Projekt, an das Sie das Formular anhängen möchten, und klicken Sie dann **linken Bereich** Business Case“.

   Der Business Case wird angezeigt.

1. Wählen **Abschnitt „Benutzerdefiniertes Formular** aus dem Dropdown-Menü das benutzerdefinierte Formular aus, das Sie anhängen möchten.

   ![Benutzerdefinierte Formulare - Dropdown](assets/custom-forms-drop-down-menu.png)

1. (Optional) Wählen Sie **Benutzerdefiniertes Formular bearbeiten** aus.\
   ![Benutzerdefiniertes Formular bearbeiten](assets/acf1-350x122.png)

1. (Optional) Geben Sie Informationen in die Felder des benutzerdefinierten Formulars ein und klicken Sie dann auf **Speichern** .
