---
product-area: projects
navigation-topic: use-the-home-area
title: Elemente in der [!UICONTROL Arbeitsliste] im Bereich „Startseite“ anzeigen
description: Jedes Widget enthält eine eigene Arbeitsliste. Arbeitslisten zeigen alle Arbeitselemente an, die Ihnen zugewiesen sind. Mithilfe von Filtern und Gruppierungen können Sie steuern[!UICONTROL  welche Elemente in Ihrer ]Arbeitsliste“ angezeigt werden.
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
TQID: https://experienceleague.adobe.com/fITdY6-HlQ-4527-RiI9m52-Kg3nRUxsk32vjpw-A-g
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 990
ht-degree: 7%

---

# Elemente in der [!UICONTROL Arbeitsliste] im Bereich [!UICONTROL Startseite] anzeigen

<!-- Audited: 1/2024 -->

Jedes Widget enthält eine eigene Arbeitsliste. Arbeitslisten zeigen alle Arbeitselemente an, die Ihnen zugewiesen sind. Mithilfe von Filtern und Gruppierungen können Sie steuern[!UICONTROL  welche Elemente in Ihrer ]Arbeitsliste“ angezeigt werden.

>[!IMPORTANT]
>
>* Um Aufgaben und Probleme in den Startseiten-Widgets anzuzeigen, muss das übergeordnete Projekt den Status Aktuell aufweisen oder einen Status aufweisen, der dem aktuellen entspricht.
>* Projekte müssen außerdem den Status „Aktuell“ oder einen Status aufweisen, der der Anzeige auf der Startseite entspricht.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz</strong></td> 
   <td><ul><li>[!UICONTROL Contributor] nur für Genehmigungen</li> <li>[!UICONTROL Standard] oder höher für alle anderen Objekte</li> <p>ODER</p> 
  </ul><ul><li>[!UICONTROL Überprüfung] nur für Genehmigungen</li> <li>[!UICONTROL Work] oder höher für alle anderen Objekte</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene</strong></td> 
   <td> <p>Zugriff auf Projekte, Aufgaben, Probleme und Dokumente in [!UICONTROL View] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Tragen Sie Berechtigungen oder höher zu den Aufgaben und Problemen bei, an denen Sie arbeiten müssen</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen für Arbeitselemente, die in der Arbeitsliste angezeigt werden

Es gibt integrierte Anforderungen, für die Arbeitselemente in bestimmten Widget-Arbeitslisten angezeigt werden. Arbeitselemente müssen diese Anforderungen erfüllen, damit sie in den Arbeitslisten der folgenden Widgets angezeigt werden.

### Widget „Meine Aufgaben“

Aufgaben müssen die folgenden Anforderungen erfüllen, damit sie im Widget Meine Aufgaben angezeigt werden:

* Der Aufgabenstatus entspricht nicht „Abgeschlossen“.
* Der angemeldete Benutzer muss der Aufgabe zugewiesen sein.
* Aufgabenstatus ist nicht gleich „Fertig“.
* Das Projekt, zu dem die Aufgabe gehört, muss einen Status haben, der dem aktuellen entspricht.


### Widget „Meine Probleme“

Probleme müssen die folgenden Anforderungen erfüllen, damit sie im Widget „Meine Probleme“ angezeigt werden:

* Der angemeldete Benutzer muss dem Problem zugewiesen sein.
* Der Problemstatus entspricht nicht „Abgeschlossen“.
* Dem Problem ist kein ungelöstes Objekt beigefügt.
* Der Problemstatus ist nicht gleich „Fertig“.
* Das Projekt, zu dem das Problem gehört, muss einen Status haben, der dem aktuellen entspricht.

### Widget Meine Teams

Teamanfragen müssen die folgenden Anforderungen erfüllen, damit sie im Widget „Meine Teams“ angezeigt werden:

* Der angemeldete Benutzer gehört zum Team, dem das Arbeitselement zugewiesen ist.
* Der Status des Arbeitselements entspricht nicht „Abgeschlossen“.
* Dem Arbeitselement ist kein ungelöster Genehmigungsprozess beigefügt.
* Das Arbeitselement ist keine wiederkehrende Aufgabe.
* Das Projekt, zu dem das Arbeitselement gehört, muss einen Status aufweisen, der mit „Aktuell“ übereinstimmt.

## Filtern von Arbeit

Sie können Elemente in der (Arbeitsliste[!UICONTROL  eines Widgets filtern] um nur bestimmte Elementtypen anzuzeigen. Sie können beispielsweise „Meine Arbeit“ ([!UICONTROL ) filtern, ] nur Probleme oder Anfragen anzuzeigen.

>[!NOTE]
>
>Die Filteroptionen werden im Browser gespeichert. Wenn Sie denselben Browser auf demselben Computer verwenden (und die Site-Daten nicht löschen), ändern sich die ausgewählten Filter nicht. Wenn Sie Browser oder Computer wechseln, werden die Filter auf die Standardoption zurückgesetzt, bei der alle Filter deaktiviert sind.

So filtern Sie Ihre Arbeit:

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) Klicken Sie auf **Anpassen**, um eines der folgenden Widgets hinzuzufügen:

   | Widget | Beschreibung |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Pinnwände | Zeigt alle Boards an, die Sie erstellt haben oder zur Verwendung eingeladen wurden |
   | Meine Arbeit | Zeigt Ihnen zugewiesene Aufgaben und Probleme an |
   | Meine Projekte | Zeigt Projekte an, deren Inhaber Sie sind oder an denen Sie mitarbeiten |
   | Meine Aufgaben | Zeigt die Ihnen zugewiesenen Aufgaben an |
   | Meine Probleme | Zeigt Ihnen zugewiesene Probleme an |
   | Meine Anfragen | Zeigt alle von Ihnen gesendeten Anfragen an |
   | Meine Genehmigungen | Zeigt alle ausstehenden, zugewiesenen, delegierten und gesendeten Genehmigungen an |

