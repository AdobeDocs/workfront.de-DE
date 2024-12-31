---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Einrichten von Wechselkursen
description: Als Adobe Workfront-Administrator können Sie in Workfront Wechselkurse einrichten.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '533'
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

Wechselkurse wirken sich auf alle Finanzelemente in Workfront aus. Die Basiswährung ist die Standardwährung für alle Projekte im gesamten System, es sei denn, sie wird für ein bestimmtes Projekt oder Aufgabengebiet überschrieben. Sie können auch festlegen, dass Finanzinformationen in Währungen angezeigt werden sollen, die in Ihrem System verfügbar sind und sich von der Basiswährung oder der des Projekts unterscheiden, wenn Sie sie in einem Bericht oder einer Liste anzeigen. Weitere Informationen finden Sie unter [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

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

1. Klicken Sie **Projektvoreinstellungen** > **Wechselkurse.**

1. Klicken Sie **Währung hinzufügen.**
1. Geben Sie den Namen der Währung ein und klicken Sie dann auf die Währung, wenn sie in der Dropdown-Liste angezeigt wird.

1. Geben Sie im bereitgestellten Feld den Kurs für die von Ihnen ausgewählte Währung an, da dieser sich auf die Währung bezieht, die im System als Basiswährung festgelegt ist.
1. (Optional) Legen Sie die Währung als Basiswährung (Standard) für Workfront fest.

   Dies ist die Währung, die als Standard für alle Projekte und Berichte im System verwendet wird.

1. Klicken Sie **Speichern**, um Ihre Änderungen zu speichern.

## Benutzern ermöglichen, die Standardwährung für ein Projekt zu ändern

Benutzer können die Standardwährung für ein Projekt ändern, wenn die folgenden Bedingungen erfüllt sind:

* Der Benutzer verfügt über eine Planlizenz mit administrativem Zugriff auf Wechselkurse.

  Weitere Informationen finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Auf dem Workfront-System ist mehr als eine Währung aktiviert.

Informationen dazu, wie Benutzer die Standardwährung für ein bestimmtes Projekt ändern können, finden Sie unter [Ändern der ](../../../manage-work/projects/project-finances/change-project-currency.md).

## Benutzern ermöglichen, die Standardwährung für ein Aufgabengebiet zu ändern

Benutzer können die Währung für ein Aufgabengebiet ändern, wenn die folgenden Bedingungen erfüllt sind:

* Der Benutzer verfügt über eine Planlizenz mit administrativem Zugriff auf Aufgabengebiete.

  Weitere Informationen finden Sie unter [Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Im Workfront-System sind mehrere Währungen aktiviert.

Informationen dazu, wie Benutzer die Standardwährung für ein bestimmtes Aufgabengebiet ändern können, finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
