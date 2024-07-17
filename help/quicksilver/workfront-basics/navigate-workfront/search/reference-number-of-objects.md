---
content-type: reference
navigation-topic: search
title: Referenzanzahl von Objekten verwenden
description: In  [!DNL Adobe Workfront] werden Elemente als Objekte identifiziert. Objekte entsprechen der Datenbank und werden verwendet, um Daten mit einem Element zu korrelieren. Referenznummern sind nützlich, um zwischen zwei ansonsten ähnlichen Objekten zu unterscheiden (z. B. Aufgaben mit demselben Namen). Sie können nach Referenznummern suchen und diese in Berichte aufnehmen.
feature: Get Started with Workfront
author: Lisa
exl-id: 94f5a174-21cc-4c10-88ed-89a8014d28f4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 0%

---

# Referenzanzahl von Objekten verwenden

In [!DNL Adobe Workfront] werden Elemente als Objekte identifiziert. Objekte entsprechen der Datenbank und werden verwendet, um Daten mit einem Element zu korrelieren.

Workfront weist jedem der folgenden Objekte automatisch eine eindeutige Referenznummer zu, wenn das Objekt erstellt wird:

* Projekte
* Aufgaben
* Probleme
* Dokumente

Referenznummern sind nützlich, um zwischen zwei ansonsten ähnlichen Objekten zu unterscheiden (z. B. Aufgaben mit demselben Namen). Sie können nach Referenznummern suchen und diese in Berichte aufnehmen.

>[!IMPORTANT]
>
>* [!DNL Workfront] weist Referenznummern kontinuierlich allen Kunden und allen Objekten zu. Wenn Sie beispielsweise eine Aufgabe erstellen, kann [!DNL Workfront] ihr die Referenznummer 0005 zuweisen. Wenn ein anderer Kunde als Nächstes ein Projekt erstellt, erhält sein Projekt möglicherweise die nächste verfügbare Referenznummer, z. B. 00006. Wenn Sie als Nächstes ein Problem erstellen, erhält Ihr Problem möglicherweise die Referenznummer 0007 usw.
>* Sie können die Reihenfolge der Referenznummern für Objekte in [!DNL Workfront] nicht steuern. Die Reihenfolge wird immer von unserer Datenbank gesteuert.
>



## Referenznummer eines Objekts anzeigen

Standardmäßig werden Referenznummern für Aufgaben und Probleme angezeigt. Sie können auch einfach [!DNL Workfront] so konfigurieren, dass Referenznummern für andere Objekttypen angezeigt werden.

* [Anzeigen von Referenznummern für Aufgaben und Probleme](#view-reference-numbers-for-tasks-and-issues)
* [Anzeigen von Referenznummern für andere Objekte](#view-reference-numbers-for-other-objects)
* [Anzeigen von Referenznummern in Berichten](#view-reference-numbers-in-reports)

### Anzeigen von Referenznummern für Aufgaben und Probleme

Referenznummern werden standardmäßig bei der Anzeige einer Aufgabe oder eines Problems angezeigt.  Um die Referenznummer anzuzeigen, klicken Sie im linken Bereich auf **[!UICONTROL Aufgabendetails]** oder **[!UICONTROL Problemdetails]** und suchen Sie dann den Abschnitt **[!UICONTROL Grundlegende Informationen]** in der Übersicht.

![](assets/reference-number-nwe-350x184.png)

### Anzeigen von Referenznummern für andere Objekte

Um Referenznummern für Objekte anzuzeigen, können Sie eine benutzerdefinierte Ansicht erstellen oder eine vorhandene Ansicht ändern und das Feld [!UICONTROL Referenznummer] zu einer Spalte in der Ansicht hinzufügen. Sie können beispielsweise die Ansicht [!UICONTROL Projekte] ändern, um die Referenznummer für alle Ihre Projekte anzuzeigen.

Informationen zum Erstellen oder Ändern einer Ansicht finden Sie unter [Übersicht über Ansichten in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

### Anzeigen von Referenznummern in Berichten

Sie können die Referenznummer für Objekte in Berichten anzeigen, indem Sie die Spalte [!UICONTROL Referenznummer] zum Bericht hinzufügen.

Informationen zum Hinzufügen einer Spalte zu einem Bericht finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Suchen nach einem Objekt anhand einer Referenznummer

Mit [!DNL Workfront] können Sie nach einem Objekt anhand der Referenznummer suchen.

Geben Sie die Referenznummer eines Objekts in das Feld **[!UICONTROL Suche]** ein und drücken Sie dann die **[!UICONTROL Eingabetaste]**.

Weitere Informationen zur Suche in Workfront finden Sie unter [Suchen [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/search/search-workfront.md).
