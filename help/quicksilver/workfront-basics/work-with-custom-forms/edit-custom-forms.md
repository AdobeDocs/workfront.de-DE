---
product-area: projects;user-management
keywords: Bearbeiten,Formulare,Rich,Text,Special,Format,Felder,Benutzerdefiniert,Informationen,Anpassen,Objekte
navigation-topic: work-with-custom-forms
title: Bearbeiten von Informationen in benutzerdefinierten Formularfeldern
description: Sie können Informationen in einem benutzerdefinierten Formular bearbeiten, nachdem das Formular mit einem Objekt verbunden wurde. Informationen zum Hinzufügen benutzerdefinierter Formulare zu Objekten finden Sie unter Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt.
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6ded38ef130fbcdde8d680f77f6db38fbd81efb4
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 0%

---

# Bearbeiten von Informationen in benutzerdefinierten Formularfeldern

<!--Audited: 10/2025-->

Sie können Informationen in einem benutzerdefinierten Formular bearbeiten, nachdem das Formular mit einem Objekt verbunden wurde. Informationen zum Hinzufügen benutzerdefinierter Formulare zu Objekten finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Paket</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Lizenz</p> </td> 
   <td> <p>Mitwirkender oder höher</p> 
   <p>Anfrage oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Bearbeitungszugriff auf das Objekt, für das Sie das benutzerdefinierte Formular bearbeiten möchten</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektberechtigungen</p> </td> 
   <td> 
    <ul> 
     <li> <p>Tragen Sie Berechtigungen oder höhere Berechtigungen für das Objekt bei, für das Sie das benutzerdefinierte Formular bearbeiten möchten</p> </li> 
     <li><p>Anzeigen von Berechtigungen für die Felder, die Sie bearbeiten möchten.</p></li> 
     <li><p>Bearbeitungsberechtigungen für die Abschnitte im Formular, in denen sich die zu bearbeitenden Felder befinden</p></li> 
    </ul></td> 
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
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Voraussetzungen

