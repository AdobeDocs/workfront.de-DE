---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Delegieren von Arbeiten - Übersicht
description: Wenn Sie planen, für kurze Zeit abwesend zu sein, können Sie Ihre Arbeit vorübergehend an andere Benutzer delegieren, um sicherzustellen, dass Ihre Abwesenheit nicht zu einem Hindernis für die Fertigstellung der Arbeit wird.
author: Lisa
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 1%

---

# Delegieren von Arbeiten - Übersicht

Wenn Sie planen, für kurze Zeit abwesend zu sein, können Sie Ihre Arbeit vorübergehend an andere Benutzer delegieren, um sicherzustellen, dass Ihre Abwesenheit nicht zu einem Hindernis für die Fertigstellung der Arbeit wird.

Wenn beispielsweise bestimmte Aufgaben vor der Rückkehr fällig sind, Sie jedoch keine Zeit haben, sie vor dem Verlassen abzuschließen, können Sie Ihre Aufgaben an einen anderen Benutzer delegieren, damit dieser sie rechtzeitig abschließen und den Abschluss des Projekts nicht bis nach der Rückkehr verzögern kann.

Sie können die folgenden Objekte in [!DNL Adobe Workfront] zuweisen:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Ihnen zugewiesene Aufgaben
* Ihnen zugewiesene Probleme
* Ihnen zugewiesene Projekt-, Aufgaben- oder Problemgenehmigungen.

  >[!TIP]
  >
  >   Sie können keine Zeitblatt-, Dokument- oder Testversandgenehmigungen delegieren.


Dieser Artikel enthält allgemeine Informationen zum Delegieren von Aufgaben und Problemen, die Ihnen zugewiesen sind.

