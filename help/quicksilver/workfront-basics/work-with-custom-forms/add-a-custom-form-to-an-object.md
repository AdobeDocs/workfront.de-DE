---
product-area: projects;user-management
keywords: anhängen,anwenden
navigation-topic: work-with-custom-forms
title: Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt
description: Sie können ein vorhandenes benutzerdefiniertes Formular zu jedem der unten aufgeführten Objekte hinzufügen. Ein benutzerdefiniertes Formular enthält benutzerdefinierte Felder, in denen Sie Informationen über das Objekt speichern können.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 7b9989b73f7be46690073f323203ae2d9ca1a4b5
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 2%

---

# Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Sie können ein vorhandenes benutzerdefiniertes Formular zu jedem der unten aufgeführten Objekte hinzufügen. Ein benutzerdefiniertes Formular enthält benutzerdefinierte Felder, in denen Sie Informationen über das Objekt speichern können.

* Projekte (einschließlich Business Cases)
* Aufgaben
* Probleme
* Firmen
* Portfolios
* Programme
* Dokumente
* Benutzende
* Gruppen
* Wiederholungen
* Ausgaben
* Abrechnungs-Datensätze

Sie können ein benutzerdefiniertes Formular nur zu den Objekttypen hinzufügen, für die das Formular erstellt wurde.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Aktionen durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront-Lizenz</td> 
  <td> <p>Neu: Mitwirkender oder höher </p>
 <p>oder</p> 
<p>Aktuell: Anforderung oder höher </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf die Objekte bearbeiten, für die Sie benutzerdefinierte Formulare verwalten</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für das Objekt, für das Sie ein benutzerdefiniertes Formular anhängen möchten.</p> <p>Anzeigen von oder höhere Berechtigungen für das benutzerdefinierte Formular mit der Berechtigung <b>An benutzerdefinierte Daten anhängen</b> (Projekte, Aufgaben und Probleme). Weitere Informationen finden Sie unter <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Freigeben eines benutzerdefinierten Formulars</a>.</p> <p>Wichtig: Wenn Sie keine Planlizenz mit administrativem Zugriff auf benutzerdefinierte Forms haben, müssen Sie bestimmte Berechtigungen haben, um zumindest das benutzerdefinierte Formular anzuzeigen, wie in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Freigeben eines benutzerdefinierten Formulars</a> beschrieben. Diese Berechtigungen müssen Ihnen auch dann gewährt werden, wenn das Formular systemweit sichtbar ist. </p> <p>Weitere Informationen zum Anfordern von Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriff auf Objekte</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Ihr Workfront-Administrator oder ein Benutzer mit einer Planlizenz und administrativem Zugriff auf benutzerdefinierte Formulare muss benutzerdefinierte Formulare in Ihrer Umgebung erstellen, bevor Sie sie Objekten hinzufügen können. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt

Sie haben zwei Möglichkeiten, um ein benutzerdefiniertes Formular zu einem Objekt hinzuzufügen:

* [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt durch Bearbeiten des Objekts](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt aus dem Bereich Details](#add-a-custom-form-to-an-object-from-the-details-area)

### Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt durch Bearbeiten des -Objekts {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Wechseln Sie zu dem Objekt, dem Sie das benutzerdefinierte Formular hinzufügen möchten.
1. Klicken Sie auf die ![](assets/more-icon.png) **Mehr** und dann auf **Bearbeiten** ![](assets/edit-icon.png).
1. Klicken Sie **Benutzerdefinierte Forms** > **Forms hinzufügen** und wählen Sie dann aus dem Dropdown-Menü bis zu 10 Formulare aus.

1. (Optional) Aktualisieren Sie die Informationen in den bearbeitbaren Feldern im benutzerdefinierten Formular.

   Sie müssen alle erforderlichen Felder in den Formularen aktualisieren, die Sie hinzufügen.

1. Klicken Sie auf **Speichern**.

### Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt aus dem Bereich Details {#add-a-custom-form-to-an-object-from-the-details-area}

1. Wechseln Sie zu dem Objekt, dem Sie das benutzerdefinierte Formular hinzufügen möchten.
1. Klicken Sie im linken Bedienfeld **Abschnitt**`<Object type>` . Klicken Sie beispielsweise auf **Projektdetails**, um einem Projekt benutzerdefinierte Formulare hinzuzufügen, oder auf **Problemdetails**, um einem Problem benutzerdefinierte Formulare hinzuzufügen.
1. Klicken Sie oben rechts **das Feld** Benutzerdefiniertes Formular hinzufügen“ und wählen Sie dann bis zu 10 benutzerdefinierte Formulare aus der angezeigten Liste aus.

   Wenn das Formular Pflichtfelder enthält (mit einem roten Sternchen gekennzeichnet), müssen Sie diese derzeit nicht ausfüllen.

   Die ausgewählten Formulare werden automatisch an das Objekt angehängt.

1. (Optional) Aktualisieren Sie die Informationen in den benutzerdefinierten Feldern des Formulars und klicken Sie dann auf **Änderungen speichern**.

## Mehrere benutzerdefinierte Formulare in einem Objekt

Sie können bis zu 10 benutzerdefinierte Formulare zu einem bestimmten Objekt hinzufügen, sodass Sie Felder für einige Benutzer und nicht für andere verfügbar machen können oder die Formularanforderungen mehrerer Projekte besser erfüllen können.

**Beispiel** Wenn ein vorhandenes Projekt bereits über ein benutzerdefiniertes Formular verfügt und für dieses Projekt weitere benutzerdefinierte Felder benötigt werden, die in einem anderen benutzerdefinierten Formular vorhanden sind, können Sie dem Projekt ein zweites Formular mit den zusätzlichen Feldern hinzufügen, anstatt die Felder dem vorhandenen benutzerdefinierten Formular hinzuzufügen.

## Hinzufügen eines benutzerdefinierten Formulars zu mehreren Objekten in großen Mengen

Sie können benutzerdefinierte Formulare mehreren Objekten hinzufügen, indem Sie sie in einer Liste auswählen.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Das Hinzufügen benutzerdefinierter Formulare zu Objekten ist für alle Objekte mit Ausnahme von Projekten identisch.
>
>Informationen zum Massenhinzufügen von benutzerdefinierten Formularen zu Projekten finden Sie im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).


1. Navigieren Sie zu einer Liste von Objekten.
1. Mehrere Objekte in der Liste auswählen.

1. Klicken Sie auf die ![](assets/more-icon.png) **Mehr** und dann auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

   Oder

   Klicken Sie oben **der Liste** das Symbol „Bearbeiten“ ![](assets/edit-icon.png).
1. Klicken Sie **linken Bedienfeld** Benutzerdefinierte Forms&quot;.
1. Wählen Sie **Dropdown-Menü** Auswahl treffen“ das Formular aus, das Sie mit allen ausgewählten Objekten verknüpfen möchten.

   >[!NOTE]
   >
   >Wenn Sie das Formular im Dropdown-Menü nicht finden können, bedeutet dies, dass mindestens einem der Objekte das Formular bereits zugeordnet ist. Bestimmen Sie, welches Objekt das ist, und entfernen Sie es aus Ihrer Auswahl, bevor Sie das Formular zu den verbleibenden Objekten hinzufügen können.


1. Klicken Sie auf **Änderungen speichern**.

   Wenn das Formular Pflichtfelder enthält (mit einem roten Sternchen gekennzeichnet), müssen Sie diese derzeit nicht ausfüllen.
