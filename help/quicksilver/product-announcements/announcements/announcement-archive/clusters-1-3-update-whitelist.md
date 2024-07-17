---
content-type: reference
navigation-topic: announcements
title: Kunden mit Clustern 1, 2 und 3 müssen alle IP-Blöcke der Zulassungsliste aktualisieren, um das Blockieren von Adobe Workfront-Diensten zu verhindern
description: Zur Verbesserung und Verbesserung unserer Kerninfrastruktur werden wir Adobe Workfront-Kunden in den Clustern 01, 02 und 03 bald in die öffentliche Cloud von AWS migrieren.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Kunden mit Clustern 1, 2 und 3 müssen alle IP-Blöcke der Zulassungsliste aktualisieren, um das Blockieren von Adobe Workfront-Diensten zu verhindern

Zur Verbesserung und Verbesserung unserer Kerninfrastruktur werden wir Adobe Workfront-Kunden in den Clustern 01, 02 und 03 bald in die öffentliche Cloud von AWS migrieren.

Im Rahmen dieser Änderung müssen Sie die folgenden IPs zu Ihren Zulassungsliste-IP-Blöcken hinzufügen, um das Blockieren von Workfront-Diensten zu verhindern:

Für SSO und POP:

* 34 215 145 168
* 54 69 155 48
* 35 160 44 226
* 34 213 96 218
* 3 16 210 22
* 3 16 229 153
* 18 224 117 99
* 3 18 123 153
* 3 211 159 196
* 3 85 255 45
* 3 210 78 197
* 3 211 23 183

E-Mail:

* 54 240 60 174
* 54 240 60 175

Stellen Sie sicher, dass die IP-Blöcke Ihrer Zulassungsliste bis zum 13. Mai 2019 aktualisiert sind. Weitere Informationen finden Sie unter [Konfigurieren der Zulassungsliste Ihrer Firewall-](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Vielen Dank für Ihre kontinuierliche Unterstützung von Workfront, da wir daran arbeiten, unseren Kunden ein zuverlässigeres und robusteres Erlebnis zu bieten.

Wenn Sie weitere Fragen haben, wenden Sie sich bitte an unser Support-Team unter experience.workfront.com oder unter der Telefonnummer +44.306.4357 (US) oder +44.1256.274200 (EMEA).

## FAQs

### Warum nimmt Workfront diese Änderung vor?

Um unseren Kunden den bestmöglichen Service zu bieten, sucht Workfront ständig nach Möglichkeiten, das Benutzererlebnis zu verbessern. Diese Änderung nutzt neue Technologien, die es uns ermöglichen, das bestmögliche Erlebnis zu bieten und unser bereits robustes Sicherheitsmodell zu verbessern.

### Welche Maßnahmen benötige ich als Workfront-Administrator?

Wenden Sie sich an Ihre interne IT- oder Sicherheitsabteilung, um Hilfe beim Überprüfen der IP-Blöcke Ihrer Zulassungsliste und beim Hinzufügen der oben aufgeführten IPs zu erhalten.

### Was kann meine Organisation erwarten, wenn wir diese Änderung nicht vornehmen?

Sie können nicht auf Workfront-Dienste zugreifen, wenn wir Dienste zu den neuen IPs migrieren.
