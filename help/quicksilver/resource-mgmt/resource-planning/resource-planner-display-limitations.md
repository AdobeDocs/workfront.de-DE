---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Anzeigebeschränkungen für den Ressourcenplaner
description: Um die Leistung zu verbessern, beschränkt Adobe Workfront die Menge der angezeigten Informationen sowie die Menge der Informationen, die Sie aus dem Ressourcenplaner exportieren können.
author: Alina
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Anzeigebeschränkungen für den Ressourcenplaner

Um die Leistung zu verbessern, beschränkt Adobe Workfront die Menge der angezeigten Informationen sowie die Menge der Informationen, die Sie aus dem Ressourcenplaner exportieren können.

Wenn Sie diese Grenze erreichen, zeigt Workfront eine Warnmeldung an, in der Sie darüber informiert werden, dass Sie diese Grenze erreicht haben.

Wenn die Informationen, die Sie im Ressourcenplaner erwarten, nicht angezeigt werden, ist es möglich, dass Sie versuchen, zu viele Informationen anzuzeigen, und einige Daten wurden aufgrund dieser Einschränkung nicht angezeigt.

Für eine optimale Leistung beim Anzeigen und Exportieren des Ressourcen-Planers wird Folgendes empfohlen:

* Verwenden Sie Filter, um die Anzahl der im Ressourcenplaner angezeigten Informationen zu reduzieren und nur für Sie relevante Informationen anzuzeigen.
* Verwenden Sie alle Exportoptionen, um die Anzahl der gleichzeitig exportierten Informationen zu reduzieren und sicherzustellen, dass Sie nur relevante Informationen exportieren.\
   Weitere Informationen zur Verwendung von Filtern und zum Exportieren von Optionen im Ressourcenplaner finden Sie unter [Filtern von Informationen im Ressourcenplaner](../../resource-mgmt/resource-planning/filter-resource-planner.md).

   Informationen zum Exportieren von Informationen aus dem Ressourcen-Planer finden Sie unter [Exportieren von Informationen aus dem Ressourcenplaner](../../resource-mgmt/resource-planning/export-resource-planner.md).

Die Menge an Informationen, die Sie anzeigen oder exportieren können, hängt davon ab, welche Ansicht Sie anwenden und welche Umgebung Sie für den Zugriff auf den Ressourcenplaner verwenden.

## Einschränkungen in der Projektansicht

Beachten Sie beim Anwenden der Projektansicht auf den Ressourcenplaner Folgendes:

* Sie können nur Projekte sehen, auf die Sie Zugriff haben.
* Sie können jedes Projekt erweitern, um die damit verbundenen Rollen und die einzelnen Rollen anzuzeigen und die mit ihm verbundenen Benutzer anzuzeigen.

   Sie können bis zu 300 Projekte anzeigen, wenn Sie zum Ende der Liste blättern, es sei denn, es gibt mehr als 30.000 Zeilen mit Projekten, Rollen und Benutzern. Dann erhalten Sie eine Warnmeldung, dass Sie das 30.000 Zeilenlimit erreicht haben.

* Je nach Bildschirmgröße können Sie drei oder vier Zeiträume gleichzeitig anzeigen.

Beachten Sie Folgendes, wenn Sie Informationen aus der Projektansicht des Ressourcen-Planers exportieren, nachdem Sie alle entsprechenden Filter und Exportoptionen angewendet haben:

* Wenn Sie im Ressourcenplaner auswählen, dass alle Objekte (Projekte, Rollen und Benutzer) exportiert werden sollen, werden alle Objekte, die Ihren Kriterien entsprechen, in der exportierten Datei angezeigt, unabhängig davon, ob Sie einen Bildlauf zum Ende der Liste durchgeführt haben, um sie anzuzeigen.
* Zeilen ohne Zuordnungsinformationen sind in der exportierten Datei enthalten.

* Sie können bis zu 30.000 Zeilen exportieren.

## Einschränkungen in der Rollenansicht

Beachten Sie Folgendes beim Anwenden der Rollenansicht auf den Ressourcenplaner, nachdem Sie alle entsprechenden Filter angewendet haben:

