---
product-area: projects
navigation-topic: use-lists
title: Inline-Bearbeitungselemente in einer Liste in [!DNL Adobe Workfront]
description: Sie können Objekte inline bearbeiten, wenn sie in einer Liste oder einem Bericht angezeigt werden. Wenn Sie die Informationen zu Objekten bearbeiten, die in einer Liste oder einem Bericht angezeigt werden, wird das Objekt sofort aktualisiert.
feature: Get Started with Workfront
author: Lisa
exl-id: a94b5aaf-71de-4fcd-946b-459ca3edf7e4
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '734'
ht-degree: 0%

---

# Inline-Bearbeitungselemente in einer Liste in [!DNL Adobe Workfront]

Sie können Objekte inline bearbeiten, wenn sie in einer Liste oder einem Bericht angezeigt werden. Wenn Sie die Informationen zu Objekten bearbeiten, die in einer Liste oder einem Bericht angezeigt werden, wird das Objekt sofort aktualisiert.

Wenn Sie ein Feld inline bearbeiten, das in einem benutzerdefinierten Formular enthalten ist, das nicht an das Objekt angehängt ist, wird das benutzerdefinierte Formular automatisch zum Objekt hinzugefügt. Wenn das Feld in mehreren benutzerdefinierten Formularen vorhanden ist, wird das benutzerdefinierte Formular, das zuletzt aktualisiert wurde, an das Objekt angehängt.

Weitere Informationen zu Listen finden Sie unter [Erste Schritte mit Listen in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Die meisten in Listen oder Berichten angezeigten Objekte können in [!DNL Adobe Workfront], gibt es einige Einschränkungen, die Folgendes umfassen:

* Berechnete Felder können nicht bearbeitet werden oder [!DNL Workfront] integrierte Felder, die Berechnungen sind.
* Sie können nur Felder bearbeiten, die direkt mit den Objekten in der Liste verknüpft sind. Felder, die zu Objekten gehören, die mit den Objekten in der Liste verknüpft sind, können nicht bearbeitet werden.\
   Sie können beispielsweise den Status einer Aufgabe in einem Aufgabenbericht bearbeiten, aber Sie können den Namen des Projekts, mit dem die Aufgabe in demselben Bericht verknüpft ist, nicht bearbeiten. Sie können den Namen des Projekts nur in einem Projektbericht bearbeiten.
* Sie können Felder nicht inline bearbeiten, wenn in der Listenansicht nicht die Standardwährung angezeigt wird.\
   Informationen zur Anzeige der Standardwährung finden Sie im Abschnitt [Berichte mit eindeutigen Währungen bearbeiten](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md#editing-reports-with-unique-currencies) im Artikel [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

* In einer Liste angezeigte Flags und Symbole können nicht bearbeitet werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Zugriff auf den Bereich bearbeiten, in dem sich die Liste befindet</p> <p>Um beispielsweise Aufgaben in einem Projekt inline zu bearbeiten, benötigen Sie Zugriff auf Projekte.</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen.<br>Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Verwalten]</p> <p>Sie müssen auch über Berechtigungen zum Bearbeiten bestimmter Felder verfügen, z. B. benutzerdefinierte Felder, Status usw.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

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
   >   * **Paginierung**: Klicken Sie auf die Pfeile nach hinten und nach vorne, um zwischen Seiten zu navigieren.\
      >     In der rechten unteren Ecke der Liste befindet sich das [!UICONTROL Paginierung] bleibt beim Scrollen durch die Liste fixierbar.
   >   * **Schnellfilter**: Klicken Sie auf das Filtersymbol oder geben Sie Alt+F ein, um den Schnellfilter zu öffnen. Geben Sie dann Text ein, um nur die Elemente anzuzeigen, die den eingegebenen Text enthalten.\
      >     Der Schnellfilter befindet sich in der Symbolleiste der Liste. Weitere Informationen finden Sie unter [Schnellfilter auf Listen anwenden](../../../workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).



   Wenn das Feld bearbeitet werden kann, werden das Feld und alle anderen in der Liste angezeigten Felder in bearbeitbare Zellen umgewandelt.

   ![](assets/nwe-editable-cells-350x131.png)

1. Bearbeiten Sie die Informationen in dieser Zelle und drücken Sie dann die [!UICONTROL Eingabe].

   >[!NOTE]
   >
   >Wenn ein benutzerdefiniertes Feld so konfiguriert wurde, dass eine Formatierung zulässig ist, können Sie Text beim Inline-Bearbeiten des Felds in einer aktualisierten Liste fett, kursiv oder unterstrichen formatieren.\
   >Informationen zum Konfigurieren der Formatierung für ein benutzerdefiniertes Feld finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).\
   >Informationen zu aktualisierten Listen finden Sie im Artikel im Abschnitt &quot;Unterschied zwischen den aktualisierten und den alten Listen&quot; [Erste Schritte mit Listen in [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

1. Presse [!UICONTROL Registerkarte] , um zur nächsten bearbeitbaren Zelle zu wechseln.
1. (Bedingt) Wenn Sie Ihre Änderungen nicht speichern können und die Zelle rot hervorgehoben ist, klicken Sie in das Feld, um die Validierungsmeldung zu überprüfen, die neben der Zelle angezeigt wird, und nehmen Sie die entsprechenden Aktualisierungen vor.

   Meistens passiert dies, wenn das falsche Format verwendet oder ein erforderliches Feld leer gelassen wurde.

1. Nachdem Sie die Bearbeitung aller Zellen abgeschlossen haben, drücken Sie die [!UICONTROL Eingabe] , um Ihre Änderungen zu speichern.
