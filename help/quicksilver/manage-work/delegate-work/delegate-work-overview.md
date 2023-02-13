---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Delegieren von Arbeiten - Übersicht
description: Wenn Sie planen, für kurze Zeit abwesend zu sein, können Sie Ihre Arbeit vorübergehend an andere Benutzer delegieren, um sicherzustellen, dass Ihre Abwesenheit nicht zu einem Hindernis für die Fertigstellung der Arbeit wird.
author: Alina
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: f3ae487f53f7c4f8c389cf0d35323f21e76ece35
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 1%

---

# Delegieren von Arbeiten - Übersicht

Wenn Sie planen, für kurze Zeit abwesend zu sein, können Sie Ihre Arbeit vorübergehend an andere Benutzer delegieren, um sicherzustellen, dass Ihre Abwesenheit nicht zu einem Hindernis für die Fertigstellung der Arbeit wird.

Wenn beispielsweise bestimmte Aufgaben vor der Rückkehr fällig sind, Sie jedoch keine Zeit haben, sie vor dem Verlassen abzuschließen, können Sie Ihre Aufgaben an einen anderen Benutzer delegieren, damit dieser sie rechtzeitig abschließen und den Abschluss des Projekts nicht bis nach der Rückkehr verzögern kann.

Sie können die folgenden Objekte in [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Ihnen zugewiesene Aufgaben
* Ihnen zugewiesene Probleme
* Projekt-, Aufgaben-, Problem-, Dokumentgenehmigungen, die Ihnen zugewiesen sind.

Dieser Artikel enthält allgemeine Informationen zum Delegieren von Aufgaben und Problemen.

Informationen zum Delegieren von Projekt-, Aufgaben-, Problem- und Dokumentgenehmigungen finden Sie unter [Validierungsanfrage delegieren](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Informationen zum Delegieren von Aufgaben und Problemen finden Sie unter [Aufgaben und Probleme delegieren](../../manage-work/delegate-work/how-to-delegate-work.md).

## Delegieren von Arbeiten - Übersicht

Beachten Sie Folgendes, wenn Sie Aufgaben und Probleme delegieren:

* Ihre [!DNL Workfront] oder der Gruppenadministrator muss die Delegationsvoreinstellungen im [!UICONTROL Einrichtung] -Bereich, bevor Sie Ihre Arbeit an andere delegieren können.

   Weitere Informationen finden Sie unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Sie können Aufgaben und Probleme nur über die [!UICONTROL Startseite] Bereich.
* Für die folgenden Lizenztypen gibt es Ausnahmen:

   * Sie können die Arbeit an Überprüfer oder Anforderer delegieren. [!DNL Workfront] empfiehlt es nicht.
   * Überprüfer können Arbeiten an andere delegieren. Sie können keine Arbeitselemente in ihrer [!UICONTROL Startseite] Bereich. Sie können nur Genehmigungen anzeigen.
   * Anfragende können keine Arbeit an andere delegieren. Sie können keine Arbeitselemente in ihrer [!UICONTROL Startseite] area
* Sie können nur die Ihnen zugewiesenen Aufgaben und Probleme delegieren. Sie können keine Aufgaben und Probleme delegieren, die anderen Benutzern, Teams oder Auftragsrollen zugewiesen sind.
* Sie können nur Aufgaben und Probleme delegieren, die vor dem Beginn der Delegation noch nicht abgeschlossen sind.
* Wenn ein Arbeitselement während des Zeitrahmens der Delegierung abgeschlossen wird, bleibt der Punkt im Home-Bereich des Delegierten und des Bevollmächtigten zwei Wochen vor [!DNL Workfront] entfernt sie automatisch.
* Die Benutzer, die Sie als Delegierte auswählen, erhalten dieselben Berechtigungen wie Ihre Berechtigungen für die Aufgaben und Probleme, die Sie ihnen zuweisen. Die Berechtigungen müssen innerhalb ihrer Zugriffsstufen funktionieren, und manchmal können ihre Zugriffsebenen niedriger sein als Ihre.

>[!NOTE]
>
>  Bei Elementen, die zugewiesen werden, nachdem die Zuweisung der Zuweisung bereits begonnen hat, kann es bis zu eine Stunde dauern, bis das Element zugewiesen wurde für [!DNL Workfront] , um die neu zugewiesenen Elemente für den Delegaten freizugeben.

* Wenn Ihnen während der ausgewählten Zeit zusätzliche Aufgaben und Probleme zugewiesen werden, damit Ihre Arbeit anderen Benutzern zugewiesen werden kann, wird die neu zugewiesene Arbeit automatisch an dieselbe Person für den ausgewählten Zeitraum delegiert, wenn die Aufgabe oder das Ausgabedatum innerhalb dieses Zeitrahmens liegt.
* Derselbe Benutzer kann von mehreren Benutzern als Delegate ausgewählt werden.
* Delegierte Aufgaben und Probleme werden nicht in Tools zur Ressourcenverwaltung angezeigt, wie z. B. [!UICONTROL Lastenausgleich] oder [!UICONTROL Ressourcenplaner] für die delegierten Benutzer.
* Sie können delegierte Arbeiten und Delegationsnamen in verschiedenen Bereichen von [!DNL Workfront]. Weitere Informationen finden Sie im Abschnitt &quot;Delegierte Arbeit lokalisieren und Informationen delegieren&quot;im Artikel [Verwalten der Zuweisung von Aufgaben und Ausgaben](../delegate-work/how-to-delegate-work.md).


   >[!IMPORTANT]
   >
   >  Wenn ein Benutzer nur Zugriff auf Aufgaben in ihrer Zugriffsstufe anzeigen hat und Sie über Verwaltungsberechtigungen für die Aufgaben verfügen, die Sie ihm zuweisen, erhält er Verwaltungsberechtigungen für die Aufgaben, die Sie ihm zuweisen. Sie können jedoch nicht dieselben Aktionen wie Sie für die delegierten Aufgaben durchführen. Sie müssen vom Systemadministrator Zugriff auf Aufgaben bearbeiten anfordern, um in Ihrer Abwesenheit Aufgaben aktualisieren zu können.

* Durch das Beenden der Zuweisung werden die den delegierten Benutzern erteilten Berechtigungen für die Aufgaben und Probleme, für die sie delegiert wurden, nicht entfernt.
* Wenn ein System oder das [!UICONTROL Delegieren von Aufgaben und Problemen durch Benutzer zulassen] -Einstellung in [!UICONTROL Einrichtung] -Bereich, werden die derzeit zugewiesenen Benutzer aus den Aufgaben und Problemen entfernt, denen sie zuvor zugewiesen wurden. Ihre Berechtigungen für die Aufgaben oder Probleme werden nicht entfernt.

## Unterschiede und Ähnlichkeiten zwischen Zuweisungen und Delegationen

| Aktion | Arbeitsaufträge | Delegierungen |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Ein zugewiesener oder delegierter Benutzer kann das Arbeitselement, dem er zugewiesen oder zugewiesen wurde, bearbeiten oder löschen | Basierend auf Berechtigungen und Zugriffsebene | Basierend auf Berechtigungen und Zugriffsebene |
| Ein zugewiesener oder delegierter Benutzer wird in der Kopfzeile des Arbeitselements angezeigt | Ja | Ja |
| Die zugewiesenen oder zugewiesenen Aufgaben oder Probleme werden im Home-Bereich des Verantwortlichen oder Delegierten angezeigt | Ja, bis das Element abgeschlossen ist | Ja, nur für den Zeitrahmen der Delegation |
| Sie können Benutzer über den Startbereich Aufgaben zuweisen oder delegieren | Ja | Ja |
| Sie können Benutzern mithilfe der | Ja | Nein |
| Sie können Benutzern in einer Liste oder in der Kopfzeile eines Arbeitselements Arbeit zuweisen oder zuweisen. | Ja | Nein |
| Jeder Benutzer kann anderen Benutzern Arbeitselemente zuweisen oder zuweisen, mit denen sie nicht verknüpft sind | Basierend auf Berechtigungen und Zugriffsebene | Nein. Nur der Bevollmächtigte kann seine eigenen Elemente delegieren. |
| Geplante, tatsächliche oder budgetierte Stunden für die einem Benutzer zugewiesene oder zugewiesene Arbeit, die für diesen Benutzer in Tools zur Ressourcenverwaltung angezeigt wird | Ja | Nein |
