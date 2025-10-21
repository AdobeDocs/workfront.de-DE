---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Gesperrte und entsperrte Status auf Systemebene
description: Durch das Sperren benutzerdefinierter Status können Sie sicherstellen, dass die Personen in Ihrem Unternehmen in ihrem Arbeitsablauf dieselben Prozesse verwenden. Wenn ein Status gesperrt ist, steht er allen Benutzenden im System zur Verfügung. Sie können sie zwar bearbeiten oder löschen, Gruppenadministratoren können dies jedoch nicht für ihre Gruppen tun. Umgekehrt ermöglicht das Entsperren benutzerdefinierter Status Gruppenadministratoren mehr Flexibilität bei der Verwaltung der in ihren Gruppen verwendeten eindeutigen Workflows. Sie können die Attribute eines entsperrten Status ändern oder ihn für ihre Gruppen löschen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0e58a1d6-5e0c-4445-a5ac-400dfd4c4948
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Gesperrte und entsperrte Status auf Systemebene

Durch das Sperren benutzerdefinierter Status können Sie sicherstellen, dass die Personen in Ihrem Unternehmen in ihrem Arbeitsablauf dieselben Prozesse verwenden. Wenn ein Status gesperrt ist, steht er allen Benutzenden im System zur Verfügung. Sie können zwar einen Status bearbeiten oder löschen, den Sie gesperrt haben, Gruppenadministratoren können dies jedoch nicht für ihre Gruppen tun, sondern nur die Anzeigereihenfolge in der Statusliste ändern.

Umgekehrt ermöglicht das Entsperren benutzerdefinierter Status Gruppenadministratoren mehr Flexibilität bei der Verwaltung der in ihren Gruppen verwendeten eindeutigen Workflows. Wenn ein Status entsperrt wird, können Gruppenadministratoren seine Attribute ändern oder ihn für ihre Gruppen löschen.

>[!IMPORTANT]
>
>Wenn Sie einen benutzerdefinierten Status sperren, nachdem er über einen bestimmten Zeitraum entsperrt wurde, ersetzen Ihre systemweiten Einstellungen für den Status die von Gruppenadministratoren vorgenommenen Einstellungen. Solange der Status gesperrt ist, können Gruppenadministratoren den Status für ihre Gruppen nicht ändern oder löschen.

Anweisungen zum Sperren oder Entsperren eines Status auf Systemebene finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Entsperrte Status in Genehmigungsprozessen

Sie können in einem Systemgenehmigungsprozess sowohl den Status „Gesperrt“ als auch den Status „Entsperrt“ verwenden. Wenn Sie einen Systemgenehmigungsprozess mit einem entsperrten Systemstatus erstellen, können Benutzer im gesamten System den Genehmigungsprozess an jedes Projekt, jede Aufgabe oder jedes Problem im System anhängen.

Warnmeldungen werden in den folgenden Szenarien angezeigt, um Ihnen und Ihren Benutzern zu helfen, die Ergebnisse der folgenden Szenarien zu verstehen:

* Ein Administrator entsperrt einen Status auf Systemebene, der in einem Genehmigungsprozess verwendet wird. Eine Meldung warnt davor, dass der entsperrte Status für die Gruppen gelöscht werden könnte, was verhindern würde, dass Gruppenmitglieder diesen Genehmigungsprozess ordnungsgemäß für Objekte verwenden, die ihrer Gruppe zugewiesen sind.
* Ein Benutzer beginnt mit der Bearbeitung eines Genehmigungsprozesses, der einen entsperrten Status verwendet. Eine Meldung informiert den Benutzer über den entsperrten Status, damit er beurteilen kann, ob es sinnvoll wäre, ihn erneut zu sperren oder zu ersetzen.
* Ein Genehmigungsprozess auf Systemebene mit einem entsperrten Status wird an ein Objekt angehängt und der Status wurde für die dem Objekt zugewiesene Gruppe gelöscht. Wenn ein Gruppenmitglied zum Abschnitt Genehmigungen für das Objekt wechselt, wird in einer Meldung erklärt, dass der Genehmigungsprozess für das Objekt nicht gestartet werden kann.

Sie können in einem Gruppengenehmigungsprozess sowohl den Status „Gesperrt“ als auch den Status „Entsperrt“ verwenden. Wenn Sie einen Gruppengenehmigungsprozess mit einem nicht gesperrten Gruppenstatus erstellen, können Benutzer den Genehmigungsprozess an jedes Projekt, jede Aufgabe oder jedes Problem anhängen, das mit der Gruppe verknüpft ist.
