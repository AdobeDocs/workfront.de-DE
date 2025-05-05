---
content-type: release-notes
navigation-topic: 2020-2-release-activity
title: 'Verbesserungen beim Ressourcenmanagement in 2020.2: Der Workload-Balancer'
description: Auf dieser Seite werden alle Verbesserungen des Ressourcen-Managements beschrieben, die mit der Version 2020.2 in der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 11. Mai 2020 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00cc1205-5d58-485b-8076-e177f1d931f9
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1741'
ht-degree: 0%

---

# Verbesserungen beim Ressourcenmanagement in 2020.2: Der Workload-Balancer

Auf dieser Seite werden alle Verbesserungen des Ressourcen-Managements beschrieben, die mit der Version 2020.2 in der Produktionsumgebung vorgenommen wurden. Diese Verbesserungen wurden in der Woche vom 11. Mai 2020 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller mit Version 2020.2 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 2020.2](../../../product-announcements/product-releases/2020.2.-release-activity/2020-2-release-overview.md).

Personen sind ein Tier-1-Asset. Mit dem Workload Balancer können Sie sie vor Burnout schützen und sie in die Lage versetzen, ihre beste Arbeit zu leisten, während sie gleichzeitig an wichtigen Unternehmensstrategien ausgerichtet werden. Ein überarbeitetes Planerlebnis, mit dem Sie die Arbeitslasten und Anforderungen Ihrer Mitarbeiter in derselben Ansicht visualisieren und verwalten können. Die Benutzeroberfläche bietet eine klare visuelle Zuordnung von Über- und Unterauslastung und ist für alle Beteiligten transparent. Personen und Manager können diese Informationen als Eingabe verwenden und vom gleichen Bildschirm aus den Aufwand über die Zeitleiste neu ausbalancieren, was sich dann im Rest der Workfront-Plattform widerspiegelt.

