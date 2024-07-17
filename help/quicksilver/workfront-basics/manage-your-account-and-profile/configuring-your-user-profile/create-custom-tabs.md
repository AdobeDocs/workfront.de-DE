---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Erstellen benutzerdefinierter Abschnitte
description: Die Informationen, die Sie in der [!DNL Workfront] Webanwendung sehen, werden häufig standardmäßig in den Abschnitten im linken Bereich angezeigt. Jeder Abschnitt enthält verschiedene Informationen zu einem  [!DNL Workfront] Bereich oder Objekt.
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---

# Erstellen benutzerdefinierter Abschnitte

## [!DNL Adobe Workfront] Abschnitte

Die Informationen, die Sie in der Webanwendung &quot;[!DNL Workfront]&quot;sehen, werden häufig standardmäßig in den linken Bedienfeldern angezeigt. Jeder Abschnitt enthält verschiedene Informationen zu einem [!DNL Workfront] -Bereich oder -Objekt.\
Weitere Informationen zu den Standardbereichen von [!DNL Workfront] finden Sie im Artikel [Über das standardmäßige [!DNL Adobe Workfront] Layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Zusätzlich zu den Abschnitten, die standardmäßig mit [!DNL Workfront] geliefert werden, können Sie ein Dashboard hinzufügen, in dem Sie Informationen anzeigen können, die für Ihren Workflow relevant sind. Dashboards können nicht allen Bereichen und Objekten hinzugefügt werden.

In der folgenden Tabelle sind alle [!DNL Workfront] -Bereiche und -Objekte aufgeführt, die Abschnitte im linken Bereich enthalten und die angepasst werden können:

| **[!DNL Workfront]Bereich oder Objekt** | **Standardsystemabschnitte** | **Benutzerdefinierte Abschnitte** |
|---|---|---|
| Bereich [!UICONTROL Projekte] | ✓ | ✓ |
| [!UICONTROL Team] | ✓ |   |
| Bereich [!UICONTROL Anforderungen] | ✓ |   |
| Bereich [!UICONTROL Timesheets] | ✓ |   |
| [!UICONTROL Portfolio] | ✓ | ✓ |
| [!UICONTROL Programm] | ✓ | ✓ |
| [!UICONTROL Projekt] | ✓ | ✓ |
| [!UICONTROL Aufgabe] | ✓ |  ✓ |
| [!UICONTROL Probleme] |  ✓ |  ✓ |
| [!UICONTROL Benutzer] |  ✓ |  ✓ |
| [!UICONTROL Document] |  ✓ |  ✓ |

{style="table-layout:auto"}

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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
   <td>[!UICONTROL Reviewer] oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td>Zugriff auf den Objekttyp anzeigen</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um herauszufinden, welchen Plan oder welchen Lizenztyp Sie haben.

## Hinzufügen eines Dashboards im linken Bereich eines [!DNL Workfront] -Objekts oder -Bereichs

Bevor Sie ein Dashboard hinzufügen können, müssen Sie das Dashboard mit allen gewünschten Informationen erstellen. Sie können auch eine externe Seite erstellen.\
Weitere Informationen zum Erstellen von Dashboards finden Sie im Artikel [Dashboard erstellen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md) .\
Weitere Informationen zum Erstellen externer Seiten finden Sie im Artikel [Einbetten einer externen Webseite in ein Dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Nachdem Sie das Dashboard oder die externe Seite erstellt haben, können Sie sie zum linken Bereich hinzufügen.

1. Navigieren Sie zu einem der Bereiche oder Objekte mit dem Namen &quot;[!DNL Workfront]&quot;, in denen Sie einen benutzerdefinierten Abschnitt im linken Bereich hinzufügen können.\
   Oder
1. Navigieren Sie zu einem Objekt, dem Sie im linken Bereich ein [!UICONTROL Dashboard] hinzufügen können.\
   Weitere Informationen dazu, welchen Bereichen und Objekten Sie benutzerdefinierte Abschnitte hinzufügen können, finden Sie unter [[!DNL Adobe Workfront] Abschnitte](#adobe-workfront-sections).
1. Klicken Sie im linken Bereich auf **[!UICONTROL Dashboard hinzufügen]** .
1. Geben Sie im Feld **[!UICONTROL Name des Quick-Links]** einen Namen für das Dashboard ein. Dies ist nur für Sie sichtbar.
1. Geben Sie den Namen eines vorhandenen Dashboards oder einer externen Seite in das Feld **[!UICONTROL Dashboard auswählen]** ein und wählen Sie dann das Dashboard aus, wenn es in der Liste angezeigt wird.
1. Klicken Sie auf **[!UICONTROL Hinzufügen]**.
1. (Optional) Ziehen Sie die Abschnitte in die Reihenfolge, in der sie angezeigt werden sollen.

   Der obere Abschnitt ist der Standardabschnitt für die Seite.

   Die Abschnitte, die Sie für einzelne Objekte erstellt haben, werden angezeigt, wenn Sie auf alle Objekte desselben Typs zugreifen und nur für Sie verfügbar sind.

## Anzeigen von Dashboards im linken Bereich von Objekten

Weitere Informationen zum Hinzufügen eines Dashboards unter einem Objekt finden Sie im Abschnitt [[!UICONTROL Dashboard hinzufügen] im linken Bereich eines Workfront-Objekts oder -Bereichs](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) in diesem Artikel.

Wenn Sie ein Dashboard zu einem benutzerdefinierten Abschnitt unter einem Objekt hinzufügen, dient das Objekt als Filter für das Dashboard. Wenn Sie beispielsweise einen Aufgabenbericht zu einem Dashboard hinzufügen und das Dashboard zu einem Projekt hinzufügen, zeigt der benutzerdefinierte Abschnitt, der das Dashboard im Projekt enthält, nur Aufgaben für das Projekt an, das Sie anzeigen.

Die folgenden Objekte werden nach dem Objekt gefiltert, unter dem sie angezeigt werden, wenn dieses Objekt in der Hierarchie höher ist als sie:

* Projekt
* Aufgabe
* Problem
* Genehmigungsprozess
* Notiz
* Dokument

Weitere Informationen zur Hierarchie und Interdependenz von Objekten finden Sie im Abschnitt [Interdependenz und Hierarchie von Objekten](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) im Artikel [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Anpassen des linken Bereichs in einer Layoutvorlage

Wenn Sie Ihrer [!DNL Workfront] -Instanz Dashboards hinzufügen, sind diese nur für Sie sichtbar.

Sie können die Abschnitte in [!DNL Workfront] anpassen und das neue Layout für mehrere Benutzer in einer Layoutvorlage freigeben. Nur ein System- oder Gruppenadministrator kann sie für andere Benutzer in einer Layoutvorlage freigeben. Weitere Informationen zum Anpassen des linken Bedienfelds mit einer Layoutvorlage finden Sie unter [Anpassen des linken Bedienfelds mit einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
