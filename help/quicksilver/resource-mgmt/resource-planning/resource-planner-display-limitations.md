---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Einschränkungen bei der Ressourcenplaner-Anzeige
description: Um die Leistung zu verbessern, beschränkt Adobe Workfront die Menge an Informationen, die Sie anzeigen können, sowie die Menge an Informationen, die Sie aus dem Ressourcenplaner exportieren können.
author: Lisa
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Anzeigebeschränkungen des Ressourcenplaners

Um die Leistung zu verbessern, beschränkt Adobe Workfront die Menge an Informationen, die Sie anzeigen können, sowie die Menge an Informationen, die Sie aus dem Ressourcenplaner exportieren können.

Wenn Sie sich diesem Limit nähern, zeigt Workfront eine Warnmeldung an, die Sie darüber informiert, dass Sie dieses Limit erreicht haben.

Wenn die Informationen, die Sie im Ressourcenplaner erwarten, nicht angezeigt werden, ist es möglich, dass Sie versuchen, zu viele Informationen anzuzeigen, und einige Daten wurden aufgrund dieser Einschränkung nicht angezeigt.

Für eine optimale Leistung beim Anzeigen und Exportieren des Ressourcenplaners wird Folgendes empfohlen:

* Verwenden Sie Filter, um die Menge an Informationen zu reduzieren, die Sie im Ressourcenplaner anzeigen, und nur Informationen anzuzeigen, die für Sie relevant sind.
* Verwenden Sie alle Ihre Exportoptionen, um die Menge der gleichzeitig exportierten Informationen zu reduzieren und sicherzustellen, dass Sie nur relevante Informationen exportieren.\
  Weitere Informationen zur Verwendung von Filtern und Exportoptionen im Ressourcenplaner finden Sie unter [Filterinformationen im Ressourcenplaner](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  Informationen zum Exportieren von Informationen aus dem Ressourcenplaner finden Sie unter [Exportieren von Informationen aus dem Ressourcenplaner](../../resource-mgmt/resource-planning/export-resource-planner.md).

Die Menge an Informationen, die Sie anzeigen oder exportieren können, hängt davon ab, welche Ansicht Sie anwenden und welche Umgebung Sie für den Zugriff auf den Ressourcenplaner verwenden.

## Einschränkungen in der Projektansicht

Beachten Sie beim Anwenden der Projektansicht auf den Ressourcenplaner Folgendes:

* Es werden nur Projekte angezeigt, auf deren Verwaltung Sie Zugriff haben.
* Sie können jedes Projekt erweitern, um die mit ihm verknüpften Rollen anzuzeigen, und jede Rolle, um die mit ihm verknüpften Benutzer anzuzeigen.

  Sie können bis zu 300 Projekte anzeigen, wenn Sie zum Ende der Liste scrollen, es sei denn, es gibt mehr als 30.000 Zeilen mit Projekten, Rollen und Benutzern. Anschließend erhalten Sie eine Warnmeldung, dass Sie das Limit von 30.000 Zeilen erreicht haben.

* Je nach Bildschirmgröße können Sie drei oder vier Zeiträume gleichzeitig anzeigen.

Beachten Sie beim Exportieren von Informationen aus der Projektansicht des Ressourcenplaners Folgendes, nachdem Sie alle entsprechenden Filter und Exportoptionen angewendet haben:

* Wenn Sie im Ressourcenplaner alles exportieren (Projekte, Rollen und Benutzer), werden alle Objekte, die Ihren Kriterien entsprechen, in der exportierten Datei angezeigt, unabhängig davon, ob Sie zum unteren Rand der Liste gescrollt haben oder nicht.
* Zeilen ohne Zuordnungsinformationen sind in der exportierten Datei enthalten.

* Sie können bis zu 30.000 Zeilen exportieren.

## Einschränkungen in der Rollenansicht

Beachten Sie Folgendes, wenn Sie die Rollenansicht auf den Ressourcenplaner anwenden, nachdem Sie alle entsprechenden Filter angewendet haben:

* Sie können nur Rollen sehen, die mit Projekten verknüpft sind, die Sie verwalten können.

* Beim Scrollen nach unten in der Liste können Sie bis zu 300 Rollen sehen, es sei denn, es gibt mehr als 30.000 Zeilen mit Rollen, Projekten und Benutzern. Dann erhalten Sie eine Warnmeldung, dass Sie die 30.000-Zeilen-Grenze für das erreicht haben, was Sie auf dem Bildschirm anzeigen können.
* Sie können jede Rolle erweitern, um eine Liste von Projekten anzuzeigen, und jedes Projekt, um eine Liste von Benutzern anzuzeigen, die diese Rollen in den Projekten erfüllen können.

  Standardmäßig werden 20 Projekte angezeigt. Mit der Option Mehr laden können Sie zusätzliche Projekte anzeigen. Sie können auch unter jedem Projekt scrollen, um mehr Benutzer zu laden.

* Je nach Bildschirmgröße können Sie drei oder vier Zeiträume anzeigen.

Beachten Sie beim Exportieren von Informationen aus der Rollenansicht des Ressourcenplaners Folgendes, nachdem Sie alle entsprechenden Filter und Exportoptionen angewendet haben:

* Wenn Sie im Ressourcenplaner alles exportieren (Rollen, Projekte und Benutzer), werden alle Objekte, die Ihren Kriterien entsprechen, in der exportierten Datei angezeigt, unabhängig davon, ob Sie einen Bildlauf zum unteren Rand der Liste durchgeführt haben oder nicht.
* Zeilen ohne Zuordnungsinformationen sind in der exportierten Datei enthalten.
* Sie können bis zu 30.000 Zeilen exportieren.

## Einschränkungen in der Benutzeransicht

Beachten Sie beim Anwenden der Benutzeransicht auf den Ressourcenplaner Folgendes:

* Sie können alle Benutzer anzeigen, die die folgenden Kriterien erfüllen:

   * Sie haben Zugriff auf die Anzeige
   * Sind aktiv
   * Sie haben sich mindestens einmal angemeldet.

* Sie können jeden Benutzer erweitern, um die ihm zugeordneten Projekte anzuzeigen, und jedes Projekt, um die ihm zugeordneten Rollen anzuzeigen.\
  Die ersten 50 Projekte und Rollen werden standardmäßig angezeigt, und Sie können die Option Mehr laden verwenden, um zusätzliche Projekte oder Rollen anzuzeigen.

  >[!NOTE]
  >
  >Wenn Sie die Liste der Benutzer nach Projekten gefiltert haben, können nur die mit den gefilterten Projekten verknüpften Benutzer erweitert werden und auch Ihre Informationen anzeigen

* In der Web-Oberfläche werden bis zu 2.000 Benutzer angezeigt. Workfront zeigt beim Erreichen dieses Grenzwerts eine Warnmeldung an.
* Je nach Bildschirmgröße können Sie drei oder vier Zeiträume anzeigen.

Beachten Sie beim Exportieren von Informationen aus der Benutzeransicht des Ressourcenplaners Folgendes, nachdem Sie alle entsprechenden Filter und Exportoptionen angewendet haben:

* Wenn Sie im Ressourcenplaner alles exportieren (Benutzer, Rollen und Projekte), sind alle Rollen, Projekte und Benutzer in der exportierten Datei enthalten, unabhängig davon, ob sie in der Web-Oberfläche erweitert sind oder nicht.

* Sie können bis zu 30.000 Zeilen exportieren, die Benutzer sowie die darunter aufgeführten Projekte und Rollen enthalten, unabhängig davon, ob Sie einen Bildlauf zum Ende der Liste durchgeführt haben oder nicht. Alle Benutzer, Projekte und Rollen sind in der exportierten Datei enthalten, unabhängig davon, ob sie in der Web-Oberfläche erweitert sind oder nicht.
* Zeilen ohne Zuordnungsinformationen sind in der exportierten Datei enthalten.
