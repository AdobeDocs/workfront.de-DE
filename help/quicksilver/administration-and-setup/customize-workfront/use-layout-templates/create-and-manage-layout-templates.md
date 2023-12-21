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
source-git-commit: 5d8e189f01a52b2d1b605b497ed17737fb0a0924
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Erstellen und Verwalten von Layoutvorlagen

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.</p>
<p>Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>NOTE</b>:</p> <p>Wenn Sie keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt.

Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

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

1. Klicks **Neue Layout-Vorlage**.

   Oder

   Klicken Sie auf den Namen der Layout-Vorlage, die Sie ändern möchten.

1. Wenn Sie eine neue Layoutvorlage erstellen, geben Sie einen **Name der Layout-Vorlage** und (optional) a **Beschreibung** verwendet werden.

1. Passen Sie Bereiche der Benutzeroberfläche an, wie in den folgenden Artikeln beschrieben:

   * [Hauptmenü mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Anpassen des linken Bedienfelds mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Anpassen von fixierten Seiten mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Detailansicht mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Landingpage mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Benutzeroberflächenterminologie mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Testen Sie weiterhin Ihre Layoutvorlage und stellen Sie sie den Benutzern zur Verfügung, wie in den folgenden Artikeln beschrieben:

   * [Testen einer neuen Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Administratorzugriff für eine Layoutvorlage gewähren](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Benutzer einer Layoutvorlage zuweisen](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>Sie können auch eine Layoutvorlage erstellen, indem Sie sie kopieren und die Kopie ändern. Weitere Informationen finden Sie unter [Layout-Vorlage kopieren](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

