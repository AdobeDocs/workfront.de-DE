---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: Benutzer,Zeitplan
navigation-topic: configure-timesheets-and-schedules
title: Zeitpläne - Übersicht
description: Sie können Ihre Arbeitswoche mithilfe von Zeitplänen definieren. Sie können einen Zeitplan mit einem Benutzer oder Projekt verknüpfen. Dies ermöglicht  [!DNL Adobe Workfront]  Berechnung von Zeitplänen und Benutzerverfügbarkeit. Anweisungen finden Sie unter Erstellen eines Zeitplans.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Zeitpläne - Übersicht

<!-- Audited: 1/2024 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Sie können Ihre Arbeitswoche mithilfe von Zeitplänen definieren und einen Zeitplan einem Benutzer oder Projekt zuordnen. Auf diese Weise können [!DNL Adobe Workfront] Timelines und die Benutzerverfügbarkeit berechnen. Anweisungen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Beachten Sie beim Arbeiten mit Zeitplänen in Workfront Folgendes:

* Der [!DNL Workfront] Administrator identifiziert die Betriebsstunden für die Organisation in einem Zeitplan.

  Auf ähnliche Weise kann ein Gruppenadministrator die Betriebsstunden eines Zeitplans identifizieren, der von einer von ihm verwalteten Gruppe verwaltet wird. Weitere Informationen zu Gruppenadministratoren finden Sie unter [Gruppenadministratoren](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Beispielsweise kann ein Zeitplan wie folgt definiert werden: Montag bis Freitag, 8 bis 17 Uhr, mit einer Stunde Pause für das Mittagessen.

* [!DNL Workfront] verwendet den Zeitplan, um festzulegen, wann der Arbeitstag beginnt und endet.

  Dies hindert einen Benutzer nicht daran, außerhalb der normalen Geschäftszeiten [!DNL Workfront] zu bearbeiten oder abzuschließen. Im Allgemeinen ist es nicht erforderlich, einen neuen Zeitplan oder eine Zeitplanausnahme zu erstellen, um sich auf die am Abend geplanten Arbeiten zu konzentrieren.

  Ebenso kann Ihr Unternehmen flexible Ankunftszeiten für Ihren Arbeitstag haben. Sie können eine Gruppe von Mitarbeitern haben, die um 8 Uhr morgens ankommt, und eine andere Gruppe, die um 9 Uhr morgens ankommt. Es ist nicht erforderlich, für jede Gruppe individuelle Zeitpläne zu erstellen, wenn die Gruppen ähnliche oder identische Zeitpläne haben. Wenn die Gruppen jedoch stark unterschiedliche Zeitpläne haben, sollten ihre Benutzer mit eindeutigen Zeitplänen verknüpft werden. Ein Mitarbeiter versteht, wenn ein Arbeitsauftrag um 17 Uhr beendet werden soll. Das bedeutet, dass die Arbeit bis zum Ende des Arbeitstages erledigt sein muss, unabhängig von der Zeit, zu der er zur Arbeit kommt.

* Es wird empfohlen, für jede mit der Organisation verknüpfte Zeitzone separate Zeitpläne zu erstellen.

  Sie können jedem Zeitplan eine bestimmte Zeitzone zuweisen, um sicherzustellen, dass die Arbeit für Benutzer, die in verschiedenen Zeitzonen arbeiten, entsprechend geplant ist.

* Der [!DNL Workfront] Standardzeitplan wird in Zeitleistenberechnungen verwendet, wenn Benutzende oder Projekte nicht mit einem Zeitplan verknüpft sind.

  Der Standardzeitplan wird mit Ihrem [!DNL Workfront] System geliefert und kann nur gelöscht werden, wenn er durch einen von Ihnen erstellten neuen Zeitplan ersetzt wird.

* Zusätzlich zur Berechnung von Zeitplänen verwendet [!DNL Workfront] Zeitpläne, um die Benutzerverfügbarkeit zu berechnen.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] verwendet entweder den Benutzer oder den Projektzeitplan, um die Ressourcenverfügbarkeit im Ressourcenplaner zu ermitteln. Welcher Zeitplan verwendet wird, hängt davon ab, was der [!DNL Workfront]-Administrator für die Einstellung [!UICONTROL Ressourcenverfügbarkeit mithilfe von berechnen] ausgewählt hat. Informationen zu den Einstellungen für die Ressourcenverwaltung finden Sie [Konfigurieren der Voreinstellungen für die ](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)).

