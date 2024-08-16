---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Löschen eines benutzerdefinierten Felds oder Widgets aus dem System
description: Um die Systemleistung zu verbessern und die Verwendung von Formularen für Benutzer zu vereinfachen, sollten Sie benutzerdefinierte Felder und Widgets aus Ihrem System entfernen, wenn sie nicht mehr verwendet werden.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 3f7f4557c18bbb91ece850f910350d926a9e84bf
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 0%

---

# Löschen eines benutzerdefinierten Felds oder Widgets aus dem System

Um die Systemleistung zu verbessern und die Verwendung von Formularen für Benutzer zu vereinfachen, sollten Sie benutzerdefinierte Felder und Widgets aus Ihrem System entfernen, wenn sie nicht mehr verwendet werden.

>[!CAUTION]
>
>Beim Löschen eines benutzerdefinierten Felds werden auch alle benutzerdefinierten Daten gelöscht, die Benutzer in das Feld eingegeben haben, wenn benutzerdefinierte Formulare ausgefüllt werden, die an Objekte angehängt sind. Diese gelöschten Daten können nicht wiederhergestellt werden.
>
>Sie können alle benutzerdefinierten Formulare und Berichte anzeigen, die ein benutzerdefiniertes Feld verwenden, das Sie löschen möchten, um die möglichen Auswirkungen abzuschätzen. Weitere Informationen finden Sie unter [Alle benutzerdefinierten Formulare anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) und [Alle Berichte anzeigen, die ein bestimmtes benutzerdefiniertes Feld oder Widget verwenden](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>Alternativ können Sie eine Problemumgehung verwenden, um zu verhindern, dass Daten in nicht mehr verwendeten Feldern verloren gehen, siehe [Benutzerdefiniertes Feld entfernen, ohne Daten zu verlieren, die Benutzer in ](#remove-a-custom-field-without-losing-data-that-users-have-entered) in diesem Artikel eingegeben haben.

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Administratorzugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen eines benutzerdefinierten Felds oder Widgets aus dem System

{{step-1-to-setup}}

1. Klicken Sie auf **Benutzerdefinierter Forms.**
1. Klicken Sie auf **Felder** , um den Bereich Felder zu öffnen.
1. Wählen Sie das benutzerdefinierte Feld oder Widget aus und klicken Sie dann auf **Löschen**.
1. Wenn Sie sicher sind, dass Sie das Element und (im Fall eines benutzerdefinierten Felds) alle zugehörigen Daten zu Objekten, an die es angehängt wurde, dauerhaft löschen möchten, klicken Sie auf **Ja, Löschen Sie es**.

## Benutzerdefiniertes Feld entfernen, ohne die von Benutzern eingegebenen Daten zu verlieren {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>Das Entfernen eines benutzerdefinierten Felds aus einem benutzerdefinierten Formular mit mehr als 500 Feldern und Widgets kann nicht rückgängig gemacht werden. Wenn Sie das Feld entfernen, können Sie es erst erneut hinzufügen, wenn das Formular weniger als 500 Felder und Widgets enthält.

1. Bestimmen Sie, welche benutzerdefinierten Felder Sie aus dem ursprünglichen benutzerdefinierten Formular entfernen möchten, aber entfernen Sie sie zu diesem Zeitpunkt nicht.
1. Erstellen Sie ein neues benutzerdefiniertes Formular:

   1. Fügen Sie die benutzerdefinierten Felder zum neuen Formular hinzu, das Sie aus dem ursprünglichen benutzerdefinierten Formular entfernen möchten.

      Weitere Informationen finden Sie im Abschnitt [Hinzufügen neuer oder vorhandener Felder zu Ihrem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form) in [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

   1. Speichern Sie das neue benutzerdefinierte Formular.

1. Beschränken Sie den Zugriff auf das benutzerdefinierte Formular auf Benutzer mit Administratorzugriff, wie unter [Freigeben eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md) beschrieben.
1. Wenden Sie das neue benutzerdefinierte Formular auf die Objekte an, auf die bereits das ursprüngliche benutzerdefinierte Formular angewendet wurde, wie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md) beschrieben.

   Durch Anwendung des neuen benutzerdefinierten Formulars auf diese Objekte wird sichergestellt, dass historische Berichtsdaten nicht betroffen sind.

1. Ändern Sie das ursprüngliche benutzerdefinierte Formular und entfernen Sie die benutzerdefinierten Felder, die Sie zum neuen Formular hinzugefügt haben (in Schritt 2).

   Die Felder, die Sie aus dem ursprünglichen benutzerdefinierten Formular entfernt haben, sind jetzt nur noch für das neue benutzerdefinierte Formular verfügbar, das Sie erstellt haben. Benutzer können das benutzerdefinierte Formular im Objekt anzeigen, Benutzer ohne Administratorzugriff können das benutzerdefinierte Formular jedoch nicht ändern.