* Ihr Workfront-Administrator oder ein Plan-Benutzer mit administrativem Zugriff auf benutzerdefinierte Formulare muss benutzerdefinierte Formulare in Ihrer Umgebung erstellen. Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
* Benutzerdefinierte Formulare müssen an ein Objekt angehängt sein.

  Informationen zum Anwenden benutzerdefinierter Formulare auf ein Objekt finden Sie unter [Hinzufügen eines benutzerdefinierten Formulars zu einem Objekt](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## Bearbeiten von Informationen in einem benutzerdefinierten Formular

Die Bearbeitung von Informationen in einem benutzerdefinierten Formular, das an ein Objekt angehängt ist, ist für alle Objekte identisch. Informationen dazu, welche Objekte ein benutzerdefiniertes Formular haben können, finden Sie unter [Übersicht über benutzerdefinierte Formulare](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. Navigieren Sie zu einem Objekt, für das Sie Informationen im benutzerdefinierten Formular bearbeiten möchten.
1. Klicken Sie im **`<Object type>`Bedienfeld auf** Details.

   Wenn Sie beispielsweise Informationen in einem benutzerdefinierten Formular eines Projekts bearbeiten, klicken Sie auf **Projektdetails**.

1. Scrollen Sie zum benutzerdefinierten Formular. Wenn ein benutzerdefiniertes Formular an das -Objekt angehängt ist, wird der Name des Formulars als Bereich im Abschnitt Details angezeigt.
1. Klicken Sie ggf. auf den Pfeil ![](assets/expand-arrow-right.png) links neben dem Namen des benutzerdefinierten Formulars, um es zu erweitern.
1. Klicken Sie oben rechts auf der Seite auf das Symbol Bearbeiten ![](assets/edit-icon.png).
1. Beginnen Sie mit der Eingabe von Informationen in einem beliebigen Feld, auf das Sie Zugriff haben.

   ![](assets/click-in-field-to-edit-info-350x132.png)

   Oder

   Wenn noch keine Informationen in das Formular eingegeben wurden, klicken Sie auf **Hinzufügen+** für jedes Feld, auf das Sie Zugriff haben, und geben Sie die Informationen ein.

   ![](assets/plus-add-to-edit-info-350x180.png)

   Wenn mehrere benutzerdefinierte Formulare an das Objekt angehängt sind, können Sie dies für jedes Formular tun.

   Beachten Sie je nach Typ des Felds, in dem Sie arbeiten, Folgendes:

   * Für Optionsfeldfelder können Sie nur eine Option auswählen.
   * Sie können eine oder mehrere Optionen in einem Kontrollkästchenfeld auswählen, je nachdem, wie der Formularersteller das Feld konfiguriert hat.
   * Je nachdem, wie der Formularersteller das Feld konfiguriert hat, können Sie in einem Dropdown-Feld mit mehreren Auswahlmöglichkeiten eine oder mehrere Optionen auswählen.
   * Sie können Textfelder (fett, kursiv oder unterstrichen) nur formatieren, wenn der Benutzer, der das Formular erstellt hat, sie als Textfeld mit dem Feldtyp Formatierung eingerichtet hat. Einzelzeilige Textfelder und Absatztextfelder können nicht formatiert werden.
   * Sie können die Tageszeit in einem Datumsfeldtyp nur aktualisieren, wenn der Benutzer, der das Formular erstellt hat, es bei der Erstellung des Felds eingeschlossen hat.

   Informationen zu allen Feldtypen finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicken Sie auf **Änderungen speichern**.

   >[!IMPORTANT]
   >
   >Sie müssen alle erforderlichen Felder im Formular ausfüllen, bevor Sie das Formular speichern können. Auf den Namen eines erforderlichen Felds folgt ein Sternchen.
   >
   >![](assets/nwe-required-custom-field.png)

   Wenn jemand Daten in einem anderen Objekt ändert, auf das von berechneten benutzerdefinierten Feldern in Ihrem Objekt verwiesen wird, werden die Änderungen nicht automatisch in Ihrem Objekt übernommen. Informationen zum manuellen Aktualisieren aller berechneten benutzerdefinierten Felder in Ihrem Objekt finden Sie unter [Alle berechneten benutzerdefinierten Felder für ein Objekt neu berechnen](#recalculate-all-calculated-custom-fields-for-an-object) in diesem Artikel.

   Wenn abhängige Felder auf der Seite geändert werden, werden berechnete Felder im benutzerdefinierten Formular in Echtzeit dynamisch neu berechnet. Sie können den neuen berechneten Feldwert sehen, ohne das Formular zu speichern. Er wird jedoch erst dann auf das Formular und das Objekt angewendet, wenn Sie die Änderungen speichern. Dies gilt sowohl für berechnete Felder in Standardformularen als auch für benutzerdefinierte Formulare.

   Sie können auch alle berechneten benutzerdefinierten Felder für ein Objekt manuell aktualisieren, wenn Sie das Objekt zusammen mit anderen Objekten in einer Liste stapelweise bearbeiten. Anweisungen finden Sie unter [Alle berechneten benutzerdefinierten Felder für mehrere Objekte in einer Liste beim Bearbeiten der Objekte neu berechnen](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) in diesem Artikel.

## Alle berechneten benutzerdefinierten Felder für ein Objekt neu berechnen  {#recalculate-all-calculated-custom-fields-for-an-object}

>[!IMPORTANT]
>
>Sie müssen über ein benutzerdefiniertes Formular mit berechneten Feldern verfügen, die an das -Objekt angehängt sind, bevor Sie die Schritte in diesem Abschnitt ausführen können.


1. Navigieren Sie zur Hauptseite des Objekts, dessen benutzerdefinierte Felder Sie neu berechnen möchten.
1. Klicken Sie auf das **Mehr**-Menü ![](assets/more-icon.png) rechts neben dem Namen des Objekts und dann auf **Ausdrücke neu berechnen**.

   Dadurch werden alle benutzerdefinierten Felder im Formular des -Objekts neu berechnet.

## Alle berechneten benutzerdefinierten Felder für mehrere Objekte in einer Liste beim Bearbeiten der Objekte neu berechnen {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

Je nachdem, für welche Objekte Sie die benutzerdefinierten Ausdrücke neu berechnen möchten, können Sie dies in den folgenden Bereichen tun:

* In einer Liste von Objekten über das Menü Mehr oben in der Liste.
* Wenn Sie im Bearbeitungsfeld mehrere Objekte gleichzeitig auswählen und bearbeiten.

So berechnen Sie die benutzerdefinierten Felder mehrerer Objekte manuell neu, indem Sie sie stapelweise aus einer Liste oder einem Bericht bearbeiten:

1. Navigieren Sie zu einer Liste von Objekten, die benutzerdefinierte Formulare mit berechneten Feldern enthalten.
1. Wählen Sie die Objekte aus, deren berechnete benutzerdefinierte Felder Sie aktualisieren möchten.
1. Klicken Sie auf **Bearbeiten**.
1. Klicken Sie **linken Menü auf** Benutzerdefinierte Forms&quot; und wählen Sie dann **Benutzerdefinierte Ausdrücke neu berechnen**.
1. Klicken Sie **Speichern** **Änderungen**.

   Workfront berechnet alle benutzerdefinierten Felder für alle ausgewählten Objekte.

So berechnen Sie benutzerdefinierte Ausdrücke aus einer Objektliste neu:

1. Gehen Sie zu einer Projektliste oder einem Bericht und wählen Sie ein oder mehrere Projekte aus.
1. Klicken Sie auf die **** Mehr![](assets/more-icon.png) und dann auf **Benutzerdefinierte Ausdrücke neu berechnen**.

![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

Workfront berechnet sofort alle benutzerdefinierten Felder für alle ausgewählten Projekte.
Nicht alle Listen aller Objekte verfügen über diese Funktion.

>[!NOTE]
>
>Je nach Komplexität Ihrer Projekte empfehlen wir, bei der Massenberechnung berechneter benutzerdefinierter Felder keine große Anzahl von Projekten auszuwählen, um eine optimale Leistung sicherzustellen. Ein Projekt zu komplex kann beispielsweise durch mehrere Abhängigkeiten oder Zuweisungen oder eine große Anzahl benutzerdefinierter Felder werden.

