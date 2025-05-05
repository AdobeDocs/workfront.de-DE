---
product-area: projects
navigation-topic: use-lists
title: Inline-Bearbeitung von Elementen in einer Liste in  [!DNL Adobe Workfront]
description: Sie können Objekte inline bearbeiten, wenn sie in einer Liste oder einem Bericht angezeigt werden. Wenn Sie die Informationen zu Objekten bearbeiten, die in einer Liste oder einem Bericht angezeigt werden, wird das Objekt sofort aktualisiert.
feature: Get Started with Workfront
author: Nolan
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# Inline-Bearbeitung von Elementen in einer Liste in [!DNL Adobe Workfront]

<!--Audited: 11/2024-->

Sie können Objekte inline bearbeiten, wenn sie in einer Liste oder einem Bericht angezeigt werden. Wenn Sie die Informationen zu Objekten bearbeiten, die in einer Liste oder einem Bericht angezeigt werden, wird das Objekt sofort aktualisiert.

Wenn Sie ein Feld inline bearbeiten, das in einem benutzerdefinierten Formular enthalten ist, das nicht an das -Objekt angehängt ist, wird das benutzerdefinierte Formular automatisch zum -Objekt hinzugefügt. Wenn das Feld in mehreren benutzerdefinierten Formularen vorhanden ist, wird das zuletzt aktualisierte benutzerdefinierte Formular an das -Objekt angehängt.

Weitere Informationen zu Listen finden Sie unter [Erste Schritte mit Listen in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Während die meisten Objekte, die in Listen oder Berichten angezeigt werden, in [!DNL Adobe Workfront] inline bearbeitbar sind, gibt es einige Einschränkungen, darunter:

* Berechnete Felder oder integrierte Felder, bei denen es sich um Berechnungen handelt, können nicht bearbeitet [!DNL Workfront].
* Sie können nur Felder bearbeiten, die direkt mit den Objekten in der Liste verknüpft sind. Sie können keine Felder bearbeiten, die zu Objekten gehören, die mit den Objekten in der Liste verknüpft sind.

  Sie können beispielsweise den Status einer Aufgabe in einem Aufgabenbericht bearbeiten, aber nicht den Namen des Projekts, dem die Aufgabe im selben Bericht zugeordnet ist. Der Projektname kann nur in einem Projektbericht bearbeitet werden.
* Sie können Felder nicht inline bearbeiten, wenn in der Ansicht für eine Liste nicht die Standardwährung angezeigt wird.

  Informationen zur Anzeige der Standardwährung finden Sie im Abschnitt [Berichte mit eindeutigen Währungen bearbeiten](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) im Artikel [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).
* Sie können keine Flags und Symbole bearbeiten, die in einer Liste angezeigt werden.
* Berichtsfelder, die aus anderen Berichten bezogen werden, können nicht inline bearbeitet werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender oder höher </p></li>
   </ul>

<p>Aktuell:</p>
   <ul><li><p>Anfrage oder höher</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf den Bereich der Liste</p> <p>Um beispielsweise Aufgaben in einem Projekt inline zu bearbeiten, benötigen Sie [!UICONTROL Bearbeiten]-Zugriff auf Projekte.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL verwalten]</p> <p>Sie müssen auch über Berechtigungen zum Bearbeiten bestimmter Felder verfügen, z. B. benutzerdefinierte Felder, Status usw.</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objekte inline bearbeiten

1. Navigieren Sie zu einer Liste von Objekten, die Sie inline bearbeiten möchten.

   Die Liste sollte Felder anzeigen, die zu den Objekten gehören, oder Felder, die zu den Objekten gehören, die mit den Objekten in der Liste verknüpft sind.

1. Suchen Sie das Objekt, das Sie bearbeiten möchten, und klicken Sie dann in ein beliebiges Feld in der Liste.

   >[!TIP]
   >
   >Wenn Sie über mehrere Seiten verfügen, können Sie ein -Objekt mithilfe von Folgendem finden:
   >
   >   * **Paginierung**: Klicken Sie auf die Rückwärts- und Vorwärtspfeile, um zwischen Seiten zu navigieren.
   >     Der Bereich [!UICONTROL Paginierung“ befindet sich in der rechten unteren Ecke &#x200B;] Liste und bleibt beim Bildlauf beibehalten.
   >   * **Schnellfilter**: Klicken Sie auf das Filtersymbol oder geben Sie Alt+F ein, um den Schnellfilter zu öffnen, und geben Sie dann Text ein, um nur Elemente anzuzeigen, die den eingegebenen Text enthalten.
   >     Der Schnellfilter befindet sich in der Listen-Symbolleiste. Weitere Informationen finden Sie unter [Anwenden des Schnellfilters auf eine Liste](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

   Wenn das Feld bearbeitet werden kann, werden das Feld und alle anderen Felder, die in der Liste angezeigt werden, zu bearbeitbaren Zellen.

   ![Bearbeitbare Zellen](assets/nwe-editable-cells-350x131.png)

1. Bearbeiten Sie die Informationen in dieser Zelle und drücken Sie dann die [!UICONTROL Eingabetaste].

   >[!NOTE]
   >
   >Wenn ein benutzerdefiniertes Feld für die Formatierung konfiguriert wurde, können Sie Text fett, kursiv oder unterstreichen, wenn Sie das Feld in einer aktualisierten Liste inline bearbeiten.
   >Informationen zum Konfigurieren der Formatierung für ein benutzerdefiniertes Feld finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
   >Informationen zu aktualisierten Listen finden Sie im Abschnitt „Der Unterschied zwischen den aktualisierten und den veralteten Listen“ im Artikel [Erste Schritte mit Listen in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Drücken Sie [!UICONTROL Tabulatortaste], um zur nächsten bearbeitbaren Zelle zu wechseln.
1. (Bedingt) Wenn Sie Ihre Änderungen nicht speichern können und die Zelle rot umrandet ist, klicken Sie in das Feld, um die neben der Zelle angezeigte Validierungsmeldung zu überprüfen und die entsprechenden Aktualisierungen vorzunehmen.

   Dies geschieht meist, wenn das falsche Format verwendet wird oder ein erforderliches Feld leer gelassen wurde.

1. Nachdem Sie alle Zellen bearbeitet haben, drücken Sie [!UICONTROL Eingabetaste] um Ihre Änderungen zu speichern.
