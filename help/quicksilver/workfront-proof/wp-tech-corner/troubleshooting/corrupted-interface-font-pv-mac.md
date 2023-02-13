---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Fehlerbehebung - Beschädigte Schnittstellenschriftart im Testversand-Viewer auf Mac
description: Wenn Sie feststellen, dass der Proofing-Viewer die Schriftart der Benutzeroberfläche nicht richtig anzeigt, kann dies auf einige Probleme mit den Schriftarten auf Ihrem Mac-Computer zurückzuführen sein. Um das Problem zu lösen, versuchen Sie die folgenden Lösungen - BEARBEITEN SIE MICH.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 1e96720a-b967-4447-bd14-26fc6a502b25
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 0%

---

# Fehlerbehebung - Beschädigte Schnittstellenschriftart im Testversand-Viewer auf Mac

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie feststellen, dass der Proofing-Viewer die Schriftart der Benutzeroberfläche nicht richtig anzeigt, kann dies auf einige Probleme mit den Schriftarten auf Ihrem Mac-Computer zurückzuführen sein. Um das Problem zu beheben, versuchen Sie die folgenden Lösungen:

## Schriftduplikate entfernen

Überprüfen Sie, ob sich im System doppelte Schriftarten befinden.

1. Schließen Sie den verwendeten Browser.
1. Öffnen Sie die Anwendung &quot;Font Book&quot;in Ihrem Ordner &quot;Applications&quot;.
1. Klicken **[!UICONTROL Alle Schriftarten]** Absatz 1.
1. Klicken **[!UICONTROL Bearbeiten]** > **[!UICONTROL Suchen nach aktivierten Duplikaten]**.

1. Klicken **[!UICONTROL Ja]** , um Duplikate aufzulösen.
1. Wenn eine Warnung zu beschädigten Schriftarten angezeigt wird, klicken Sie auf **[!UICONTROL Ja]**.
1. Starten Sie den Computer neu.
1. Testen Sie den Testversand erneut.

## Löschen Sie den Schriftartencache

Manchmal sind die Schriftarten-Caches in Mac OS X beschädigt. Wenn beispielsweise eine Schriftart oder eine Schriftfamilie mehrmals neu installiert wird oder eine Anwendung aktualisiert oder neu installiert wurde. Neben den Schriftarten-Cache-Dateien des Betriebssystems verfügen einige Anwendungen möglicherweise über einen eigenen Schriftarten-Cache. Das Löschen dieser Schriftarten-Cachedateien kann das Problem mit durcheinandergezogenem Text beheben.

Zunächst müssen Sie das Schriftbuch starten, die Schriftart oder die Schriftfamilie auswählen, mit der Sie Probleme haben, und die Taste Löschen auf Ihrer Tastatur drücken. Sie können auch mit der rechten Maustaste klicken und [!UICONTROL Familie löschen]. Wenn Sie sich nicht sicher sind, welche Schriftart oder Familie die Probleme verursacht, sollten Sie versuchen, zunächst die Duplikate zu entfernen, wie oben beschrieben.

Der zweite Schritt besteht darin, den Schriftartencache zu löschen, und es gibt mehrere Möglichkeiten, dies zu erreichen.

Die erste besteht darin, einfach in den abgesicherten Modus neu zu starten, indem Sie die Umschalttaste sofort gedrückt halten, wenn Sie die Bootmodelle beim Start hören. Wenn dieser Modus geladen wird, sollte ein Fortschrittsbalken angezeigt werden, in dem das System verschiedene Prüfungen und Wartungsroutinen durchführt, darunter das Löschen des Schriftarten-Caches.

Der zweite Ansatz besteht in der Verwendung des Terminals, was durch Ausführen des folgenden Befehls in einem Administratorkonto möglich ist: *sutil-Datenbanken sudo -remove*

>[!NOTE]
>
>Für diesen Befehl müssen Sie Ihr Passwort eingeben, das bei der Eingabe nicht angezeigt wird. Wir empfehlen Ihnen, sich mit Ihrer IT-Abteilung zu beraten, da dies möglicherweise Administratorberechtigungen auf Ihrem Computer erfordert.

Ein anderer Ansatz wäre die Verwendung eines Schriftartencache-Dienstprogramms wie z. B. FontNuke und das Löschen des Caches mit seiner Hilfe.

Viele Druckvorschub- und Bildbearbeitungs-/Designstudios verwenden auch Universal Type Server-Software, um die Lizenzierung und Verteilung von Schriftarten zu verwalten. Manchmal kann ein Problem mit dem universellen Server-Schriftartencache auftreten, das die [!DNL Workfront Proof] -Anmerkungen nicht mehr angezeigt werden.

Um dieses Problem zu beheben, löschen Sie den Schriftartencache für universellen Typ Server und starten Sie den Server für universellen Typ neu.

## Fehlerbehebung [!DNL Flash] Schriftkonflikt

Möglicherweise haben Sie keinen Zugriff auf diese Funktion, da sie von [!DNL Flash], die in den meisten Umgebungen nicht mehr unterstützt wird.

Der alte Testversand-Viewer basiert auf [!DNL Flash Player] und manchmal, wenn der Text im Testversand-Viewer fehlt, kann es zu einem Schriftkonflikt zwischen OS X und [!DNL Flash Player]. Versuchen Sie Folgendes:

1. Öffnen Sie Finder und öffnen Sie die **[!UICONTROL Los]** Registerkarte.
1. Drücken Sie die Wahltaste ( ⌥ Alt ), um die [!UICONTROL Bibliothek] in der Dropdown-Liste.
1. Klicken Sie bei gedrückter Wahltaste auf die [!UICONTROL Bibliothek] Ordner.
1. Nach dem [!UICONTROL Bibliothek] Ordner geöffnet, navigieren Sie zu [!UICONTROL Schriftarten] Ordner in
1. Verschieben Sie alle Schriftarten, die sich im [!UICONTROL Schriftarten] in einen anderen Ordner, vielleicht auf Ihrem Desktop (erstellen Sie bitte keinen weiteren Ordner im Ordner &quot;Schriftarten&quot;).
1. Diese Aktion blendet alle benutzerdefinierten Schriften aus. sollten Sie die Standardsystemschriftarten weiterhin an ihrem eigenen Speicherort speichern.
1. Beenden und neu starten [!DNL Safari].
1. Öffnen Sie den Testversand erneut.

Sie sollten Ihre Schriftarten jetzt sehen. Wenn Sie keine der Schriftarten benötigen, die Sie aus Ihrem Basisverzeichnis entfernt haben, können Sie sie sicher löschen. Andernfalls durchgehen Sie sie in Stapeln, kopieren Sie sie zurück in den Ordner &quot;Bibliothek/Schriftarten&quot;und sehen Sie, welcher das Problem verursacht.
