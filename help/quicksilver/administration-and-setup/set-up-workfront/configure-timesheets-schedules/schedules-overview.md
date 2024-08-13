---
user-type: administrator
content-type: overview
product-area: system-administration;timesheets
keywords: user,schedule
navigation-topic: configure-timesheets-and-schedules
title: Zeitpläne - Übersicht
description: Sie können Ihre Arbeitswoche mithilfe von Zeitplänen definieren. Sie können einen Zeitplan mit einem Benutzer oder einem Projekt verknüpfen. Dadurch kann [!DNL Adobe Workfront] die Zeitpläne und die Benutzerverfügbarkeit berechnen. Anweisungen finden Sie unter Zeitplan erstellen .
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 02350860-f997-4a76-8aec-c6c813d58e2d
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Zeitpläne - Übersicht

<!-- Audited: 1/2024 -->

Sie können Ihre Arbeitswoche mithilfe von Zeitplänen definieren und einen Zeitplan mit einem Benutzer oder Projekt verknüpfen. Dadurch kann [!DNL Adobe Workfront] die Zeitpläne und die Benutzerverfügbarkeit berechnen. Anweisungen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Beachten Sie beim Arbeiten mit Zeitplänen in Workfront Folgendes:

* Der [!DNL Workfront] -Administrator identifiziert die Betriebsstunden für die Organisation in einem Zeitplan.

  Auf ähnliche Weise kann ein Gruppenadministrator die Betriebsstunden eines Zeitplans identifizieren, der von einer von ihm verwalteten Gruppe verwaltet wird. Weitere Informationen zu Gruppenadministratoren finden Sie unter [Gruppenadministratoren](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

  Beispielsweise kann ein Zeitplan wie folgt definiert werden: Montag bis Freitag, 8:00 bis 17:00 Uhr mit einer Stundenpause für das Mittagessen.

* [!DNL Workfront] verwendet den Zeitplan, um zu bestimmen, wann der Arbeitstag beginnt und endet.

  Dies verhindert nicht, dass ein Benutzer außerhalb der normalen Geschäftszeiten an der Arbeit in [!DNL Workfront] arbeitet oder diese abschließt. Im Allgemeinen ist es nicht erforderlich, einen neuen Zeitplan oder eine Planungsausnahme zu erstellen, um sich auf die abends geplanten Arbeiten zu konzentrieren.

  Ebenso kann Ihre Organisation flexible Ankunftszeiten für Ihren Arbeitstag haben. Sie können eine Gruppe von Mitarbeitern haben, die um 8 Uhr ankommen, und eine andere Gruppe, die um 9 Uhr ankommt. Es ist nicht erforderlich, für jede Gruppe eindeutige Zeitpläne zu erstellen, wenn die Gruppen ähnliche oder identische Zeitpläne haben. Wenn die Gruppen jedoch drastisch unterschiedliche Zeitpläne haben, sollten ihre Benutzer eindeutigen Zeitplänen zugeordnet werden. Ein Mitarbeiter versteht, ob eine Aufgabe um 17 Uhr abgeschlossen sein soll, es bedeutet, dass die Arbeit am Ende des Arbeitstages unabhängig von der Arbeitszeit durchgeführt werden muss.

* Es wird empfohlen, für jede mit der Organisation verbundene Zeitzone separate Zeitpläne zu erstellen.

  Sie können jedem Zeitplan eine bestimmte Zeitzone zuweisen, um sicherzustellen, dass die Arbeit für Benutzer, die in verschiedenen Zeitzonen arbeiten, entsprechend geplant ist.

* Der Standardzeitplan &quot;[!DNL Workfront]&quot; wird in Timeline-Berechnungen verwendet, wenn Benutzer oder Projekte keinem Zeitplan zugeordnet sind.

  Der Standardzeitplan wird mit Ihrem [!DNL Workfront] -System geliefert und kann nur gelöscht werden, wenn er durch einen von Ihnen erstellten neuen Zeitplan ersetzt wurde.

* Zusätzlich zur Berechnung der Zeitpläne verwendet [!DNL Workfront] Zeitpläne, um die Benutzerverfügbarkeit zu berechnen.

  >[!IMPORTANT]
  >
  >[!DNL Workfront] verwendet entweder den Benutzer oder den Projektplan, um die Ressourcenverfügbarkeit im Ressourcen-Planer zu bestimmen. Welcher Zeitplan verwendet wird, hängt davon ab, was der [!DNL Workfront] -Administrator für die Einstellung [!UICONTROL Ressourcenverfügbarkeit berechnen mit ] ausgewählt hat. Weitere Informationen zu Einstellungen für die Ressourcenverwaltung finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

## Hierarchie der Zeitpläne

Wenn eine Aufgabe einem Benutzer zugewiesen ist, der mit einem Zeitplan verknüpft ist, und sich in einem Projekt befindet, das mit einem zweiten Zeitplan verknüpft ist, verfügen Sie über mindestens 2 Zeitpläne, die möglicherweise auf Ihre Zeitleistenberechnungen angewendet werden können.

>[!IMPORTANT]
>
>[!DNL Workfront] verwendet den Zeitplan eines Benutzers nur, wenn die Einstellung [!UICONTROL Ressourcenverfügbarkeit berechnen mithilfe von ] auf [!UICONTROL Zeitplan des Benutzers] im Bereich [!UICONTROL Ressourcenverwaltung] von [!UICONTROL Einrichtung] gesetzt ist. Informationen dazu, wie die Einstellung [!UICONTROL Ressourcenverfügbarkeit berechnen mit ] beeinflusst, welcher Zeitplan für die Ressourcenverwaltung verwendet wird, finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

Die Reihenfolge, in der die Zeitpläne vom System verwendet werden, wenn mehrere Zeitpläne vorhanden sind, lautet:

* Wenn ein Benutzer einer Aufgabe zugewiesen wird, verwendet [!DNL Workfront] den Zeitplan des Benutzers für die Berechnung der Zeitleiste der Aufgabe. Dies schließt auch die persönliche Zeit des Benutzers ein. Der Zeitplan des Projekts wird ignoriert.

  Weitere Informationen zur persönlichen Zeit finden Sie unter [Persönliche Zeit von ](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md) konfigurieren.

* Wenn einer Aufgabe mehrere Benutzer zugewiesen sind und die Benutzer während des Zeitrahmens der Aufgabe unterschiedliche Zeitpläne haben, verwendet [!DNL Workfront] einen der folgenden Zeitpläne, wie im Bereich [!UICONTROL Projektvoreinstellungen] von [!UICONTROL Einrichtung] definiert:

   * Der Zeitplan des Benutzers, der als Primärer Bevollmächtigter benannt wurde
   * Der mit dem Projekt verknüpfte Zeitplan.

     Weitere Informationen zu den Projektanvoreinstellungen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Wenn der der Aufgabe zugewiesene Benutzer keinen Zeitplan hat oder die Aufgabe nur einer Auftragsrolle, einem Team oder einer nicht zugewiesenen Zuweisung zugewiesen ist, verwendet [!DNL Workfront] den Projektzeitplan für die Timeline-Berechnungen.
* Wenn der der Aufgabe zugewiesene Benutzer keinen Zeitplan hat oder die Aufgabe nur einer Auftragsrolle, einem Team oder einer nicht zugewiesenen Zuweisung zugewiesen ist und das Projekt keinen Zeitplan hat, verwendet [!DNL Workfront] den Zeitplan im System, der als Standardzeitplan für Timeline-Berechnungen festgelegt wurde.

  ![](assets/default-schedule.png)

## Collaboration in [!DNL Workfront] über Zeitzonen hinweg

Informationen zur Verwendung von Zeitplänen zur Unterstützung der Zusammenarbeit von Benutzern in [!DNL Workfront] über Zeitzonen hinweg finden Sie unter [Arbeiten über Zeitzonen hinweg](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).
