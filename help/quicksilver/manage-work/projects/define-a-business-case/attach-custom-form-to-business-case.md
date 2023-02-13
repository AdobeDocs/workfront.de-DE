---
navigation-topic: business-case-and-scorecards
title: Anhängen eines benutzerdefinierten Formulars an einen Geschäftsfall
description: Benutzerdefinierter Forms wird verwendet, um Informationen zu erfassen, die nicht in vorhandenen Adobe Workfront-Feldern angezeigt werden.
author: Alina
feature: Work Management
exl-id: f781fd00-968c-4e5d-b82c-a74acedb2734
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# Anhängen eines benutzerdefinierten Formulars an einen Geschäftsfall

Benutzerdefinierter Forms wird verwendet, um Informationen zu erfassen, die nicht in vorhandenen Adobe Workfront-Feldern angezeigt werden. 

Weitere Informationen zum Erstellen von benutzerdefinierten Forms finden Sie im Artikel [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt verwalten oder höher</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Anhängen benutzerdefinierter Forms an Projekte

Sie können benutzerdefinierte Forms in den folgenden Bereichen an ein Projekt anhängen:

* Beim Bearbeiten eines Projekts im Abschnitt Projektdetails .
* Beim Bearbeiten eines Projekts im Feld Projekt bearbeiten .
* Beim Massenbearbeitung mehrerer Projekte aus einer Liste von Projekten.

   Informationen zum Anhängen von benutzerdefinierten Formularen an Projekte beim Bearbeiten eines oder mehrerer Projekte finden Sie im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

* Beim Erstellen des Geschäftsfalls eines Projekts im Geschäftsfall, wie in diesem Artikel beschrieben.

Weitere Informationen zum Anhängen von benutzerdefinierten Formularen an Objekte finden Sie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Anhängen von benutzerdefiniertem Forms an den Geschäftsfall

Um einem Geschäftsfall eine benutzerdefinierte Option von hinzuzufügen, muss Ihr Workfront-Administrator diese Option unter &quot;Einrichtung&quot;auswählen. Weitere Informationen zum Aktivieren benutzerdefinierter Formulare in der Einrichtung finden Sie im Abschnitt . [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) im Artikel [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

So fügen Sie ein benutzerdefiniertes Formular hinzu:

1. Wechseln Sie zu dem Projekt, an das Sie das Formular anhängen möchten, und klicken Sie dann auf **Geschäftsfall** im linken Bereich.

   Der Geschäftsfall wird angezeigt.

1. Im **Benutzerdefiniertes Formular** wählen Sie im Dropdown-Menü das benutzerdefinierte Formular aus, das Sie anhängen möchten.

   ![](assets/custom-forms-drop-down-menu.png)

1. (Optional) Wählen Sie **Benutzerdefiniertes Formular bearbeiten**.\
   ![](assets/acf1-350x122.png)

1. (Optional) Geben Sie Informationen in die Felder des benutzerdefinierten Formulars ein und klicken Sie dann auf **Speichern** .
