---
title: 22.4 Administrator-Verbesserungen
description: 22.4 Administrator-Verbesserungen
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

# 22.4 Administrator-Verbesserungen

Auf dieser Seite werden alle Admin-Verbesserungen beschrieben, die mit Version 22.4 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 3. Oktober 2022 zur Verfügung gestellt.

Eine Liste aller in Version 22.4 verfügbaren Änderungen finden Sie in der Übersicht über [ Version 22.4 ](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Verwenden entsperrter Status in einem Genehmigungsprozess

>[!NOTE]
>
>Diese Funktion wurde erstmals in der Vorschau -Umgebung im Zeitrahmen der Version 22.3 eingeführt. Am 15. September 2022 wurde die Veröffentlichung in der Produktionsumgebung veröffentlicht.

Um Ihnen mehr Kontrolle über die Genehmigungsprozesse und -status in Ihrem System zu geben, haben wir es ermöglicht, einen Genehmigungsprozess basierend auf einem entsperrten Systemstatus zu erstellen. Darüber hinaus können Sie jetzt jeden Status entsperren, der bereits in einem Genehmigungsprozess verwendet wird. Zuvor musste ein in einem Genehmigungsprozess verwendeter Systemstatus gesperrt werden. Dadurch war sie für alle Gruppen verfügbar - ohne die Möglichkeit, sie zu entfernen oder umzubenennen -, sodass Gruppenadministratoren die Statusliste ihrer Gruppe nicht an ihre spezifischen Anforderungen anpassen konnten.

## Blueprints-Symbol im Hauptmenü wird jetzt über Layout-Vorlagen gesteuert

Systemadministratoren können jetzt über die Konfiguration der Layout-Vorlage das Symbol Blueprints im Hauptmenü hinzufügen oder entfernen. Dies bietet eine bessere Kontrolle darüber, wer den Blueprint-Katalog durchsuchen kann.

Das Blueprints -Symbol wird im Hauptmenü angezeigt, wenn:

* Dem Benutzer wurde keine Layoutvorlage zugewiesen

* Die Layout-Vorlage des Benutzers verfügt über die Option Blueprints in der Liste Aktive Elemente .

* Die Layout-Vorlage des Benutzers verfügt über die Option Blueprints in der Liste Verfügbare Elemente . Das Symbol wird nicht im Hauptmenü angezeigt.

Vorhandene Layout-Vorlagen enthalten automatisch das Symbol Blueprints , und Admins können das Symbol aus den Layout-Vorlagen entfernen, um die Sichtbarkeit des Blueprint-Katalogs zu beschränken. Bei neuen Layout-Vorlagen, die nach der Version 22.4 erstellt wurden, wird das Blueprints-Symbol in die Liste der aktiven Elemente aufgenommen.

Weitere Informationen finden Sie unter [Zugriff auf Blueprints konfigurieren](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Sehen Sie sich eine Videodemonstration dieser Funktion an](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Anpassung der Anfragekopfzeile

Als Workfront- oder Gruppenadministrator können Sie jetzt die Felder anpassen, die in der Kopfzeile eines Problems angezeigt werden, wenn Sie eine Layout-Vorlage verwenden.

Dieses Update enthält die folgenden Verbesserungen:

* Entfernen Sie vorhandene Felder aus der Anfragekopfzeile oder ordnen Sie sie neu an.

* Neue, nicht bearbeitbare Felder zur Problemübersicht hinzufügen. Sie können keine benutzerdefinierten Felder oder Felder hinzufügen, die bearbeitet werden können. Sie können auch bearbeitbare Felder anzeigen, die sich derzeit in der Kopfzeile des Problems befinden (z. B. Status oder Prozent abgeschlossen).

* Die Problem-Kopfzeile kann bis zu fünf Felder enthalten.

* Sie können jetzt das Feld „Gelöst von“ zur Problem-Kopfzeile hinzufügen. Wenn ein Lösungsobjekt mit dem Problem verknüpft ist, ändert sich das Feld „Gelöst von“ in „Problem lösen“, „Aufgabe lösen“ oder „Projekt lösen“, je nach dem Typ des Objekts, das mit dem Problem verknüpft ist.

Vor dieser Version konnten nur Projekt- und Aufgabenkopfzeilen angepasst werden.



Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Sehen Sie sich eine Videodemonstration dieser Funktion an](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Anpassung der Aufgabenkopfzeile

Als Workfront- oder Gruppenadministrator bzw. -administratorin können Sie jetzt die Felder anpassen, die in der Kopfzeile einer Aufgabe angezeigt werden, wenn Sie eine Layout-Vorlage verwenden.

Dieses Update enthält die folgenden Verbesserungen:

* Entfernen oder Neuanordnen vorhandener Felder aus der Aufgabenkopfzeile.

* Neue, nicht bearbeitbare Felder für Aufgabenübersicht hinzufügen. Sie können keine benutzerdefinierten Felder oder Felder hinzufügen, die bearbeitet werden können. Sie können auch bearbeitbare Felder anzeigen, die sich derzeit in der Aufgabenkopfzeile befinden (z. B. Status oder Prozent abgeschlossen).

* Die Aufgabenkopfzeile kann bis zu fünf Felder enthalten.

Vor dieser Version konnten nur die Projekt-Kopfzeilen angepasst werden.

Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Frühzeitiges Opt-in für die neuesten Funktionen auf Pinnwänden

Wir freuen uns, neue Boards und Funktionen für frühzeitiges Opt-in zu öffnen. Dieses optionale Tool steht allen Organisationen zur Verfügung.

Nur ein Workfront-Administrator kann sich für die frühen Funktionen anmelden. Wenn sich der Administrator für frühe Funktionen entscheidet, werden alle Benutzenden im Unternehmen angemeldet, und die zusätzlichen Funktionen werden in Ihrer Workfront-Produktionsumgebung aktiviert.

Weitere Informationen finden Sie unter [Early Feature Opt-in for Adobe Workfront Boards](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## Im Editor zur Berechnung von benutzerdefinierten Formularfeldern werden Fehlerinformationen angezeigt

>[!NOTE]
>
>Diese Funktion wurde erstmals in der Vorschau -Umgebung im Zeitrahmen der Version 22.3 eingeführt. Mit Version 22.4 wird sie in die Produktion verschoben.

Die Bearbeitung von Berechnungen für benutzerdefinierte Felder ist jetzt einfacher, da hilfreiche Fehlerinformationen direkt in der Berechnung angezeigt werden. Beim Erstellen eines berechneten Felds in einem benutzerdefinierten Formular werden Fehler in rosa hervorgehoben. Wenn Sie den Mauszeiger über den hervorgehobenen Teil bewegen, wird eine QuickInfo angezeigt, die das Problem beschreibt.

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migration zu Adobe Unified Experience

HINWEIS: Diese Migration wurde auf das 1. bis 2. Quartal 2023 verschoben. Alle betroffenen Kunden werden zu diesem Zeitpunkt benachrichtigt.

Wenn Ihr Unternehmen Adobe Admin Console verwendet hat, wird Ihre Workfront-Instanz auf das einheitliche Adobe-Erlebnis mit Version 22.4 migriert.

Das einheitliche Adobe-Erlebnis umfasst:

* Eine einzige Anmeldung für alle Adobe-Anwendungen über Adobe Experience Cloud

* Ein „Organisationswechsel“, um zwischen Workfront-Organisationen und -Umgebungen zu wechseln

* Navigation mit Optionen für Workfront-Seiten, Adobe Experience Cloud-Voreinstellungen und Ihr Workfront-Profil

Weitere Informationen finden Sie unter [Adobe Unified Experience für Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an.](https://video.tv.adobe.com/v/3412388/){target=_blank}
