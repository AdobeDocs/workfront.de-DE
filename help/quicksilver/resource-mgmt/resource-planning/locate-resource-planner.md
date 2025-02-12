---
product-area: resource-management
navigation-topic: resource-planning
title: Suchen des Ressourcenplaners
description: Sie können den Ressourcenplaner verwenden, um die Zuordnung Ihrer Ressourcen zu Projekten zu verwalten. Sie können über den Business Case des Projekts auf den Ressourcenplaner für mehrere Projekte gleichzeitig oder für ein Projekt zugreifen.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: a3b2ac192e1f37e0c3d16d059ed96e8d5cadf8be
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 0%

---

# Suchen des Ressourcenplaners

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Sie können den Ressourcenplaner verwenden, um die Zuordnung Ihrer Ressourcen zu Projekten zu verwalten. Sie können über den Business Case des Projekts auf den Ressourcenplaner für mehrere Projekte gleichzeitig oder für ein Projekt zugreifen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Licht oder höher;</br>
          Standard, um den Ressourcenplaner im Hauptmenü zu finden</p>
       <p>oder</p>
       <p>Aktuell: Überprüfung oder höher;</br>
       Den Ressourcenplaner im Hauptmenü finden</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen des Zugriffs auf das Ressourcenmanagement oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für Projekte und Benutzer </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Stellen Sie sicher, dass alle Voraussetzungen für den Zugriff auf und die Arbeit mit dem Ressourcenplaner erfüllt sind, bevor Sie ihn verwenden. Auf diese Weise stellen Sie sicher, dass der Ressourcenplaner die richtigen Informationen anzeigt, bevor Sie mit der Budgetierung Ihrer Ressourcen beginnen.

Informationen zu den Voraussetzungen für den Ressourcenplaner finden Sie unter [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Suchen des Ressourcenplaners

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Sie können den Ressourcenplaner in zwei Bereichen von Workfront platzieren, je nachdem, ob Sie Ihre Ressourcen für mehrere Projekte oder nur für ein Projekt budgetieren möchten.

* [Verwenden Sie den Ressourcenplaner für mehrere Projekte](#use-the-resource-planner-for-multiple-projects)
* [Verwenden des Ressourcenplaners für ein Projekt](#use-the-resource-planner-for-one-project)

### Verwenden des Ressourcenplaners für mehrere Projekte {#use-the-resource-planner-for-multiple-projects}

Wenn Sie den Ressourcenplaner für mehrere Projekte verwenden, stellen die Zuordnungsnummern für Ihre Ressourcen Zahlen über mehrere Projekte hinweg dar.

So greifen Sie auf den Bereich „Planer“ im Bereich „Ressourcen“ zu:

{{step1-to-resourcing}}

Der Planer wird standardmäßig angezeigt.  Informationen zur Budgetierung von Ressourcen im Ressourcenplaner finden Sie im Artikel [Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Aufgabenansichten](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![Ressourcenplaner als Standard](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Klicken Sie **linken Bedienfeld**Ressourcenpools“.
Informationen zum Erstellen von Ressourcenpools finden Sie unter [Ressourcenpools erstellen](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Verwenden des Ressourcenplaners für ein Projekt {#use-the-resource-planner-for-one-project}

Wenn Sie den Ressourcenplaner für ein Projekt verwenden, stellen die Zuordnungsnummern für Ihre Ressourcen Zahlen für das ausgewählte Projekt dar.

1. Zu einem Projekt gehen, für das Ressourcen budgetiert werden sollen.
1. Klicken Sie **linken Bedienfeld** Business Case“.
1. Scrollen Sie zum Abschnitt **Ressourcenbudgetierung** des Business-Case.
1. Klicken Sie **Ressourcenbudgetierung bearbeiten**, um Ressourcenpools zu Ihrem Projekt hinzuzufügen und mit der Budgetierung Ihrer Ressourcen zu beginnen.

   >[!TIP]
   >
   >Sie können einen Ressourcenpool im Bereich Ressourcenbudgetierung des Business Case nur hinzufügen, wenn dem Projekt keine Ressourcenpools zugeordnet sind. Wenn das Projekt bereits über einen Ressourcenpool verfügt, werden die Benutzer im Pool und ihre Aufgabengebiete standardmäßig im Bereich Ressourcenbudgetierung angezeigt.

   ![Ressourcenbudgetierung](assets/resource-budgeting-area-on-project-350x70.png)

   Informationen zur Budgetierung von Ressourcen für ein Projekt finden Sie im Artikel [Budgetressourcen im Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
