---
title: Hinzufügen oder Löschen von Objekttypen aus einem vorhandenen benutzerdefinierten Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Mit dem Formular-Designer können Sie Objekttypen zu benutzerdefinierten Formularen hinzufügen oder daraus entfernen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 0%

---

# Hinzufügen oder Löschen von Objekttypen aus einem vorhandenen benutzerdefinierten Formular

Mit dem Formular-Designer können Sie Objekttypen in einem vorhandenen benutzerdefinierten Formular hinzufügen oder löschen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td><p>Administrativer Zugriff auf benutzerdefinierte Formulare</p></td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen von Objekttypen zu einem vorhandenen benutzerdefinierten Formular

Sie können dem Formular zusätzliche Objekttypen hinzufügen, damit es mit mehreren Objekten verbunden werden kann.

>[!NOTE]
>
>Berechtigungen zum Abschnittsumbruch können vom Objekttyp beeinflusst werden. Die Berechtigung zum eingeschränkten Bearbeiten für Abschnittsumbrüche in benutzerdefinierten Formularen ist nur für die Objekttypen „Projekt“, „Aufgabe“, „Problem“ und „Benutzer“ verfügbar.
>
>Weitere Informationen finden Sie unter [Wie mehrere Objekttypen sich auf die Berechtigungen für den Abschnittsumbruch auswirken können](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Klicken Sie **linken Bedienfeld** Benutzerdefinierte Forms&quot;.

   In der angezeigten Ansicht können Sie alle benutzerdefinierten Formulare überprüfen, die für Ihre Organisation erstellt wurden. Sie können auch sehen, wer die einzelnen Formulare erstellt hat, mit welchem Objekttyp sie funktionieren und ob sie aktiv sind.

1. Wählen Sie das benutzerdefinierte Formular aus, dem Sie zusätzliche Objekttypen hinzufügen möchten, und klicken Sie dann auf ![Symbol „Bearbeiten](assets/edit-icon2.png).

1. Klicken Sie oben im Formular auf das Pluszeichen + nach **Objekttypen** und wählen Sie dann im angezeigten Menü den gewünschten Typ aus. Sie können dies wiederholen, um beliebig viele Objekttypen hinzuzufügen.

   ![Neues Objekt hinzufügen](assets/add-new-object.png)

1. Klicken Sie **Speichern und schließen**.

   >[!TIP]
   >
   >Sie können jederzeit auf **Anwenden** klicken, während Sie ein benutzerdefiniertes Formular erstellen, um Ihre Änderungen zu speichern und das Formular offen zu halten.

## Löschen von Objekttypen in einem benutzerdefinierten Formular

Sie können Objekttypen aus einem vorhandenen benutzerdefinierten Formular löschen. Ein benutzerdefiniertes Formular muss mindestens einen Objekttyp haben.

>[!CAUTION]
>
>Wenn Personen das benutzerdefinierte Formular bereits an Objekte des Typs angehängt haben, den Sie löschen möchten, und ihm Daten hinzugefügt haben, werden diese Daten dauerhaft gelöscht, wenn Sie diesen Objekttyp im Formular löschen. Sie kann historische Informationen enthalten, die Benutzende später benötigen werden.
>
>Im Allgemeinen empfehlen wir, die Anzahl der Bearbeitungen eines benutzerdefinierten Formulars, das bereits verwendet wird, zu minimieren. Es gibt kein Benachrichtigungssystem, um Personen, die das benutzerdefinierte Formular verwenden, über Ihre Änderungen zu informieren.

So löschen Sie einen Objekttyp:

{{step-1-to-setup}}

1. Klicken Sie **linken Bedienfeld** Benutzerdefinierte Forms&quot;.
1. Wählen Sie das benutzerdefinierte Formular aus, das Sie bearbeiten möchten, und klicken Sie dann auf ![Symbol „Bearbeiten](assets/edit-icon2.png).
1. Klicken Sie auf das X auf einem der **Objekttypen** die Sie aus dem Formular löschen möchten.

   ![Objekttypen löschen](assets/delete-object-types.png)

1. (Optional) Wiederholen Sie den vorherigen Schritt für jeden anderen Objekttyp, den Sie aus dem Formular entfernen möchten.
1. Klicken Sie **Anwenden** und anschließend auf **Speichern und schließen**.
