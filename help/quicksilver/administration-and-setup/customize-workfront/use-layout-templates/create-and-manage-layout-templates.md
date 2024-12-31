---
title: Erstellen und Verwalten von Layout-Vorlagen
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Als Workfront-Administrator oder Gruppenadministrator können Sie Layout-Vorlagen erstellen und ändern, um Layout-Elemente in Workfront für Ihre Benutzerinnen und Benutzer anzupassen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 1%

---

# Layout-Vorlagen erstellen und verwalten

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Als Adobe Workfront-Administrator oder Gruppenadministrator können Sie Layout-Vorlagen erstellen und ändern, um die folgenden Layout-Elemente in Workfront für Ihre Benutzerinnen und Benutzer anzupassen:

* Hauptmenü
* Linkes Navigationsfenster
* Wohngebiet
* Bedienfeld „Zusammenfassung“
* Ansichten, Filter und Gruppierungen, die Benutzer mit Listen und Berichten verwenden.
* Terminologie auf dem Bildschirm
* Kopfzeilen von Projekten, Aufgaben und Problemen

Nachdem Sie eine Layout-Vorlage erstellt oder geändert haben, können Sie sie einzelnen Benutzern, Teams, Gruppen oder Aufgabengebieten zuweisen.

Das standardmäßige Workfront-Layout jedes Benutzers hängt von seiner Zugriffsebene und seinem Lizenztyp ab. Beispielsweise werden einigen Benutzern möglicherweise nicht alle Bereiche im Hauptmenü angezeigt. Weitere Informationen finden Sie unter [Über das standardmäßige Adobe Workfront-Layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.
Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Erstellen und Verwalten von Layout-Vorlagen

* Benutzer können einige Bereiche ihres eigenen Layouts anpassen. Wenn Sie eine Layout-Vorlage ändern, werden Ihre Änderungen mit allen vorgenommenen Anpassungen zusammengeführt, ohne sie zu überschreiben oder zurückzusetzen. Dies gilt auch, wenn Sie Benutzende einer neuen Layout-Vorlage zuweisen.
* Gruppenadministratoren und Benutzer mit einer Planlizenz, die andere Benutzer bearbeiten können, können den Benutzern, die sie bei der Bearbeitung ihres Profils verwalten können, Layoutvorlagen auf Systemebene und Gruppenebene hinzufügen.
* Gruppenadministratoren können Aufgabengebieten oder Teams keine Layoutvorlagen zuweisen.

Weitere Informationen zu Layout-Vorlagen finden Sie unter [Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## Layout-Vorlage erstellen oder ändern

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Schnittstelle** > **Layoutvorlagen**.

1. Klicken Sie **Neue Layout-Vorlage**.

   Oder

   Klicken Sie auf den Namen der Layout-Vorlage, die Sie ändern möchten.

1. Wenn Sie eine neue Layout-Vorlage erstellen, geben Sie einen **Namen der Layout-Vorlage** und (optional) eine **Beschreibung** ein.

1. Passen Sie Bereiche der Benutzeroberfläche an, wie in den folgenden Artikeln beschrieben:

   * [Anpassen des Hauptmenüs mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Passen Sie den linken Bereich mithilfe einer Layout-Vorlage an](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Passen Sie angeheftete Seiten mithilfe einer Layout-Vorlage an](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Passen Sie die Detailansicht mithilfe einer Layout-Vorlage an](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Passen Sie das Bedienfeld Zusammenfassung mithilfe einer Layout-Vorlage an](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Anpassen der Startseite mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   * [Landingpage mithilfe einer Layout-Vorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Anpassen der Terminologie der Benutzeroberfläche mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Testen Sie Ihre Layout-Vorlage weiter und stellen Sie sie den Benutzern zur Verfügung, wie in den folgenden Artikeln beschrieben:

   * [Testen einer neuen Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Gewähren des administrativen Zugriffs für eine Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Zuweisen von Benutzern zu einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>Sie können eine Layout-Vorlage auch erstellen, indem Sie sie kopieren und die Kopie ändern. Weitere Informationen finden Sie unter [Kopieren einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

