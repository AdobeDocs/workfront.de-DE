---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Voraussetzungen für die Verwendung von Workfront-Zielen
description: Ihr Adobe Workfront-Administrator muss sicherstellen, dass bestimmte Bedingungen erfüllt sind, bevor Sie auf Adobe Workfront-Ziele zugreifen können.
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Voraussetzungen für die Verwendung von Workfront-Zielen

Ihr Adobe Workfront-Administrator muss sicherstellen, dass alle folgenden Bedingungen erfüllt sind, bevor Sie auf Adobe Workfront-Ziele zugreifen können:

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* Ihr Unternehmen muss die richtige Lizenz für Workfront Goals erwerben. Weitere Informationen finden Sie im Abschnitt . [Zugriff der Workfront Goals-Organisation erhalten](#obtain-workfront-goals-organization-access)in diesem Artikel.

* Weisen Sie den richtigen Workfront-Lizenztyp zu. Weitere Informationen zur Zuweisung von Lizenztypen und Zugriffsebenen finden Sie im Abschnitt . [Aktualisierung der Lizenztypen und Einstellungen der Zugriffsebene](#update-license-types-and-access-level-settings) in diesem Artikel.

>[!NOTE]
>
>Benutzer mit externem Lizenztyp können nicht auf Workfront-Ziele zugreifen.

* Gewähren Sie Zugriff auf Ziele in Ihrer Zugriffsebene. Weitere Informationen finden Sie unter [Zugriff auf Adobe Workfront-Ziele gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

* Weisen Sie eine Layout-Vorlage zu, die den Bereich Ziele im Hauptmenü enthält.

  >[!NOTE]
  >
  >Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält.

  Weitere Informationen finden Sie im Abschnitt [Hinzufügen von Workfront-Zielen zu einer Layoutvorlage](#add-workfront-goals-to-a-layout-template) in diesem Artikel.

* Wenn Sie Ziele ändern müssen, die Sie nicht selbst erstellt haben, muss der Zielersteller die Ziele für Sie freigeben und Ihnen Verwaltungsberechtigungen erteilen.

  Weitere Informationen finden Sie im Abschnitt . [Freigeben einzelner Ziele für andere Benutzer](#share-individual-goals-with-other-users) in diesem Artikel.

## Zugriff der Workfront Goals-Organisation erhalten {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

Ihr Unternehmen muss zusätzlich zur Workfront-Lizenz eine zusätzliche Lizenz erwerben, damit Ihre Benutzer auf Workfront Goals zugreifen können. Nachdem Ihr Unternehmen die zusätzliche Lizenz erworben hat, aktiviert Workfront Workfront Goals für Ihr Konto. Informationen zum Erwerb einer Lizenz für Workfront Goals erhalten Sie von Ihrem Workfront-Kundenbetreuer.

## Aktualisierung der Lizenztypen und Einstellungen der Zugriffsebene  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

Ihr Workfront-Administrator muss Ihnen einen der folgenden Workfront-Lizenztypen für den Zugriff auf Workfront-Ziele gewähren:

* Plan
* Arbeit
* Überprüfung
* Anfrage

Nachdem Ihr Workfront-Administrator Ihnen einen dieser Lizenztypen gewährt hat, müssen Sie darüber hinaus auf der Zugriffsebene auf Ziele zugreifen können. Informationen zum Zugriff auf Ziele finden Sie unter [Zugriff auf Adobe Workfront-Ziele gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

Als Workfront-Administrator können Sie die Anzahl der Workfront Goals-Lizenzen in Ihrem System überprüfen und verstehen, wie viele derzeit aktiviert sind. Weitere Informationen finden Sie unter [Verwalten der verfügbaren Lizenzen in Ihrem System](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

>[!NOTE]
>
>Mit Workfront können Sie weitere Workfront Goals-Lizenzen zuweisen, die Sie erworben haben. Wenn Sie jedoch mehr Lizenzen zuweisen, als Ihr Workfront Goals-Vertrag zulässt, setzt sich ein Workfront-Kundenbetreuer mit Ihnen in Verbindung, um Ihnen mitzuteilen, dass Sie Ihre Vertragsnummer überschritten haben.

## Hinzufügen von Workfront-Zielen zu einer Layoutvorlage {#add-workfront-goals-to-a-layout-template}

Ihr Workfront- oder Gruppenadministrator muss Ihnen eine Layout-Vorlage zuweisen, die den Bereich Ziele im Hauptmenü enthält, damit Sie auf Workfront-Ziele zugreifen können.

![](assets/layout-template-align-highlighted-350x220.png)

Ihr Workfront-Administrator oder Gruppenadministrator kann Ihrer Layoutvorlage auch Folgendes hinzufügen, damit Sie mühelos auf Workfront-Ziele zugreifen können:

* Eine fixierte Registerkarte
* Festlegen des Zielbereichs für Ihre Landingpage

Informationen zum Aktualisieren der Layout-Vorlage finden Sie in den folgenden Artikeln:

* [Erstellen und Verwalten von Layoutvorlagen](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [Hauptmenü mithilfe einer Layoutvorlage anpassen](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [Anpassen von fixierten Seiten mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [Landingpage mithilfe einer Layoutvorlage anpassen](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [Benutzer einer Layoutvorlage zuweisen](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## Freigeben einzelner Ziele für andere Benutzer {#share-individual-goals-with-other-users}

Standardmäßig können alle Benutzer, die mindestens Zugriff auf Ziele in ihrer Zugriffsebene haben, alle Ziele in Workfront anzeigen.

Jeder Benutzer mit Zugriff auf Ziele bearbeiten kann Ziele erstellen und erhält automatisch Zugriff auf die von ihm erstellten Ziele. Wenn sie die Ziele anderer Benutzer bearbeiten müssen, muss jemand mit der Berechtigung zum Verwalten dieser Ziele die Ziele, die sie nicht erstellt haben, für sie freigeben.

Informationen zum Freigeben von Zielen für Benutzer und zum Gewähren von Verwaltungsberechtigungen finden Sie unter [Freigeben eines Ziels in Workfront-Zielen](../../workfront-goals/workfront-goals-settings/share-a-goal.md).
