---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Delegieren von Arbeit - Übersicht
description: Wenn Sie planen, für kurze Zeit abwesend zu sein, können Sie Ihre Arbeit vorübergehend an andere Benutzer delegieren, um sicherzustellen, dass Ihre Abwesenheit nicht zu einer Hürde für die Fertigstellung der Arbeit wird.
author: Becky
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/O-G3HS2JWZB36Y-kSloHo6u4--Z3q40fwAgfcEuELi4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: c33d85a1-be85-4290-854c-87408c10aa80
  - id: d1573eb8-a2e8-4a06-9526-9c3410bf4914
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 906
ht-degree: 2%

---

# Delegieren von Arbeit - Übersicht

Wenn Sie planen, für kurze Zeit abwesend zu sein, können Sie Ihre Arbeit vorübergehend an andere Benutzer delegieren, um sicherzustellen, dass Ihre Abwesenheit nicht zu einer Hürde für die Fertigstellung der Arbeit wird.

Wenn beispielsweise bestimmte Aufgaben fällig sind, bevor Sie zurückkehren, Sie aber nicht die Zeit haben, sie vor Ihrer Abreise abzuschließen, können Sie Ihre Aufgaben an einen anderen Benutzer delegieren, damit er sie rechtzeitig abschließen kann, und den Abschluss des Projekts nicht bis nach Ihrer Rückkehr verzögern.

Sie können die folgenden Objekte in [!DNL Adobe Workfront] delegieren:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Ihnen zugewiesene Aufgaben
* Ihnen zugewiesene Anfragen
* Ihnen zugewiesene Genehmigungen für Projekte, Aufgaben oder Probleme.

  >[!TIP]
  >
  >   Sie können keine Genehmigungen für Arbeitszeittabellen, Dokumente oder Korrekturabzüge delegieren.


Dieser Artikel enthält allgemeine Informationen zum Delegieren von Aufgaben und Problemen, die Ihnen zugewiesen wurden.

