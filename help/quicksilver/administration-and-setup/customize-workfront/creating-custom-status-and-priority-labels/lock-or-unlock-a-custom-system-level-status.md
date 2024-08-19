---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Gesperrte und entsperrte Systemstatus
description: Das Sperren benutzerdefinierter Status ist eine Möglichkeit, sicherzustellen, dass Personen in Ihrem gesamten Unternehmen dieselben Prozesse in ihrem Arbeitsablauf verwenden. Wenn ein Status gesperrt ist, steht er allen Benutzern im System zur Verfügung. Obwohl Sie sie bearbeiten oder löschen können, können Gruppenadministratoren dies nicht für ihre Gruppen tun. Umgekehrt ermöglicht das Entsperren benutzerdefinierter Status Gruppenadministratoren mehr Flexibilität bei der Verwaltung der eindeutigen Workflows, die in ihren Gruppen verwendet werden. Sie können die Attribute eines entsperrten Status ändern oder sie für ihre Gruppen löschen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Status auf Systemebene gesperrt und entsperrt

Das Sperren benutzerdefinierter Status ist eine Möglichkeit, sicherzustellen, dass Personen in Ihrem gesamten Unternehmen dieselben Prozesse in ihrem Arbeitsablauf verwenden. Wenn ein Status gesperrt ist, steht er allen Benutzern im System zur Verfügung. Sie können zwar einen Status bearbeiten oder löschen, den Sie sperren, doch Gruppenadministratoren können dies nicht für ihre Gruppen tun. Sie können jedoch nur die Anzeigereihenfolge in der Liste &quot;Status&quot;ändern.

Umgekehrt ermöglicht das Entsperren benutzerdefinierter Status Gruppenadministratoren mehr Flexibilität bei der Verwaltung der eindeutigen Workflows, die in ihren Gruppen verwendet werden. Wenn ein Status entsperrt ist, können Gruppenadministratoren seine Attribute ändern oder für ihre Gruppen löschen.

>[!IMPORTANT]
>
>Wenn Sie einen benutzerdefinierten Status sperren, nachdem er für einen beliebigen Zeitraum entsperrt wurde, ersetzen Ihre systemweiten Einstellungen für den Status die von Gruppenadministratoren vorgenommenen Einstellungen. Während der Status gesperrt ist, können Gruppenadministratoren den Status für ihre Gruppen nicht ändern oder löschen.

Anweisungen zum Sperren oder Entsperren eines Status auf Systemebene finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Entsperrte Status in Genehmigungsprozessen

Sie können sowohl gesperrte als auch entsperrte Status in einem Systemgenehmigungsprozess verwenden. Wenn Sie einen Systemgenehmigungsprozess mit einem entsperrten Systemstatus erstellen, können Benutzer im gesamten System den Genehmigungsprozess an jedes Projekt, jede Aufgabe oder jedes Problem im System anhängen.

Warnmeldungen werden in den folgenden Szenarien angezeigt, damit Sie und Ihre Benutzer die Ergebnisse der folgenden Szenarien verstehen können:

* Ein Administrator entsperrt den Status auf Systemebene, der in einem Genehmigungsprozess verwendet wird. In einer Meldung wird gewarnt, dass der entsperrte Status für ihre Gruppen möglicherweise gelöscht wird, was verhindert, dass Gruppenmitglieder diesen Genehmigungsprozess ordnungsgemäß für Objekte verwenden, die ihrer Gruppe zugewiesen sind.

* Ein Benutzer beginnt mit der Bearbeitung eines Genehmigungsprozesses, der einen entsperrten Status verwendet. Eine Meldung informiert den Benutzer über den entsperrten Status, damit er beurteilen kann, ob es sinnvoll wäre, ihn erneut zu sperren oder zu ersetzen.

* Ein Genehmigungsprozess auf Systemebene mit einem entsperrten Status wird an ein Objekt angehängt und der Status wurde für die dem Objekt zugewiesene Gruppe gelöscht. Wenn ein Gruppenmitglied zum Bereich Validierungen für das Objekt wechselt, wird in einer Meldung erläutert, dass der Validierungsprozess für das Objekt nicht initiiert werden kann.

Sie können sowohl gesperrte als auch entsperrte Status in einem Gruppengenehmigungsprozess verwenden. Wenn Sie einen Gruppengenehmigungsprozess mit einem entsperrten Gruppenstatus erstellen, können Benutzer den Genehmigungsprozess an jedes Projekt, jede Aufgabe oder jedes Problem anhängen, das mit der Gruppe verknüpft ist.