>[!NOTE]
>
>Der Workload Balancer begann mit der Veröffentlichung der Betaversion 2019.4. Alle Verbesserungen am Workload Balancer sind generell in der Version 2020.2 verfügbar. Die auf dieser Seite beschriebenen Verbesserungen wurden mit der Version 2020.2 hinzugefügt. Einen Überblick über den Workload-Balancer finden Sie unter [Übersicht über den Workload-Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

## Tägliche und wöchentliche Zuordnung im Workload Balancer anpassen

Um ein Burnout Ihrer Ressourcen zu vermeiden, können Sie jetzt die tägliche und wöchentliche Zuordnung Ihrer Benutzer für die Arbeit mit dem Workload Balancer anpassen.

Vor dieser Verbesserung war dies nur mit den Tools für die Ressourcenplanung möglich.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(DO NOT ADD THIS, JUST ADD THE VIDEO FOR NOW: For information about managing allocations in the Workload Balancer, see /Content/Resource Mgmt/Workload Balancer/Manage hours in the Workload Balancer.htm.)</p>
-->

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Workload Balancer-Filter

Damit die Informationen im Workload-Balancer für Sie relevant sind, können Sie jetzt Filter sowohl für die Bereiche Nicht zugewiesene Arbeit als auch für die Bereiche Zugewiesene Arbeit des Workload-Balancer erstellen und für die zukünftige Verwendung speichern. Sie können dann die gespeicherte Version bearbeiten, um kleine Änderungen daran vorzunehmen, anstatt von Grund auf mit einem neuen Filter zu beginnen.

Weitere Informationen zum Filtern im Workload Balancer finden Sie unter [Filter im Workload Balancer verwalten](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(or if you are using Adobe Workfront Classic, see )
</MadCap:conditionalText>
-->

.

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Verbleibende Stunden im Workload Balancer anzeigen

Um Ihnen bei korrekten Zuweisungsentscheidungen zu helfen, können Sie jetzt mit einer neuen Einstellung den Stundenunterschied zwischen den Stunden anzeigen, die ein(e) Benutzende(r) gemäß seinem/ihrem Zeitplan arbeiten kann, und den Stunden, die ihm/ihr bereits zugewiesen wurden (die verbleibenden Stunden). Die neue Einstellung ist jetzt im Workload Balancer verfügbar.

Weitere Informationen zum Anzeigen von Informationen im Workload-Balancer finden Sie unter [Navigieren im Workload-Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Navigieren im Workload-Balancer](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Das neue Adobe Workfront-Erlebnis

## Täglich geplante Stunden für Aufgaben und Projekte im Bereich Nicht zugewiesene Arbeit des Workload Balancer anzeigen

Damit Sie besser verstehen können, wie sich Aufgaben auf den Arbeitsaufwand Ihrer Benutzer auswirken, bevor Sie sie zuweisen, verwaltet die Einstellung „Zuordnungen anzeigen“ jetzt, welche Informationen im Bereich Nicht zugewiesene Arbeit des Workload Balancer angezeigt werden. Wenn diese Einstellung aktiviert ist, werden die geplanten Stunden für Aufgaben und Projekte im Bereich Nicht zugewiesene Arbeit des Workload-Balancer angezeigt.

Vor dieser Änderung wurden mit dieser Einstellung nur Informationen im Bereich Zugewiesene Arbeit des Balancers aktualisiert.

Weitere Informationen zum Navigieren im Workload Balancer finden Sie unter [Navigieren im Workload-Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Navigieren im Workload-Balancer](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis (zuvor nur für Aufgaben verfügbar)

## Neues Feld „Einstellungen“ für den Workload Balancer

Um Ihr Erlebnis zu optimieren, ist jetzt ein Feld Einstellungen verfügbar, in dem zusätzliche Tools angezeigt werden, um die Ansicht im Workload Balancer zu aktualisieren. Dieses Feld enthält die folgenden Einstellungen:

* Gruppe nach Projekt
* Zeigt entweder die zugewiesenen Stunden oder die verbleibenden Stunden für Ihre Aufgaben und Projekte an.

Weitere Informationen zum Anzeigen von Informationen im Workload-Balancer finden Sie unter [Navigieren im Workload-Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Navigieren im Workload-Balancer](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Freigeben des Workload Balancer für einen Link

Jetzt können Sie den Arbeitsaufwand Ihrer Mitarbeiter für Führungskräfte aufteilen, damit diese über Kontext zu Ihrem Personalbedarf verfügen. Dazu können Sie jetzt den Workload-Balancer freigeben, indem Sie eine eindeutige URL für den Workload-Balancer für andere freigeben.

Weitere Informationen zum Navigieren im Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Navigieren im Workload Balancer](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Ändern des Datumsbereichs im Workload Balancer

Damit Sie die Zeitleistendauer für den Workload Balancer besser an Ihre Anforderungen anpassen können, können Sie jetzt einen benutzerdefinierten Zeitraum von 2, 4 oder 6 Wochen auswählen, der gleichzeitig angezeigt werden soll.

Vor dieser Verbesserung hat der Workload Balancer immer Informationen angezeigt, die mit der aktuellen Woche beginnen.

Weitere Informationen zum Navigieren im Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Navigieren im Workload Balancer](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis (zuvor verfügbar)

## Beim Verschieben und Kopieren von Aufgaben in ein anderes Projekt bleibt die Aufgabenbeschränkung erhalten, wenn Aufgaben in die Zeitleiste des Projekts passen

Wir haben die Art und Weise verbessert, wie Workfront die datumsspezifische Aufgabenbeschränkung einer Aufgabe handhabt, wenn Sie die Aufgabe kopieren oder in ein anderes Projekt verschieben. Beispiele für datumsspezifische Aufgabenbeschränkungen sind „Muss am“, „Muss am“, „Festes Datum“, „Start nicht später als“ usw.

Wenn Sie z. B. einen Vorgang mit der Einschränkung Muss beginnen am in ein anderes Projekt verschieben oder kopieren, dessen geplantes Startdatum vor dem Startdatum des Vorgangs liegt, behält der Vorgang die Einschränkung bei, nachdem er kopiert oder verschoben wurde. Wenn Sie einen Vorgang mit der Einschränkung Muss beginnen bei in ein Projekt verschieben oder kopieren, dessen geplantes Startdatum nach dem Startdatum des Vorgangs liegt, ändert sich die Aufgabenbeschränkung in So bald wie möglich.

Vor dieser Änderung wird die Aufgabenbeschränkung immer auf „So bald wie möglich“ geändert.

Informationen zum Verschieben von Aufgaben finden Sie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md) (oder bei Verwendung von Adobe Workfront Classic unter [Verschieben von Aufgaben](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

Informationen zum Kopieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Aufgaben kopieren und duplizieren](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

Eine Übersicht über alle Aufgabeneinschränkungen finden Sie unter [Übersicht über Aufgabeneinschränkungen](../../../manage-work/tasks/task-constraints/task-constraint-overview.md) (bzw. bei Verwendung von Adobe Workfront Classic unter [Übersicht über Aufgabeneinschränkungen](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Verhindern von Datenverlust bei Änderungen auf der Registerkarte „Details“ oder in einer Aufgabenliste

Um Datenverluste beim manuellen Speichern von Änderungen auf Projektebene beim Aktualisieren von Informationen auf der Detailseite eines Objekts oder von Aufgaben in einer Aufgabenliste zu vermeiden, wird jetzt eine Warnmeldung angezeigt, die Sie darüber informiert, dass Sie ungespeicherte Änderungen haben, bevor Sie versuchen, Informationen in der Kopfzeile zu bearbeiten. Die einzigen Aktionen, die vor dem Speichern der Änderungen zulässig sind, sind das Abonnieren oder Hinzufügen des -Objekts zu Ihren Favoriten.

Informationen zum Bearbeiten von Aufgaben in einer Liste finden Sie unter [Bearbeiten von Aufgaben in einer Liste](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md)

**In diesen Umgebungen verfügbar:**

* Das neue Adobe Workfront-Erlebnis

## Erstellen von Genehmigungsprozessen für Gruppen mit benutzerdefinierten Status

Um es Gruppen zu erleichtern, ihre eigenen eindeutigen Workflows zu verwalten, können Sie jetzt gruppenspezifische benutzerdefinierte Status in Genehmigungsprozessen verwenden.

Zuvor konnte eine Gruppe keine eigenen benutzerdefinierten Status mit ihren gruppenspezifischen Genehmigungsprozessen verwenden. Es waren nur systemweite Status verfügbar, die nicht immer den Gruppengenehmigungsprozessen entsprachen.

Benutzerdefinierte Status können jetzt sowohl in einmaligen als auch systemweiten Genehmigungsprozessen verwendet werden:

* Erstellen Sie einen einmaligen Genehmigungsprozess für ein Objekt (Projekt, Aufgabe oder Problem) und basieren Sie ihn auf Status, die mit der Gruppe verknüpft sind, die an diesem Objekt arbeitet. Dazu gehören alle benutzerdefinierten Status, die mit der Gruppe verknüpft sind.
* Erstellen Sie einen globalen Genehmigungsprozess und stellen Sie ihn nur für die Gruppe oder für alle Personen im System zur Verfügung.

Für Benutzer mit administrativem Zugriff auf Genehmigungsprozesse sind Informationen zum Konfigurieren von Genehmigungsprozessen unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) verfügbar (oder wenn Sie Adobe Workfront Classic verwenden, siehe [Erstellen von Genehmigungsprozessen](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

Für Benutzende sind Informationen zum Verknüpfen von Genehmigungsprozessen mit Arbeitselementen unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) verfügbar (oder wenn Sie Adobe Workfront Classic verwenden, siehe &quot;[ eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](https://experienceleague.adobe.com/de/docs/workfront/using/home)).

**In diesen Umgebungen verfügbar:**

* Adobe Workfront Classic
* Das neue Adobe Workfront-Erlebnis

## Eine bequemere Methode zur Aktualisierung von Zuweisungen im Workload Balancer

Um die Zuordnung von Benutzenden zu einem Arbeitselement im Workload Balancer zu verwalten, können Sie jetzt auf das Arbeitselement doppelklicken. Sie können auch weiterhin die Menüoption Zuordnungen bearbeiten verwenden. Außerdem müssen Sie die Anzeige von Zuordnungen nicht mehr aktivieren, um sie aktualisieren zu können.

Informationen zum Verwalten von Zuweisungen im Workload Balancer finden Sie unter [Verwalten von Benutzerzuweisungen im Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Geplante Stunden für Aufgaben im Workload Balancer aktualisieren

>[!NOTE]
>
>Diese Verbesserung wird kurz nach der Veröffentlichung von Version 2020.2 in der Produktion verfügbar sein.

Eine neue Option im Bereich Ressourcen-Management der Zugriffsebene ermöglicht es Benutzenden mit diesem Zugriff jetzt, die geplanten Stunden über den Workload Balancer zu bearbeiten. Wenn Sie Zuweisungen im Workload Balancer anpassen, muss die Gesamtzahl der täglichen Zuweisungen nicht mit der Anzahl der geplanten Stunden der Aufgaben übereinstimmen. Nachdem Sie die Zuteilungen gespeichert haben, wird die Summe der Zuteilungsstunden zu den geplanten Stunden der Aufgabe. Dies ist nur für Aufgaben mit dem Typ Einfache Dauer möglich.

Informationen zum Verwalten von Zuweisungen im Workload Balancer finden Sie unter [Verwalten von Benutzerzuweisungen im Workload Balancer](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

Informationen zum Gewähren des Zugriffs auf die Ressourcenverwaltung finden Sie unter [Zugriff auf die Ressourcenverwaltung gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).

## Entfernen der Bezeichnung „Beta“ aus dem Workload-Balancer

Mit der Version 2020.2 befindet sich der Workload Balancer nicht mehr im Beta-Zustand, und Sie können den Ressourcen-Balancer zur Überprüfung und Verwaltung Ihrer Ressourcenzuweisungen und -zuweisungen verwenden. Die Bezeichnung „Beta“ wurde in der Vorschau-Umgebung entfernt. Dieselbe Änderung wird mit der Produktionsversion 20.2 vorgenommen. Weitere Informationen zum Workload-Balancer finden Sie unter [Übersicht über den Workload-Balancer](../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).
