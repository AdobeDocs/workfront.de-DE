---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: Es gibt ein leichtes Problem. Dieses Feld wird in einer Multi-Form-Konfiguration verwendet'
description: Wenn Sie eine Berechnung in einem berechneten benutzerdefinierten Feld in einem benutzerdefinierten Formular ändern und eine Fehlermeldung Ihnen mitteilt, dass das Feld in einer Multi-Form-Konfiguration verwendet wird, müssen Sie das Feld durch ein neues Feld ersetzen, das die Berechnung enthält, die Sie verwenden möchten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: 8b93842d7ce61c7c84b07639b6329bedf4254ffd
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 0%

---

# Fehlermeldung: Es gibt ein leichtes Problem. Dieses Feld wird in einer Multi-Form-Konfiguration verwendet

## Problem

Wenn Sie eine Berechnung für ein berechnetes benutzerdefiniertes Feld in einem benutzerdefinierten Formular ändern, wird [!DNL Adobe Workfront] möglicherweise die folgende Warnung angezeigt:

Hier gibt es ein kleines Problem.

[Das Feld] wird in einer Multi-Form-Konfiguration verwendet. Wenn Sie diese Formel ändern möchten, müssen Sie dieses Feld entfernen und durch ein neues ersetzen, das die gewünschte Berechnung enthält.

## Ursache

Mindestens zwei benutzerdefinierte Formulare, die das berechnete benutzerdefinierte Feld enthalten, das Sie ändern möchten, werden an ein einzelnes Objekt in Ihrer [!DNL Workfront] angehängt.

**Beispiel** Benutzerdefinierte Formulare A und B sind beide an dieselbe Aufgabe angehängt. Beide Formulare enthalten ein berechnetes benutzerdefiniertes Feld namens Gewinn . Der Fehler tritt auf, wenn Sie versuchen, die Berechnung im Feld „Gewinn“ im benutzerdefinierten Formular A zu bearbeiten.

Sie können die Berechnung für das benutzerdefinierte Feld in einem der Formulare nicht ändern, da dies mit der Formel im selben Feld im anderen Formular kollidieren würde.
Um diesen Konflikt zu lösen, müssen Sie das -Objekt finden, an das mehrere Formulare mit demselben berechneten benutzerdefinierten Feld angehängt sind, und dann einen der folgenden Schritte ausführen:

* Entfernen Sie eines der Formulare aus dem -Objekt.
* Ändern Sie die Berechnung nach Bedarf, tun Sie dies jedoch in allen benutzerdefinierten Formularen, die mit dem -Objekt verbunden sind.
* Fügen Sie in allen benutzerdefinierten Formularen, die an das -Objekt angehängt sind, ein neues berechnetes benutzerdefiniertes Feld hinzu, das die benötigte Berechnung enthält, und markieren Sie das alte berechnete benutzerdefinierte Feld als veraltet.

In diesem Artikel wird erläutert, wie Sie das Objekt finden und dann das Problem auf eine dieser drei Arten beheben können.

>[!NOTE]
>
>Wenn der Fehler angezeigt wird, Sie jedoch nicht mehr als ein Objekt finden können, das das benutzerdefinierte Feld enthält, überprüfen Sie den Papierkorb. Es ist möglich, dass ein Objekt im Papierkorb das Feld enthält. Da Objekte im Papierkorb jederzeit wiederhergestellt werden können, tritt der Multiform-Konfliktfehler weiterhin auf, bis der Konflikt behoben ist.
>
>Um ein Feld mit einem anderen Ausdruck hinzuzufügen, müssen Sie diesen Konflikt lösen, indem Sie einen der folgenden Schritte ausführen:
>
>* Entfernen des Felds aus dem widersprüchlichen benutzerdefinierten Formular
>* Stellen Sie das gelöschte Objekt wieder her, trennen Sie eines der widersprüchlichen benutzerdefinierten Formulare, und löschen Sie das Objekt dann bei Bedarf erneut.

## Suchen des Objekts, an das die benutzerdefinierten Formulare angehängt sind {#find-the-object-where-the-custom-forms-are-attached}

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Benutzerdefinierte Forms]** > **[!UICONTROL Felder]**.
1. Wenden Sie die Ansicht **[!UICONTROL Feldliste]** an, um das berechnete Feld zu finden, das Sie ändern möchten, und notieren Sie sich jedes benutzerdefinierte Formular, für das es verwendet wird (z. B. Formular 1, Formular 2, Formular 3) .
1. Klicken Sie auf **[!UICONTROL Forms]** und wenden Sie dann die Ansicht **[!UICONTROL Formularliste]** an.
1. Klicken Sie auf **[!UICONTROL Dropdown]** Liste „Filter“ und dann auf **[!UICONTROL Neuer Filter]**.

