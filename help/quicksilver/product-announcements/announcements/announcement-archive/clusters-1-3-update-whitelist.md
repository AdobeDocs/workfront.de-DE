---
content-type: reference
navigation-topic: announcements
title: Kunden mit den Clustern 1, 2 und 3 müssen alle Zulassungsliste-IP-Blöcke aktualisieren, um die Blockierung von Adobe Workfront-Services zu verhindern
description: Zur Verbesserung unserer Kerninfrastruktur werden wir in Kürze Adobe Workfront-Kunden der Cluster 01, 02 und 03 in die öffentliche Cloud von AWS migrieren.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Kunden mit den Clustern 1, 2 und 3 müssen alle Zulassungsliste-IP-Blöcke aktualisieren, um die Blockierung von Adobe Workfront-Services zu verhindern

Zur Verbesserung unserer Kerninfrastruktur werden wir in Kürze Adobe Workfront-Kunden der Cluster 01, 02 und 03 in die öffentliche Cloud von AWS migrieren.

Im Rahmen dieser Änderung müssen Sie die folgenden IP-Adressen zu Ihren Zulassungsliste-IP-Blöcken hinzufügen, um die Blockierung von Workfront-Services zu verhindern:

Für SSO und POP:

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

Für E-Mail:

* 54.240.60.174
* 54.240.60.175

Auf die Zulassungsliste setzen Stellen Sie sicher, dass Ihre IP-Blöcke bis zum 13. Mai 2019 aktualisiert werden. Weitere Informationen finden Sie [Zulassungsliste zum Konfigurieren der Firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Vielen Dank für Ihre kontinuierliche Unterstützung von Workfront, da wir daran arbeiten, unseren Kunden ein zuverlässigeres und stabileres Erlebnis zu bieten.

Wenn Sie weitere Fragen haben, wenden Sie sich bitte an unser Support-Team unter experience.workfront.com oder telefonisch unter 844.306.4357 (USA) oder +44.1256.274200 (EMEA).

## FAQs

### Warum nimmt Workfront diese Änderung vor?

In dem Bestreben, unseren Kunden den bestmöglichen Service zu bieten, sucht Workfront ständig nach Möglichkeiten, das Anwendererlebnis zu verbessern. Diese Änderung macht Gebrauch von neuen Technologien, die es uns ermöglichen, das bestmögliche Erlebnis zu bieten und unser bereits robustes Sicherheitsmodell zu verbessern.

### Welche Maßnahmen sind für mich als Workfront-Administrator erforderlich?

Auf die Zulassungsliste setzen Wenden Sie sich an Ihre IT- oder Sicherheitsabteilung, um Unterstützung bei der Überprüfung Ihrer IP-Blöcke und beim Hinzufügen der oben aufgeführten IPs zu erhalten.

### Was kann mein Unternehmen erwarten, wenn wir diese Änderung nicht vornehmen?

Sie können nicht auf Workfront-Services zugreifen, da wir Services zu den neuen IP-Adressen migrieren.
