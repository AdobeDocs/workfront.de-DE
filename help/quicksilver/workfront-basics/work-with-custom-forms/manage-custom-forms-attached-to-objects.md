---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Verwalten benutzerdefinierter Formulare, die an Objekte angehängt sind
description: Sie können die Reihenfolge aktualisieren, in der die benutzerdefinierten Formulare, die an ein Objekt angehängt sind, angezeigt werden, sie entfernen oder die Darstellung benutzerdefinierter Formulare auf mehreren Objekten stapelweise bearbeiten.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 2%

---

# Verwalten benutzerdefinierter Formulare, die an Objekte angehängt sind

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Sie können die Reihenfolge aktualisieren, in der die benutzerdefinierten Formulare, die an ein Objekt angehängt sind, angezeigt werden, sie entfernen oder die Darstellung benutzerdefinierter Formulare auf mehreren Objekten stapelweise bearbeiten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Mitwirkender oder höher</p> 
   <p>Anfrage oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf die Objekte bearbeiten, für die Sie benutzerdefinierte Formulare verwalten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen oder höher für die Objekte beisteuern, für die Sie benutzerdefinierte Formulare verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to the objects for which you manage custom forms</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions or higher to the objects for which you manage custom forms</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Voraussetzungen

* Ihr Workfront-Administrator oder ein Plan-Benutzer mit administrativem Zugriff auf benutzerdefinierte Formulare muss benutzerdefinierte Formulare in Ihrer Umgebung erstellen. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Benutzerdefinierte Formulare müssen an ein Objekt angehängt sein.

  Informationen zum Anwenden benutzerdefinierter Formulare auf ein Objekt finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Mehrere benutzerdefinierte Formulare, die an ein Objekt angehängt sind, neu anordnen {#reorder-multiple-custom-forms-attached-to-an-object}

1. Wechseln Sie zum -Objekt, in dem Sie die Reihenfolge der hinzugefügten benutzerdefinierten Formulare ändern möchten, und beginnen Sie dann mit der Bearbeitung des -Objekts.

   **Beispiel:** Um beispielsweise die benutzerdefinierten Formulare eines Projekts zu verwalten, wechseln Sie zum Projekt, klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-icon.png) und klicken Sie dann auf **Bearbeiten** .

1. Klicken Sie **Abschnitt „Benutzerdefinierte Forms** für Projekte, Aufgaben und Probleme auf das ![Verschieben-Symbol](assets/move-icon---dots.png) neben dem Namen eines benutzerdefinierten Formulars. Klicken Sie für alle anderen Objekte auf **Forms verwalten**. Diese Option wird nur angezeigt, wenn mindestens ein benutzerdefiniertes Formular an das Objekt angehängt ist.
1. Ziehen Sie ein Formular ![Symbol Verschieben](assets/move-icon---dots.png) an eine neue Position in der Liste.
1. Klicken Sie für Projekte, Aufgaben und Probleme in benutzerdefinierten Formularen auf **Speichern**.

   Klicken Sie für alle anderen Objekte auf **Ich bin fertig mit Verwaltung** > **Änderungen speichern**.

## Entfernen eines benutzerdefinierten Formulars aus einem Objekt {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Wenn Sie ein benutzerdefiniertes Formular aus einem Objekt entfernen, gehen alle in den benutzerdefinierten Feldern des Formulars erfassten Informationen verloren und können nicht wiederhergestellt werden.

1. Wechseln Sie zu dem Objekt, von dem Sie das benutzerdefinierte Formular entfernen möchten, und klicken Sie dann im linken Bedienfeld **Details** für das Objekt.

   Gehen Sie beispielsweise zu einem Projekt und klicken Sie auf den Abschnitt **Projektdetails**.

1. Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png) in der oberen rechten Ecke der Seite des Objekts und dann auf **Alle bearbeiten**.
1. Klicken Sie auf das **Löschen**-Symbol ![Löschen](assets/delete-icon.png) rechts neben einem benutzerdefinierten Formularnamen und klicken Sie dann auf **Löschen**, um das Formular zu bestätigen und aus dem Objekt zu entfernen, oder **Abbrechen**, um das Entfernen zu verhindern.
1. Klicken Sie **Änderungen speichern** .

## Verwalten mehrerer benutzerdefinierter Formulare, die dieselben benutzerdefinierten Felder enthalten

Möglicherweise wird dasselbe Feld in mehreren benutzerdefinierten Formularen angezeigt, die an dasselbe Objekt angehängt sind. Beachten Sie in diesem Fall Folgendes:

* Der Wert des Felds ist in allen Formularen identisch.

  Sie können nicht unterschiedliche Werte für dieselben Felder in verschiedenen Formularen haben, die an dasselbe Objekt angehängt sind.

* Wenn Sie dieselben berechneten Felder auf zwei verschiedenen Objekten haben, müssen ihre Berechnungen identisch sein, um Fehler zu vermeiden. Informationen zum Hinzufügen berechneter Felder zu benutzerdefinierten Formularen, einschließlich mehrerer Formulare, finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