1. Klicken Sie **[!UICONTROL Filterregel hinzufügen]**, geben Sie dann „Name des benutzerdefinierten Formulars“ ein und wählen Sie diesen Wert aus, wenn er in der Liste angezeigt wird.
1. Wählen Sie **[!UICONTROL Gleich]** für den Filtermodifikator, tippen Sie den Namen jedes Formulars ein, auf das Sie sich in Schritt 1 notiert haben, und wählen Sie es aus, wenn es angezeigt wird.

   **Beispiel:** benutzerdefinierte Formularname ist gleich Formular 1, Formular 2, Formular 3.

1. Klicken Sie auf **[!UICONTROL Filter speichern]** benennen Sie dann den neuen Filter und klicken Sie auf **[!UICONTROL Filter speichern]**.

1. Notieren Sie sich in der Liste der Formulare den Objekttyp des Filters, z. B. Aufgabe oder Problem, der in der Spalte **[!UICONTROL Typ]** angezeigt wird.
1. Erstellen Sie für jedes benutzerdefinierte Formular, das Sie in Schritt 1 gefunden haben, ein neues benutzerdefiniertes Kontrollkästchen mit dem einzigen Standardwert Ja .

   **Beispiel:** Feld 1 im Formular 1 = Ja, Feld 2 im Formular 2 = Ja, Feld 3 im Formular 3 = Ja. Dies bedeutet: „Das berechnete benutzerdefinierte Feld ist in Formular 1 vorhanden“ oder „Das berechnete benutzerdefinierte Feld ist in Formular 2 vorhanden“ usw.

1. Klicken Sie **[!UICONTROL Suchsymbol]** ![Suchsymbol](assets/search-icon.png) in der rechten oberen Ecke des Bildschirms auf **[!UICONTROL Erweiterte Suche]**.
1. Klicken Sie auf das Objekt Ihres benutzerdefinierten Formulars (z. B. „Problem„), klicken Sie **[!UICONTROL Ergebnisse filtern]** und dann auf **[!UICONTROL Filter hinzufügen]**.
1. Beginnen Sie mit der Eingabe des Namens eines Kontrollkästchenfelds in das Feld **[!UICONTROL Beginnen Sie mit der Eingabe des Feldnamens]** und wählen Sie es aus, wenn es in der Liste angezeigt wird. Wählen Sie dann **[!UICONTROL Gleich]** aus und geben Sie **[!UICONTROL Ja]** (ohne Anführungszeichen) in das folgende Feld ein.

   **Beispiel:** Feld 1 ist gleich (Groß-/Kleinschreibung beachten) Ja.

1. Klicken Sie **[!UICONTROL Filter hinzufügen]** und fügen Sie alle Kontrollkästchen zu Ihrer erweiterten Suche hinzu.

   Suchen Sie nach jeder möglichen Kombination.

   **Beispiel** Erstellen Sie mehrere Filter mit den gefundenen Kombinationen, wie unten aufgeführt. Sie sollten Objekte mit mehreren angehängten benutzerdefinierten Formularen finden, die dieselben berechneten Felder enthalten. Möglicherweise werden die folgenden Szenarien angezeigt:

   * Feld 1= Ja + Feld 2 = Ja + Feld 3 = Ja (z. B. keine Objekte)
   * Feld 1= Ja + Feld 2 = Ja (z. B. keine Objekte)
   * Feld 1= Ja + Feld 3 = Ja (z. B. zwei Objekte)

   Das bedeutet, dass das berechnete Feld sowohl auf Formular 1 als auch auf Formular 3 vorhanden ist, da die entsprechenden Kontrollkästchen-Felder (Feld 1 und Feld 3) auf diesen Objekten vorhanden sind.

   Feld 2 = Ja + Feld 3 = Ja (z. B. keine Objekte)