* Sie sehen nur Rollen, die mit von Ihnen verwalteten Projekten verknüpft sind.

* Sie können bis zu 300 Rollen sehen, wenn Sie zum unteren Rand der Liste blättern, es sei denn, es gibt mehr als 30.000 Zeilen mit Rollen, Projekten und Benutzern. Dann erhalten Sie eine Warnmeldung, dass Sie die Zeilenbegrenzung von 30.000 Zeilen für die Anzeige auf dem Bildschirm erreicht haben.
* Sie können jede Rolle erweitern, um eine Liste von Projekten anzuzeigen, und jedes Projekt, um eine Liste von Benutzern anzuzeigen, die diese Rollen in den Projekten erfüllen können.

   Standardmäßig werden 20 Projekte angezeigt. Mit der Option Mehr laden können Sie zusätzliche Projekte anzeigen oder unter jedem Projekt einen Bildlauf durchführen, um weitere Benutzer zu laden.

* Je nach Bildschirmgröße können drei oder vier Zeiträume angezeigt werden.

Beachten Sie Folgendes beim Exportieren von Informationen aus der Rollenansicht des Ressourcen-Planers, nachdem Sie alle entsprechenden Filter und Exportoptionen angewendet haben:

* Wenn Sie im Ressourcenplaner auswählen, dass alles (Rollen, Projekte und Benutzer) exportiert werden soll, werden alle Objekte, die Ihren Kriterien entsprechen, in der exportierten Datei angezeigt, unabhängig davon, ob Sie einen Bildlauf zum unteren Rand der Liste durchgeführt haben, um sie anzuzeigen.
* Zeilen ohne Zuordnungsinformationen sind in der exportierten Datei enthalten.
* Sie können bis zu 30.000 Zeilen exportieren.

## Einschränkungen in der Benutzeransicht

Beachten Sie beim Anwenden der Benutzeransicht auf den Ressourcenplaner Folgendes:

* Sie können alle Benutzer anzeigen, die die folgenden Kriterien erfüllen:

   * Sie haben Zugriff auf die Ansicht
   * sind aktiv
   * Sie haben sich mindestens einmal angemeldet.

* Sie können jeden Benutzer erweitern, um die ihm zugeordneten Projekte anzuzeigen, und jedes Projekt, um die damit verbundenen Rollen anzuzeigen.\
   Die ersten 50 Projekte und Rollen werden standardmäßig angezeigt. Mit der Option Mehr laden können Sie weitere Projekte oder Rollen anzeigen.

   >[!NOTE]
   >
   >Wenn Sie die Liste der Benutzer nach Projekten gefiltert haben, können nur die mit den gefilterten Projekten verknüpften Benutzer erweitert und auch die Stundeninformationen angezeigt werden

* Sie können bis zu 2.000 Benutzer in der Web-Oberfläche sehen. Workfront zeigt eine Warnmeldung an, wenn Sie diese Grenze erreichen.
* Je nach Bildschirmgröße können drei oder vier Zeiträume angezeigt werden.

Beachten Sie Folgendes beim Exportieren von Informationen aus der Benutzeransicht des Ressourcen-Planers, nachdem Sie alle entsprechenden Filter und Exportoptionen angewendet haben:

* Wenn Sie im Ressourcenplaner auswählen, dass alle Rollen (Benutzer, Rollen und Projekte) in die exportierte Datei exportiert werden sollen, unabhängig davon, ob sie in der Web-Oberfläche erweitert wurden oder nicht.

* Sie können bis zu 30.000 Zeilen exportieren, die Benutzer sowie die darunter aufgelisteten Projekte und Rollen enthalten, unabhängig davon, ob Sie einen Bildlauf zum Ende der Liste durchgeführt haben, um sie anzuzeigen oder nicht. Alle Benutzer, Projekte und Rollen sind in der exportierten Datei enthalten, unabhängig davon, ob sie in der Web-Oberfläche erweitert wurden oder nicht.
* Zeilen ohne Zuordnungsinformationen sind in der exportierten Datei enthalten.
