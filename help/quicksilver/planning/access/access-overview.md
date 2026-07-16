---
title: Zugriffsübersicht für Adobe Workfront Planning
description: Nicht alle Benutzenden in der Organisation haben dieselben Berechtigungen für die Verwendung von Adobe Workfront Planning. In diesem Artikel werden der Zugriff und die Berechtigungen beschrieben, die Benutzer haben können, um die Funktionen von Adobe Workfront Planning verwenden zu können.
author: Alina
feature: Workfront Planning
recommendations: noDisplay, noCatalog
role: User, Admin
exl-id: 99fac041-a235-4991-b826-d19944164bc9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/QuLxjUMlRgN0FvlDwR0JVQ-m-wV-z3C6sh30lJYRKfU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: ab0d036ea3bbcdad2daaed6b09864272fd1beb11
workflow-type: tm+mt
source-wordcount: 1010
ht-degree: 3%

---

# Überblick über den Zugriff auf Adobe Workfront-Planung

<!--do not use the snippet for IMPORTANT , as it links to this article-->


<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Workfront Planning. Workfront Planning ist entweder ein eigenständiges Produkt oder eine zusätzlich erworbene Funktion von Adobe Workfront.
>
>
>Dieser Artikel enthält allgemeine Informationen zu Workfront Planning, wenn Kunden auch ein Workfront- oder Workflow-Paket erwerben.
>
>Eine vollständige Liste der Artikel mit Dokumentationen zu Workfront Planning finden Sie unter [Allgemeine Informationen und Artikelindex für Adobe Workfront Planning](/help/quicksilver/planning/planning-information.md).
>
>Informationen zu Workfront Planning als eigenständiges Produkt finden Sie unter [Erste Schritte mit Adobe Workfront Planning als eigenständiges Produkt](/help/quicksilver/planning/planning-sta/planning-sta-overview.md).

In diesem Artikel werden der Zugriff und die Einstellungen beschrieben, die Sie zur Verwendung der Funktionen von Workfront Planning benötigen.

## Zugriffsanforderungen

<!--do not collapse the access requirements below - this is the main article about Access overview-->

<!--*********ensure that the link ^^^^^^^^below^^^^^^^^ to Workfront Pricing and Packaging now also includes information about Workfront Planning. If not, talk with Lauren S.***************-->

Sie müssen über die folgenden Zugriffsrechte verfügen, um Workfront Planning verwenden zu können:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
   <tr>
   <tr>
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td>
   <td>
   <p>Beliebiges Workfront- oder Workflow-Planungspaket
   und jedes Workfront-Planungspaket</p>
   <p><b>NOTIZ</b></p>
   <p>Zugriff auf verbindbare Datensatztypen:</p>
   <ul><li><p>Beliebiges Workfront-Paket und ein Planungspaket</p></li>
   <li><p>Beliebiger Workflow und ein Planning Prime- und Ultimate-Paket</p></li></ul>

<p>Für den Zugriff auf globale Datensatztypen:</p>
   <ul><li><p>Beliebiges Workfront-Paket und Planning Plus-Paket</p></li>
   <li><p>Beliebiges Workflow-Paket und ein Planning Prime- und Ultimate-Paket</p></li></ul> </td></tr>
   <!--
   <tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
   <p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
   <p><b>IMPORTANT</b></p>
   <p>Only users added to the Adobe Identity Management System (IMS) can be granted permissions and added to Planning fields.</p>
   <p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
   </tr>
   -->
   <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <ul><li><p>Beliebiger Workflow und jede Planungslizenz, um Workfront-Planungsinformationen anzuzeigen</p></li>
   <li><p>Workflow-Standard und Planungsstandard zur Erstellung von Arbeitsbereichen und Ansichten</p></li></ul>
    </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td>
   <td> <p>Beliebiger Workflow und beliebiger Planungs-Lizenztyp auf der Zugriffsebene</p>  
   </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <ul>
   <li><p>Zeigen Sie oder höhere Berechtigungen für Arbeitsbereiche, Datensatztypen und Ansichten an, die Sie nicht für den Zugriff auf sie und ihre Objekte erstellt haben.</p></li>
   <li><p>Tragen Sie oder höhere Berechtigungen zu Arbeitsbereichen und Datensatztypen bei, die Sie nicht erstellt haben, um sie zu bearbeiten und Datensatztypen zu erstellen, zu bearbeiten oder zu löschen.</p></li>
   <li><p><span class="preview">Verwalten Sie Berechtigungen für Datensätze, um sie zu bearbeiten, freizugeben oder zu löschen.</p>
   <li><p>Beitragen oder höhere Berechtigungen für Ansichten, die Sie nicht erstellt haben, zum Bearbeiten, Löschen und Freigeben</p>
   </li>
    <li><p>Planungsadministratoren können Workspaces verwalten, die sie nicht erstellt haben. </p></li>
    <li><p>Planning-Administratoren können nicht auf Ansichten zugreifen, die sie nicht erstellt haben. </p></li></ul>
   <p>Informationen zu Freigabeberechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Übersicht über Freigabeberechtigungen in Adobe Workfront Planning</a> 
   </td>
   </tr>
   <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> 
   <p>Für Planning Standard-Benutzer und -Administratoren sind die Planungsbereiche standardmäßig aktiviert.</p>
   <p> Benutzenden mit einer Lizenz für Workflow-Light oder Planning Contributor muss eine Layout-Vorlage zugewiesen werden, die die Planungsoption in den folgenden Bereichen enthält:</p>
   <ul><li>Hauptmenü</li>
   <li>Linkes Bedienfeld mit Projekten, Portfolios und Programmen</li>
   </ul>   
   </td>
  </tr>
 </tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Zugriffsebenen und Lizenzen in Workfront Planning

