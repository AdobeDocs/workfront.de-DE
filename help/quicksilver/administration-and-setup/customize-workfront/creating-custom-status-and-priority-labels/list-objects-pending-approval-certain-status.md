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

1. Wechseln Sie in der Leiste &quot;Globale Navigation&quot;zum Bereich **Berichterstellung** und wählen Sie dann die Registerkarte **Berichte** aus.
1. Klicken Sie oben rechts auf das Hauptmenü-Symbol ![](assets/main-menu-icon.png) und dann auf **Berichte**.
1. Klicken Sie auf &quot;**Neuer Bericht**&quot;und wählen Sie dann &quot;**Projektbericht**&quot;, &quot;**Aufgabenbericht**&quot;oder &quot;**Problembericht**&quot;.
1. Öffnen Sie die Registerkarte **Filter** .
1. Klicken Sie auf **Filterregel hinzufügen** und führen Sie dann die folgenden Schritte aus, um die Regel einzurichten:
   1. Beginnen Sie mit der Eingabe von `status` und wählen Sie dann **Status** aus, wenn es angezeigt wird.
   1. Belassen Sie **Equal** im zweiten Feld.
   1. Wählen Sie im dritten Feld den Namen des Status aus.
1. Klicken Sie erneut auf **Filterregel hinzufügen** und führen Sie dann die folgenden Schritte aus, um die Regel einzurichten
   1. Beginnen Sie mit der Eingabe von `pending status` und wählen Sie dann dieses Element aus, wenn es unter dem Objekttyp angezeigt wird, in dem Sie suchen (**Projekt**, **Aufgabe** oder **Problem**).
   1. Belassen Sie **Equal** im zweiten Feld.
   1. Geben Sie `in` in das dritte Feld ein.
1. Klicken Sie erneut auf **Filterregel hinzufügen** und führen Sie dann die folgenden Schritte aus, um die Regel einzurichten
   1. Starten Sie den Typisierungsprozess und wählen Sie dann **Gruppen-ID** aus, wenn er unter **Genehmigungsprozess** angezeigt wird.
   1. Wählen Sie im zweiten Feld **Ist leer** aus.
1. Klicken Sie auf **Speichern + Schließen** , um den Bericht auszuführen und alle Objekte des Typs aufzulisten, die Sie mit Genehmigungsprozessen im ausstehenden Status basierend auf dem von Ihnen angegebenen Status (**Projekt**, **Aufgabe** oder **Problem**) angegeben haben.
1. Wiederholen Sie diese Schritte, um dieselben Informationen für die beiden anderen Objektarten zu finden.


## Im Textmodus

1. Klicken Sie oben rechts auf das Hauptmenü-Symbol ![](assets/main-menu-icon.png) und dann auf **Berichte**.
1. Klicken Sie auf &quot;**Neuer Bericht**&quot;und wählen Sie dann &quot;**Projektbericht**&quot;, &quot;**Aufgabenbericht**&quot;oder &quot;**Problembericht**&quot;.
1. Öffnen Sie die Registerkarte **Filter** .
1. Wählen Sie **In den Textmodus wechseln** aus.
1. Kopieren Sie Folgendes und fügen Sie es in das Bearbeitungsfenster ein. Ersetzen Sie dabei XXX durch die 3-Buchstaben-Taste für den Status:

   `status=XXX`

   `status_Mod=in`

   `approvalProcess:groupID_Mod=isblank`

   Sie können den Schlüssel in der Liste der Status anzeigen, wie in den folgenden Artikeln dargestellt:
   * [Zugriff auf die Liste der Systemprojektstatus](project-statuses.md)
   * [Zugriff auf die Liste der Systemaufgabenstatus](task-statuses.md)
   * [Zugriff auf die Liste der Systemfehlerstatus](issue-statuses.md)

1. Klicken Sie auf **Speichern + Schließen** , um den Bericht auszuführen und alle Objekte des Typs aufzulisten, die Sie mit Genehmigungsprozessen im ausstehenden Status basierend auf dem von Ihnen angegebenen Status (**Projekt**, **Aufgabe** oder **Problem**) angegeben haben.
1. Wiederholen Sie diese Schritte, um dieselben Informationen für die beiden anderen Objektarten zu finden.
