---
title: Übertragen von benutzerdefinierten Formulardaten beim Konvertieren eines Objekts
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wenn die in einem Arbeitselement definierte Arbeit zu groß wird, können Sie es in ein größeres Arbeitselement konvertieren.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Übertragen von benutzerdefinierten Formulardaten beim Konvertieren eines Objekts

Je nach den Geschäftsanforderungen Ihres Unternehmens kann die in einer Aufgabe oder einem Problem definierte Arbeit zu groß werden, um innerhalb der Aufgabe oder des Problems verwaltet werden zu können. In diesem Fall können Sie sie in ein größeres Arbeitselement konvertieren:

* Sie können Probleme in Aufgaben oder Projekte konvertieren
* Sie können Aufgaben in Projekte konvertieren

Um benutzerdefinierte Formulardaten von einem Problem in eine Aufgabe oder ein Projekt zu übertragen, müssen Sie die beiden Aufgaben in diesem Artikel in der folgenden Reihenfolge ausführen.

Weitere Informationen finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md) oder [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront-Plan</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstens: Hinzufügen zusätzlicher Objekte zum benutzerdefinierten Formular

{{step-1-to-setup}}

1. Klicken Sie **Benutzerdefinierte Forms**.
1. Suchen Sie das gewünschte Formular und klicken Sie auf ![Bearbeiten-Symbol](assets/edit-icon.png).
1. Fügen Sie oben im Formular das Objekt hinzu, in das Sie die Aufgabe oder das Problem konvertieren möchten.

   >[!INFO]
   >
   >**Beispiel**: Wenn Sie die benutzerdefinierten Formulardaten in ein Projekt übertragen möchten, wählen Sie „Projekt“ aus.

1. Klicken **unten** Formular auf „Anwenden“.

1. Fahren Sie fort mit [Sekunde: Konvertieren Sie das Problem oder die Aufgabe und übertragen Sie die benutzerdefinierten Formulardaten](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Zweitens: Konvertieren des Problems oder der Aufgabe und Übertragen der benutzerdefinierten Formulardaten {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Fügen Sie dem benutzerdefinierten Formular für das Problem oder die Aufgabe, das bzw. die Sie konvertieren, zusätzliche Objekte hinzu, wie in Abschnitt [Erste: Hinzufügen zusätzlicher Objekte zum benutzerdefinierten Formular](#first-add-additonal-objects-to-the-custom-form) in diesem Artikel erläutert.
1. Konvertieren Sie das Problem oder die Aufgabe mithilfe **Option „Benutzerdefinierte Forms** in dem Feld, das angezeigt wird, um das gewünschte benutzerdefinierte Formular auszuwählen. Anweisungen finden Sie in den folgenden Artikeln:

   * [Konvertieren eines Problems in ein Projekt in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Konvertieren eines Problems in eine Aufgabe in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Konvertieren einer Aufgabe in ein Projekt](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. Klicken Sie **angezeigten Dialogfeld** In (Objekttyp) auf das Dropdown-Menü **Forms hinzufügen** und wählen Sie das Formular aus, das Sie im vorherigen Abschnitt kopiert haben.

   Die in den benutzerdefinierten Feldern des Problems erfassten Informationen werden jetzt in das benutzerdefinierte Formular für die Aufgabe übertragen.


<!--
## First: Copy the custom form {#first-copy-the-custom-form}

First you need to make sure that you retain any custom form data on a task or issue you want to convert. Because the custom form data must be an exact match on the converted item, it is best practice to duplicate the form so that you can attach it to the new object.

>[!TIP]
>
>Another way to retain custom form data in this situation is to add the larger object type to the custom form. For instructions, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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