1. Fahren Sie mit einem der folgenden Abschnitte in diesem Artikel fort:

   * [Entfernen Sie eines der benutzerdefinierten Formulare aus dem Objekt und bearbeiten Sie dort die Berechnung](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Nehmen Sie in der Berechnung in allen angehängten benutzerdefinierten Formularen identische Änderungen vor](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Ein neues berechnetes Feld mit der bearbeiteten Berechnung zu einem oder allen angehängten benutzerdefinierten Formularen hinzufügen](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Entfernen Sie eines der benutzerdefinierten Formulare aus dem Objekt und bearbeiten Sie dort die Berechnung {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Suchen Sie das -Objekt, an das die benutzerdefinierten Formulare angehängt sind, wie in [Suchen des -Objekts, an das die benutzerdefinierten Formulare angehängt sind](#find-the-object-where-the-custom-forms-are-attached) in diesem Artikel beschrieben, und öffnen Sie dann das -Objekt.
1. Entfernen Sie eines der benutzerdefinierten Formulare aus dem -Objekt und speichern Sie dann das -Objekt.

   >[!NOTE]
   >
   >Um die Felder aus dem Formular hinzuzufügen, das Sie aus dem Objekt entfernt haben, müssen Sie möglicherweise das benutzerdefinierte Formular bearbeiten, das mit dem Objekt verbunden bleibt. Auf diese Weise können Sie die benutzerdefinierten Dateninformationen des -Objekts beibehalten.

1. Bearbeiten Sie im entfernten benutzerdefinierten Formular die Berechnung für das benutzerdefinierte Feld, das Sie ursprünglich aktualisieren wollten, und klicken Sie dann auf **[!UICONTROL Speichern]**.

   Diesmal sollte [!DNL Workfront] auf keinen Konflikt stoßen.

1. (Optional) Entfernen Sie die Kontrollkästchen-Felder aus den benutzerdefinierten Formularen oder löschen Sie sie aus [!DNL Workfront].

## Nehmen Sie in der Berechnung in allen angehängten benutzerdefinierten Formularen identische Änderungen vor {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Daten gehen in den Objekten verloren, an die das benutzerdefinierte Formular bereits angehängt ist, wenn Sie diese Schritte ausführen. Wenn das berechnete Feld jedoch auf statische Felder und nicht auf berechnete Felder verweist, können Sie die Option [!UICONTROL Benutzerdefinierte Ausdrücke neu berechnen] auf dem -Objekt verwenden, um die verlorenen Daten wiederherzustellen

1. Suchen Sie das -Objekt, an das die benutzerdefinierten Formulare angehängt sind, wie in [Suchen des -Objekts, an das die benutzerdefinierten Formulare angehängt sind](#find-the-object-where-the-custom-forms-are-attached) in diesem Artikel erläutert.
1. Entfernen Sie das Feld aus allen benutzerdefinierten Formularen, die mit dem -Objekt verbunden sind, und speichern Sie dann die Formulare.

1. Fügen Sie das benutzerdefinierte Feld, das die neue Berechnung enthält, wieder zu den benutzerdefinierten Formularen hinzu.

   >[!IMPORTANT]
   >
   >Die Berechnungen müssen in allen beigefügten benutzerdefinierten Formularen identisch sein.

1. (Optional) Entfernen Sie die Kontrollkästchen aus den Formularen oder löschen Sie sie aus [!DNL Workfront].

## Ein neues berechnetes Feld mit der bearbeiteten Berechnung zu einem oder allen angehängten benutzerdefinierten Formularen hinzufügen {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

Um zu vermeiden, dass Daten im vorhandenen berechneten benutzerdefinierten Feld verloren gehen, oder wenn Sie die bearbeitete Berechnung in nur einem der benutzerdefinierten Formulare anhängen müssen, die an das gefundene Objekt angehängt sind:

1. Suchen Sie das -Objekt, an das die benutzerdefinierten Formulare angehängt sind, wie in [Suchen des -Objekts, an das die benutzerdefinierten Formulare angehängt sind](#find-the-object-where-the-custom-forms-are-attached) in diesem Artikel erläutert.
1. Fügen Sie ein neues berechnetes benutzerdefiniertes Feld hinzu, das die Berechnung enthält, die Sie für eines oder alle Formulare benötigen.
1. Benennen Sie das alte berechnete benutzerdefinierte Feld um **Veraltet**.

   Bei allen Formularen, die mit dem Objekt verbunden waren, behält dieses ältere berechnete benutzerdefinierte Formular seine historischen Daten bei, Benutzer verwenden es jedoch nicht mehr.

   >[!IMPORTANT]
   >
   >Das ältere Feld kann in anderen berechneten benutzerdefinierten Feldern referenziert werden, sodass Sie diese Berechnungen aktualisieren müssen, nachdem Sie seinen Namen geändert haben.

1. (Optional) Entfernen Sie die Kontrollkästchen aus den Formularen oder löschen Sie sie aus Workfront.

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
</blockquote>
-->
