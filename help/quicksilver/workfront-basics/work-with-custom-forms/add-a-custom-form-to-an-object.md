---
product-area: projects;user-management
keywords: attach,apply
navigation-topic: work-with-custom-forms
title: Benutzerdefiniertes Formular zu einem Objekt hinzufügen
description: Sie können einem der unten aufgeführten Objekte ein vorhandenes benutzerdefiniertes Formular hinzufügen. Ein benutzerdefiniertes Formular enthält benutzerdefinierte Felder, in denen Sie Informationen zum Objekt speichern können.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 1%

---

# Benutzerdefiniertes Formular zu einem Objekt hinzufügen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Sie können einem der unten aufgeführten Objekte ein vorhandenes benutzerdefiniertes Formular hinzufügen. Ein benutzerdefiniertes Formular enthält benutzerdefinierte Felder, in denen Sie Informationen zum Objekt speichern können.

* Projekte (einschließlich Geschäftsfälle)
* Aufgaben
* Probleme
* Firmen
* Portfolios
* Programme
* Dokumente
* Benutzende
* Wiederholungen
* Ausgaben
* Rechnungsdatensätze

Sie können ein benutzerdefiniertes Formular nur zu den Objekttypen hinzufügen, für die das Formular erstellt wurde.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf die Objekte bearbeiten, für die Sie benutzerdefinierte Formulare verwalten</p> <p><b>NOTIZ</b></p>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für das Objekt, an das Sie ein benutzerdefiniertes Formular anhängen möchten.</p> <p>Anzeigen von oder höheren Berechtigungen für das benutzerdefinierte Formular mit der Berechtigung zum <b>Anhängen an benutzerdefinierte Daten</b> Objekte (Projekte, Aufgaben und Probleme). Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Freigeben eines benutzerdefinierten Formulars</a>.</p> <p>Wichtig: Wenn Sie nicht über eine Planungslizenz mit Administratorzugriff auf Custom Forms verfügen, müssen Sie über bestimmte Berechtigungen verfügen, um zumindest das benutzerdefinierte Formular anzuzeigen, wie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Freigeben eines benutzerdefinierten Formulars</a>. Diese Berechtigungen müssen Ihnen gewährt werden, selbst wenn das Formular systemweit sichtbar ist. </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzung

Ihr Workfront-Administrator oder ein Benutzer mit einer Planungslizenz und Administratorzugriff auf benutzerdefinierte Formulare muss benutzerdefinierte Formulare in Ihrer Umgebung erstellen, bevor Sie sie zu Objekten hinzufügen können. Weitere Informationen finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Benutzerdefiniertes Formular zu einem Objekt hinzufügen

Sie können einem Objekt auf zwei Arten ein benutzerdefiniertes Formular hinzufügen:

* [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt durch Bearbeiten des Objekts](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt aus dem Bereich &quot;Details&quot;](#add-a-custom-form-to-an-object-from-the-details-area)

### Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt durch Bearbeiten des Objekts {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Wechseln Sie zu dem Objekt, dem Sie das benutzerdefinierte Formular hinzufügen möchten.
1. Klicken Sie auf **Mehr** Menü ![](assets/more-icon.png)Klicken Sie auf **Bearbeiten** ![](assets/edit-icon.png).
1. Klicken **Benutzerdefinierte Forms** > **Forms hinzufügen** und wählen Sie dann bis zu 10 Formulare aus dem Dropdown-Menü aus.

1. (Optional) Aktualisieren Sie die Informationen in den bearbeitbaren Feldern des benutzerdefinierten Formulars.

   Sie müssen alle erforderlichen Felder in den Formularen aktualisieren, die Sie hinzufügen.

1. Klicken Sie auf **Speichern**.

### Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt aus dem Bereich &quot;Details&quot; {#add-a-custom-form-to-an-object-from-the-details-area}

1. Wechseln Sie zu dem Objekt, dem Sie das benutzerdefinierte Formular hinzufügen möchten.
1. Klicken Sie auf **`<Object type>`Details** im linken Bereich. Klicken Sie beispielsweise auf **Projektdetails** zum Hinzufügen benutzerdefinierter Formulare zu einem Projekt oder **Problemdetails** , um einem Problem benutzerdefinierte Formulare hinzuzufügen.
1. Klicken Sie auf **Benutzerdefiniertes Formular hinzufügen** in der oberen rechten Ecke und wählen Sie dann bis zu 10 benutzerdefinierte Formulare aus der angezeigten Liste aus.

   Wenn das Formular erforderliche Felder enthält (mit einem roten Sternchen markiert), müssen Sie sie derzeit nicht ausfüllen.

   Die ausgewählten Formulare werden automatisch an das Objekt angehängt.

1. (Optional) Aktualisieren Sie die Informationen in den benutzerdefinierten Feldern des Formulars und klicken Sie auf **Änderungen speichern**.

## Mehrere benutzerdefinierte Formulare auf einem Objekt

Sie können bis zu 10 benutzerdefinierte Formulare zu einem bestimmten Objekt hinzufügen, sodass Sie Felder einigen Benutzern und nicht anderen zur Verfügung stellen können oder die Formularanforderungen mehrerer Projekte besser erfüllen können.

**Beispiel:** Wenn ein vorhandenes Projekt bereits über ein benutzerdefiniertes Formular verfügt und mehr benutzerdefinierte Felder in einem anderen benutzerdefinierten Formular benötigt werden, können Sie dem Projekt ein zweites Formular mit den zusätzlichen Feldern hinzufügen, anstatt die Felder zum vorhandenen benutzerdefinierten Formular hinzuzufügen, wenn diese Felder nur für dieses Projekt benötigt werden.

## Benutzerdefiniertes Formular zu mehreren Objekten als Stapel hinzufügen

Sie können benutzerdefinierte Formulare zu mehreren Objekten hinzufügen, indem Sie sie in einer Liste auswählen.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Das Hinzufügen benutzerdefinierter Formulare zu Objekten ist für alle Objekte mit Ausnahme von Projekten identisch.
>
>Informationen zum Hinzufügen benutzerdefinierter Formulare zu Projekten in Stapeln finden Sie im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).


1. Navigieren Sie zu einer Liste von Objekten.
1. Wählen Sie mehrere Objekte in der Liste aus.

1. Klicken Sie auf **Mehr** Menü ![](assets/more-icon.png)und klicken Sie dann auf **Bearbeiten** icon  ![](assets/edit-icon.png)oder klicken Sie einfach auf **Bearbeiten** icon ![](assets/edit-icon.png) oben in der Liste.
1. Klicken **Benutzerdefinierte Forms** im linken Bereich.
1. Wählen Sie das Formular aus, das Sie mit allen ausgewählten Objekten im **Auswahl treffen** Dropdown-Menü.
   >[!NOTE]
   >
   >Wenn Sie das Formular nicht im Dropdown-Menü finden können, bedeutet dies, dass mindestens einem der Objekte das Formular bereits zugeordnet ist. Bestimmen Sie, welches Objekt das Element ist, und entfernen Sie es aus Ihrer Auswahl, bevor Sie das Formular zu den restlichen Objekten hinzufügen können.


1. Klicken **Änderungen speichern**.

   Wenn das Formular erforderliche Felder enthält (mit einem roten Sternchen markiert), müssen Sie sie derzeit nicht ausfüllen.
