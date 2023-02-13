---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Fehlermeldung: Es gibt ein leichtes Problem. Dieses Feld wird in einer Konfiguration mit mehreren Formularen verwendet."'
description: Wenn Sie eine Berechnung in einem berechneten benutzerdefinierten Feld in einem benutzerdefinierten Formular ändern und eine Fehlermeldung angibt, dass das Feld in einer Konfiguration mit mehreren Formularen verwendet wird, müssen Sie das Feld durch ein neues Feld ersetzen, das die gewünschte Berechnung enthält.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# Fehlermeldung: Es gibt ein leichtes Problem. Dieses Feld wird in einer Konfiguration mit mehreren Formularen verwendet

## Problem

Wenn Sie eine Berechnung für ein berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular ändern, [!DNL Adobe Workfront] kann die folgende Warnung anzeigen:

Hier gibt es ein kleines Problem.

[Das Feld] wird in einer Konfiguration mit mehreren Formularen verwendet. Wenn Sie diese Formel ändern möchten, müssen Sie dieses Feld entfernen und durch ein neues Feld mit der gewünschten Berechnung ersetzen.

## Ursache

Mindestens zwei benutzerdefinierte Formulare, die das berechnete benutzerdefinierte Feld enthalten, das Sie ändern möchten, werden an ein einzelnes Objekt in Ihrem [!DNL Workfront] -Instanz.

**Beispiel:** Benutzerdefinierte Formulare A und B werden jeweils an dieselbe Aufgabe angehängt. Beide Formulare enthalten ein berechnetes benutzerdefiniertes Feld namens &quot;Profit&quot;. Dieser Fehler tritt auf, wenn Sie versuchen, die Berechnung im Feld Gewinn in benutzerdefiniertem Formular A zu bearbeiten.

Sie können die Berechnung für das benutzerdefinierte Feld in einem der Formulare nicht ändern, da dies mit der Formel im selben Feld im anderen Formular in Konflikt gerät.
Um diesen Konflikt zu beheben, müssen Sie das Objekt finden, an das mehrere Formulare mit demselben berechneten benutzerdefinierten Feld angehängt sind. Führen Sie dann einen der folgenden Schritte aus:

* Entfernen Sie eines der Formulare aus dem Objekt.
* Ändern Sie die Berechnung nach Bedarf, aber tun Sie dies in allen benutzerdefinierten Formularen, die an das Objekt angehängt sind.
* Fügen Sie in allen benutzerdefinierten Formularen, die mit dem Objekt verbunden sind, ein neues berechnetes benutzerdefiniertes Feld hinzu, das die erforderliche Berechnung enthält, und markieren Sie das alte berechnete benutzerdefinierte Feld als veraltet.

In diesem Artikel wird erläutert, wie Sie das Objekt finden und dann das Problem auf eine dieser drei Arten lösen können.

## Suchen Sie das Objekt, an das die benutzerdefinierten Formulare angehängt sind. {#find-the-object-where-the-custom-forms-are-attached}

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Benutzer]** ![](assets/users-icon-in-main-menu.png).

1. Klicken **[!UICONTROL Benutzerdefinierte Forms]** > **[!UICONTROL Felder]**.
1. Wenden Sie die **[!UICONTROL Feldliste]** anzeigen, um das berechnete Feld zu finden, das Sie ändern möchten, und notieren Sie sich jedes benutzerdefinierte Formular, in dem es verwendet wird (z. B. Formular 1, Formular 2, Formular 3) .
1. Klicken **[!UICONTROL Forms]**, wenden Sie dann die **[!UICONTROL Formularliste]** anzeigen.
1. Klicken Sie auf **[!UICONTROL Filter]** Dropdown-Liste und **[!UICONTROL Neuer Filter]**.

1. Klicken **[!UICONTROL Filterregel hinzufügen]** Geben Sie dann &quot;benutzerdefinierten Formularnamen&quot;ein und wählen Sie diesen Wert aus, wenn er in der Liste angezeigt wird.
1. Auswählen **[!UICONTROL Gleich]** Geben Sie für den Filter-Modifikator den Namen jedes Formulars ein, das Sie in Schritt 1 zur Kenntnis genommen haben, und wählen Sie es dann aus, wenn es angezeigt wird.

   **Beispiel:** Benutzerdefinierter Formularname entspricht Formular 1, Formular 2, Formular 3.

