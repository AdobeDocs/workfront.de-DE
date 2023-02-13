---
title: Übertragen benutzerdefinierter Formulardaten beim Konvertieren eines Objekts
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Wenn die in einem Arbeitselement definierte Arbeit zu groß wird, können Sie sie in ein größeres Arbeitselement konvertieren.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2d4d104a-1465-43e2-8184-83dd63d9681c
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Übertragen benutzerdefinierter Formulardaten beim Konvertieren eines Objekts

Je nach den Geschäftsanforderungen Ihrer Organisation kann die in einer Aufgabe oder einem Problem definierte Arbeit zu groß werden, um sie innerhalb der Aufgabe oder des Problems zu verwalten. In diesem Fall können Sie sie in ein größeres Arbeitselement konvertieren:

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
   <td role="rowheader"> <p>Adobe Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> <p>Informationen dazu, wie Workfront-Administratoren diesen Zugriff gewähren, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welche Konfigurationen für Plan, Lizenztyp oder Zugriffsstufe Sie verwenden.

## Erste: Benutzerdefiniertes Formular kopieren {#first-copy-the-custom-form}

Zuerst müssen Sie sicherstellen, dass Sie alle benutzerdefinierten Formulardaten für eine Aufgabe oder ein Problem speichern, die bzw. das konvertiert werden soll. Da die benutzerdefinierten Formulardaten exakt mit dem konvertierten Element übereinstimmen müssen, empfiehlt es sich, das Formular zu duplizieren, damit Sie es an das neue Objekt anhängen können.

>[!TIP]
>
>Eine andere Möglichkeit, benutzerdefinierte Formulardaten in dieser Situation beizubehalten, besteht darin, den größeren Objekttyp zum benutzerdefinierten Formular hinzuzufügen. Anweisungen finden Sie im Abschnitt . [Bearbeiten eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start2) im Artikel [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **Benutzerdefinierte Forms**.
1. Wählen Sie das benutzerdefinierte Formular vom Typ Aufgabe oder Problem aus und klicken Sie auf **Kopieren**.
1. Im **Benutzerdefiniertes Formular** Geben Sie einen Namen für das neue Formular an.

1. Aus dem **Formulartyp** Dropdown-Menü den Objekttyp auswählen, für den Sie das neue benutzerdefinierte Formular erstellen möchten

   **Beispiel:** Wenn Sie die benutzerdefinierten Formulardaten an ein Projekt übertragen möchten, wählen Sie Projekt aus.

1. Klicken **Formular kopieren**.

   Dieses kopierte benutzerdefinierte Formular kann jetzt an eine Aufgabe oder ein Projekt angehängt werden.

1. Fahren Sie fort mit [Zweitens: Konvertieren des Problems oder der Aufgabe und Übertragen der benutzerdefinierten Formulardaten](#second-convert-the-issue-or-task-and-transfer-the-custom-form-data).

## Zweitens: Konvertieren des Problems oder der Aufgabe und Übertragen der benutzerdefinierten Formulardaten {#second-convert-the-issue-or-task-and-transfer-the-custom-form-data}

1. Kopieren Sie das benutzerdefinierte Formular zu dem Problem oder der Aufgabe, das/die Sie konvertieren, wie im Abschnitt beschrieben. [Erste: Benutzerdefiniertes Formular kopieren](#first-copy-the-custom-form) in diesem Artikel.
1. Konvertieren Sie das Problem oder die Aufgabe mithilfe des **Benutzerdefinierte Forms** in dem Feld, das angezeigt wird, um das benutzerdefinierte Formular auszuwählen, das Sie kopiert haben. Anweisungen finden Sie in den folgenden Artikeln:

   * [Konvertieren eines Problems in ein Projekt in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-project.md)
   * [Konvertieren eines Problems in eine Aufgabe in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issue-to-task.md)
   * [Konvertieren einer Aufgabe in ein Projekt](../../../manage-work/tasks/manage-tasks/convert-task-to-project.md)

1. Im **Konvertieren in (Objekttyp)** angezeigt wird, klicken Sie auf das **Forms hinzufügen** und wählen Sie das Formular aus, das Sie im vorherigen Abschnitt kopiert haben.

   Die in den benutzerdefinierten Feldern des Problems erfassten Informationen werden jetzt in das benutzerdefinierte Formular für die Aufgabe übertragen.

