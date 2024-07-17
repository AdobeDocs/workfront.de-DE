---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Andere Gruppen des Benutzers für die Massenbearbeitung
description: Bei der Massenbearbeitung habe ich versucht, eine einzelne Andere Gruppen zu zahlreichen Benutzern hinzuzufügen. Nach dem Speichern der Änderungen wurden alle vorhandenen "Sonstige Gruppen"entfernt und nur die neue "Sonstige"-Gruppe blieb erhalten.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Andere Gruppen des Benutzers für die Massenbearbeitung

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

## Problem:

Bei der Massenbearbeitung habe ich versucht, eine einzelne Andere Gruppen zu zahlreichen Benutzern hinzuzufügen.
Nach dem Speichern der Änderungen wurden alle vorhandenen &quot;Sonstige Gruppen&quot;entfernt und nur die neue &quot;Sonstige&quot;-Gruppe blieb erhalten.

## Antwort:

Das resultierende Verhalten hängt von der aktuellen Gruppenmitgliedschaft der ausgewählten Benutzer ab:

* Wenn alle ausgewählten Benutzer Andere Gruppenmitgliedschaften exakt übereinstimmen ...
Nachdem Sie die Benutzer ausgewählt und [!UICONTROL Bearbeiten] ausgewählt haben, wird im Feld [!UICONTROL Andere Gruppen] die vollständige Liste angezeigt
der Gruppen, zu denen diese Benutzer gehören.

* Wenn die ausgewählten Benutzer über verschiedene Mitglieder der Gruppe Andere Gruppen verfügen..
Nachdem Sie die Benutzer ausgewählt und auf [!UICONTROL Bearbeiten] geklickt haben, ist das Feld [!UICONTROL Andere Gruppen] leer.

Wenn Sie auf **[!UICONTROL Änderungen speichern]** klicken, wird das im Feld &quot;Andere Gruppen&quot;angezeigte Element gespeichert.

Der vorherige Inhalt des Felds wird überschrieben.