Informationen zum Delegieren von Projekt-, Aufgaben- und Problem-Genehmigungen finden Sie unter [Genehmigungsanforderung delegieren](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Informationen zum Delegieren von Aufgaben und Problemen finden Sie unter [Delegieren von Aufgaben und Problemen](../../manage-work/delegate-work/how-to-delegate-work.md).

## Überblick über das Delegieren von Aufgaben und Problemen

Beachten Sie beim Delegieren von Aufgaben und Problemen Folgendes:

* Ihr [!DNL Workfront]- oder Gruppenadministrator muss die Voreinstellungen für die Delegierung im Bereich [!UICONTROL Setup] aktivieren, bevor Sie Ihre Arbeit an andere delegieren können.

  Weitere Informationen finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemvoreinstellungen](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

* Sie können Aufgaben und Probleme nur über den Bereich &quot;[!UICONTROL &quot; &#x200B;].
* Beim Delegieren von Arbeit gibt es Ausnahmen für die folgenden Lizenztypen:

   * Sie können Arbeit an Prüfer oder Auftraggeber delegieren, obwohl [!DNL Workfront] dies nicht empfiehlt.
   * Reviewer können ihre Arbeit an Dritte delegieren. Sie können Arbeitselemente nicht in ihrem [!UICONTROL Home]Bereich anzeigen. Sie können nur Genehmigungen anzeigen.
   * Auftraggeber können keine Arbeit an Dritte delegieren. Sie können Arbeitselemente nicht in ihrem [!UICONTROL Home]Bereich anzeigen
* Sie können nur die Ihnen zugewiesenen Aufgaben und Probleme delegieren. Sie können keine Aufgaben und Probleme delegieren, die anderen Benutzern, Teams oder Aufgabengebieten zugewiesen sind.
* Sie können nur Aufgaben und Probleme delegieren, die nicht vor dem Startdatum der Delegierung abgeschlossen wurden.
* Wenn ein Arbeitselement während des Zeitrahmens der Delegierung abgeschlossen wird, bleibt das Element für 2 Wochen im Home-Bereich des Beauftragten und des Verantwortlichen, bevor [!DNL Workfront] es automatisch entfernt.
* Die Benutzer, die Sie als Delegierte auswählen, erhalten dieselben Berechtigungen wie Ihre Berechtigungen für die Aufgaben und Probleme, die Sie an sie delegieren. Die Berechtigungen müssen innerhalb ihrer Zugriffsebenen funktionieren, und manchmal können ihre Zugriffsebenen niedriger sein als Ihre.

>[!NOTE]
>
>  Bei Elementen, die zugewiesen werden, nachdem die Delegierung bereits gestartet wurde, kann es bis zu einer Stunde dauern, nachdem das Element für [!DNL Workfront] zugewiesen wurde, um die neu zugewiesenen Elemente für den Beauftragten freizugeben.

* Wenn Ihnen in dem Zeitraum, den Sie für die Delegierung Ihrer Arbeit an andere Benutzer ausgewählt haben, zusätzliche Aufgaben und Probleme zugewiesen werden, wird die neu zugewiesene Arbeit automatisch derselben Person für den von Ihnen ausgewählten Zeitraum zugewiesen, wenn die Aufgaben- oder Problemdaten innerhalb dieses Zeitraums liegen.
* Derselbe Benutzer kann von mehreren Benutzern als Vertreter ausgewählt werden.
* Delegierte Aufgaben und Probleme werden in Ressourcen-Management-Tools wie dem [!UICONTROL Workload Balancer] oder dem [!UICONTROL Ressourcenplaner] für die delegierten Benutzer nicht angezeigt.
* Delegierte Arbeiten und Delegatennamen können in verschiedenen [!DNL Workfront] angezeigt werden. Weitere Informationen finden Sie im Abschnitt „Suchen von delegierten Arbeiten und Delegieren von Informationen“ im Artikel [Delegieren von Aufgaben und Problemen](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Wenn ein(e) Benutzende(r) nur Lesezugriff auf Aufgaben in seiner/ihrer Zugriffsebene hat und Sie Verwaltungsberechtigungen für die Aufgaben haben, die Sie an ihn/sie delegieren, erhalten er/sie Verwaltungsberechtigungen für die Aufgaben, die Sie an ihn/sie delegieren. Sie können jedoch nicht dieselben Aktionen wie Sie für die delegierten Aufgaben ausführen. Sie müssen Bearbeitungszugriff auf Aufgaben vom Systemadministrator anfordern, damit er die Aufgaben in Ihrer Abwesenheit aktualisieren kann.

* Durch das Beenden der Delegierung werden die den delegierten Benutzern erteilten Berechtigungen für die Aufgaben und Probleme, für die sie delegiert wurden, nicht entfernt.
* Wenn ein System oder die Einstellung [!UICONTROL Erlauben Sie Benutzern, ihre Aufgaben und Probleme zu delegieren] im Bereich [!UICONTROL Setup] deaktiviert, werden die aktuell delegierten Benutzer aus den Aufgaben und Problemen entfernt, an die sie zuvor delegiert wurden. Ihre Berechtigungen für die Aufgaben oder Probleme werden nicht entfernt.

## Unterschiede und Ähnlichkeiten zwischen Zuweisungen und Zuweisungen

| Aktion | Arbeitsaufträge | Delegierungen |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Ein zugewiesener oder delegierter Benutzer kann das Arbeitselement, dem er zugewiesen oder zugewiesen wurde, bearbeiten oder löschen | Basierend auf Berechtigungen und Zugriffsebene | Basierend auf Berechtigungen und Zugriffsebene |
| Ein zugewiesener oder delegierter Benutzer wird in der Kopfzeile des Arbeitselements angezeigt | Ja | Ja |
| Die zugewiesenen oder delegierten Aufgaben oder Probleme werden im Bereich Startseite des Verantwortlichen oder des Beauftragten angezeigt | Ja, bis das Element abgeschlossen ist | Ja, nur für den Zeitrahmen der Delegierung |
| Sie können Benutzern im Bereich Startseite Arbeit zuweisen oder delegieren | Ja | Ja |
| Mit dem Workload-Balancer können Sie Benutzern Arbeit zuweisen oder delegieren | Ja | Nein |
| Sie können Benutzern in einer Liste oder in der Kopfzeile eines Arbeitselements Arbeit zuweisen oder delegieren | Ja | Nein |
| Jeder Benutzer kann anderen Benutzern Arbeitselemente zuweisen oder delegieren, mit denen er nicht verknüpft ist | Basierend auf Berechtigungen und Zugriffsebene | Nein. Nur der Beauftragte kann seine eigenen Elemente delegieren. |
| Geplante, tatsächliche oder budgetierte Stunden für Arbeit, die einem/r Benutzenden zugewiesen oder delegiert wurde, werden für diesen/n Benutzenden in Ressourcen-Management-Tools angezeigt | Ja | Nein |
