---
title: 22.3 Verbesserungen für Administratoren
description: 22.3 Verbesserungen für Administratoren
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 22.3 Verbesserungen für Administratoren

Auf dieser Seite werden alle Verbesserungen für Administratoren beschrieben, die mit Version 22.3 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 11. Juli 2022 bereitgestellt. Eine Liste aller in Version 22.3 verfügbaren Änderungen finden Sie unter [2.3 Versionsübersicht](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrieren von Adobe Workfront mit JumpSeat

Sie können jetzt JumpSeat in Workfront integrieren, um benutzerdefinierte, produktinterne Anleitungen für Ihre Benutzer zu erstellen. Sie müssen über eine Adobe Workfront-Unternehmenslizenz und ein aktives JumpSeat-Abonnement verfügen, um die Integration zu ermöglichen.

Weitere Informationen finden Sie unter [Konfigurieren der JumpSeat-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Standardeinstellungen für den Testversand wurden in Workfront verschoben

Sie können jetzt die folgenden Testversandeinstellungen im Workfront-Setup-Bereich bearbeiten:

* Standardeinstellungen für Testversand

* Entscheidungseinstellungen für Testsendungen

Weitere Informationen finden Sie unter [Konfigurieren der standardmäßigen Testversandeinstellungen](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Verwenden entsperrter Status in einem Genehmigungsprozess

**Hinweis:** Aus der Produktionsversion 22.3 entfernt. Diese Funktion soll am 15. September 2022 für die Produktion freigegeben werden.

Um Ihnen mehr Kontrolle über die Validierungsprozesse und Status in Ihrem System zu geben, haben wir es ermöglicht, einen Validierungsprozess zu erstellen, der auf einem entsperrten Systemstatus basiert. Darüber hinaus können Sie jetzt jeden Status entsperren, der bereits in einem Genehmigungsprozess verwendet wird.

Zuvor musste ein in einem Genehmigungsprozess verwendeter Systemstatus gesperrt werden. Dadurch wurde sie für alle Gruppen verfügbar - ohne dass sie entfernt oder umbenannt werden konnten - sodass Gruppenadministratoren die Statusliste ihrer Gruppe nicht an ihre spezifischen Anforderungen anpassen konnten.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Erstellen eines Genehmigungsprozesses für Arbeitselemente](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Erstellen oder Bearbeiten eines Status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Status auf Systemebene gesperrt und entsperrt](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## PDF-Datei zu einem benutzerdefinierten Formular hinzufügen

Wir unterstützen Sie weiterhin dabei, benutzerdefinierte Formulare mit neuen Asset-Widgets, die Sie hinzufügen können, visueller und informativer zu gestalten, z. B. mit Bildern und Videos. Jetzt können Sie einem benutzerdefinierten Formular einen Link zu einer PDF-Datei hinzufügen. Wenn das Formular an ein Objekt angehängt wird, können Benutzer, die mit dem Objekt arbeiten, die PDF innerhalb des Formulars anzeigen und damit interagieren.

Weitere Informationen finden Sie unter [Hinzufügen oder Bearbeiten von Bildern oder anderen Asset-Widgets in einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Der Berechnungseditor für benutzerdefinierte Formularfelder zeigt Fehlerinformationen an

>[!NOTE]
>
>Diese Funktion ist vorübergehend nicht verfügbar. Diese Seite wird aktualisiert, sobald die Funktion verfügbar ist.

Die Bearbeitung von Berechnungen für benutzerdefinierte Felder ist jetzt einfacher, da hilfreiche Fehlerinformationen direkt in der Berechnung angegeben werden. Während Sie ein berechnetes Feld in einem benutzerdefinierten Formular erstellen, werden die Fehler rosa hervorgehoben. Wenn Sie den Mauszeiger über den markierten Teil bewegen, wird eine QuickInfo angezeigt, in der beschrieben wird, was das Problem ist.

Weitere Informationen finden Sie unter [Hinzufügen errechneter Daten zu einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Anpassung von Projektkopfzeilen

Als Workfront- oder Gruppenadministrator können Sie jetzt die Felder anpassen, die in der Kopfzeile eines Projekts angezeigt werden, wenn Sie eine Layoutvorlage verwenden.

Dieses Update umfasst die folgenden Verbesserungen:

* Entfernen Sie vorhandene Felder aus der Projektheader.

* Fügen Sie neue, nicht bearbeitbare Felder für die Projektübersicht hinzu. Sie können keine benutzerdefinierten Felder oder Felder hinzufügen, die bearbeitet werden können. Bearbeitbare Felder, die sich derzeit in der Projektheader befinden, können in der Kopfzeile verbleiben.

* Die Objektüberschrift kann bis zu fünf Felder enthalten.


Vor dieser Version konnten Felder in den Objektüberschriften nicht angepasst werden.

Weitere Informationen finden Sie unter [Objektüberschriften mithilfe einer Layoutvorlage anpassen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Erstellen eines leeren Projekts steuern

Als System- oder Gruppenadministrator können Sie jetzt steuern, ob Benutzer leere Projekte erstellen können, ohne eine Vorlage zu verwenden. Im Bereich &quot;Projekteinstellungen&quot;der Einrichtung wurde eine neue Einstellung eingeführt, mit der Sie die Erstellung von leeren Projekten in den folgenden Bereichen deaktivieren können:

* Über die Option &quot;Neues Projekt&quot;in einer Liste von Projekten

* Beim Konvertieren eines Problems von der Problemseite in ein Projekt


Die neue Einstellung lautet &quot;Benutzer können Projekte erstellen, ohne eine Vorlage zu verwenden&quot;. Sie ist standardmäßig aktiviert.

**Hinweis:** Benutzer können eine Aufgabe weiterhin in ein leeres Projekt konvertieren.

Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Gruppe auf der Seite &quot;Gruppen&quot;deaktivieren

Kürzlich wurde die Möglichkeit hinzugefügt, Gruppen zu deaktivieren und zu reaktivieren. Um diese Aktion schneller und einfacher zu gestalten, haben wir sie der Seite einer Gruppe hinzugefügt. Nachdem Sie nun auf den Namen einer Gruppe geklickt haben, um zu ihrer Seite zu gelangen, können Sie das Menü Mehr auswählen ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) neben dem Namen der Gruppe und wählen Sie dann Deaktivieren oder Reaktivieren aus.

Bisher konnten Sie eine Gruppe nur über das Kontrollkästchen Ist aktiv auf der Detailseite deaktivieren oder reaktivieren.

Weitere Informationen finden Sie unter [Gruppe deaktivieren oder reaktivieren](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Hinzufügen von Videos zu benutzerdefinierten Formularen

Jetzt können Sie einem benutzerdefinierten Formular einen neuen Modus für Informationen, visuelles Interesse und Kreativität bereitstellen, indem Sie ein Video hinzufügen. Wenn das Formular an ein Objekt angehängt wird, können Benutzer, die mit dem Objekt arbeiten, das Video jederzeit wiedergeben.

Zuvor konnten Sie einem benutzerdefinierten Formular nur textbasierte Felder und Bilder hinzufügen.

Weitere Informationen finden Sie unter [Hinzufügen oder Bearbeiten eines Bild- oder Video-Asset-Widgets in einem benutzerdefinierten Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

