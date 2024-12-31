---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Massenbearbeitung der „Andere Gruppen“ des Benutzers
description: Bei der Massenbearbeitung habe ich versucht, einer Vielzahl von Benutzern eine einzelne „Andere Gruppen“ hinzuzufügen. Nach dem Speichern der Änderungen wurden alle vorhandenen „Andere Gruppe“ entfernt, und nur die neue „Andere Gruppe“ blieb erhalten.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Massenbearbeitung der „Andere Gruppen“ des Benutzers

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

## Problem:

Bei der Massenbearbeitung habe ich versucht, einer Vielzahl von Benutzern eine einzelne „Andere Gruppen“ hinzuzufügen.
Nach dem Speichern der Änderungen wurden alle vorhandenen „Andere Gruppe“ entfernt, und nur die neue „Andere Gruppe“ blieb erhalten.

## Antwort:

Das resultierende Verhalten hängt von der aktuellen Gruppenmitgliedschaft der ausgewählten Benutzer ab:

* Wenn alle ausgewählten Benutzer und die Mitgliedschaften in anderen Gruppen genau übereinstimmen…
Nachdem Sie die Benutzer ausgewählt und auf [!UICONTROL Bearbeiten] geklickt haben, wird [!UICONTROL  Feld „Andere ]&quot; die vollständige Liste anzeigen
aller Gruppen, denen diese Benutzer angehören.

* Wenn die ausgewählten Benutzer unterschiedliche Andere Gruppenmitgliedschaften haben…
Nachdem Sie die Benutzer ausgewählt und auf [!UICONTROL Bearbeiten] geklickt haben, ] das Feld „Andere Gruppen[!UICONTROL  leer.

Wenn Sie auf **[!UICONTROL Änderungen speichern]** klicken, werden alle Elemente gespeichert, die im Feld Andere Gruppen angezeigt werden.

Der vorherige Inhalt des Felds wird überschrieben.
