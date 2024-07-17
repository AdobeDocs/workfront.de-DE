---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Fehlerbehebung - Beschädigte Schnittstellenschriftart im Testversand-Viewer auf Mac
description: Fehlerbehebung bei beschädigter Schnittstellenschriftart im Testversand-Viewer auf Mac
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: c3e15a052533d43065b50a9f56169b82f8dc3765
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Fehlerbehebung - Beschädigte Schnittstellenschriftart im Testversand-Viewer auf Mac

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie feststellen, dass der Proofing-Viewer die Schriftart der Benutzeroberfläche nicht richtig anzeigt, kann dies auf einige Probleme mit den Schriftarten auf Ihrem Mac-Computer zurückzuführen sein. Um das Problem zu beheben, versuchen Sie die folgenden Lösungen:

## Schriftduplikate entfernen

Überprüfen Sie, ob sich im System doppelte Schriftarten befinden.

1. Schließen Sie den verwendeten Browser.
1. Öffnen Sie die Anwendung &quot;Font Book&quot;in Ihrem Ordner &quot;Applications&quot;.
1. Klicken Sie auf **[!UICONTROL Alle Schriftarten]** (1).
1. Klicken Sie auf **[!UICONTROL Bearbeiten]** > **[!UICONTROL Suchen Sie nach aktivierten Duplikaten]**.

1. Klicken Sie auf **[!UICONTROL Ja]** , um Duplikate aufzulösen.
1. Wenn eine Warnung zu beschädigten Schriftarten angezeigt wird, klicken Sie auf **[!UICONTROL Ja]**.
1. Starten Sie den Computer neu.
1. Testen Sie den Testversand erneut.

## Löschen Sie den Schriftartencache

Manchmal sind die Schriftarten-Caches in Mac OS X beschädigt. Wenn beispielsweise eine Schriftart oder eine Schriftfamilie mehrmals neu installiert wird oder eine Anwendung aktualisiert oder neu installiert wurde. Neben den Schriftarten-Cache-Dateien des Betriebssystems verfügen einige Anwendungen möglicherweise über einen eigenen Schriftarten-Cache. Das Löschen dieser Schriftarten-Cachedateien kann das Problem mit durcheinandergezogenem Text beheben.

Zunächst müssen Sie das Schriftbuch starten, die Schriftart oder die Schriftfamilie auswählen, mit der Sie Probleme haben, und die Taste Löschen auf Ihrer Tastatur drücken. Sie können auch mit der rechten Maustaste klicken und [!UICONTROL Familie entfernen] auswählen. Wenn Sie sich nicht sicher sind, welche Schriftart oder Familie die Probleme verursacht, sollten Sie versuchen, zunächst die Duplikate zu entfernen, wie oben beschrieben.

Der zweite Schritt besteht darin, den Schriftartencache zu löschen, und es gibt mehrere Möglichkeiten, dies zu erreichen.

Die erste besteht darin, einfach in den abgesicherten Modus neu zu starten, indem Sie die Umschalttaste sofort gedrückt halten, wenn Sie die Bootmodelle beim Start hören. Wenn dieser Modus geladen wird, sollte ein Fortschrittsbalken angezeigt werden, in dem das System verschiedene Prüfungen und Wartungsroutinen durchführt, von denen einer darin besteht, den Schriftarten-Cache zu leeren.

Der zweite Ansatz besteht in der Verwendung des Terminals, was durch Ausführen des folgenden Befehls in einem Administratorkonto möglich ist: *sudo atsutil database -remove*

>[!NOTE]
>
>Für diesen Befehl müssen Sie Ihr Passwort eingeben, das bei der Eingabe nicht angezeigt wird. Wir empfehlen Ihnen, sich mit Ihrer IT-Abteilung zu beraten, da dies möglicherweise Administratorberechtigungen auf Ihrem Computer erfordert.

Ein anderer Ansatz wäre die Verwendung eines Schriftartencache-Dienstprogramms wie z. B. FontNuke und das Löschen des Caches mit seiner Hilfe.

Viele Druckvorschub- und Bildbearbeitungs-/Designstudios verwenden auch Universal Type Server-Software, um die Lizenzierung und Verteilung von Schriftarten zu verwalten. Manchmal kann ein Problem mit dem universellen Server-Schriftartencache auftreten, das dazu führen kann, dass die [!DNL Workfront Proof] -Anmerkungen verschwinden.

Um dieses Problem zu beheben, löschen Sie den Schriftartencache für universellen Typ Server und starten Sie den Server für universellen Typ neu.

## Schriftkonflikt mit [!DNL Flash] beheben

Möglicherweise haben Sie keinen Zugriff auf diese Funktion, da sie von [!DNL Flash] unterstützt wird, das in den meisten Umgebungen nicht mehr unterstützt wird.

Der alte Testversand-Viewer basiert auf &quot;[!DNL Flash Player]&quot;. Wenn der Text im Testversand-Viewer fehlt, kann es sein, dass zwischen OS X und [!DNL Flash Player] ein Schriftartkonflikt vorliegt. Versuchen Sie Folgendes:

1. Öffnen Sie Finder und öffnen Sie die Registerkarte **[!UICONTROL Los]** .
1. Drücken Sie die Wahltaste ( ⌥ Alt), um den Ordner [!UICONTROL Bibliothek] in der Dropdown-Liste zu öffnen.
1. Klicken Sie bei gedrückter Optionstaste auf den Ordner [!UICONTROL Bibliothek] .
1. Nachdem der Ordner [!UICONTROL Bibliothek] geöffnet wurde, wechseln Sie zum Ordner [!UICONTROL Schriftarten] im Ordner.
1. Verschieben Sie alle Schriftarten, die sich im Ordner [!UICONTROL Schriftarten] befinden, in einen anderen Ordner, möglicherweise auf Ihrem Desktop (erstellen Sie keinen weiteren Ordner im Ordner &quot;Schriftarten&quot;).
1. Durch diese Aktion werden alle benutzerdefinierten Schriftarten ausgeblendet. Die Standardsystemschriftarten sollten weiterhin an einem anderen Speicherort gespeichert werden.
1. Beenden und starten Sie [!DNL Safari] neu.
1. Öffnen Sie den Testversand erneut.

Sie sollten Ihre Schriftarten jetzt sehen. Wenn Sie keine der Schriftarten benötigen, die Sie aus Ihrem Basisverzeichnis entfernt haben, können Sie sie sicher löschen. Andernfalls durchgehen Sie sie in Stapeln, kopieren Sie sie zurück in den Ordner &quot;Bibliothek/Schriftarten&quot;und sehen Sie, welcher das Problem verursacht.
