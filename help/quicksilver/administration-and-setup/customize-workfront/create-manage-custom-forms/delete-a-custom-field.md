---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Löschen eines benutzerdefinierten Felds oder Widgets aus dem System
description: Um die Systemleistung zu verbessern und die Verwendung von Formularen für Benutzende zu vereinfachen, sollten Sie benutzerdefinierte Felder und Widgets aus Ihrem System entfernen, wenn sie nicht mehr verwendet werden.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Löschen eines benutzerdefinierten Felds oder Widgets aus dem System

Um die Systemleistung zu verbessern und die Verwendung von Formularen für Benutzende zu vereinfachen, sollten Sie benutzerdefinierte Felder und Widgets aus Ihrem System entfernen, wenn sie nicht mehr verwendet werden.

>[!CAUTION]
>
>Durch Löschen eines benutzerdefinierten Felds werden auch alle benutzerdefinierten Daten gelöscht, die Benutzende beim Ausfüllen benutzerdefinierter Formulare, die an Objekte angehängt sind, in das Feld eingegeben haben. Diese gelöschten Daten können nicht wiederhergestellt werden. Außerdem gibt es kein Benachrichtigungssystem, um Personen, die das benutzerdefinierte Formular verwenden, darüber zu informieren, dass es gelöscht wurde.
>
>Sie können alle benutzerdefinierten Formulare und Berichte anzeigen, die ein benutzerdefiniertes Feld verwenden, das Sie löschen möchten, um die möglichen Auswirkungen zu bewerten. Weitere Informationen finden Sie unter [Anzeigen aller benutzerdefinierten Formulare, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) und [Anzeigen aller Berichte, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Alternativ können Sie für eine Problemumgehung verwenden, um zu vermeiden, dass Daten in nicht mehr verwendeten Feldern verloren gehen. Weitere Informationen finden Sie unter [Entfernen eines benutzerdefinierten Felds, ohne Daten zu verlieren, die von Benutzenden eingegeben wurden](#remove-a-custom-field-without-losing-data-that-users-have-entered) in diesem Artikel.

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

## Löschen eines benutzerdefinierten Felds oder Widgets aus dem System

{{step-1-to-setup}}

1. Klicken Sie auf **Benutzerdefinierte Forms.**
1. Klicken Sie auf **Felder**, um den Bereich Felder zu öffnen.
1. Wählen Sie das benutzerdefinierte Feld oder Widget aus und klicken Sie dann auf **Löschen**.
1. Wenn Sie das Element und (im Falle eines benutzerdefinierten Felds) alle zugehörigen Daten zu Objekten, an die es angehängt war, wirklich dauerhaft löschen möchten, klicken Sie auf **Ja, Löschen**.

## Entfernen eines benutzerdefinierten Felds ohne Datenverlust, das Benutzer eingegeben haben {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>Das Entfernen eines benutzerdefinierten Felds aus einem benutzerdefinierten Formular mit mehr als 500 Feldern und Widgets kann nicht rückgängig gemacht werden. Wenn Sie das Feld entfernen, können Sie es erst dann erneut hinzufügen, wenn das Formular weniger als 500 Felder und Widgets enthält.

1. Legen Sie fest, welche benutzerdefinierten Felder Sie aus dem ursprünglichen benutzerdefinierten Formular entfernen möchten, entfernen Sie sie jedoch jetzt nicht.
1. Erstellen Sie ein neues benutzerdefiniertes Formular:

   1. Fügen Sie die benutzerdefinierten Felder zu dem neuen Formular hinzu, das Sie aus dem ursprünglichen benutzerdefinierten Formular entfernen möchten.

      Weitere Informationen finden Sie im Abschnitt [Hinzufügen neuer oder vorhandener Felder zu Ihrem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form) in [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   1. Speichern Sie das neue benutzerdefinierte Formular.

1. Beschränken Sie den Zugriff auf das benutzerdefinierte Formular auf Benutzer mit Administratorzugriff, wie unter [Freigeben eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md) beschrieben.
1. Wenden Sie das neue benutzerdefinierte Formular auf die Objekte an, auf die das ursprüngliche benutzerdefinierte Formular bereits angewendet wurde, wie in [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt“ ](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   Wenn Sie das neue benutzerdefinierte Formular auf diese Objekte anwenden, wird sichergestellt, dass historische Berichtsdaten nicht betroffen sind.

1. Ändern Sie das ursprüngliche benutzerdefinierte Formular und entfernen Sie die benutzerdefinierten Felder, die Sie dem neuen Formular hinzugefügt haben (in Schritt 2).

   Die Felder, die Sie aus dem ursprünglichen benutzerdefinierten Formular entfernt haben, sind jetzt nur noch in dem neuen benutzerdefinierten Formular verfügbar, das Sie erstellt haben. Benutzende können das benutzerdefinierte Formular auf dem Objekt sehen, Benutzende ohne Administratorzugriff können das benutzerdefinierte Formular jedoch nicht ändern.
