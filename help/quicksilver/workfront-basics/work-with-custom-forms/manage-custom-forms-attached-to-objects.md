---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: Verwalten von benutzerdefinierten Formularen, die an Objekte angehängt werden
description: Sie können die Reihenfolge aktualisieren, in der die an ein Objekt angehängten benutzerdefinierten Formulare angezeigt, entfernt oder die Anzeige von benutzerdefinierten Formularen auf mehreren Objekten durch Massenbearbeitung geändert werden.
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 0%

---

# Verwalten von benutzerdefinierten Formularen, die an Objekte angehängt werden

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Sie können die Reihenfolge aktualisieren, in der die an ein Objekt angehängten benutzerdefinierten Formulare angezeigt, entfernt oder die Anzeige von benutzerdefinierten Formularen auf mehreren Objekten durch Massenbearbeitung geändert werden.

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
   <td> <p>Zugriff auf die Objekte bearbeiten, für die Sie benutzerdefinierte Formulare verwalten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen Sie Berechtigungen oder höher zu den Objekten, für die Sie benutzerdefinierte Formulare verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

* Ihr Workfront-Administrator oder ein Planbenutzer mit Administratorzugriff auf benutzerdefinierte Formulare muss benutzerdefinierte Formulare in Ihrer Umgebung erstellen. Weitere Informationen finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* Sie müssen benutzerdefinierte Formulare an ein Objekt anhängen.

   Informationen zum Anwenden von benutzerdefinierten Formularen auf ein Objekt finden Sie unter [Benutzerdefiniertes Formular zu einem Objekt hinzufügen](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Mehrere benutzerdefinierte Formulare neu anordnen, die an ein Objekt angehängt sind {#reorder-multiple-custom-forms-attached-to-an-object}

1. Wechseln Sie zu dem Objekt, an dem Sie die Reihenfolge der hinzugefügten benutzerdefinierten Formulare ändern möchten, und bearbeiten Sie dann das Objekt.

   **Beispiel:** Um beispielsweise die benutzerdefinierten Formulare eines Projekts zu verwalten, gehen Sie zum Projekt und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-icon.png)Klicken Sie auf **Bearbeiten** .

1. Im **Benutzerdefinierte Forms** für Projekte, Aufgaben und Probleme klicken Sie auf die Schaltfläche ![](assets/move-icon---dots.png) neben dem Namen eines benutzerdefinierten Formulars. Klicken Sie für alle anderen Objekte auf **Verwalten von Forms**. Diese Option wird nur angezeigt, wenn mindestens ein benutzerdefiniertes Formular an das Objekt angehängt ist.
1. Formular ziehen ![](assets/move-icon---dots.png) an eine neue Position in der Liste.
1. Klicken Sie für Projekte, Aufgaben und Probleme mit benutzerdefinierten Formularen auf **Speichern**.

   Klicken Sie für alle anderen Objekte auf **Ich bin mit der Verwaltung fertig** > **Änderungen speichern**.

## Benutzerdefiniertes Formular aus einem Objekt entfernen {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>Wenn Sie ein benutzerdefiniertes Formular aus einem Objekt entfernen, gehen alle in den benutzerdefinierten Feldern des Formulars erfassten Informationen verloren und können nicht wiederhergestellt werden.

1. Wechseln Sie zu dem Objekt, in dem Sie das benutzerdefinierte Formular entfernen und mit der Bearbeitung des Objekts beginnen möchten.

   Wechseln Sie beispielsweise zu einem Projekt und klicken Sie auf das **Mehr** Menü ![](assets/more-icon.png)Klicken Sie auf **Bearbeiten** .

1. Klicken **Benutzerdefinierte Forms**.
1. Klicken Sie bei Projekten, Aufgaben und Problemen mit benutzerdefinierten Formularen auf die **X** rechts neben einem Formular, um es aus dem Objekt zu entfernen.

   Klicken Sie für alle anderen Objekte auf **Verwalten von Forms** und klicken Sie dann auf **X** rechts neben einem Formular, um es aus dem Objekt zu entfernen.

1. Klicken Sie auf **Speichern** .

## Verwalten mehrerer benutzerdefinierter Formulare, die dieselben benutzerdefinierten Felder enthalten

Möglicherweise wird dasselbe Feld in mehreren benutzerdefinierten Formularen angezeigt, die an dasselbe Objekt angehängt sind. Beachten Sie in diesem Fall Folgendes:

* Der Wert des Felds ist in allen Formularen identisch.

   Sie können für dieselben Felder in verschiedenen Formularen, die an dasselbe Objekt angehängt sind, keine unterschiedlichen Werte haben.

* Wenn Sie für zwei verschiedene Objekte dieselben berechneten Felder haben, müssen deren Berechnungen identisch sein, um Fehler zu vermeiden. Weitere Informationen zum Hinzufügen berechneter Felder zu benutzerdefinierten Formularen einschließlich mehrerer Formulare finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## Verwalten mehrerer benutzerdefinierter Formulare bei der Massenbearbeitung von Objekten

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Die Verwaltung benutzerdefinierter Formulare für Objekte ist für alle Objekte mit Ausnahme von Projekten identisch.
>
>Informationen zum Hinzufügen benutzerdefinierter Formulare zu Projekten in Stapeln finden Sie im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

Wenn Sie mehrere benutzerdefinierte Formulare auf Objekte anwenden, die als Massenbearbeitung dienen, können Sie die Art und Weise bearbeiten, wie benutzerdefinierte Formulare auf diesen Objekten angezeigt werden, und gemeinsame Felder in den benutzerdefinierten Formularen bearbeiten.

Nur die benutzerdefinierten Formulare, die an alle ausgewählten Objekte angehängt sind, können bei einer Massenbearbeitung bearbeitet werden.

So bearbeiten Sie mehrere benutzerdefinierte Formulare bei der Massenbearbeitung von Objekten:

1. Wählen Sie in Listenobjekten die Objekte aus, an die die benutzerdefinierten Formulare angehängt sind, und klicken Sie dann auf das **Bearbeiten** icon ![](assets/edit-icon.png).
1. Klicken **Benutzerdefinierte Forms**.

   Sie können nur die benutzerdefinierten Formulare bearbeiten, die an alle ausgewählten Objekte angehängt sind.

   Benutzerdefinierte Formulare, die nur an einige der Objekte angehängt sind, werden nicht angezeigt.

1. Beginnen Sie mit der Bearbeitung von Feldern in den benutzerdefinierten Formularen.

   Wenn die Felder bearbeitet werden, wird im Feld ein visueller Indikator angezeigt, der anzeigt, dass das Feld bearbeitet wurde.

   Wenn ein Feld in mehr als einem benutzerdefinierten Formular enthalten ist, werden alle Werte dieser Felder in jedem Formular aktualisiert, wenn Sie das Feld in einem der Formulare aktualisieren.

1. Klicken Sie auf **Auswahl treffen** Dropdown-Menü und wählen Sie zusätzliche Formulare aus, die zu allen ausgewählten Objekten hinzugefügt werden sollen.

   Beachten Sie beim Anwenden zusätzlicher Formulare Folgendes:

   * Objekte können über bis zu 10 benutzerdefinierte Formulare verfügen.
   * Sie können Formulare nur dann anwenden, wenn das Formular noch nicht auf eines der bearbeiteten Objekte angewendet wurde. Ein Formular, das bereits an eines der Objekte angehängt ist, wird nicht im Dropdown-Menü angezeigt.
   * Nachdem Sie ein zusätzliches Formular angewendet haben, werden alle Felder, die das Formular mit anderen Formularen verbindet, im **Allgemeine Felder** und sie können bearbeitet werden.

1. (Optional) Wenn Sie benutzerdefinierte Formulare zu allen Objekten hinzugefügt, die Objekte jedoch noch nicht gespeichert haben, können Sie die Reihenfolge ändern, in der die benutzerdefinierten Formulare auf den Objekten angezeigt werden.

   Weitere Informationen zum Ändern der Reihenfolge der Formulare finden Sie unter [Mehrere benutzerdefinierte Formulare neu anordnen, die an ein Objekt angehängt sind](#reorder-multiple-custom-forms-attached-to-an-object) in diesem Artikel.

1. Klicken **Formular entfernen** , um ein benutzerdefiniertes Formular aus den Objekten zu entfernen.

   Weitere Informationen zum Entfernen von benutzerdefinierten Formularen aus Objekten finden Sie unter [Benutzerdefiniertes Formular aus einem Objekt entfernen](#remove-a-custom-form-from-an-object).

   Beachten Sie Folgendes, wenn Sie Formulare stapelweise aus mehreren Objekten entfernen:

   * Wenn Sie Änderungen am Formular vorgenommen haben, führt das Entfernen des Formulars dazu, dass Ihre Änderungen verloren gehen und nicht wiederhergestellt werden können.
   * Nachdem Sie ein Formular entfernt haben, werden alle Felder aus diesem Formular, die sich im **Allgemeine Felder** aus diesem Abschnitt entfernt und kann hier nicht mehr bearbeitet werden.

1. Klicken **Formular wiederherstellen** , um das Formular wieder in den Zustand zu versetzen, in dem es sich vor der Bearbeitung der Objekte befand.
1. (Optional) Klicken Sie auf den Reduzierungspfeil neben dem Namen des Formulars, um ein Formular nach dem anderen auszublenden.

   Oder

   Klicken **Forms reduzieren** um alle Formulare gleichzeitig zu reduzieren.

1. (Optional) Klicken Sie auf den Pfeil neben dem Namen des Formulars, um ein Formular gleichzeitig zu erweitern.

   Oder

   Klicken **Forms erweitern** , um alle Formulare gleichzeitig zu erweitern. 

1. Klicken **Änderungen speichern**.