1. Klicken Sie auf **Filter**-Symbol ![Filtersymbol](assets/filter-nwepng.png) in der rechten oberen Ecke der Widget-Arbeitsliste.
1. Wählen Sie **Filter**Vorgeschlagen“ oder einen von Ihnen erstellten Filter aus.
Detaillierte Informationen zu vorgeschlagenen Filtern finden Sie unter [Übersicht über Widget-Filter für Startseite](/help/quicksilver/workfront-basics/using-home/using-the-home-area/widget-filter-overview-home.md).
1. (Optional) Schalten Sie **Filter stapeln** ein, um mehrere Filteroptionen auszuwählen.

   ![Filter „Meine Aufgabe“ geöffnet](assets/my-task-filter-open.png)


## Arbeiten gruppieren

Sie können das Widget &quot;[!UICONTROL &quot; gruppieren] um Ihre Arbeitselemente zu organisieren.

So gruppieren Sie Ihre Arbeitsliste:

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) Klicken Sie auf **Anpassen**, um eines der folgenden Widgets hinzuzufügen:

   | Widget | Beschreibung |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Pinnwände | Zeigt alle Boards an, die Sie erstellt haben oder zur Verwendung eingeladen wurden |
   | Meine Arbeit | Zeigt Ihnen zugewiesene Aufgaben und Probleme an |
   | Meine Projekte | Zeigt Projekte an, deren Inhaber Sie sind oder an denen Sie mitarbeiten |
   | Meine Aufgaben | Zeigt die Ihnen zugewiesenen Aufgaben an |
   | Meine Probleme | Zeigt Ihnen zugewiesene Probleme an |
   | Meine Anfragen | Zeigt alle von Ihnen gesendeten Anfragen an |
   | Meine Genehmigungen | Zeigt alle ausstehenden, zugewiesenen, delegierten und gesendeten Genehmigungen an |

1. Klicken Sie auf **Gruppen**-Symbol ![Gruppensymbol](assets/group-icon.png) in der rechten oberen Ecke der Widget-Arbeitsliste.
1. Wählen Sie eine **vorgeschlagene** Gruppierung oder eine von Ihnen erstellte Gruppierung aus.
   ![Gruppierung erweitert](assets/grouping-expanded.png)


## Anpassen von Arbeitslistenspalten

Sie können auswählen, welche Spalten in der Widget-Arbeitsliste angezeigt werden sollen:

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) Klicken Sie auf **Anpassen**, um eines der folgenden Widgets hinzuzufügen:

   | Widget | Beschreibung |
   |--------------|---------------------------------------------------------------------------------------------------|
   | Pinnwände | Zeigt alle Boards an, die Sie erstellt haben oder zur Verwendung eingeladen wurden |
   | Meine Arbeit | Zeigt Ihnen zugewiesene Aufgaben und Probleme an |
   | Meine Projekte | Zeigt Projekte an, deren Inhaber Sie sind oder an denen Sie mitarbeiten |
   | Meine Aufgaben | Zeigt die Ihnen zugewiesenen Aufgaben an |
   | Meine Probleme | Zeigt Ihnen zugewiesene Probleme an |
   | Meine Anfragen | Zeigt alle von Ihnen gesendeten Anfragen an |
   | Meine Genehmigungen | Zeigt alle ausstehenden, zugewiesenen, delegierten und gesendeten Genehmigungen an |

1. Klicken Sie auf **Spalten**-Symbol ![Spaltensymbol](assets/column-icon.png) in der rechten oberen Ecke der Widget-Arbeitsliste.
1. Schalten Sie die Spalten je nach Ihren Voreinstellungen ein oder aus.
1. (Optional) Klicken Sie auf das Symbol **Ziehen** ![Ziehen-Symbol](assets/drag-icon.png), um die Spalten neu anzuordnen.
   ![Spalten erweitert](assets/columns-expanded.png)


## Verspätete Elemente anzeigen

[!DNL Adobe Workfront] ermittelt anhand der folgenden Daten, ob Arbeitsaufträge in Verzug sind:

* **Aufgaben**: [!UICONTROL Geplantes Abschlussdatum]
* **Probleme**: [!UICONTROL Geplantes Abschlussdatum]
* **Dokumente**: [!UICONTROL Einreichungsdatum]
* **Arbeitszeittabellen**: [!UICONTROL Gesendet am]
* **Genehmigungen**: [!UICONTROL Einreichungsdatum]
* **Genehmigungen von Korrekturabzügen**: [!UICONTROL Frist für Korrekturabzüge]