Informationen zum Delegieren von Projekt-, Aufgaben- und Problemgenehmigungen finden Sie unter [Genehmigungsanfrage delegieren](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Informationen zum Delegieren von Aufgaben und Problemen finden Sie unter [Aufgaben und Probleme delegieren](../../manage-work/delegate-work/how-to-delegate-work.md).

## Delegieren von Aufgaben und Problemen - Übersicht

Beachten Sie Folgendes, wenn Sie Aufgaben und Probleme delegieren:

* Ihr [!DNL Workfront]- oder Gruppenadministrator muss die Delegationsvoreinstellungen im Bereich [!UICONTROL Einrichtung] aktivieren, bevor Sie Ihre Arbeit an andere delegieren können.

  Weitere Informationen finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Sie können Aufgaben und Probleme nur über den Bereich [!UICONTROL Home] delegieren.
* Für die folgenden Lizenztypen gibt es Ausnahmen:

   * Sie können Arbeiten an Überprüfer oder Anforderer delegieren, obwohl [!DNL Workfront] dies nicht empfiehlt.
   * Überprüfer können Arbeiten an andere delegieren. Arbeitselemente können nicht in ihrem Bereich [!UICONTROL Home] angezeigt werden. Sie können nur Genehmigungen anzeigen.
   * Antragsteller können keine Arbeit an andere delegieren. Arbeitselemente können nicht in ihrem [!UICONTROL Home] -Bereich angezeigt werden
* Sie können nur die Ihnen zugewiesenen Aufgaben und Probleme delegieren. Sie können keine Aufgaben und Probleme delegieren, die anderen Benutzern, Teams oder Auftragsrollen zugewiesen sind.
* Sie können nur Aufgaben und Probleme delegieren, die vor dem Beginn der Delegation noch nicht abgeschlossen sind.
* Wenn ein Arbeitselement während des Zeitrahmens der Zuweisung abgeschlossen wird, bleibt das Element im Home-Bereich des Delegierten und des Verantwortlichen 2 Wochen lang, bevor [!DNL Workfront] es automatisch entfernt.
* Die Benutzer, die Sie als Delegierte auswählen, erhalten dieselben Berechtigungen wie Ihre Berechtigungen für die Aufgaben und Probleme, die Sie ihnen zuweisen. Die Berechtigungen müssen innerhalb ihrer Zugriffsstufen funktionieren, und manchmal können ihre Zugriffsebenen niedriger sein als Ihre.

>[!NOTE]
>
>  Bei Elementen, die zugewiesen werden, nachdem die Zuweisung bereits begonnen hat, kann es bis zu eine Stunde dauern, bis das Element für [!DNL Workfront] zugewiesen wurde, um die neu zugewiesenen Elemente für den Delegaten freizugeben.

* Wenn Ihnen während der ausgewählten Zeit zusätzliche Aufgaben und Probleme zugewiesen werden, damit Ihre Arbeit anderen Benutzern zugewiesen werden kann, wird die neu zugewiesene Arbeit automatisch an dieselbe Person für den ausgewählten Zeitraum delegiert, wenn die Aufgabe oder das Ausgabedatum innerhalb dieses Zeitrahmens liegt.
* Derselbe Benutzer kann von mehreren Benutzern als Delegate ausgewählt werden.
* Delegierte Aufgaben und Probleme werden nicht in den Tools zur Ressourcenverwaltung angezeigt, wie z. B. der [!UICONTROL Lastenausgleich] oder der [!UICONTROL Ressourcenplaner] für die delegierten Benutzer.
* Sie können delegierte Arbeiten und Delegationsnamen in mehreren Bereichen von [!DNL Workfront] anzeigen. Weitere Informationen finden Sie im Abschnitt &quot;Lokalisieren von delegierten Arbeiten und Delegierungsinformationen&quot;im Artikel [Delegieren von Aufgaben und Problemen](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Wenn ein Benutzer nur Zugriff auf Aufgaben in ihrer Zugriffsstufe anzeigen hat und Sie über Verwaltungsberechtigungen für die Aufgaben verfügen, die Sie ihm zuweisen, erhält er Verwaltungsberechtigungen für die Aufgaben, die Sie ihm zuweisen. Sie können jedoch nicht dieselben Aktionen wie Sie für die delegierten Aufgaben durchführen. Sie müssen vom Systemadministrator Zugriff auf Aufgaben bearbeiten anfordern, um in Ihrer Abwesenheit Aufgaben aktualisieren zu können.

* Durch das Beenden der Zuweisung werden die den delegierten Benutzern erteilten Berechtigungen für die Aufgaben und Probleme, für die sie delegiert wurden, nicht entfernt.
* Wenn ein System oder die Einstellung [!UICONTROL Benutzern erlauben, ihre Aufgaben und Probleme zu delegieren] im Bereich [!UICONTROL Einrichtung] deaktiviert, werden die derzeit zugewiesenen Benutzer aus den Aufgaben und Problemen entfernt, denen sie zuvor zugewiesen wurden. Ihre Berechtigungen für die Aufgaben oder Probleme werden nicht entfernt.

## Unterschiede und Ähnlichkeiten zwischen Zuweisungen und Delegationen

| Aktion | Arbeitsaufträge | Delegierungen |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Ein zugewiesener oder delegierter Benutzer kann das Arbeitselement, dem er zugewiesen oder zugewiesen wurde, bearbeiten oder löschen | Basierend auf Berechtigungen und Zugriffsebene | Basierend auf Berechtigungen und Zugriffsebene |
| Ein zugewiesener oder delegierter Benutzer wird in der Kopfzeile des Arbeitselements angezeigt | Ja | Ja |
| Die zugewiesenen oder zugewiesenen Aufgaben oder Probleme werden im Home-Bereich des Verantwortlichen oder Delegierten angezeigt | Ja, bis das Element abgeschlossen ist | Ja, nur für den Zeitrahmen der Delegation |
| Sie können Benutzer über den Startbereich Arbeitsaufgaben zuweisen oder delegieren | Ja | Ja |
| Sie können Benutzern mithilfe der | Ja | Nein |
| Sie können Benutzern in einer Liste oder in der Kopfzeile eines Arbeitselements Arbeit zuweisen oder zuweisen. | Ja | Nein |
| Jeder Benutzer kann anderen Benutzern Arbeitselemente zuweisen oder zuweisen, mit denen sie nicht verknüpft sind | Basierend auf Berechtigungen und Zugriffsebene | Nein. Nur der Bevollmächtigte kann seine eigenen Elemente delegieren. |
| Geplante, tatsächliche oder budgetierte Stunden für die einem Benutzer zugewiesene oder zugewiesene Arbeit, die für diesen Benutzer in Tools zur Ressourcenverwaltung angezeigt wird | Ja | Nein |
