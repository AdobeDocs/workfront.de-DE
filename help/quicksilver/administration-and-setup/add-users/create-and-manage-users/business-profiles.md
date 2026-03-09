---
title: Übersicht über Geschäftsprofile
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: add-users-to-workfront
description: Geschäftsprofile sind ein erweitertes Berechtigungsmodell, das es Kunden wie Agenturen ermöglicht, den Benutzerzugriff effizient zu verwalten und eine präzise Kontrolle über Berechtigungen auf Gruppenebene sicherzustellen. In einem Geschäftsprofil haben Benutzer unterschiedliche Berechtigungen für gruppenspezifische Objekte. Zusätzliche Objekte können auch direkt für das Geschäftsprofil freigegeben werden.
author: Becky
feature: System Setup and Administration
role: Admin
hide: true
hidefromtoc: true
exl-id: 7f62de33-e544-4be9-8dcf-03a2e09e8a05
source-git-commit: 1389c6a1f41a14bafd6b70e2e079e40d22d47b07
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 0%

---

# Übersicht über Geschäftsprofile

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für bestimmte Kunden verfügbar.</span>

Geschäftsprofile sind ein erweitertes Berechtigungsmodell, das es Kunden wie Agenturen ermöglicht, den Benutzerzugriff effizient zu verwalten und eine präzise Kontrolle über Berechtigungen auf Gruppenebene sicherzustellen. In einem Geschäftsprofil haben Benutzer unterschiedliche Berechtigungen für gruppenspezifische Objekte. Zusätzliche Objekte können auch direkt für das Geschäftsprofil freigegeben werden.

Ein Geschäftsprofil für einen Benutzer ähnelt dem eines Benutzers, der eine bestimmte Rolle in einer Gruppe innehat, z. B. ein Finanzcontroller oder Projektmanager, und der die Berechtigungen erhält, die mit dieser Rolle für die angegebene Gruppe einhergehen. Das Geschäftsprofil kann temporär sein, sodass die Berechtigungen für einen Zeitraum ablaufen können und Datenbeschränkungen für die Gruppe oder Agentur beibehalten werden.

Der Workfront-Systemadministrator:

* Erstellt die Zugriffsebenen und definiert bei Bedarf eingeschränkte Felder.
* Aktualisiert das Benutzerprofil mit der Gruppe und die Zugriffsebene für diese Gruppe (das Geschäftsprofil)
* Definiert nach Bedarf effektive Termine für das Geschäftsprofil
* Weist den Zugriffsebenen Layoutvorlagen zu

Jeder Benutzer, der Zugriff auf das Freigeben von Objekten hat, kann diese für das Geschäftsprofil freigeben, und alle Benutzer mit dem Profil sehen das Objekt.

## Beispiel für ein Geschäftsprofil

>[!BEGINSHADEBOX]

SAM benötigt unterschiedlichen Zugang zu Projekten für Agentur A und Agentur B. Beide Agenturen werden in Workfront als Gruppen eingerichtet. (Informationen zu Gruppen finden Sie unter Gruppen - Übersicht.)

Für die Agentur A fungiert Sam als Finanzkontrolleur und benötigt Zugriff, um alle finanziellen Bereiche ihrer Projekte zu sehen. Für die Agentur B fungiert Sam als Projekt-Manager und muss die Aufgaben und Probleme verwalten, sollte jedoch nicht in der Lage sein, die Finanzinformationen einzusehen.

Der Workfront-Systemadministrator erstellt neue Zugriffsebenen namens „Finanzcontroller“ und „Projektmanager“. Diese Zugriffsebenen erhalten für Finanzdaten den richtigen Zugriff. Anschließend öffnet der Administrator das Benutzerprofil von Sam und wählt „Agentur A“ als Gruppe mit der Zugriffsebene „Finanzcontroller“ aus, um das erste Geschäftsprofil zu erstellen, und „Agentur B“ als Gruppe mit der Zugriffsebene „Projektmanager“, um das zweite Geschäftsprofil zu erstellen.

