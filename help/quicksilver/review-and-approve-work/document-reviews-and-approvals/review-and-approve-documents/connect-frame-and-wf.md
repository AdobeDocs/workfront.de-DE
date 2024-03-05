---
product-area: projects
navigation-topic: approvals
title: Verbinden von Workfront und Frame.io
description: Workfront verwendet Frame.io im Überprüfungs- und Genehmigungsprozess, um Personen dort zu treffen, wo sie arbeiten möchten. Der Projektmanagement- und Genehmigungsprozess wird in Workfront verwaltet und der Überprüfungsprozess erfolgt in Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: cf8501ff21dc9f3a3c66d8e98555986f18aeaa80
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---


# Verbinden von Workfront und Frame.io

Workfront verwendet Frame.io im Überprüfungs- und Genehmigungsprozess, um Personen dort zu treffen, wo sie arbeiten möchten. Der Projektmanagement- und Genehmigungsprozess wird in Workfront verwaltet und der Überprüfungsprozess wird in Frame.io abgeschlossen. Sie müssen alle folgenden Abschnitte ausführen, um die Integration erfolgreich einzurichten:

* [Verbinden einer Workfront-Gruppe mit einem Frame.io-Team](#connect-a-workfront-group-to-a-frameio-team)
* [Erstellen eines Workfront-Projekts und Hinzufügen einer verbundenen Gruppe](#create-a-workfront-project-and-add-a-connected-group)

Der Inhalt dieses Artikels bezieht sich auf die aktualisierte Funktion zur Dokumentgenehmigung, die nur für bestimmte Konten verfügbar ist. Informationen zu Standardgenehmigungsverfahren finden Sie in den Artikeln unter [Arbeitsgenehmigungen](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Zugriffsanforderungen

* Ihr Unternehmen muss manuell integriert werden, um die in diesem Artikel beschriebene Funktion verwenden zu können. Weitere Informationen finden Sie unter [Alpha-Integration von Adobe Workfront und Frame.io - Überblick](/help/quicksilver/product-announcements/betas/frame-io-wf-integration-alpha/frame-io-wf-integration-alpha-overview.md).


## Verbinden einer Workfront-Gruppe mit einem Frame.io-Team

Wir verbessern diese Funktion aktiv für die allgemeine Verfügbarkeit im Mai.

### Voraussetzungen

* Erstellen Sie ein Frame.io-Team, das einer Workfront-Gruppe zugeordnet werden soll.
* Suchen Sie das API-Entwicklungstoken für das -Team. Weitere Informationen finden Sie unter [Entwicklungstoken](https://developer.frame.io/docs/getting-started/authentication#developer-tokens) auf der Entwickler-Site Frame.io.

### Verbinden einer Workfront-Gruppe mit einem Frame.io-Team

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen**.
1. Wählen Sie eine bestehende Gruppe aus oder klicken Sie auf **Gruppe erstellen**.
1. Klicken Sie im linken Bereich auf **Verbinden mit Frame.io**.
   ![](assets/connect-frame-group.png)
1. Geben Sie das API-Entwicklungstoken ein.
1. Klicks **Verbindung initiieren**.
1. (Bedingt) Wenn Sie Administrator von mehr als einem Frame.io-Konto sind, wählen Sie das Konto aus, das Sie verwenden möchten.

## Erstellen eines Workfront-Projekts und Hinzufügen einer verbundenen Gruppe

Nachdem Sie eine Workfront-Gruppe mit einem Frame.io-Team verbunden haben, müssen Sie ein Projekt mit dieser verbundenen Gruppe erstellen.

### Voraussetzungen

* Sie müssen eine Workfront-Gruppe mit einem Frame.io-Team verbinden, wie im vorherigen Abschnitt beschrieben.

### Erstellen eines Workfront-Projekts und Hinzufügen einer verbundenen Gruppe

{{step1-to-projects}}

1. Erstellen Sie ein neues Projekt von Grund auf oder eine Vorlage. Informationen zum Erstellen eines Projekts finden Sie unter [Projekt erstellen](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

1. Suchen Sie im linken Bereich nach **Projektdetails**.

1. Suchen Sie die **Gruppe** auf der rechten Bildschirmseite ein und entfernen Sie die Standardgruppe.

1. Suchen Sie im Dropdown-Menü die gewünschte Gruppe. Mit Frame.io verbundene Gruppen zeigen das Symbol Frame.io an.
   ![](assets/add-frame-group.png)

1. Nehmen Sie alle anderen Änderungen an der Projektkonfiguration vor.

1. Klicken Sie auf **Änderungen speichern**.

1. Fahren Sie mit dem nächsten Abschnitt fort.

### Hinzufügen einer Aufgabe und Festlegen des Integrationsstatus auf Aktiv

>[!NOTE]
>
>Unteraufgaben werden derzeit nicht in verbundenen Frame.io-Projekten unterstützt.


1. Erstellen Sie die Aufgaben, die Sie in Frame.io ausfüllen müssen

1. Wählen Sie die benötigten Aufgaben aus und klicken Sie auf **Bearbeiten**.

1. Scrollen Sie zum **Benutzerdefinierte Forms** und suchen Sie das Integrationsformular Frame.io.

   >[!IMPORTANT]
   >
   >Damit dieses Formular angezeigt wird, muss im Bereich Projektdetails eine verbundene Frame.io-Gruppe zugewiesen werden. Weitere Informationen finden Sie unter [Erstellen eines Workfront-Projekts und Hinzufügen einer verbundenen Gruppe](#create-a-workfront-project-and-add-a-connected-group) in diesem Artikel.


1. Aktivieren Sie die **Integrationsstatus dieser Aufgabe** und wählen Sie **Aktiv**.
   ![](assets/frame-custom-form.png)

1. Klicks **Änderungen speichern**. Neben dem Projektnamen wird ein Frame.io-Symbol angezeigt.

1. Weisen Sie Aufgaben Benutzer oder Teams zu.

   >[!NOTE]
   >
   >Benutzer oder Teams, die zu den Aufgaben hinzugefügt wurden, werden ebenfalls zum Projekt Frame.io hinzugefügt.

1. Laden Sie alle Dokumente oder kreativen Briefs im Bereich Projektdokumente hoch.

Das Projekt ist noch nicht verbunden. Sie müssen mit dem nächsten Abschnitt fortfahren, um die Integration abzuschließen.

### Aktivieren Sie das Projekt in Frame.io

1. Ändern Sie den Projektstatus in **Planung** nach **Aktuell** oder einen benutzerdefinierten Status, der dem aktuellen Wert entspricht. Dadurch wird die Integration abgeschlossen und das Projekt, die Aufgaben und alle Dokumente in Frame.io generiert.

Das Symbol Frame.io neben dem Projektnamen zeigt violett an, dass die Integration erfolgreich war. Benutzer erhalten eine E-Mail, in der sie zum Projekt Frame.io eingeladen werden.

>[!IMPORTANT]
>
>Sobald das Projekt für Frame.io verbunden ist, werden an der Projektgruppe vorgenommene Änderungen nicht in Frame.io angezeigt.