## Verwalten mehrerer benutzerdefinierter Formulare bei der Massenbearbeitung von Objekten

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Die Verwaltung von benutzerdefinierten Formularen für Objekte ist mit Ausnahme von Projekten für alle Objekte identisch.
>
>Informationen zum Massenhinzufügen von benutzerdefinierten Formularen zu Projekten finden Sie im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

Wenn Sie Objekte mit mehreren benutzerdefinierten Formularen stapelweise bearbeiten, können Sie die Art und Weise bearbeiten, wie benutzerdefinierte Formulare auf diese Objekte angezeigt werden, sowie die allgemeinen Felder zwischen den benutzerdefinierten Formularen bearbeiten.

Nur die benutzerdefinierten Formulare, die an alle ausgewählten Objekte angehängt sind, können im Massenvorgang bearbeitet werden.

So bearbeiten Sie mehrere benutzerdefinierte Formulare, wenn Sie Objekte stapelweise bearbeiten:

1. Wählen Sie in einer Objektliste die Objekte aus, an die die benutzerdefinierten Formulare angehängt sind, und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).
1. Klicken Sie **Benutzerdefinierte Forms**.

   Sie können nur die benutzerdefinierten Formulare bearbeiten, die an alle ausgewählten Objekte angehängt sind.

   Benutzerdefinierte Formulare, die nur mit einigen der Objekte verbunden sind, werden nicht angezeigt.

1. Beginnen Sie mit der Bearbeitung von Feldern in den benutzerdefinierten Formularen.

   Wenn Felder bearbeitet werden, wird ein visueller Indikator für das Feld angezeigt, der anzeigt, dass das Feld bearbeitet wurde.

   Wenn ein Feld in mehr als einem benutzerdefinierten Formular enthalten ist, werden alle Werte dieser Felder in jedem Formular aktualisiert, wenn Sie das Feld in einem der Formulare aktualisieren.

1. Klicken Sie auf **Dropdown-Menü** Auswahl treffen“ und wählen Sie zusätzliche Formulare aus, die allen ausgewählten Objekten hinzugefügt werden sollen.

   Beachten Sie beim Anwenden zusätzlicher Formulare Folgendes:

   * Objekte können bis zu 10 benutzerdefinierte Formulare haben.
   * Sie können Formulare nur anwenden, wenn das Formular noch nicht auf eines der Objekte angewendet wurde, die Sie bearbeiten. Ein Formular, das bereits mit einem der Objekte verbunden ist, wird nicht im Dropdown-Menü angezeigt.
   * Nachdem Sie ein zusätzliches Formular angewendet haben, werden alle Felder, die das Formular mit anderen Formularen gemeinsam hat, im Abschnitt **Gemeinsame Felder** angezeigt und können bearbeitet werden.

1. (Optional) Wenn Sie allen Objekten benutzerdefinierte Formulare hinzugefügt, die Objekte jedoch noch nicht gespeichert haben, können Sie die Reihenfolge ändern, in der die benutzerdefinierten Formulare auf den Objekten angezeigt werden.

   Weitere Informationen zum Ändern der Reihenfolge der Formulare finden Sie unter [Mehrere benutzerdefinierte Formulare, die an ein Objekt angehängt sind, neu &#x200B;](#reorder-multiple-custom-forms-attached-to-an-object) diesem Artikel.

1. Klicken Sie **Formular entfernen**, um ein benutzerdefiniertes Formular aus den Objekten zu entfernen.

   Weitere Informationen zum Entfernen benutzerdefinierter Formulare aus Objekten finden Sie unter [Entfernen eines benutzerdefinierten Formulars aus einem Objekt](#remove-a-custom-form-from-an-object).

   Beachten Sie Folgendes, wenn Sie Formulare stapelweise aus mehreren Objekten entfernen:

   * Wenn Sie Änderungen am Formular vorgenommen haben, führt das Entfernen dazu, dass Ihre Änderungen verloren gehen und nicht wiederhergestellt werden können.
   * Nachdem Sie ein Formular entfernt haben, werden alle Felder aus diesem Formular, die sich im Abschnitt **Allgemeine Felder** befanden, aus diesem Abschnitt entfernt und können hier nicht mehr bearbeitet werden.

1. Klicken Sie **Formular wiederherstellen**, um das Formular in dem Zustand wiederherzustellen, in dem es sich vor der Bearbeitung der Objekte befand.
1. (Optional) Klicken Sie auf den Pfeil zum Reduzieren neben dem Namen des Formulars, um jeweils ein Formular auszublenden.

   ODER

   Klicken Sie **Forms reduzieren**, um alle Formulare gleichzeitig zu reduzieren.

1. (Optional) Klicken Sie auf den Erweiterungspfeil neben dem Namen des Formulars, um jeweils ein Formular zu erweitern.

   ODER

   Klicken Sie **Forms erweitern**, um alle Formulare gleichzeitig zu erweitern.

1. Klicken Sie auf **Änderungen speichern**.
