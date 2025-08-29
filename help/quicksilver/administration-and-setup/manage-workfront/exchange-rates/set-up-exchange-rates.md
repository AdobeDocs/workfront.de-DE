---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Einrichten von Wechselkursen
description: Wechselkurse wirken sich auf alle Finanzelemente in Workfront aus. Die Basiswährung ist die Standardwährung für alle Projekte im System.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc820b4012fec494ce5ebb1baefb4ee0df214916
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 2%

---

# Einrichten von Wechselkursen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Als Adobe Workfront-Administrator können Sie in Workfront Wechselkurse einrichten. Dazu gehört Folgendes:

* Festlegen der Standardwährung für das Workfront-System
* Wechselkurse in Workfront werden entsprechend den aktuellen Wechselkursen aktualisiert
* Konfigurieren der Wechselkurse für mehrere Währungen (dadurch können Benutzer eine Standardwährung für einzelne Projekte auswählen)

Wechselkurse wirken sich auf alle Finanzelemente in Workfront aus. Die Basiswährung ist die Standardwährung für alle Projekte im gesamten System, es sei denn, sie wird für ein bestimmtes Projekt oder Aufgabengebiet überschrieben. Die aktuelle Basis- oder Standardwährung wird in der Liste mit einem Symbol ![Standardwährungssymbol](assets/default-icon.png) gekennzeichnet. Sie können auch festlegen, dass Finanzinformationen in Währungen angezeigt werden sollen, die in Ihrem System verfügbar sind und sich von der Basiswährung oder der des Projekts unterscheiden, wenn Sie sie in einem Bericht oder einer Liste anzeigen. Weitere Informationen finden Sie unter [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Weitere Informationen zum Überschreiben der Basiswährung in Workfront für Projekte und Aufgabengebiete finden Sie in den folgenden Artikeln:

* [Ändern der Projektwährung](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

Die Art und Weise, wie Sie Wechselkurse einrichten, wirkt sich darauf aus, ob die Benutzer die Wechselkurse für ein bestimmtes Projekt ändern können.

>[!IMPORTANT]
>
>Wechselkurse in Workfront sind nicht dynamisch. Der von Ihnen festgelegte Wert muss aktualisiert werden, wenn Wechselkursänderungen auftreten.

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
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einrichten von Wechselkursen

{{step-1-to-setup}}

1. Klicken Sie **Projektvoreinstellungen** > **Wechselkurse**.

1. Klicken Sie **Währung hinzufügen**.
1. Beginnen Sie im Feld **Währung hinzufügen** mit der Eingabe des Namens der Währung, und klicken Sie dann auf sie, wenn sie in der Dropdown-Liste angezeigt wird.
1. Geben **im Feld** den Kurs für die gewählte Währung ein, verglichen mit der Währung, die im System als Basiswährung festgelegt ist.
1. Klicken Sie **Hinzufügen**, um die neue Währung und deren Wechselkurs hinzuzufügen.
1. (Optional) Führen Sie einen der folgenden Schritte aus, um die Basiswährung (Standard) zu ändern:

   * Aktivieren Sie das Kontrollkästchen neben dem Währungsnamen und wählen Sie **Standard festlegen** in der Aktionsleiste am unteren Bildschirmrand aus.
   * Bewegen Sie den Mauszeiger über den Währungsnamen und klicken Sie auf das **** Mehr. Wählen Sie dann **Als Standard festlegen** aus.

     Die neue Standardwährung wird mit dem Symbol aktualisiert.

     >[!NOTE]
     >
     >Die Standardwährung wird immer zuerst in der Liste angezeigt, unabhängig davon, wie die Liste sortiert ist.

1. (Optional) Um eine Währung zu löschen, aktivieren Sie das Kontrollkästchen neben dem Währungsnamen und wählen **Löschen** in der Aktionsleiste am unteren Bildschirmrand. Die Standardwährung kann nicht gelöscht werden.

## Benutzern ermöglichen, die Standardwährung für ein Projekt zu ändern

Benutzer können die Standardwährung für ein Projekt ändern, wenn die folgenden Bedingungen erfüllt sind:

* Der Benutzer verfügt über eine Standard- oder Planlizenz mit administrativem Zugriff auf Wechselkurse.

  Weitere Informationen finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Auf dem Workfront-System ist mehr als eine Währung aktiviert.

Informationen dazu, wie Benutzer die Standardwährung für ein bestimmtes Projekt ändern können, finden Sie unter [Ändern der ](../../../manage-work/projects/project-finances/change-project-currency.md).

## Benutzern ermöglichen, die Standardwährung für ein Aufgabengebiet zu ändern

Benutzer können die Währung für ein Aufgabengebiet ändern, wenn die folgenden Bedingungen erfüllt sind:

* Der Benutzer verfügt über eine Standard- oder Planlizenz mit administrativem Zugriff auf Aufgabengebiete.

  Weitere Informationen finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Im Workfront-System sind mehrere Währungen aktiviert.

Informationen dazu, wie Benutzer die Standardwährung für ein bestimmtes Aufgabengebiet ändern können, finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).


<!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->