Wenn die Geschäftsprofile eingerichtet sind und Sam zur Projektliste wechselt, werden alle Projekte für Agentur A und Agentur B angezeigt (zusammen mit allen anderen Projekten, die Sam erstellt hat oder für die ihm Berechtigungen erteilt wurden). Die Finanzfelder der Projekte der Agentur A sind für Sam sowohl in der Listenansicht als auch in den Projektdetails sichtbar, aber die Finanzfelder der Projekte der Agentur B sind ausgeblendet. Die Feldnamen werden angezeigt, die Felddaten sind jedoch leer.

Wenn andere Benutzer in einer der Agenturen Projekte mit dem Geschäftsprofil „Finanzkontrolleur - Agentur A“ oder „Projektmanager - Agentur B“ teilen, sind diese Projekte für Sam sichtbar. Die Finanzfelder der Projekte der Agentur B bleiben immer ausgeblendet, weil dies in der Zugriffsebene definiert ist.

>[!ENDSHADEBOX]

## Wie Geschäftsprofile definiert werden

Der Adobe Workfront-Systemadministrator ist für die Definition aller Bereiche eines Geschäftsprofils verantwortlich.

### Zugriffsebene erstellen

Der Workfront-Systemadministrator erstellt die Zugriffsebene mit dem erforderlichen Zugriff und definiert ggf. eingeschränkte Felder.

Weitere Informationen finden Sie unter [Erstellen und Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Geschäftsprofil zum Benutzer hinzufügen

Der Workfront-Systemadministrator fügt das Geschäftsprofil einem Benutzerprofil hinzu, indem er eine Gruppen- und Zugriffsebene auswählt. Die Kombination der beiden schafft das Geschäftsprofil. Jede Gruppe kann nur in einem Geschäftsprofil pro Benutzer verwendet werden. <!--how does this combine with more than one access level per group. As far as I can see a business profile is one level and one group-->

Das Geschäftsprofil kann über mehr als eine Zugriffsebene pro Gruppe verfügen. Die Ebene mit dem höchsten Zugriff hat Vorrang.

Der Administrator kann einem Geschäftsprofil Gültigkeitsdaten zuweisen, sodass der Benutzerzugriff zu einem späteren Zeitpunkt abläuft. Das Start- und Enddatum geben an, wann der Benutzer mit dem Halten des Profils in dieser Gruppe beginnt und endet. Durch die Verwendung effektiver Daten zum Beenden des Zugriffs anstelle des Löschens des Profils kann das Profil in Zukunft erneut aktiviert werden.

Für einen Benutzer sind mehrere Geschäftsprofile zulässig.

<!--image?-->

Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md). <!--may be separate article now since it's not in the profile-->

### Zuweisen von Layout-Vorlagen zur Zugriffsebene

Der Workfront-Systemadministrator kann optional der Zugriffsebene eine Layout-Vorlage zuweisen, um sicherzustellen, dass Benutzende mit dem zugehörigen Geschäftsprofil relevante Informationen und Aktionen basierend auf ihrer Rolle innerhalb des Systems sehen.

Weitere Informationen finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

## Funktionsweise von Geschäftsprofilen

Wenn ein Geschäftsprofil einem Benutzer hinzugefügt wird, bestimmen die Berechtigungen in der Kombination aus der Gruppe und der Zugriffsebene, was der Benutzer in Workfront sehen wird.

### Workfront-Layout

Wenn die Gruppe im Geschäftsprofil mit einem Projekt verknüpft ist, wird die Layout-Vorlage für die Zugriffsebene im Geschäftsprofil angewendet. Alle Benutzer mit dem Geschäftsprofil sehen die Menüelemente, die Startseite und andere Layout-Elemente, die in der Vorlage enthalten sind. Die Layoutvorlage Geschäftsprofil hat Vorrang vor einer dem Benutzer zugewiesenen Layoutvorlage.

Wenn das Geschäftsprofil über mehrere Zugriffsebenen mit derselben Gruppe verfügt, werden die Layout-Vorlagen für beide Zugriffsebenen kombiniert. Alle verfügbaren Layout-Elemente werden angezeigt. Wenn ein Menüelement in einer Vorlage angezeigt, aber in einer anderen ausgeblendet wird, wird es angezeigt. Nur Elemente, die in allen Vorlagen für das Geschäftsprofil ausgeblendet sind, werden ausgeblendet.

In Situationen, in denen dieselben Elemente in mehreren Layout-Vorlagen angezeigt werden, die Reihenfolge der Elemente jedoch unterschiedlich ist (z. B. bei der linken Navigation oder bei Pins), wird die Reihenfolge aus der Vorlage der Zugriffsebene verwendet, die zuerst im Geschäftsprofil aufgeführt ist.

