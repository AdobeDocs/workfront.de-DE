---
title: 22.4 Administratorverbesserungen
description: 22.4 Administratorverbesserungen
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 0876d4d47aad701d5ffadc88868217ebae7e4790
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 22.4 Administratorverbesserungen

Auf dieser Seite werden alle Verbesserungen für Administratoren beschrieben, die mit Version 22.4 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 3. Oktober 2022 verfügbar gemacht.

Eine Liste aller in Version 22.4 verfügbaren Änderungen finden Sie unter [22.4 - Versionsübersicht](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Verwenden entsperrter Status in einem Genehmigungsprozess

>[!NOTE]
>
>Diese Funktion wurde erstmals während des Veröffentlichungszeitrahmens 22.3 in der Vorschau-Umgebung eingeführt. Es wird am 15. September 2022 in der Produktion veröffentlicht.

Um Ihnen mehr Kontrolle über die Validierungsprozesse und Status in Ihrem System zu geben, haben wir es ermöglicht, einen Validierungsprozess zu erstellen, der auf einem entsperrten Systemstatus basiert. Darüber hinaus können Sie jetzt jeden Status entsperren, der bereits in einem Genehmigungsprozess verwendet wird. Zuvor musste ein in einem Genehmigungsprozess verwendeter Systemstatus gesperrt werden. Dadurch wurde sie für alle Gruppen verfügbar - ohne dass sie entfernt oder umbenannt werden konnten - sodass Gruppenadministratoren die Statusliste ihrer Gruppe nicht an ihre spezifischen Anforderungen anpassen konnten.

## Blueprints-Symbol im Hauptmenü wird jetzt über Layoutvorlagen gesteuert

Systemadministratoren können jetzt das Blueprints-Symbol im Hauptmenü über die Layout-Vorlagenkonfiguration hinzufügen oder entfernen. Dadurch erhalten Sie mehr Kontrolle darüber, wer den Blueprints-Katalog durchsuchen kann.

Das Symbol Blueprints wird im Hauptmenü angezeigt, wenn:

* Dem Benutzer ist keine Layoutvorlage zugewiesen

* Die Layoutvorlage des Benutzers enthält in der Liste &quot;Aktive Elemente&quot;die Option &quot;Blueprints&quot;

* Die Layoutvorlage des Benutzers enthält in der Liste Verfügbare Elemente die Option Blueprints . Das Symbol wird nicht im Hauptmenü angezeigt.

Vorhandene Layoutvorlagen enthalten automatisch das Symbol Blueprints . Administratoren können das Symbol aus Layoutvorlagen entfernen, um die Sichtbarkeit des Blueprints-Katalogs zu beschränken. Neue Layoutvorlagen, die nach Version 22.4 erstellt wurden, enthalten das Blueprints-Symbol in der Liste &quot;Aktive Elemente&quot;.

Weitere Informationen finden Sie unter [Zugriff auf Blueprints konfigurieren](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Sehen Sie sich eine Videodemonstration für diese Funktion an](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Anpassung der Problemkopfzeilen

Als Workfront- oder Gruppenadministrator können Sie jetzt die Felder anpassen, die in der Kopfzeile eines Problems angezeigt werden, wenn Sie eine Layout-Vorlage verwenden.

Dieses Update umfasst die folgenden Verbesserungen:

* Entfernen oder ordnen Sie vorhandene Felder aus der Kopfzeile des Problems neu.

* Fügen Sie neue, nicht bearbeitbare Felder mit Problemübersicht hinzu. Sie können keine benutzerdefinierten Felder oder Felder hinzufügen, die bearbeitet werden können. Sie können auch bearbeitbare Felder anzeigen, die sich derzeit in der Kopfzeile des Problems befinden (z. B. Status oder Prozent abgeschlossen).

* Die Kopfzeile der Ausgabe kann bis zu fünf Felder enthalten.

* Sie können jetzt das Feld &quot;Gelöst von&quot;zur Kopfzeile des Problems hinzufügen. Wenn ein aufgelöstes Objekt mit dem Problem verknüpft ist, ändert sich das Feld &quot;Gelöst von&quot;in &quot;Beheben eines Problems&quot;, &quot;Auflösen einer Aufgabe&quot;oder &quot;Auflösen eines Projekts&quot;, je nachdem, welcher Objekttyp mit dem Problem verknüpft ist.

Vor dieser Version konnten nur Projekt- und Aufgabenkopfzeilen angepasst werden.



Weitere Informationen finden Sie unter [Anpassen von Objektüberschriften mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Sehen Sie sich eine Videodemonstration für diese Funktion an](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Anpassung von Aufgabenkopfzeilen

Als Workfront- oder Gruppenadministrator können Sie jetzt die Felder anpassen, die in der Kopfzeile einer Aufgabe angezeigt werden, wenn Sie eine Layout-Vorlage verwenden.

Dieses Update umfasst die folgenden Verbesserungen:

* Entfernen oder ordnen Sie vorhandene Felder aus der Aufgabenkopfzeile neu.

* Fügen Sie neue, nicht bearbeitbare Aufgabenübersichtsfelder hinzu. Sie können keine benutzerdefinierten Felder oder Felder hinzufügen, die bearbeitet werden können. Sie können auch bearbeitbare Felder anzeigen, die sich derzeit in der Kopfzeile der Aufgabe befinden (z. B. Status oder Prozent abgeschlossen).

* Der Aufgabenheader kann bis zu fünf Felder enthalten.

Vor dieser Version konnten nur Projektheader angepasst werden.

Weitere Informationen finden Sie unter [Anpassen von Objektüberschriften mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Sehen Sie sich eine Videodemonstration für diese Funktion an.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Früheres Feature Opt-in für die neuesten Funktionen auf Pinnwänden

Wir freuen uns, neue Pinnwände-Funktionen für eine frühzeitige Anmeldung zu öffnen. Dieses optionale Tool ist für alle Organisationen verfügbar.

Nur ein Workfront-Administrator kann sich für die frühen Funktionen anmelden. Wenn sich der Administrator für frühe Funktionen entscheidet, werden alle Benutzer der Organisation angemeldet und die zusätzlichen Funktionen sind in Ihrer Workfront-Produktionsumgebung aktiviert.

Weitere Informationen finden Sie unter [Früheres Feature Opt-in für Adobe Workfront-Pinnwände](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Sehen Sie sich eine Videodemonstration für diese Funktion an.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## Der Berechnungseditor für benutzerdefinierte Formularfelder zeigt Fehlerinformationen an

>[!NOTE]
>
>Diese Funktion wurde erstmals während des Veröffentlichungszeitrahmens 22.3 in der Vorschau-Umgebung eingeführt. Es wird mit Version 22.4 für die Produktion freigegeben.

Die Bearbeitung von Berechnungen für benutzerdefinierte Felder ist jetzt einfacher, da hilfreiche Fehlerinformationen direkt in der Berechnung angegeben werden. Während Sie ein berechnetes Feld in einem benutzerdefinierten Formular erstellen, werden die Fehler rosa hervorgehoben. Wenn Sie den Mauszeiger über den markierten Teil bewegen, wird eine QuickInfo angezeigt, in der beschrieben wird, was das Problem ist.

[Sehen Sie sich eine Videodemonstration für diese Funktion an.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migration zu Adobe Unified Experience

HINWEIS: Diese Migration wurde auf Q1-Q2 von 2023 verschoben. Betroffene Kunden werden zu diesem Zeitpunkt benachrichtigt.

Wenn Ihr Unternehmen in Adobe Admin Console integriert wurde, wird Ihre Workfront-Instanz mit Version 22.4 in die Adobe Unified Experience migriert.

Das Adobe Unified Experience umfasst:

* Eine Anmeldung für alle Adobe-Anwendungen über Adobe Experience Cloud

* Ein &quot;Organisationswechsel&quot; für den Wechsel zwischen Workfront-Organisationen und -Umgebungen

* Navigation mit Optionen für Workfront-Seiten, Adobe Experience Cloud-Voreinstellungen und Ihr Workfront-Profil

Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Sehen Sie sich eine Videodemonstration für diese Funktion an.](https://video.tv.adobe.com/v/3412388/){target=_blank}
