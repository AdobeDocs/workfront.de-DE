---
title: Hinzufügen oder Löschen von Objekttypen aus einem vorhandenen benutzerdefinierten Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Mit dem Formularentwickler können Sie Objekttypen zu benutzerdefinierten Formularen hinzufügen oder daraus entfernen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: c1bc2832d1c52885e737056172e7aec93a951e6c
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Hinzufügen oder Löschen von Objekttypen aus einem vorhandenen benutzerdefinierten Formular

Mit dem Formularentwickler können Sie Objekttypen zu einem vorhandenen benutzerdefinierten Formular hinzufügen oder löschen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td><p>Administratorzugriff auf benutzerdefinierte Formulare</p></td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen von Objekttypen zu einem vorhandenen benutzerdefinierten Formular

Sie können dem Formular weitere Objekttypen hinzufügen, damit es an mehrere Objekte angehängt werden kann.

>[!NOTE]
>
>Die Berechtigungen für Abschnittsumbrüche können vom Objekttyp beeinflusst werden. Die eingeschränkte Berechtigung zum Bearbeiten für benutzerdefinierte Formularabschnitte ist nur für die Objekttypen Projekt, Aufgabe, Problem und Benutzer verfügbar.
>
>Weitere Informationen finden Sie unter [Wie sich mehrere Objekttypen auf die Berechtigungen für Abschnittsumbrüche auswirken können](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions).


{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms** .

   In der angezeigten Ansicht können Sie alle benutzerdefinierten Formulare überprüfen, die für Ihr Unternehmen erstellt wurden. Sie können auch sehen, wer jedes Formular erstellt hat, mit welchem Objekttyp es funktioniert und ob es aktiv ist.

1. Wählen Sie das benutzerdefinierte Formular aus, dem Sie weitere Objekttypen hinzufügen möchten, und klicken Sie dann auf das Symbol ![Bearbeiten](assets/edit-icon2.png).

1. Klicken Sie oben im Formular auf das Pluszeichen + nach **Objekttypen** und wählen Sie dann den gewünschten Typ im angezeigten Menü aus. Sie können dies wiederholen, um beliebig viele Objekttypen hinzuzufügen.

   ![](assets/add-new-object.png)

1. Klicken Sie auf **Speichern und schließen**.

   >[!TIP]
   >
   >Sie können jederzeit während der Erstellung eines benutzerdefinierten Formulars auf **Anwenden** klicken, um Ihre Änderungen zu speichern und das Formular offen zu halten.

## Löschen von Objekttypen in einem benutzerdefinierten Formular

Sie können Objekttypen aus einem vorhandenen benutzerdefinierten Formular löschen. Ein benutzerdefiniertes Formular muss mindestens einen Objekttyp aufweisen.

>[!CAUTION]
>
>Wenn Personen das benutzerdefinierte Formular bereits an Objekte des Typs angehängt haben, den Sie löschen möchten, und dem das Formular Daten hinzugefügt haben, werden diese Daten beim Löschen dieses Objekttyps im Formular dauerhaft gelöscht. Sie kann historische Informationen enthalten, die Benutzer später benötigen.
>
>Im Allgemeinen empfehlen wir, die Anzahl der Bearbeitungen eines bereits verwendeten benutzerdefinierten Formulars zu minimieren. Es gibt kein Benachrichtigungssystem, um Benutzer, die das benutzerdefinierte Formular verwenden, über Ihre Änderungen zu informieren.

So löschen Sie einen Objekttyp:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms** .
1. Wählen Sie das benutzerdefinierte Formular aus, das Sie bearbeiten möchten, und klicken Sie dann auf das Symbol ![Bearbeiten](assets/edit-icon2.png).
1. Klicken Sie auf das X eines der **Objekttypen**, die Sie aus dem Formular löschen möchten.

   ![](assets/delete-object-types.png)

1. (Optional) Wiederholen Sie den vorherigen Schritt für jeden anderen Objekttyp, den Sie aus dem Formular entfernen möchten.
1. Klicken Sie auf **Anwenden** und dann auf **Speichern und schließen**.
