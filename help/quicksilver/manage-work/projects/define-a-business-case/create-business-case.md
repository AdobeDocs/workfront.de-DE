---
navigation-topic: business-case-and-scorecards
title: Erstellen eines Business Case für ein Projekt
description: Sie können den Business Case verwenden, um ein Projekt anzufordern und den Zweck, das Budget und den potenziellen Nutzen für das Projekt zu definieren. Der Portfolio-Manager oder Projektsponsor verwendet die Informationen aus dem Business Case, um das Projekt zu analysieren und zu priorisieren, bevor es genehmigt wird.
author: Alina
feature: Work Management
exl-id: db69b3bf-04e3-49b4-ae0d-ab6145389db5
source-git-commit: fedb0328450896d212081715df4cde7644b169bc
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 0%

---

# Erstellen eines Business Case für ein Projekt

Sie können den Business Case verwenden, um ein Projekt anzufordern und den Zweck, das Budget und den potenziellen Nutzen für das Projekt zu definieren. Der Portfolio-Manager oder Projektsponsor verwendet die Informationen aus dem Business Case, um das Projekt zu analysieren und zu priorisieren, bevor es genehmigt wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Plan oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte, Finanzdaten und Ressourcenmanagement bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von oder höheren Berechtigungen für das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Beachten Sie Folgendes, wenn Sie ein Projekt über einen Business Case anfordern:

* Ihr Adobe Workfront-Administrator oder Gruppenadministrator muss die Abschnitte des Business Case aktivieren, bevor sie in Ihrem Projekt angezeigt werden.\
  Informationen zur Aktivierung der Abschnitte im Business Case auf Systemebene finden Sie im Artikel [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  Informationen zu den Bereichen des Business Case finden Sie im Artikel [Überblick über die Bereiche des Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

* Sie müssen alle Bereiche des Business Case mit Ausnahme des Bereichs Ziele abschließen, wenn Sie möchten, dass Ihr Projekt in Portfolio Optimizer eine Bewertung erhält. Das Ausfüllen des Bereichs Ziele ist optional. Das Projekt erhält eine Bewertung in Portfolio Optimizer, auch wenn dieser Bereich nicht abgeschlossen ist.

  Informationen zum Arbeiten mit Scorecards und mit Portfolio Optimizer finden Sie im Artikel [Anwenden einer Scorecard auf ein Projekt und Generieren eines Ausrichtungswerts](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

## Erstellen eines Business Case

{{step1-to-projects}}

1. Klicken Sie **Neues Projekt** und wählen Sie dann **Projekt anfragen** aus der angezeigten Dropdown-Liste aus. Das Projekt wird erstellt und **Ideenstatus** wird standardmäßig zugewiesen.

   >[!CAUTION]
   >
   >Wenn der Ideenstatus in Ihrer Workfront-Instanz gelöscht wurde, wird das Projekt in den Standardstatus für neue Projekte versetzt, wie im Bereich Projektvoreinstellungen definiert. Informationen zum Einrichten von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. Geben Sie im Feld Projekttitel einen Namen ein.
1. (Optional) Klicken Sie auf das **Mehr**-Symbol ![Mehr-Symbol](assets/qs-more-icon-on-an-object.png) und dann **Vorlage anhängen**, um die Arbeitsaufschlüsselungsstruktur Ihres Projekts zu erstellen.

   Oder

   Beginnen Sie damit, dem Projekt manuell Aufgaben hinzuzufügen.

1. (Bedingt) Wenn Sie ausgewählt haben, dass eine Vorlage angehängt werden soll, fügen Sie die Vorlage weiterhin dem Projekt hinzu.
1. Klicken Sie im linken Bedienfeld auf **Business Case**.
1. (Optional) Um den Abschnitt **Projektinformationen** zu bearbeiten, klicken Sie auf **Projektinformationen bearbeiten**. 

   Weitere Informationen zum Bearbeiten der Felder **Projektinfo** finden Sie im Abschnitt [Projektinfo](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#project-info) im Artikel [Überblick über die Bereiche des Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) Um den Abschnitt &quot;**&quot;** bearbeiten, klicken Sie auf **Ziele bearbeiten**.

   Weitere Informationen zur Bearbeitung des Abschnitts **Ziele** des Business Case finden Sie im Abschnitt [Ziele](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#goals) im Artikel [Überblick über die Bereiche des Business Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) Um den Abschnitt &quot;**&quot;** bearbeiten, klicken Sie auf **Ausgaben bearbeiten**.

   Weitere Informationen zur Bearbeitung des **Ausgaben**-Abschnitts des Business-Case finden Sie im Abschnitt [Ausgaben](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#expenses) im Artikel [Überblick über die Bereiche des Business-Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Optional) Klicken Sie auf **Ressourcenbudgetierung bearbeiten** um Ihre Ressourcen zu budgetieren und die budgetierten Lohnkosten abzurufen, die mit den Aufgabengebieten im Projekt verknüpft sind. Weitere Informationen finden Sie unter [Budgetressourcen im Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

   >[!TIP]
   >
   >Die hier angezeigten Informationen entsprechen den Informationen, die in den Tools für die Ressourcenbudgetierung auf Systemebene angezeigt werden.

1. (Optional) Klicken Sie auf **Risiken bearbeiten**, um diesem Projekt potenzielle Risiken hinzuzufügen. Informationen zum Hinzufügen von Risiken zum Business-Case finden Sie [ Abschnitt ](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md#risks)Risiken“ im Artikel [Überblick über die Bereiche des Business-Case](../../../manage-work/projects/define-a-business-case/areas-of-business-case.md).
1. (Optional) Wählen Sie im Dropdown **&#x200B;**&#x200B;Menü **Eine Scorecard zu diesem Projekt hinzufügen** eine Scorecard aus.

   Scorecards müssen erstellt werden, bevor sie mit Projekten verbunden werden können.

   Weitere Informationen zu Scorecards finden Sie im Artikel [Anwenden einer Scorecard auf ein Projekt und Generieren eines Alignment-Scorecards](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

1. (Optional) Wählen Sie im Dropdown **&#x200B;**&#x200B;Menü **Benutzerdefinierte Forms** ein benutzerdefiniertes Formular aus.

   Benutzerdefinierte Forms muss erstellt werden, bevor sie an Projekte angehängt werden können.

   Weitere Informationen zu benutzerdefinierten Forms finden Sie im Artikel [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Klicken Sie **Senden**. Der Projektstatus wird in **Angefordert** geändert und es wird eingereicht, um den Business Case zu genehmigen.

   Weitere Informationen zur Genehmigung eines Business-Case finden Sie im Artikel [Genehmigen eines Business-Case](../../../manage-work/projects/define-a-business-case/approve-business-case.md).


>[!TIP]
>
> Nach Abschluss des Business Case können Sie eine Kopie davon in eine PDF-Datei exportieren. Weitere Informationen zum Exportieren des Business Case in eine PDF-Datei finden Sie [Export des Business Case eines Projekts](/help/quicksilver/manage-work/projects/define-a-business-case/export-business-case.md).


