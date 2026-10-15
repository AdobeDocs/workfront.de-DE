---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Konvertieren veralteter Objekte in Adobe Cloud-Speicher
description: Lernen Sie die drei Fälle kennen, in denen Sie ein veraltetes Workfront-Speicherobjekt in Adobe-Cloud-Speicher konvertieren können, und verstehen Sie, was während jeder Konvertierung bewegt wird und was bleibt.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---
# Konvertieren veralteter Objekte in Adobe Cloud-Speicher

In den meisten Szenarien können Sie Workfront-Objekte nur zwischen Speichermodellen verschieben, kopieren und konvertieren. Sie können beispielsweise eine Aufgabe von einem Adobe-Cloud-Speicherprojekt in ein anderes Adobe-Cloud-Speicherprojekt verschieben. In drei bestimmten Fällen können Sie ein veraltetes Workfront-Speicherobjekt in Adobe Cloud-Speicher konvertieren:

* Konvertieren einer alten Workfront-Speicheraufgabe in ein Adobe-Cloud-Speicherprojekt
* Konvertieren eines alten Workfront-Speicherportfolios in ein Adobe-Cloud-Speicherportfolio
* Erstellen eines Adobe-Cloud-Speicherprojekts aus einer alten Workfront-Speichervorlage

Eine Orientierung zum Verschieben und zu den Unterschieden im Adobe Cloud-Speicher finden Sie unter [Wechseln zu Workfront im Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/workfront-storage.md).

<!-- 
need to validate with PM
>[!NOTE]
>
>In all three conversion scenarios, documents and document folders don't move from legacy Workfront storage to Adobe cloud storage. Documents that exist on the legacy object before the conversion remain on legacy storage.
-->

## Konvertieren einer Legacy-Aufgabe in ein Adobe Cloud-Speicherprojekt

Um eine ältere Workfront-Speicheraufgabe in ein Adobe-Cloud-Speicherprojekt zu konvertieren, verwenden Sie den vorhandenen Fluss „In Projekt konvertieren“ für die Aufgabe. Während der Konvertierung:

* Teilaufgaben und Probleme werden in das neue Projekt verschoben.
* An die Aufgabe angehängte Dokumente und ihre Genehmigungs-Workflows bleiben im ursprünglichen Projekt erhalten.
* Arbeitsgenehmigungen und Links für anfragelösende Objekte werden entfernt.
* Die ursprüngliche Aufgabe wird gelöscht.

## Konvertieren eines alten Portfolios in ein Adobe Cloud-Speicherportfolio

Ein Workfront-Administrator kann im Bereich „Setup“ ein veraltetes Workfront-Speicherportfolio in ein Adobe-Cloud-Speicherportfolio konvertieren. Nach der Konversion:

* Ältere Workfront-Speicherprojekte können nicht mehr in das Portfolio verschoben werden.
* Alle neuen Projekte, die im Portfolio erstellt werden, verwenden den Adobe Cloud-Speicher.
* Frame.io ist der Viewer für Dokumente in den Adobe Cloud-Speicherprojekten des Portfolios.
* Untergeordnete Projekte, die älteren Workfront-Speicher verwenden, bleiben auf dem alten Speicher.
* Untergeordnete Programme verbleiben im alten Speicher.

>[!NOTE]
>
>Ein untergeordnetes Legacy-Programm kann nur dann automatisch in den Adobe-Cloud-Speicher konvertiert werden, wenn ihm manuell ein Adobe-Cloud-Speicherprojekt hinzugefügt wird.

Weitere Informationen finden Sie unter [Ältere Portfolios in Adobe Cloud-Speicher &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md).

## Erstellen eines Adobe-Cloud-Speicherprojekts aus einer Legacy-Vorlage

Wenn Sie ein Projekt aus einer Legacy-Workfront-Speichervorlage erstellen, bestimmt **Kontrollkästchen „Dieses Projekt im Adobe-Cloud-** erstellen“ im Dialogfeld „Projekterstellung“ den Speichertyp des neuen Projekts. Das Verhalten der Kontrollkästchen hängt davon ab, wo Sie das Projekt erstellen:

* **Außerhalb eines Portfolios**: Das Kontrollkästchen ist standardmäßig verfügbar und deaktiviert. Wählen Sie es aus, um das neue Projekt im Adobe Cloud-Speicher zu erstellen.
* **Innerhalb eines Adobe Cloud-**: Das Kontrollkästchen ist aktiviert und gesperrt. Das neue Projekt muss mit dem Speichertyp des Portfolios übereinstimmen.
* **In einem alten Workfront-**: Das Kontrollkästchen ist nicht verfügbar. Das neue Projekt verwendet alten Workfront-Speicher.

Weitere Informationen finden Sie unter [Erstellen von Projekten](/help/quicksilver/manage-work/projects/create-projects/create-project.md).
