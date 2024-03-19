---
title: Übertragen benutzerdefinierter Formulardaten beim Konvertieren eines Objekts
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wenn die in einem Arbeitselement definierte Arbeit zu groß wird, können Sie sie in ein größeres Arbeitselement konvertieren.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Übertragen benutzerdefinierter Formulardaten beim Konvertieren eines Objekts

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnelle Versionen für Ihre Organisation aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Übersicht über die Version 2024 im zweiten Quartal](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Je nach den Geschäftsanforderungen Ihrer Organisation kann die in einer Aufgabe oder einem Problem definierte Arbeit für die Verwaltung innerhalb der Aufgabe oder des Problems zu groß werden. In diesem Fall können Sie sie in ein größeres Arbeitselement konvertieren:

* Sie können Probleme in Aufgaben oder Projekte konvertieren
* Sie können Aufgaben in Projekte konvertieren

Um benutzerdefinierte Formulardaten von einem Problem an eine Aufgabe oder ein Projekt zu übertragen, müssen Sie die beiden Aufgaben in diesem Artikel in der folgenden Reihenfolge ausführen.

Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) oder [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Abo</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Zuerst: Fügen Sie dem benutzerdefinierten Formular weitere Objekte hinzu

{{step-1-to-setup}}

1. Klicks **Benutzerdefinierte Forms**.
1. Suchen Sie das gewünschte Formular und klicken Sie auf **Bearbeiten** <span class="preview">oder ![Symbol Bearbeiten](assets/edit-icon.png).</span>
1. Fügen Sie oben im Formular das Objekt hinzu, in das Sie die Aufgabe oder das Problem konvertieren möchten.

   >[!INFO]
   >
   >**Beispiel**: Wenn Sie die benutzerdefinierten Formulardaten an ein Projekt übertragen möchten, wählen Sie Projekt aus.

1. Klicks **Anwenden** unten im Formular.

1. Fahren Sie mit [Zweitens: Konvertieren Sie das Problem oder die Aufgabe und übertragen Sie die benutzerdefinierten Formulardaten](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Zweitens: Konvertieren Sie das Problem oder die Aufgabe und übertragen Sie die benutzerdefinierten Formulardaten {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Fügen Sie dem benutzerdefinierten Formular zusätzliche Objekte zu dem Problem oder der Aufgabe hinzu, das/die Sie konvertieren, wie im Abschnitt beschrieben. [Zuerst: Fügen Sie dem benutzerdefinierten Formular weitere Objekte hinzu](#first-add-additonal-objects-to-the-custom-form) in diesem Artikel.
1. Konvertieren Sie das Problem oder die Aufgabe mithilfe des **Benutzerdefinierte Forms** in dem Feld, das angezeigt wird, um das gewünschte benutzerdefinierte Formular auszuwählen. Anweisungen finden Sie in den folgenden Artikeln:

   * [Konvertieren eines Problems in ein Projekt in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Konvertieren eines Problems in eine Aufgabe in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Konvertieren einer Aufgabe in ein Projekt](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. Im **Konvertieren in (Objekttyp)** angezeigt wird, klicken Sie auf das **Forms hinzufügen** und wählen Sie das Formular aus, das Sie im vorherigen Abschnitt kopiert haben.

   Die in den benutzerdefinierten Feldern des Problems erfassten Informationen werden jetzt in das benutzerdefinierte Formular für die Aufgabe übertragen.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see the section [Start editing a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) in the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Custom Forms**.
1. Select the task- or issue-type custom form, then click **Copy**.
1. In the **Custom Form** dialog box, specify a name for the new form.  

1. From the **Form Type** drop-down menu, select the type of object you want to create the new custom form for

   **Example:** If you want to transfer the custom form data to a project, select Project.

1. Click **Copy Form**.

   This copied custom form can now be attached to a task or project.

1. Continue on to [Second: Convert the issue or task and transfer the custom form data](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).
-->