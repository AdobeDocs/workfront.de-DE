---
title: Automatisches Ausfüllen einer Anfrage mit KI
content-type: reference
description: Sie können KI verwenden, um Anfragefelder automatisch auszufüllen.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Automatisches Ausfüllen einer Anfrage mit KI

KI kann Ihnen helfen, Anfragefelder automatisch auszufüllen. Er kann Feldwerte auf Grundlage vorheriger Anfragen vorschlagen oder sie aus Text wie E-Mails analysieren.

Sie können diese Übermittlungen vor dem Senden der Anfrage genehmigen oder ablehnen.

Das automatische Ausfüllen überschreibt keine bereits ausgefüllten Felder.

## Vorschläge beim Ausfüllen des Formulars einholen

Das automatische Ausfüllen kann Feldwerte beim Ausfüllen des Formulars vorschlagen. Wenn Sie Werte in die Anfragefelder eingeben, vergleicht Workfront diese Werte mit vorherigen Anfragen. Wenn der eingegebene Wert eng mit anderen Feldwerten in ähnlichen Kontexten in früheren Anfragen korreliert, schlägt Workfront diese Werte vor.

Wenn beispielsweise eine Klinik immer denselben Abrechnungscode verwendet, schlägt Workfront vor, dass sich der Abrechnungscode bei Eingabe des Kliniknamens im entsprechenden Feld befindet.

So verwenden Sie Vorschläge basierend auf früheren Anfragen:

1. Erstellen Sie eine Anfrage.

   Anweisungen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Felder ausfüllen.

   Beim Ausfüllen von Feldern können andere Felder Vorschläge anzeigen.

1. Wählen Sie für jeden Feldvorschlag unter diesem Feld **Akzeptieren** oder **Ablehnen** aus.

   Oder

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

## Abrufen von Vorschlägen aus einer Textaufforderung

Das automatische Ausfüllen kann Feldwerte basierend auf Text vorschlagen, z. B. E-Mails. Sie fügen einen Textblock ein, und Workfront hat den Text verarbeitet, um auf der Grundlage des Texts Feldwerte vorzuschlagen.

Wenn die E-Mail beispielsweise „Dies ist am 1. Juni fällig“ enthält und das Anfrageformular ein Feld für das Fälligkeitsdatum hat, schlägt Workfront für diesen Feldwert den 1. Juni vor.

Diese Art von Vorschlag überprüft auch frühere Anfragen nach ähnlichen Kontexten. Wenn in der Eingabeaufforderung beispielsweise erwähnt wird, dass die Anfrage für einen bestimmten Client gilt, kann Workfront die Rechnungsadresse für diesen Client basierend auf vorherigen Anfragen automatisch suchen und eingeben.

Sie können Text einfügen, der auf das gesamte Formular oder auf einen einzelnen Abschnitt des Formulars angewendet wird.

So verwenden Sie Vorschläge basierend auf einer eingefügten Textaufforderung:

1. Erstellen Sie eine Anfrage.

   Anweisungen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Um die Textaufforderung auf das gesamte Formular anzuwenden, klicken **oben rechts** Bildschirm auf „Automatisch mit KI ausfüllen“.

   Oder

   Um die Textaufforderung auf einen einzelnen Abschnitt anzuwenden, klicken Sie auf das KI![Symbol „KI](assets/request-prompt-icon.png)Symbol neben dem Abschnittsnamen.

1. Fügen Sie den Text in das Eingabeaufforderungsfeld ein.
1. Klicken Sie **Formular ausfüllen**.

   Workfront generiert Vorschläge für das Formular.
1. Wählen Sie für jeden Feldvorschlag unter diesem Feld **Akzeptieren** oder **Ablehnen** aus.

   Oder

   Wählen **oben auf der Seite** Alle akzeptieren **oder (Alle**) aus, um alle Vorschläge zu akzeptieren oder abzulehnen.