## Hierarchie der Zeitpläne

Wenn eine Aufgabe einem Benutzer zugewiesen wird, der mit einem Zeitplan verknüpft ist, und sich in einem Projekt befindet, das mit einem zweiten Zeitplan verknüpft ist, haben Sie mindestens zwei Zeitpläne, die auf Ihre Zeitleistenberechnungen angewendet werden können.

>[!IMPORTANT]
>
>[!DNL Workfront] verwendet den Zeitplan eines Benutzers nur, wenn die Einstellung [!UICONTROL Ressourcenverfügbarkeit berechnen mit] auf [!UICONTROL Der Zeitplan des Benutzers] im Bereich [!UICONTROL Ressourcenverwaltung] von [!UICONTROL Setup] festgelegt ist. Weitere Informationen dazu, wie sich die Einstellung [!UICONTROL Ressourcenverfügbarkeit berechnen mit] auf den für die Ressourcenverwaltung verwendeten Zeitplan auswirkt, finden Sie [Konfigurieren der Voreinstellungen für die Ressourcenverwaltung](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Die Reihenfolge, in der die Zeitpläne vom System verwendet werden, wenn mehr als ein Zeitplan vorhanden ist:


* Wenn ein(e) Benutzende(r) einer Aufgabe zugewiesen wird, verwendet [!DNL Workfront] einen der folgenden Zeitpläne, wie im Bereich [!UICONTROL Projektvoreinstellungen] von [!UICONTROL Setup] definiert:

   * Der Zeitplan des Benutzers, der der Aufgabe zugewiesen ist
   * Der mit dem Projekt verknüpfte Zeitplan.

     Weitere Informationen zur persönlichen Arbeitszeit finden Sie unter [Konfigurieren der persönlichen ](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md)).

* Wenn einer Aufgabe mehrere Benutzer zugewiesen sind und die Benutzer während des Zeitrahmens der Aufgabe unterschiedliche Zeitpläne haben, verwendet [!DNL Workfront] einen der folgenden Zeitpläne, wie im Bereich [!UICONTROL Projektvoreinstellungen] von [!UICONTROL Setup] definiert:

   * Der Zeitplan des Benutzers, der als Primärer Verantwortlicher bestimmt ist
   * Der mit dem Projekt verknüpfte Zeitplan.

     Weitere Informationen zu Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Wenn der der Aufgabe zugewiesene Benutzer keinen Zeitplan hat oder die Aufgabe nur einem Aufgabengebiet bzw. einem Team zugewiesen ist oder die Zuweisung für ihn aufgehoben wurde, verwendet [!DNL Workfront] den Projektplan für die Zeitleistenberechnungen.
* Wenn der der Aufgabe zugewiesene Benutzer keinen Zeitplan hat oder die Aufgabe nur einem Aufgabengebiet bzw. einem Team zugewiesen ist oder die Zuweisung für das Projekt aufgehoben wird und das Projekt keinen Zeitplan hat, verwendet [!DNL Workfront] den Zeitplan im System, der als Standardzeitplan für Zeitleistenberechnungen festgelegt wurde.

  ![](assets/default-schedule.png)

## Collaboration in [!DNL Workfront] über Zeitzonen hinweg

Informationen zur Verwendung von Zeitplänen zur Unterstützung der Zusammenarbeit von Benutzenden in [!DNL Workfront] über Zeitzonen hinweg finden Sie [Arbeiten über Zeitzonen hinweg](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
