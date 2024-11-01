---
product-area: projects
navigation-topic: use-lists
title: Inline-Bearbeitungselemente in einer Liste in  [!DNL Adobe Workfront]
description: Sie können Objekte inline bearbeiten, wenn sie in einer Liste oder einem Bericht angezeigt werden. Wenn Sie die Informationen zu Objekten bearbeiten, die in einer Liste oder einem Bericht angezeigt werden, wird das Objekt sofort aktualisiert.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Inline-Bearbeitungselemente in einer Liste in [!DNL Adobe Workfront]

Sie können Objekte inline bearbeiten, wenn sie in einer Liste oder einem Bericht angezeigt werden. Wenn Sie die Informationen zu Objekten bearbeiten, die in einer Liste oder einem Bericht angezeigt werden, wird das Objekt sofort aktualisiert.

Wenn Sie ein Feld inline bearbeiten, das in einem benutzerdefinierten Formular enthalten ist, das nicht an das Objekt angehängt ist, wird das benutzerdefinierte Formular automatisch zum Objekt hinzugefügt. Wenn das Feld in mehreren benutzerdefinierten Formularen vorhanden ist, wird das zuletzt aktualisierte benutzerdefinierte Formular an das Objekt angehängt.

Weitere Informationen zu Listen finden Sie unter [Erste Schritte mit Listen in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Während die meisten in Listen oder Berichten angezeigten Objekte in [!DNL Adobe Workfront] inline bearbeitbar sind, gibt es einige Einschränkungen, darunter:

* Sie können keine berechneten Felder oder integrierten [!DNL Workfront] Felder bearbeiten, bei denen es sich um Berechnungen handelt.
* Sie können nur Felder bearbeiten, die direkt mit den Objekten in der Liste verknüpft sind. Felder, die zu Objekten gehören, die mit den Objekten in der Liste verknüpft sind, können nicht bearbeitet werden.\
   Sie können beispielsweise den Status einer Aufgabe in einem Aufgabenbericht bearbeiten, aber Sie können den Namen des Projekts, mit dem die Aufgabe in demselben Bericht verknüpft ist, nicht bearbeiten. Sie können den Namen des Projekts nur in einem Projektbericht bearbeiten.
* Sie können Felder nicht inline bearbeiten, wenn in der Listenansicht nicht die Standardwährung angezeigt wird.\
   Informationen zur Anzeige der Standardwährung finden Sie im Abschnitt [Berichte mit eindeutigen Währungen bearbeiten](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) im Artikel [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).
* In einer Liste angezeigte Flags und Symbole können nicht bearbeitet werden.
* Es ist nicht möglich, Berichtsfelder inline zu bearbeiten, die aus anderen Berichten stammen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Zugriff auf den Bereich bearbeiten, in dem sich die Liste befindet</p> <p>Um beispielsweise Aufgaben in einem Projekt inline zu bearbeiten, benötigen Sie Zugriff auf Projekte.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt.<br>Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebene erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Verwalten]</p> <p>Sie müssen auch über Berechtigungen zum Bearbeiten bestimmter Felder verfügen, z. B. benutzerdefinierte Felder, Status usw.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Objekte inline bearbeiten

1. Navigieren Sie zu einer Liste von Objekten, die Sie inline bearbeiten möchten.

   Die Liste sollte Felder anzeigen, die zu den Objekten oder Feldern gehören, die mit den Objekten in der Liste verknüpft sind.

1. Suchen Sie das Objekt, das Sie bearbeiten möchten, und klicken Sie dann in ein beliebiges Feld in der Liste.

   >[!TIP]
   >
   >Wenn Sie mehrere Seiten haben, können Sie ein Objekt wie folgt finden:
   >
   >   
   >   
   >   * **Paginierung**: Klicken Sie auf die Pfeile nach hinten und nach vorne, um zwischen den Seiten zu navigieren.\
   >     Der Bereich [!UICONTROL Paginierung] in der rechten unteren Ecke der Liste bleibt beim Scrollen durch die Liste fixierbar.
   >   * **Schnellfilter**: Klicken Sie auf das Filtersymbol oder geben Sie Alt+F ein, um den Schnellfilter zu öffnen. Geben Sie dann Text ein, um nur Elemente anzuzeigen, die den eingegebenen Text enthalten.\
   >     Der Schnellfilter befindet sich in der Symbolleiste der Liste. Weitere Informationen finden Sie unter [Anwenden des Schnellfilters auf eine Liste](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).


   Wenn das Feld bearbeitet werden kann, werden das Feld und alle anderen in der Liste angezeigten Felder in bearbeitbare Zellen umgewandelt.

   ![](assets/nwe-editable-cells-350x131.png)

1. Bearbeiten Sie die Informationen in dieser Zelle und drücken Sie dann [!UICONTROL Enter].

   >[!NOTE]
   >
   >Wenn ein benutzerdefiniertes Feld so konfiguriert wurde, dass eine Formatierung zulässig ist, können Sie Text beim Inline-Bearbeiten des Felds in einer aktualisierten Liste fett, kursiv oder unterstrichen formatieren.
   >Informationen zum Konfigurieren der Formatierung für ein benutzerdefiniertes Feld finden Sie unter [Benutzerdefiniertes Formular erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
   >Informationen zu aktualisierten Listen finden Sie im Abschnitt &quot;Der Unterschied zwischen den aktualisierten und den alten Listen&quot;im Artikel [Erste Schritte mit Listen in  [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Drücken Sie [!UICONTROL Tab] , um zur nächsten bearbeitbaren Zelle zu wechseln.
1. (Bedingt) Wenn Sie Ihre Änderungen nicht speichern können und die Zelle rot hervorgehoben ist, klicken Sie in das Feld, um die Validierungsmeldung zu überprüfen, die neben der Zelle angezeigt wird, und nehmen Sie die entsprechenden Aktualisierungen vor.

   Meistens passiert dies, wenn das falsche Format verwendet oder ein erforderliches Feld leer gelassen wurde.

1. Nachdem Sie alle Zellen bearbeitet haben, drücken Sie die [!UICONTROL Eingabetaste], um Ihre Änderungen zu speichern.
