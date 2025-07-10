---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Erstellen einer Untergruppe
description: Sie können eine Untergruppe unter einer Gruppe erstellen, die Sie verwalten, um Benutzende und Projekte zu organisieren und Zugriffsrechte innerhalb von Adobe Workfront zuzuweisen. In der Regel verwalten Gruppenadministratoren Gruppen und Untergruppen. Sie können die Seite Gruppen verwenden, um ihre Gruppen und Untergruppen an einem Ort zu verwalten.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: 008f96d52632f5f05554d63ae1c38cc37d21544b
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 0%

---

# Erstellen einer Untergruppe

Sie können eine Untergruppe unter einer Gruppe erstellen, die Sie verwalten, um Benutzende und Projekte zu organisieren und Zugriffsrechte innerhalb von Adobe Workfront zuzuweisen.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

In der Regel verwalten Gruppenadministratoren jedoch Gruppen und Untergruppen. Sie können die Seite Gruppen verwenden, um ihre Gruppen und Untergruppen an einem Ort zu verwalten. Informationen zur Funktionsweise von Gruppen und Untergruppen in Workfront finden Sie unter [Gruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md) und [Untergruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen einer Untergruppe

{{step-1-to-setup}}

1. Klicken Sie **Gruppen**.

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Wählen Sie die bestehende Gruppe oder Untergruppe aus, der/der Sie eine neue Untergruppe hinzufügen möchten.
1. Klicken Sie **Neue Untergruppe**.
1. Geben Sie in das **Neue Untergruppe** angezeigte Feld einen **Gruppennamen** für die Untergruppe ein.
1. (Optional) Geben Sie eine der folgenden Informationen ein:

   * **Beschreibung**: Geben Sie eine Beschreibung für die Untergruppe ein. Sie können bis zu 512 Zeichen eingeben.
   * **Ist Aktiv**: Diese Option ist standardmäßig aktiviert und macht die Gruppe in Ihrer Workfront-Instanz aktiv.

     Wenn in Feldern mit automatischer Textvervollständigung wie dem unten gezeigten reguläre Benutzer nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder ein Objekt für sie freizugeben, werden in der Liste nur aktive Gruppen angezeigt.

     ![Typeahead-Feld für eine Gruppe](assets/typeahead-for-group.png)

     Um dies für Ihre Benutzer zu optimieren, können Sie die Option **Ist aktiv** für Gruppen deaktivieren, die derzeit nicht verwendet werden.

     In diesem Feld können Sie die Gruppenliste einfach nach dem Status Aktiv oder Inaktiv anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter [Berichterstellungselemente: Filter, Ansichten und Gruppierungen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   * **Business Leader**: Sie können einen Benutzer als Business Leader für eine von Ihnen verwaltete Untergruppe zuweisen. Ein Business Leader ist jemand, der geschäftliche Entscheidungen für die Untergruppe trifft. Weitere Informationen finden Sie unter [Business Leader - Übersicht](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

     Wenn die Person nicht bereits Mitglied der Untergruppe ist, werden sie durch Hinzufügen ihres Namens zu diesem Feld auch zur Gruppe hinzugefügt.

     >[!NOTE]
     >
     >* Bevor Sie einen Business Leader aus einer Untergruppe entfernen können, müssen Sie dessen Namen aus dem Feld Business Leader entfernen.
     >* Wenn Sie den Namen aus dem Feld „Business Leader“ entfernen, bleibt dieser Benutzer Mitglied der Untergruppe, es sei denn, Sie entfernen ihn daraus. Anweisungen zum Entfernen einer Person aus einer Gruppe finden Sie unter [Anzeigen und Verwalten der Gruppenmitgliedschaften](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

   * **Gruppenmitglieder und Gruppenadministratoren**: Um Benutzer und Gruppen als Mitglieder der Untergruppe hinzuzufügen, beginnen Sie mit der Eingabe des Namens eines vorhandenen Benutzers oder einer vorhandenen Gruppe, den/die Sie hinzufügen möchten, und wählen Sie dann den Namen aus, wenn er angezeigt wird.

     Die Benutzer und Gruppen, die Sie hinzufügen, haben Zugriff auf alle Objekte, die für die Gruppe freigegeben sind.

     Eine Untergruppe übernimmt die Gruppenadministratoren der darüber liegenden Gruppe. Die Angabe eines Benutzers als Gruppenadministrator für eine Untergruppe ist daher optional. Über das Dropdown-Menü rechts neben dem Benutzernamen können Sie ein Gruppenmitglied als Administrator für die Gruppe zuweisen.

   * **Personen und Gruppen in der Liste suchen**: Wenn Sie einen Benutzer oder eine Gruppe suchen müssen, der bzw. die dieser Untergruppe bereits zugewiesen ist, können Sie seinen Namen hier eingeben und ihn/sie auswählen, wenn er/sie angezeigt wird.

1. Klicken Sie auf **Speichern.**
