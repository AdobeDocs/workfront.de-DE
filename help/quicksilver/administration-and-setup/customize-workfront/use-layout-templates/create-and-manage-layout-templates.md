---
title: Erstellen und Verwalten von Layoutvorlagen
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Als Workfront-Administrator oder Gruppenadministrator können Sie Layoutvorlagen erstellen und ändern, um Layoutelemente in Workfront für Ihre Benutzer anzupassen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 1%

---

# Layout-Vorlagen erstellen und verwalten

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie Layoutvorlagen erstellen und ändern, um die folgenden Layoutelemente in Workfront für Ihre Benutzer anzupassen:

* Hauptmenü
* Linke Navigationsleiste
* Startbereich
* Ansichten, Filter und Gruppierungen, die für Listen und Berichte verwendet werden.
* Terminologie auf dem Bildschirm
* Projekt-, Aufgaben- und Problemkopfzeilen

Nachdem Sie eine Layoutvorlage erstellt oder geändert haben, können Sie sie einzelnen Benutzern, Teams, Gruppen oder Auftragsrollen zuweisen.

Das standardmäßige Workfront-Layout jedes Benutzers hängt von seiner Zugriffsstufe und seinem Lizenztyp ab. Einige Benutzer sehen beispielsweise möglicherweise einige Bereiche im Hauptmenü nicht. Weitere Informationen finden Sie unter [Über das standardmäßige Adobe Workfront-Layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konzepte zum Erstellen und Verwalten von Layoutvorlagen

* Benutzer können einige Bereiche ihres eigenen Layouts anpassen. Wenn Sie eine Layoutvorlage ändern, werden Ihre Änderungen mit allen von ihnen vorgenommenen Anpassungen zusammengeführt, ohne sie zu überschreiben oder zurückzusetzen. Dies gilt auch, wenn Sie Benutzer einer neuen Layoutvorlage zuweisen.
* Gruppenadministratoren und Benutzer mit einer Planungslizenz, die andere Benutzer bearbeiten können, können den Benutzern, die sie bei der Bearbeitung ihres Profils verwalten können, Layoutvorlagen auf System- und Gruppenebene hinzufügen.
* Gruppenadministratoren können Auftrags- oder Teams keine Layoutvorlagen zuweisen.

Weitere Informationen zu Layoutvorlagen finden Sie unter [Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## Layout-Vorlage erstellen oder ändern

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Schnittstelle** > **Layout-Vorlagen**.

1. Klicken Sie auf **Neue Layout-Vorlage**.

   Oder

   Klicken Sie auf den Namen der Layout-Vorlage, die Sie ändern möchten.

1. Wenn Sie eine neue Layoutvorlage erstellen, geben Sie einen **Layoutvorlagennamen** und (optional) eine **Beschreibung** ein.

1. Passen Sie Bereiche der Benutzeroberfläche an, wie in den folgenden Artikeln beschrieben:

   * [Anpassen des Hauptmenüs mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Passen Sie den linken Bereich mithilfe einer Layoutvorlage an](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Pinned-Seiten mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Anpassen der Detailansicht mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Passen Sie die Landingpage mithilfe einer Layoutvorlage an](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Benutzeroberflächenterminologie mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Testen Sie weiterhin Ihre Layoutvorlage und stellen Sie sie den Benutzern zur Verfügung, wie in den folgenden Artikeln beschrieben:

   * [Testen einer neuen Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Gewähren des Administratorzugriffs für eine Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Benutzer einer Layoutvorlage zuweisen](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>Sie können auch eine Layoutvorlage erstellen, indem Sie sie kopieren und die Kopie ändern. Weitere Informationen finden Sie unter [Kopieren einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