1. Klicken **[!UICONTROL Filter speichern]**, benennen Sie den neuen Filter und klicken Sie auf **[!UICONTROL Filter speichern]**.

1. Notieren Sie sich in der Liste der Formulare den Objekttyp des Filters, z. B. Aufgabe oder Problem, der im **[!UICONTROL Typ]** Spalte.
1. Erstellen Sie für jedes benutzerdefinierte Formular, das Sie in Schritt 1 gefunden haben, ein neues benutzerdefiniertes Kontrollkästchen mit dem Standardwert Ja .

   **Beispiel:** Feld 1 auf Formular 1 = Ja, Feld 2 auf Formular 2 = Ja, Feld 3 auf Formular 3 = Ja. Das bedeutet &quot;Das berechnete benutzerdefinierte Feld ist in Formular 1 vorhanden&quot;oder &quot;Das berechnete benutzerdefinierte Feld ist in Formular 2 vorhanden&quot;usw.

1. Im **[!UICONTROL Suchsymbol]** ![](assets/search-icon.png) Klicken Sie in der rechten oberen Ecke des Bildschirms auf **[!UICONTROL Erweiterte Suche]**.
1. Klicken Sie auf das Objekt Ihres benutzerdefinierten Formulars (z. B. Problem) und klicken Sie auf **[!UICONTROL Ergebnisse filtern]** Klicken Sie auf **[!UICONTROL Filter hinzufügen]**.
1. Geben Sie den Namen eines Kontrollkästchenfelds im **[!UICONTROL Eingabe des Feldnamens beginnen]** und wählen Sie es aus, wenn es in der Liste angezeigt wird, und wählen Sie **[!UICONTROL Gleich]** und Typ **[!UICONTROL Ja]** (ohne Anführungszeichen) im folgenden Feld.

   **Beispiel:** Feld 1 gleich (Groß-/Kleinschreibung beachten) Ja.

1. Klicken **[!UICONTROL Filter hinzufügen]** und fügen Sie alle Kontrollkästchen-Felder zu Ihrer erweiterten Suche hinzu.

   Suchen Sie nach jeder möglichen Kombination.

   **Beispiel:** Erstellen Sie mehrere Filter mit den Kombinationen, die Sie finden, wie unten aufgeführt. Sie sollten Objekte mit mehreren angehängten benutzerdefinierten Formularen finden, die dieselben berechneten Felder enthalten. Möglicherweise finden Sie die folgenden Szenarien:

   * Feld 1= Ja + Feld 2 = Ja + Feld 3 = Ja (z. B. keine Objekte)
   * Feld 1= Ja + Feld 2 = Ja (z. B. keine Objekte)
   * Feld 1 = Ja + Feld 3 = Ja (z. B. zwei Objekte)

   Das bedeutet, dass das berechnete Feld sowohl in Formular 1 als auch in Formular 3 vorhanden ist, da die entsprechenden Kontrollkästchen-Felder (Feld 1 und Feld 3) auf diesen Objekten vorhanden sind.

   Feld 2 = Ja + Feld 3 = Ja (z. B. keine Objekte)

