---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Fehlerbehebung - Schriftart für beschädigte Benutzeroberfläche im Proofing Viewer auf Mac
description: Fehlerbehebung bei beschädigter Schriftart für die Benutzeroberfläche im Proofing Viewer auf Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Fehlerbehebung - Schriftart für beschädigte Benutzeroberfläche im Proofing Viewer auf Mac

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie bemerken, dass die Schriftart der Benutzeroberfläche im Proofing Viewer nicht richtig angezeigt wird, kann dies an einigen Problemen mit den Schriftarten auf Ihrem Mac-Computer liegen. Um das Problem zu beheben, versuchen Sie die folgenden Lösungen:

## Schriftartenduplikate entfernen

Überprüfen Sie, ob das System doppelte Schriftarten enthält.

1. Schließen Sie den verwendeten Browser.
1. Öffnen Sie die Font Book-Anwendung im Programmordner.
1. Klicken Sie **[!UICONTROL Alle Schriftarten]** (1).
1. Klicken Sie **[!UICONTROL Bearbeiten]** > **[!UICONTROL Nach aktivierten Duplikaten suchen]**.

1. Klicken Sie **[!UICONTROL Ja]**, um Duplikate zu beheben.
1. Wenn Sie eine Warnung zu beschädigten Schriftarten sehen, klicken Sie auf **[!UICONTROL Ja]**.
1. Starten Sie den Computer neu.
1. Wiederholen Sie den Korrekturabzug.

## Löschen des Schriftarten-Cache

Manchmal werden die Schriftarten-Caches in Mac OS X beschädigt. Dies ist beispielsweise der Fall, wenn eine Schriftart oder eine Schriftfamilie mehrmals neu installiert wird oder wenn eine Anwendung aktualisiert oder neu installiert wurde. Abgesehen von den Schriftarten-Cache-Dateien des Betriebssystems können einige Anwendungen über einen eigenen Schriftarten-Cache verfügen. Das Löschen dieser Schriftarten-Cache-Dateien kann das Problem mit beschädigtem Text beheben.

Zunächst müssen Sie Font Book starten, die Schriftart oder Familie auswählen, mit der Sie Probleme haben, und die Löschtaste auf Ihrer Tastatur drücken. Alternativ können Sie mit der rechten Maustaste klicken und [!UICONTROL Familie entfernen] auswählen. Wenn Sie sich nicht sicher sind, welche Schriftart oder Familie die Probleme verursacht, sollten Sie versuchen, zunächst Duplikate wie oben beschrieben zu entfernen.

Der zweite Schritt besteht darin, den Schriftarten-Cache zu löschen, und es gibt mehrere Möglichkeiten, dies zu erreichen.

Die erste ist, einfach in den abgesicherten Modus neu zu starten, indem Sie die Umschalt-Taste gedrückt halten, sobald Sie das Boot-Glockenspiel beim Start hören. Wenn dieser Modus geladen wird, sollte eine Fortschrittsleiste angezeigt werden, in der das System verschiedene Prüfungen und Wartungsroutinen ausführt, von denen eine darin besteht, den Schriftarten-Cache zu löschen.

Der zweite Ansatz besteht darin, das Terminal zu verwenden. Dies kann durch Ausführen des folgenden Befehls innerhalb eines administrativen Kontos erfolgen: *sudo atsutil database -remove*

>[!NOTE]
>
>Für diesen Befehl müssen Sie Ihr Kennwort eingeben, das bei der Eingabe nicht angezeigt wird. Wir empfehlen Ihnen, sich an Ihre IT-Abteilung zu wenden, da dies möglicherweise Administratorberechtigungen auf Ihrem Computer erfordert.

Ein anderer Ansatz wäre, ein Font-Cache-Dienstprogramm wie z. B. FontNuke zu verwenden und den Cache mit seiner Hilfe zu löschen.

Viele Druckvorstufe- und Grafikstudios verwenden außerdem die Universal Type Server-Software, um die Lizenzierung und Verteilung von Schriftarten zu verwalten. Manchmal kann ein Problem mit dem Universal Type Server Font-Cache auftreten, das dazu führen kann, dass die [!DNL Workfront Proof] Anmerkungen verschwinden.

Löschen Sie zum Beheben des Problems den Universal Type Server-Schriftarten-Cache und starten Sie den Universal Type Server neu.

## Beheben [!DNL Flash] Schriftkonflikts

Möglicherweise haben Sie keinen Zugriff auf diese Funktion, da sie von [!DNL Flash] unterstützt wird, was in den meisten Umgebungen nicht mehr unterstützt wird.

Die alte Proofing Viewer basiert auf [!DNL Flash Player] und manchmal, wenn der Text im Proofing Viewer fehlt, ist es möglich, dass ein Schriftartkonflikt zwischen OS X und [!DNL Flash Player] besteht. Probieren Sie Folgendes aus:

1. Öffnen Sie den Finder und **[!UICONTROL die Registerkarte]**.
1. Drücken Sie die Wahltaste (⌥ Alt), um den Ordner [!UICONTROL Bibliothek] in der Dropdown-Liste zu öffnen.
1. Klicken Sie bei gedrückter Wahltaste auf den Ordner [!UICONTROL Bibliothek].
1. Nachdem der Ordner [!UICONTROL Bibliothek] geöffnet wurde, wechseln Sie zum Ordner [!UICONTROL Schriftarten] in .
1. Verschieben Sie alle Schriftarten aus dem Ordner [!UICONTROL Schriftarten] in einen anderen Ordner, z. B. auf Ihrem Desktop (erstellen Sie keinen anderen Ordner innerhalb des Ordners „Schriftarten„).
1. Diese Aktion blendet alle benutzerdefinierten Schriftarten aus. Die Standardsystemschriftarten sollten weiterhin an ihrem separaten Speicherort gespeichert sein.
1. Beenden und [!DNL Safari] neu starten.
1. Öffnen Sie den Korrekturabzug erneut.

Sie sollten Ihre Schriftarten jetzt sehen. Wenn Sie keine der Schriftarten benötigen, die Sie aus Ihrem Hauptverzeichnis entfernt haben, können Sie sie sicher löschen. Andernfalls sollten Sie diese in Stapeln durchgehen, sie wieder in Ihren Bibliotheks-/Schriftartenordner kopieren und feststellen, welcher das Problem verursacht.
