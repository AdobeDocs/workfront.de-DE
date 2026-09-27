---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-users-and-contacts
title: Massenbearbeitung der anderen Gruppen der Benutzenden
description: Bei der Massenbearbeitung habe ich versucht, einer Vielzahl von Benutzern eine einzelne „Andere Gruppen“ hinzuzufügen. Nach dem Speichern der Änderungen wurden alle vorhandenen „Andere Gruppe“ entfernt, und nur die neue „Andere Gruppe“ blieb erhalten.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f2402830-3263-4204-ba8a-9028ef937577
TQID: 'https://experienceleague.adobe.com/oH--gAyZgNsSf-HBHUs7TSZxW3jAktySyvZx-wNlpG0'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b18b693b-6d59-4359-95fd-a386b7a615fe
    internal-label: Workfront Proof
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 5%
---
# Massenbearbeitung der anderen Gruppen der Benutzenden

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