1. Fahren Sie mit einem der folgenden Abschnitte in diesem Artikel fort:

   * [Entfernen Sie eines der benutzerdefinierten Formulare aus dem Objekt und bearbeiten Sie dort die Berechnung.](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Bearbeiten Sie die Berechnung in allen angehängten benutzerdefinierten Formularen gleich.](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Fügen Sie ein neues berechnetes Feld mit der bearbeiteten Berechnung zu einem oder allen angehängten benutzerdefinierten Formularen hinzu.](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Entfernen Sie eines der benutzerdefinierten Formulare aus dem Objekt und bearbeiten Sie dort die Berechnung. {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Suchen Sie das Objekt, an das die benutzerdefinierten Formulare angehängt sind, wie hier beschrieben: [Suchen Sie das Objekt, an das die benutzerdefinierten Formulare angehängt sind.](#find-the-object-where-the-custom-forms-are-attached) in diesem Artikel, dann öffnen Sie das Objekt.
1. Entfernen Sie eines der benutzerdefinierten Formulare aus dem Objekt und speichern Sie dann das Objekt.

   >[!NOTE]
   >
   >Um die Felder aus dem Formular hinzuzufügen, das Sie aus dem Objekt entfernt haben, müssen Sie möglicherweise das benutzerdefinierte Formular bearbeiten, das an das Objekt angehängt bleibt. Auf diese Weise können Sie die benutzerdefinierten Dateninformationen für das Objekt beibehalten.

1. Bearbeiten Sie im entfernten benutzerdefinierten Formular die Berechnung für das benutzerdefinierte Feld, das Sie ursprünglich aktualisieren wollten, und klicken Sie dann auf **[!UICONTROL Speichern]**.

   Dieses Mal [!DNL Workfront] keinen Konflikt auslösen.

1. (Optional) Entfernen Sie die Kontrollkästchen-Felder aus den benutzerdefinierten Formularen oder löschen Sie sie aus [!DNL Workfront].

## Bearbeiten Sie die Berechnung in allen angehängten benutzerdefinierten Formularen gleich. {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Daten gehen in den Objekten verloren, an denen das benutzerdefinierte Formular bereits angehängt ist, wenn Sie diese Schritte ausführen. Wenn das berechnete Feld jedoch auf statische, nicht berechnete Felder verweist, können Sie [!UICONTROL Benutzerdefinierte Ausdrücke neu berechnen] -Option für das Objekt zum Wiederherstellen der verlorenen Daten

1. Suchen Sie das Objekt, an das die benutzerdefinierten Formulare angehängt sind, wie hier beschrieben: [Suchen Sie das Objekt, an das die benutzerdefinierten Formulare angehängt sind.](#find-the-object-where-the-custom-forms-are-attached) in diesem Artikel.
1. Entfernen Sie das Feld aus allen benutzerdefinierten Formularen, die an das Objekt angehängt sind, und speichern Sie dann die Formulare.

1. Fügen Sie das benutzerdefinierte Feld, das die neue Berechnung enthält, wieder zu den benutzerdefinierten Formularen hinzu.

   >[!IMPORTANT]
   >
   >Die Berechnungen müssen in allen angehängten benutzerdefinierten Formularen identisch sein.

1. (Optional) Entfernen Sie die Kontrollkästchen-Felder aus den Formularen oder löschen Sie sie aus [!DNL Workfront].

## Fügen Sie ein neues berechnetes Feld mit der bearbeiteten Berechnung zu einem oder allen angehängten benutzerdefinierten Formularen hinzu. {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Um zu vermeiden, dass Daten im vorhandenen berechneten benutzerdefinierten Feld verloren gehen oder wenn Sie die bearbeitete Berechnung nur in einem der benutzerdefinierten Formulare durchführen müssen, die an das gefundene Objekt angehängt sind:

1. Suchen Sie das Objekt, an das die benutzerdefinierten Formulare angehängt sind, wie hier beschrieben: [Suchen Sie das Objekt, an das die benutzerdefinierten Formulare angehängt sind.](#find-the-object-where-the-custom-forms-are-attached) in diesem Artikel.
1. Fügen Sie ein neues berechnetes benutzerdefiniertes Feld mit der erforderlichen Berechnung zu einem oder allen Formularen hinzu.
1. Umbenennen des alten berechneten benutzerdefinierten Felds **Obsolete**.

   Bei allen Formularen, die mit dem Objekt verbunden waren, behält dieses ältere, berechnete benutzerdefinierte Formular seine historischen Daten bei, die Verwendung wird jedoch eingestellt.

   >[!IMPORTANT]
   >
   >Auf das ältere Feld kann in anderen berechneten benutzerdefinierten Feldern verwiesen werden. Daher müssen Sie diese Berechnungen nach der Namensänderung aktualisieren.

1. (Optional) Entfernen Sie die Kontrollkästchen-Felder aus den Formularen oder löschen Sie sie aus Workfront.

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