Sie können einem Benutzer eine Planning Administrator-Lizenz zuweisen, wenn Sie ihn als Administrator zu Adobe Admin Console hinzufügen.

Weitere Informationen finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Sie können die Zugriffsebene des Planning-Administrators in Workfront Planning nicht ändern.

Beim Konfigurieren von Zugriffsebenen in Workfront können Sie die folgenden Lizenztypen zuweisen:

* Workflow-Lizenztypen
* Planungs-Lizenztypen

Benutzenden müssen beide Lizenztypen ihrer Zugriffsebene zugewiesen sein, um auf Workfront Planning zugreifen zu können.

Sie können einer Zugriffsebene die folgenden Planning-Lizenzen zuweisen:

* **Planungsstandard**: Gewähren Sie Benutzern diesen Zugriff, wenn sie alle Planning-Objekte erstellen und verwalten müssen, ohne Administrator zu sein.
* **Planning-Mitwirkender**: Erteilen Sie Benutzern diesen Zugriff, wenn sie zu Datensätzen beitragen müssen, aber keine Planning-Objekte erstellen müssen.

  >[!TIP]
  >
  >Der Lizenztyp „Planning Contributor“ ist nicht verfügbar, wenn Ihr Unternehmen ungleiche Lizenzen für Workflow und Planung erworben hat.


* **Keine**: Wenn Sie diesen Planning-Lizenztyp zuweisen, entfernen Sie speziell den gesamten Planning-Zugriff für die Benutzer, die dieser Zugriffsebene zugewiesen sind.

  >[!IMPORTANT]
  >
  >Planning- und Workflow-Lizenzen arbeiten zusammen, um Benutzenden Zugriff auf Workfront zu gewähren.
  >
  >Sie können einer Benutzerin bzw. einem Benutzer unterschiedliche Zugriffsebenen zwischen Workflow und Planung gewähren. Die Workflow-Lizenz darf jedoch nicht niedriger sein als die Planning-Lizenz.
  >
  >Sie können Benutzenden beispielsweise eine Lizenz für Workflow-Standard und eine Planning-Mitwirkende-Lizenz erteilen, ihnen jedoch keine Workflow-Mitwirkende- und eine Planning Standard-Lizenz.
  >
  >Der Workflow-Lizenztyp darf nicht leer sein, wenn Benutzende auf „Workflow“ oder „Planung“ zugreifen müssen.

Weitere Informationen finden Sie unter [Lizenztyp - Übersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Zugriffsebene konfigurieren

Informationen zum Konfigurieren des Zugriffs in Workfront finden Sie unter [Erstellen und Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Lizenzen Benutzern zuweisen

Lizenzen können Benutzern zugewiesen werden, wenn diese beim Bearbeiten oder Erstellen eine Zugriffsebene erhalten.

Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Berechtigungen erteilen

In Workfront Planning können Sie Berechtigungen für die folgenden Entitäten erteilen:

* Arbeitsbereiche
* Eintragstypen
* Ansichten
* Einträge

Weitere Informationen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Ihr Adobe Workfront-Lizenztyp verwendet Ihren Workfront Planning-Lizenztyp und Ihre Planning-Berechtigungen, um Ihnen Zugriff zum Anzeigen, Bereitstellen oder Verwalten von Workfront Planning-Objekten zu gewähren.

Informationen dazu, wie sich Lizenztypen auf Berechtigungsebenen für Workfront Planning-Objekte auswirken, finden Sie [Lizenztyp - Übersicht bei Verwendung von Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).

## Freigeben des Planungsbereichs mithilfe einer Layout-Vorlage

<!--First, contact your account manager to obtain access to the current Workfront Planning program.-->

Für Standardbenutzer und Systemadministratoren sind die Planungsbereiche in den folgenden Bereichen standardmäßig aktiviert:

* Hauptmenü
* Linker Bereich mit Projekten, Portfolios oder Programmen

Ihr Systemadministrator muss Ihnen die Planungsbereiche hinzufügen, falls Sie über eine andere Workfront-Lizenz verfügen und zu den Workfront-Planungsarbeiten beitragen müssen.

Der Administrator kann die Option Planung den folgenden Bereichen hinzufügen, indem er Sie ändert und einer Layoutvorlage zuweist:

* Hauptmenü
* Landingpage
* Linkes Bedienfeld für Projekte, Portfolios und Programme
* Nadeln

So fügen Sie Workfront Planning-Bereiche zu Benutzern Ihrer Workfront-Instanz hinzu oder entfernen sie daraus:

1. Melden Sie sich bei **Workfront** als Workfront-Administrator an.

1. Wechseln Sie **Hauptmenü** > **Setup** > **Schnittstelle** > **Layoutvorlagen** und öffnen oder erstellen Sie eine Layoutvorlage.

   Informationen zum Anpassen einer Layout-Vorlage finden Sie unter [Erstellen und Verwalten von Layout-Vorlagen](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Weisen Sie die Layout-Vorlage den Benutzern zu, die Zugriff auf Workfront Planning haben möchten.

   Weitere Informationen finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   Alle Benutzenden, die der Vorlage zugewiesen sind, können jetzt im Hauptmenü auf Workfront Planning zugreifen.

   Benutzer können mit der Erstellung von Arbeitsbereichen, Datensatztypen, Datensätzen und Feldern beginnen.