### Projekte und andere freigegebene Objekte

Wenn ein Projekt mit einer Gruppe verknüpft ist, kann ein Benutzer mit einem Geschäftsprofil für diese Gruppe das Projekt anzeigen. Die Sichtbarkeit der Felder im Projekt basiert auf der Zugriffsebene im Geschäftsprofil. Wenn der Gruppe im Geschäftsprofil des Benutzers mehrere Zugriffsebenen zugewiesen sind, wird die Ebene mit den höchsten Berechtigungen angewendet.

Eine Benutzerin oder ein Benutzer hat beispielsweise zwei Geschäftsprofile: Das erste ermöglicht den Zugriff eines Finanzcontrollers auf eine Gruppe (um Finanzfelder anzuzeigen) und das zweite den Zugriff eines Projektmanagers unter einer anderen Gruppe (wobei Finanzfelder nicht angezeigt werden sollten).

Der/die Benutzende würde Projekte für beide Gruppen in der Liste aller Projekte sehen. Sowohl in der Listenansicht als auch in den Projektdetails werden den Benutzenden Finanzdaten nur für die erste Gruppe angezeigt. Die Finanzierungsfelder für die Projekte der zweiten Gruppe wären leer.

Jeder Benutzer mit Zugriff auf die Freigabe von Objekten kann diese Objekte für ein Geschäftsprofil freigeben. Alle dem Profil zugewiesenen Benutzer verfügen über die angegebenen Berechtigungen für das Objekt. Wenn der Zugriff jedoch in der Zugriffsebene eingeschränkt ist, die vom Administrator im Geschäftsprofil zugewiesen wurde, hat die Zugriffsebene Vorrang vor den in der Freigabe erteilten Berechtigungen. Wenn beispielsweise die Zugriffsebene nicht zulässt, dass Aufgaben erstellt werden, kann der/die Benutzende keine Aufgaben zu einem Projekt hinzufügen, auch wenn ihm/ihr die Berechtigung Verwalten für ein Projekt erteilt wurde, wenn es für das Geschäftsprofil freigegeben wurde.

Wenn einem Benutzer ein Geschäftsprofil zugewiesen wird, nachdem ein Objekt bereits für das Profil freigegeben wurde, wird dem Benutzer das Objekt mit dem angegebenen Zugriff angezeigt.

Wenn ein Geschäftsprofil über mehrere Zugriffsebenen verfügt, hat die Ebene mit der höchsten Zugriffsmenge Vorrang.

Informationen zur Freigabe finden Sie unter [Freigeben eines Objekts](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

Informationen zur Zusammenarbeit von Zugriffsebenen und Berechtigungen finden Sie unter [Zugriffsebenen - Übersicht](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

## Überlegungen zu Geschäftsprofilen

* Ein Benutzer muss nicht Mitglied einer Gruppe sein, um ein Geschäftsprofil für diese Gruppe zu erhalten.
* Die Zugriffsebene für das Geschäftsprofil kann nur die „Basis“-Zugriffsebene eines Benutzers aktualisieren. Das Geschäftsprofil kann die Basisberechtigungen auf Zugriffsebene nicht entfernen.
* In Objektlisten und Berichten verfügt der Benutzer über alle Berechtigungen, die ihm von allen zugewiesenen Geschäftsprofilen über die Gruppen hinweg zur Verfügung stehen, die mit seiner Basiszugriffsebene zusammengeführt wurden. Auf anderen Seiten verfügt der Benutzer über Basisberechtigungen auf Zugriffsebene.
* Wenn eine Gruppe aus Workfront gelöscht wird, werden alle zugewiesenen Geschäftsprofile für diese Gruppe aus den zugehörigen Benutzenden entfernt.
* Wenn eine Zugriffsebene Teil eines Geschäftsprofils ist und Sie die Zugriffsebene löschen, werden Sie aufgefordert, stattdessen eine neue Zugriffsebene auszuwählen.
* Aktualisierungen von Geschäftsprofilen werden in den Workfront-Auditprotokollen verfolgt. Weitere Informationen finden Sie unter Übersicht über Audit-Protokolle.
