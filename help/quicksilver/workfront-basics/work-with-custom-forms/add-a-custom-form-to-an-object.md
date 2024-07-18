---
product-area: projects;user-management
keywords: attach,apply
navigation-topic: work-with-custom-forms
title: Benutzerdefiniertes Formular zu einem Objekt hinzufügen
description: Sie können einem der unten aufgeführten Objekte ein vorhandenes benutzerdefiniertes Formular hinzufügen. Ein benutzerdefiniertes Formular enthält benutzerdefinierte Felder, in denen Sie Informationen zum Objekt speichern können.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 2%

---

# Benutzerdefiniertes Formular zu einem Objekt hinzufügen

<!--Audited: 12/2023-->

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
* Abrechnungs-Datensätze

Sie können ein benutzerdefiniertes Formular nur zu den Objekttypen hinzufügen, für die das Formular erstellt wurde.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront-Lizenz</td> 
  <td> <p>Neu: Mitarbeiter oder höher </p>
 <p>oder</p> 
<p>Aktuell: Anforderung oder höher </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf die Objekte bearbeiten, für die Sie benutzerdefinierte Formulare verwalten</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für das Objekt, an das Sie ein benutzerdefiniertes Formular anhängen möchten.</p> <p>Anzeigen oder höherer Berechtigungen für das benutzerdefinierte Formular mit der Berechtigung <b>An benutzerdefinierte Datenobjekte anhängen</b> (Projekte, Aufgaben und Probleme). Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Freigeben eines benutzerdefinierten Formulars</a>.</p> <p>Wichtig: Wenn Sie keine Planungslizenz mit Administratorzugriff auf Custom Forms haben, müssen Sie über bestimmte Berechtigungen verfügen, um zumindest das benutzerdefinierte Formular anzuzeigen, wie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular freigeben</a> beschrieben. Diese Berechtigungen müssen Ihnen gewährt werden, selbst wenn das Formular systemweit sichtbar ist. </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Ihr Workfront-Administrator oder ein Benutzer mit einer Planungslizenz und Administratorzugriff auf benutzerdefinierte Formulare muss benutzerdefinierte Formulare in Ihrer Umgebung erstellen, bevor Sie sie zu Objekten hinzufügen können. Weitere Informationen finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Benutzerdefiniertes Formular zu einem Objekt hinzufügen

Sie können einem Objekt auf zwei Arten ein benutzerdefiniertes Formular hinzufügen:

* [Fügen Sie ein benutzerdefiniertes Formular zu einem Objekt hinzu, indem Sie das Objekt bearbeiten](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt aus dem Bereich &quot;Details&quot;](#add-a-custom-form-to-an-object-from-the-details-area)

### Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt durch Bearbeiten des Objekts {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Wechseln Sie zu dem Objekt, dem Sie das benutzerdefinierte Formular hinzufügen möchten.
1. Klicken Sie auf das Menü **Mehr** ![](assets/more-icon.png) und dann auf **Bearbeiten** ![](assets/edit-icon.png).
1. Klicken Sie auf **Benutzerdefinierter Forms** > **Forms hinzufügen** und wählen Sie dann aus dem Dropdownmenü bis zu 10 Formulare aus.

1. (Optional) Aktualisieren Sie die Informationen in den bearbeitbaren Feldern des benutzerdefinierten Formulars.

   Sie müssen alle erforderlichen Felder in den Formularen aktualisieren, die Sie hinzufügen.

1. Klicken Sie auf **Speichern**.

### Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt aus dem Bereich &quot;Details&quot; {#add-a-custom-form-to-an-object-from-the-details-area}

1. Wechseln Sie zu dem Objekt, dem Sie das benutzerdefinierte Formular hinzufügen möchten.
1. Klicken Sie im linken Bereich auf den Bereich **`<Object type>`Details** . Klicken Sie beispielsweise auf **Projektdetails** , um einem Projekt benutzerdefinierte Formulare hinzuzufügen, oder auf **Problemdetails** , um benutzerdefinierte Formulare zu einem Problem hinzuzufügen.
1. Klicken Sie oben rechts auf das Feld **Benutzerdefiniertes Formular hinzufügen** und wählen Sie dann bis zu 10 benutzerdefinierte Formulare aus der angezeigten Liste aus.

   Wenn das Formular erforderliche Felder enthält (mit einem roten Sternchen markiert), müssen Sie sie derzeit nicht ausfüllen.

   Die ausgewählten Formulare werden automatisch an das Objekt angehängt.

1. (Optional) Aktualisieren Sie die Informationen in den benutzerdefinierten Feldern des Formulars und klicken Sie dann auf **Änderungen speichern**.

## Mehrere benutzerdefinierte Formulare auf einem Objekt

Sie können bis zu 10 benutzerdefinierte Formulare zu einem bestimmten Objekt hinzufügen, sodass Sie Felder einigen Benutzern und nicht anderen zur Verfügung stellen können oder die Formularanforderungen mehrerer Projekte besser erfüllen können.

**Beispiel:** Wenn ein vorhandenes Projekt bereits über ein benutzerdefiniertes Formular verfügt und mehr benutzerdefinierte Felder für dieses Projekt benötigt werden, die in einem anderen benutzerdefinierten Formular vorhanden sind, können Sie dem Projekt ein zweites Formular mit den zusätzlichen Feldern hinzufügen, anstatt die Felder zum vorhandenen benutzerdefinierten Formular hinzuzufügen.

## Benutzerdefiniertes Formular zu mehreren Objekten als Stapel hinzufügen

Sie können benutzerdefinierte Formulare zu mehreren Objekten hinzufügen, indem Sie sie in einer Liste auswählen.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Das Hinzufügen benutzerdefinierter Formulare zu Objekten ist für alle Objekte mit Ausnahme von Projekten identisch.
>
>Informationen zum Hinzufügen benutzerdefinierter Formulare zu Projekten in großen Mengen finden Sie im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md) .


1. Navigieren Sie zu einer Liste von Objekten.
1. Auswählen mehrerer Objekte in der Liste.

1. Klicken Sie auf das Menü **Mehr** und dann auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).![](assets/more-icon.png)

   Oder

   Klicken Sie oben in der Liste auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) .
1. Klicken Sie im linken Bereich auf **Benutzerdefinierter Forms** .
1. Wählen Sie im Dropdownmenü **Auswahl treffen** das Formular aus, das Sie mit allen ausgewählten Objekten verknüpfen möchten.

   >[!NOTE]
   >
   >Wenn Sie das Formular nicht im Dropdown-Menü finden können, bedeutet dies, dass mindestens einem der Objekte das Formular bereits zugeordnet ist. Bestimmen Sie, welches Objekt das Element ist, und entfernen Sie es aus Ihrer Auswahl, bevor Sie das Formular zu den restlichen Objekten hinzufügen können.


1. Klicken Sie auf **Änderungen speichern**.

   Wenn das Formular erforderliche Felder enthält (mit einem roten Sternchen markiert), müssen Sie sie derzeit nicht ausfüllen.
