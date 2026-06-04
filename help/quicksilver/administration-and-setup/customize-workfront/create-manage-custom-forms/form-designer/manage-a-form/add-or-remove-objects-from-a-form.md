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
TQID: https://experienceleague.adobe.com/2nu2y2zDxTQkLnch-M8Z5jcWXw32O0crTbhmt3VjSGg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 446
ht-degree: 14%

---

# Hinzufügen oder Löschen von Objekttypen aus einem vorhandenen benutzerdefinierten Formular

Mit dem Formular-Designer können Sie Objekttypen in einem vorhandenen benutzerdefinierten Formular hinzufügen oder löschen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. Klicken Sie oben im Formular auf **Objekttypen** und wählen Sie dann den Typ aus, den Sie dem angezeigten Menü hinzufügen möchten. Sie können diesen Vorgang wiederholen, um beliebig viele Objekttypen hinzuzufügen.

   ![Neues Objekt hinzufügen](assets/add-new-object-to-custom-form-041026.png)

1. Klicken Sie auf **Speichern und schließen**.

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
1. Klicken Sie oben im Formular auf **Objekttypen** und deaktivieren Sie dann die Kontrollkästchen für die Objekte, die Sie aus dem Formular löschen möchten.
1. Klicken Sie **Anwenden** und anschließend auf **Speichern und schließen**.
