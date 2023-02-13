---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Auflisten von Objekten mit ausstehenden Genehmigungsprozessen mit einem bestimmten Status
description: Wenn Sie versuchen, einen Status zu löschen, wird Ihnen möglicherweise eine Fehlermeldung angezeigt, dass dieser nicht gelöscht werden kann, da er in ausstehenden Genehmigungsprozessen für Objekte in Ihrem System verwendet wird. Wenn Sie diese Objekte suchen und überprüfen möchten, um zu entscheiden, was Sie tun müssen, können Sie einen Bericht ausführen, der sie auflistet.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 52dd8750-9a6f-4ac6-9779-ba4ea9b6f4e0
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Auflisten von Objekten mit ausstehenden Genehmigungsprozessen mit einem bestimmten Status

Wenn Sie versuchen, einen Status zu löschen, wird Ihnen möglicherweise eine Fehlermeldung angezeigt, dass dieser nicht gelöscht werden kann, da er sich in mindestens einem ausstehenden Genehmigungsprozess in Ihrem System befindet. Sie können einen Bericht ausführen, um die Objekte aufzulisten, für die die Genehmigung aussteht, und dann für jedes Objekt entscheiden, was Sie tun müssen.

## Im Standardmodus

1. Navigieren Sie zu **Berichterstellung** Bereich in der globalen Navigationsleiste und wählen Sie dann die **Berichte** Registerkarte.
1. Klicken Sie auf das Symbol Hauptmenü . ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **Berichte**.
1. Klicken **Neuer Bericht**, wählen Sie **Projektbericht**, **Aufgabenbericht** oder **Problembericht**.
1. Öffnen Sie die **Filter** Registerkarte.
1. Klicken **Filterregel hinzufügen**, führen Sie dann die folgenden Schritte aus, um die Regel einzurichten:
   1. Typisierung beginnen `status`, wählen Sie **Status** angezeigt.
   1. Urlaub **Gleich** im zweiten Feld.
   1. Wählen Sie im dritten Feld den Namen des Status aus.
1. Klicken **Filterregel hinzufügen** wiederholen Sie dann die folgenden Schritte, um die Regel einzurichten
   1. Typisierung beginnen `pending status`und wählen Sie dann dieses Element aus, wenn es unter dem Objekttyp angezeigt wird, in dem Sie suchen (**Projekt**, **Aufgabe** oder **Problem**).
   1. Urlaub **Gleich** im zweiten Feld.
   1. Typ `in` im dritten Feld.
1. Klicken **Filterregel hinzufügen** wiederholen Sie dann die folgenden Schritte, um die Regel einzurichten
   1. Starten Sie den Typgenehmigungsprozess und wählen Sie dann **Gruppen-ID** wann sie unter angezeigt wird **Validierungsprozess**.
   1. Auswählen **Ist leer** im zweiten Feld.
1. Klicken **Speichern und schließen** , um den Bericht auszuführen und alle Objekte des Typs aufzulisten, den Sie mit Genehmigungsprozessen in ausstehendem Status basierend auf dem von Ihnen angegebenen Status (**Projekt**, **Aufgabe** oder **Problem**).
1. Wiederholen Sie diese Schritte, um dieselben Informationen für die beiden anderen Objektarten zu finden.


## Im Textmodus

1. Klicken Sie auf das Symbol Hauptmenü . ![](assets/main-menu-icon.png) in der oberen rechten Ecke und klicken Sie auf **Berichte**.
1. Klicken **Neuer Bericht**, wählen Sie **Projektbericht**, **Aufgabenbericht** oder **Problembericht**.
1. Öffnen Sie die **Filter** Registerkarte.
1. Auswählen **In den Textmodus wechseln**.
1. Kopieren Sie Folgendes und fügen Sie es in das Bearbeitungsfenster ein. Ersetzen Sie dabei XXX durch die 3-Buchstaben-Taste für den Status:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Sie können den Schlüssel in der Liste der Status anzeigen, wie in den folgenden Artikeln dargestellt:
   * [Zugriff auf die Liste der Systemprojektstatus](project-statuses.md)
   * [Zugriff auf die Liste der Systemaufgabenstatus](task-statuses.md)
   * [Zugriff auf die Liste der Systemfehlerstatus](issue-statuses.md)

1. Klicken **Speichern und schließen** , um den Bericht auszuführen und alle Objekte des Typs aufzulisten, den Sie mit Genehmigungsprozessen in ausstehendem Status basierend auf dem von Ihnen angegebenen Status (**Projekt**, **Aufgabe** oder **Problem**).
1. Wiederholen Sie diese Schritte, um dieselben Informationen für die beiden anderen Objektarten zu finden.
