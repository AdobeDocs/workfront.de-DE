---
title: Verbesserungen für Admins in Version 22.3
description: Verbesserungen für Admins in Version 22.3
author: Luke
draft: No
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
TQID: https://experienceleague.adobe.com/WCt-16lnZP57hwfKa2ejmA8-QyjQoFOEldI4TtjIdJk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 781
ht-degree: 4%

---

# Verbesserungen für Admins in Version 22.3

Auf dieser Seite werden alle Admin-Verbesserungen beschrieben, die mit Version 22.3 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 11. Juli 2022 zur Verfügung gestellt. Eine Liste aller mit Version 22.3 verfügbaren Änderungen finden Sie unter Übersicht über die Version [22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrieren von Adobe Workfront mit JumpSeat

Sie können JumpSeat jetzt mit Workfront integrieren, um benutzerdefinierte, produktinterne Anleitungen für Ihre Benutzerinnen und Benutzer zu erstellen. Sie müssen über eine Adobe Workfront Enterprise-Lizenz und ein aktives JumpSeat-Abonnement verfügen, um die Integration zu aktivieren.

Weitere Informationen finden Sie unter [Konfigurieren der JumpSeat-Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Standardeinstellungen für Korrekturabzüge wurden in Workfront verschoben

Sie können jetzt die folgenden Korrekturabzugseinstellungen im Workfront-Setup-Bereich bearbeiten:

* Standardeinstellungen für Korrekturabzüge

* Einstellungen für Korrekturabzugsentscheidungen

Weitere Informationen finden Sie unter [Konfigurieren der standardmäßigen Korrekturabzugseinstellungen](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Verwenden entsperrter Status in einem Genehmigungsprozess

**Hinweis:** wurde aus der Produktionsversion 22.3 entfernt. Diese Funktion soll am 15. September 2022 in der Produktionsumgebung veröffentlicht werden.

Um Ihnen mehr Kontrolle über die Genehmigungsprozesse und -status in Ihrem System zu geben, haben wir es ermöglicht, einen Genehmigungsprozess basierend auf einem entsperrten Systemstatus zu erstellen. Darüber hinaus können Sie jetzt jeden Status entsperren, der bereits in einem Genehmigungsprozess verwendet wird.

Zuvor musste ein in einem Genehmigungsprozess verwendeter Systemstatus gesperrt werden. Dadurch war sie für alle Gruppen verfügbar - ohne die Möglichkeit, sie zu entfernen oder umzubenennen -, sodass Gruppenadministratoren die Statusliste ihrer Gruppe nicht an ihre spezifischen Anforderungen anpassen konnten.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Einen Genehmigungsprozess für Arbeitselemente erstellen](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Status erstellen oder bearbeiten](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Gesperrte und entsperrte Status auf Systemebene](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Hinzufügen einer PDF-Datei zu einem benutzerdefinierten Formular

Wir helfen Ihnen auch weiterhin dabei, benutzerdefinierte Formulare visuell und informativer zu gestalten, indem Sie neue Asset-Widgets hinzufügen können, z. B. Bilder und Videos. Jetzt können Sie einem benutzerdefinierten Formular einen Link zu einer PDF-Datei hinzufügen. Wenn das Formular mit einem Objekt verbunden ist, können Benutzende, die mit dem Objekt arbeiten, die PDF im Formular anzeigen und damit interagieren.

## Im Editor zur Berechnung von benutzerdefinierten Formularfeldern werden Fehlerinformationen angezeigt

>[!NOTE]
>
>Diese Funktion ist vorübergehend nicht verfügbar. Diese Seite wird aktualisiert, wenn die Funktion verfügbar ist.

Die Bearbeitung von Berechnungen für benutzerdefinierte Felder ist jetzt einfacher, da hilfreiche Fehlerinformationen direkt in der Berechnung angezeigt werden. Beim Erstellen eines berechneten Felds in einem benutzerdefinierten Formular werden Fehler in rosa hervorgehoben. Wenn Sie den Mauszeiger über den hervorgehobenen Teil bewegen, wird eine QuickInfo angezeigt, die das Problem beschreibt.

## Anpassung des Projekt-Headers

Als Workfront- oder Gruppenadministrator bzw. -administratorin können Sie jetzt die Felder anpassen, die in der Kopfzeile eines Projekts angezeigt werden, wenn Sie eine Layout-Vorlage verwenden.

Dieses Update enthält die folgenden Verbesserungen:

* Entfernen Sie vorhandene Felder aus der Projektkopfzeile.

* Neue, nicht bearbeitbare Felder für die Projektübersicht hinzufügen. Sie können keine benutzerdefinierten Felder oder Felder hinzufügen, die bearbeitet werden können. Bearbeitbare Felder, die sich derzeit im Projekt-Header befinden, können in der Kopfzeile verbleiben.

* Die Objektkopfzeile kann bis zu fünf Felder enthalten.


Vor dieser Version konnten Felder in den Objekt-Headern nicht angepasst werden.

Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Steuerelement zum Erstellen eines leeren Projekts

Als System- oder Gruppenadministrator können Sie jetzt steuern, ob Benutzer leere Projekte erstellen können, ohne eine Vorlage zu verwenden. Im Bereich Projektvoreinstellungen von Setup wurde eine neue Einstellung eingeführt, mit der Sie die Erstellung leerer Projekte in den folgenden Bereichen deaktivieren können:

* über die Option Neues Projekt in einer Projektliste

* Bei der Konvertierung einer Anfrage in ein Projekt über die Anfrageseite


Die neue Einstellung ist „Benutzern erlauben, Projekte ohne Vorlage zu erstellen“ und sie ist standardmäßig aktiviert.

**Hinweis:** Benutzer können eine Aufgabe weiterhin in ein leeres Projekt konvertieren.

Weitere Informationen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Deaktivieren von Gruppen auf der Seite Gruppen

Kürzlich haben wir die Möglichkeit hinzugefügt, Gruppen zu deaktivieren und zu reaktivieren. Um diese Aktion zu beschleunigen und zu vereinfachen, wurde sie zur Seite einer Gruppe hinzugefügt. Nachdem Sie nun auf den Namen einer Gruppe geklickt haben, um zu ihrer Seite zu gelangen, können Sie das Menü Mehr ![Hauptmenüsymbol](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) neben dem Gruppennamen auswählen und dann Deaktivieren oder Reaktivieren auswählen.

Zuvor konnten Sie eine Gruppe nur mithilfe des Kontrollkästchens Ist aktiv auf ihrer Detailseite deaktivieren oder reaktivieren.

Weitere Informationen finden Sie unter [Deaktivieren oder Reaktivieren einer Gruppe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Hinzufügen von Videos zu benutzerdefinierten Formularen

Jetzt können Sie einem benutzerdefinierten Formular einen neuen Modus für Informationen, visuelles Interesse und Kreativität bereitstellen, indem Sie ein Video hinzufügen. Wenn das Formular mit einem Objekt verbunden ist, können Benutzende, die mit dem Objekt arbeiten, das Video jederzeit abspielen.

Zuvor konnten Sie nur textbasierte Felder und Bilder zu einem benutzerdefinierten Formular hinzufügen.

