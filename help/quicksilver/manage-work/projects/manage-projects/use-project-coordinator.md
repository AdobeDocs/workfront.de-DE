---
title: Verwenden des Projektkoordinators
content-type: reference
description: Erfahren Sie, wie Sie den Projektkoordinator verwenden, einen vorkonfigurierten KI-Mitarbeiter, der den Projektstatus überwacht und überfällige Aufgaben nachverfolgt.
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 6%

---
# Verwenden des Projektkoordinators

{{highlighted-preview-article-level}}

Der Projektkoordinator ist ein vorkonfigurierter KI-Mitarbeiter, der Ihr Projekt überwacht und Stakeholder über wichtige Statusinformationen informiert.

Die Verwendung eines Projektkoordinators erfordert nicht, dass Sie einen Agenten außerhalb von Workfront konfigurieren.

Anweisungen zum Konfigurieren eines Projektkoordinators finden Sie unter [Konfigurieren eines Projektkoordinators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) im Artikel Konfigurieren von KI-Mitwirkenden.

Weitere Informationen zu KI-Mitwirkenden im Allgemeinen finden Sie unter [Konfigurieren von KI-Mitwirkenden](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Auswählen von, Prime oder Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Sie müssen über Verwaltungsberechtigungen für Projekte verfügen, um einen Projektkoordinator zuzuweisen.</td> 
  </tr>
  </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Projektkoordinator - Übersicht

Der Projektkoordinator überwacht Ihr Projekt und hilft, die Arbeit auf Kurs zu halten. Wenn es einem Projekt zugewiesen wird, sendet es Projektaktualisierungen nach einem Zeitplan, den Ihr Administrator konfiguriert. Zu den Aktualisierungen können gehören:

* Eine Zusammenfassung des Fortschritts
* Projektzustand
* Überfällige oder gefährdete Aufgaben oder Genehmigungen
* Fehlende Felder oder Zuweisungen

Der Projektkoordinator kann sich auch zu dem Projekt und seinen Aufgaben äußern.

Ihr Administrator konfiguriert, wie oft Aktualisierungen gesendet werden, wann sie gesendet werden und wer sie erhält.

Sie können den Projektkoordinator auch bei Bedarf ausführen, indem Sie ihn in einer Aktualisierung des Projekts erwähnen. Der Projektkoordinator wird ausgeführt, wenn er erwähnt wird, auch wenn die Ausführung zu diesem Zeitpunkt nicht geplant ist.

>[!NOTE]
>
>Das Verhalten des Projektkoordinators kann sich vor der allgemeinen Verfügbarkeit ändern.

## Hinzufügen des Projektkoordinators zu einem Projekt

Ein Administrator muss zunächst den Projektkoordinator erstellen und das Feld **Projektkoordinator** zur Projekt-Kopfzeile in Ihrer Layout-Vorlage hinzufügen. Dann wird das Feld in der Projekt-Kopfzeile angezeigt.

Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

So weisen Sie einem Projekt einen Projektkoordinator zu:

1. Wechseln Sie zu dem Projekt, dem Sie einen Projektkoordinator zuweisen möchten.
1. Klicken Sie in der Kopfzeile des Projekts auf das Feld **Projektkoordinator**.
1. Wählen Sie den Projektkoordinator aus, den Sie zuweisen möchten.

   Im Fenster werden eine Beschreibung des ausgewählten Projektkoordinators sowie die Aktionen angezeigt, die der Projektkoordinator ausführt.
1. Klicken Sie auf **Übernehmen**.

## Ausführen des Projektkoordinators durch Erwähnung

Zusätzlich zu den geplanten Updates können Sie jederzeit Trigger mit dem Projektkoordinator aufnehmen, indem Sie ihn in einer Aktualisierung zum Projekt @mentioning. Der Projektkoordinator wird ausgeführt, sobald er erwähnt wird, auch wenn die Ausführung zu diesem Zeitpunkt nicht geplant ist.

Um den Projektkoordinator zu erwähnen:

1. Wechseln Sie zu dem Projekt, dem der Projektkoordinator zugewiesen ist.
1. Öffnen Sie **Bereich** Updates“ des Projekts.
1. Geben Sie im Feld Aktualisieren **@** ein und wählen Sie den Projektkoordinator aus.
1. Fügen Sie Ihre Nachricht hinzu und veröffentlichen Sie dann das Update.

   Der Projektkoordinator wird ausgeführt und veröffentlicht seine Antwort.

>[!NOTE]
>
>Der Projektkoordinator muss dem Projekt zugewiesen werden, bevor Sie es mit einem @mention in Trigger setzen können.

## Konfigurieren des Projektkoordinators

Anweisungen zum Konfigurieren des Projektkoordinators finden Sie unter [Konfigurieren des Projektkoordinators](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) im Artikel Konfigurieren von KI-Mitwirkenden.
