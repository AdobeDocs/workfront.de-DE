---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Anfordern von Zugriff auf Objekte
description: Ihre Sichtbarkeit von Objekten in Adobe Workfront hängt von Ihrem Zugriff auf diesen Objekttyp sowie von Ihren Berechtigungen für ein einzelnes Objekt ab.
author: Courtney
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 4897f165a7316a52b968601b45f95f7045f63840
workflow-type: tm+mt
source-wordcount: '1327'
ht-degree: 1%

---

# Anfordern des Zugriffs auf Objekte

<!-- Audited: 4/2025 -->

Ihre Sichtbarkeit von Objekten in Adobe Workfront hängt von Ihrem Zugriff auf diesen Objekttyp sowie von Ihren Berechtigungen für ein einzelnes Objekt ab.

>[!NOTE]
>
>In diesem Artikel wird beschrieben, wie Sie Berechtigungen für alle Objekte mit Ausnahme der folgenden anfordern können:
>
>* Szenario-Planer im Adobe Workfront-Szenario-Planer. Weitere Informationen finden Sie unter [Anfordern von Berechtigungen für einen Plan im Szenario-Planer](../../scenario-planner/request-access-to-plan.md). Dies erfordert eine zusätzliche Lizenz.
>
>* Ansichten und Arbeitsbereiche in Workfront Planning. Weitere Informationen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). Dies erfordert eine zusätzliche Lizenz.


Ihr Workfront-Administrator konfiguriert Ihren Zugriff auf einen Objekttyp auf Ihrer Zugriffsebene. Weitere Informationen finden Sie unter [&#x200B; der Zusammenarbeit von Zugriffsebenen und Berechtigungen](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Wenn Sie Berechtigungen für bestimmte Objekte in Workfront benötigen, können Sie Zugriff darauf anfordern. Anstatt eine E-Mail an den Workfront-Administrator oder Objektinhaber zu senden, um Ihre Anforderungen zu erläutern, können Sie in Workfront zusätzlichen Zugriff (oder Berechtigungen) anfordern.

Sie können den erstmaligen Zugriff auf Objekte anfordern, wenn jemand einen Link zum Objekt für Sie freigibt, oder Sie können zusätzlichen Zugriff auf Objekte anfordern, für die Sie bereits über Anzeigeberechtigungen verfügen. Beispielsweise können Sie für ein Projekt über Anzeigeberechtigungen verfügen, Sie müssen ihm jedoch Aufgaben hinzufügen. In diesem Fall können Sie Contribute-Berechtigungen für das Projekt anfordern.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Arbeit oder höher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen des Zugriffs auf die Objekte, für die Sie Berechtigungen anfordern, oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Grundlegendes zu standardmäßigen Freigaberegeln

Die folgenden Standardfreigaberegeln sind Standardoptionen in Ihrem Workfront-System und werden automatisch wirksam:

* Benutzende, die einer Aufgabe oder einem Problem zugewiesen sind, haben Beitragszugriff darauf.
* Projekt-, Portfolio- und Programm-Manager haben Verwaltungszugriff auf die Objekte, deren Inhaber sie sind.
* In eine Konversation einbezogene Benutzende haben Ansichtszugriff auf das Objekt, an dem die Konversation stattfindet.
* Benutzer, die als genehmigende Personen zugewiesen sind, haben Ansichtszugriff auf das Objekt, das darauf wartet, genehmigt zu werden.
* Bei der Freigabe eines Dashboards werden alle Berichte im Dashboard mit demselben Zugriff auf dieselben Benutzer freigegeben.
* Objektbesitzer können den Zugriff auf ein Objekt nicht über ihren Zugriff auf dieses Objekt hinaus erweitern, wie vom Administrator definiert.

## Zugriffsberechtigung anfordern

Sie können anfänglichen Zugriff auf Objekte anfordern, auf die Sie derzeit keinen Zugriff haben, oder Sie können zusätzlichen Zugriff auf Objekte anfordern, auf die Sie nur eingeschränkten Zugriff haben.

* [Erstzugriff anfordern](#request-initial-access)
* [Zusätzlichen Zugriff anfordern](#request-additional-access)

### Erstzugriff anfordern  {#request-initial-access}

Wenn Sie noch keinen Zugriff auf ein Objekt haben und von einem Link aus zu diesem Objekt navigieren, wird ein Bildschirm angezeigt, der Sie darüber informiert, dass Sie keinen Zugriff haben, um die Informationen anzuzeigen.

So fordern Sie den erstmaligen Zugriff auf ein Objekt an:

1. Klicken Sie **Zugriff anfordern**. Das **Zugriff anfordern** wird angezeigt.

1. (Bedingt) Wenn mehr als ein Benutzer über die entsprechenden Zugriffsrechte verfügt, um Ihnen zusätzlichen Zugriff zu gewähren, wird neben dem Namen des Benutzers ein Dropdown-Pfeil angezeigt. Wählen Sie aus der Dropdown-Liste den Benutzer aus, der Ihre Zugriffsanfrage erhalten soll.

   In der Dropdown-Liste, die alphabetisch sortiert ist, werden nur 10 Benutzer angezeigt. Weitere Informationen zur Reihenfolge der in diesem Dropdown-Menü aufgelisteten Benutzer finden Sie unter [Hierarchie der Dropdown-Menüs „Zugriff anfordern“ und „Zugriff anfordern“](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Wählen Sie aus der Dropdown-Liste den gewünschten Zugriffstyp aus.
1. (Optional) Geben Sie im Feld **P.S.** einen Hinweis ein, warum Sie zusätzlichen Zugriff benötigen.

   ![Dialogfeld „Zugriff anfordern“](assets/request-access-to-project.png)

1. Klicken Sie **Zugriff anfordern**.

<!--
If you do not have access level rights to an object and you try to access that object from a link, a screen is displayed informing you to contact the Workfront administrator.

For example, if you do not have portfolio access, but you were given a link to a portfolio, you would see the following message:  
![](assets/permission-request-initial2-350x96.png)
-->

### Zusätzlichen Zugriff anfordern {#request-additional-access}

So fordern Sie zusätzlichen Zugriff auf ein Objekt an, auf das Sie bereits eingeschränkten Zugriff haben:

1. Navigieren Sie zu dem Objekt, für das Sie zusätzlichen Zugriff anfordern möchten.

1. Klicken Sie auf das **Mehr**-Menü rechts neben dem Projektnamen und dann auf **Zusätzlichen Zugriff anfordern**.

   ![Zusätzlichen Zugriff anfordern](assets/more-menu-request-more-access.png)

1. (Bedingt) Wenn mehr als ein Benutzer über die entsprechenden Zugriffsrechte verfügt, um Ihnen zusätzlichen Zugriff zu gewähren, wird neben dem Namen des Benutzers ein Dropdown-Pfeil angezeigt. Wählen Sie aus der Dropdown-Liste den Benutzer aus, der Ihre Zugriffsanfrage erhalten soll.

   In der Dropdown-Liste, die alphabetisch sortiert ist, werden nur 10 Benutzer angezeigt. Weitere Informationen zur Reihenfolge der in diesem Dropdown-Menü aufgelisteten Benutzer finden Sie unter [Hierarchie der Dropdown-Menüs „Zugriff anfordern“ und „Zugriff anfordern“](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Wählen Sie aus der Dropdown-Liste die Zugriffsebene aus, die Sie anfordern.
1. (Optional) Geben Sie im Feld **P.S.** einen Hinweis ein, warum Sie zusätzlichen Zugriff benötigen.

   ![Dialogfeld „Zugriff anfordern“](assets/request-access-to-project.png)

1. Klicken Sie **Zugriff anfordern**.

## Hierarchie der Dropdown-Menüs „Zugriff anfordern“ und „Zugriff anfordern“ {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Verstehen Sie die Hierarchie der Benutzer, die in den Dropdown-Menüs „Zugriff anfordern“ und „Zugriff anfordern“ aufgeführt sind](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Grundlegendes zum Besitzer eines Objekts](#understand-the-owner-of-an-object)

### Machen Sie sich mit der Hierarchie der Benutzer vertraut, die in den Dropdown-Menüs Zugriff anfordern und Mehr Zugriff anfordern aufgeführt sind {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Beim Ausfüllen der Zugriffsanforderungslisten oder der Zugriffsanforderungslisten für Objekte wählt Workfront eine Liste von bis zu 10 Benutzenden aus, die verschiedene Rollen erfüllen, welche dem anfragenden Benutzer Objektzugriff gewähren können. Die resultierende Liste wird dann nach ihrem Namen in aufsteigender alphabetischer Reihenfolge sortiert.

Die Reihenfolge der Benutzer in den Dropdown-Listen Zugriff anfordern oder Mehr Zugriff anfordern wird durch die folgenden Regeln bestimmt:

* Der erste Benutzer in der Liste ist der „Eigentümer“ des Objekts, wie unter [Verstehen des Eigentümers eines Objekts](#understand-the-owner-of-an-object) beschrieben.
* Die Liste wird dann mit Benutzern gefüllt, für die das Objekt einzeln freigegeben wird. Sie sind in alphabetischer Reihenfolge aufgeführt.
* Die Liste wird dann weiter mit Benutzern gefüllt, die den erforderlichen Zugriff durch die Freigabe für ihre Teams, Gruppen oder Unternehmen erhalten. Sie sind in alphabetischer Reihenfolge aufgeführt.
* Wenn die Liste leer ist, werden die Workfront-Administratoren hinzugefügt, sodass immer jemand Zugriff von anfordern kann. Sie sind in alphabetischer Reihenfolge aufgeführt.
* Jeder Benutzer in der Liste muss den angeforderten Zugriff auf das Objekt und Zugriff haben, um das Objekt freigeben zu können.

### Grundlegendes zum Besitzer eines Objekts {#understand-the-owner-of-an-object}

Der Eigentümer eines Objekts wird wie folgt definiert:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objekt</strong> </th> 
   <th><strong>Definition des Inhabers des Objekts</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekte</td> 
   <td>Der Eigentümer ist der Projektbesitzer oder, falls er fehlt oder nicht den erforderlichen Zugriff hat, der Eigentümer des übergeordneten Portfolios. <p>Möglicherweise handelt es sich nicht um dieselbe Person wie der Projektersteller. </p></td> 
  </tr> 
  <tr> 
   <td>Aufgaben</td> 
   <td>Der Eigentümer ist der Primäre Beauftragte oder, falls er fehlt oder nicht über den erforderlichen Zugriff verfügt, der Eigentümer des Projekts, in dem sich die Aufgabe befindet, wie oben definiert. <p>Möglicherweise handelt es sich nicht um dieselbe Person wie die Person, die die Aufgabe erstellt hat. </p></td> 
  </tr> 
  <tr> 
   <td>Probleme</td> 
   <td> <p>Der Eigentümer ist der Primäre Ansprechpartner für das Problem oder, falls es fehlt oder er nicht über den erforderlichen Zugriff verfügt, der Eigentümer des Projekts, in dem das Problem liegt, wie oben definiert. </p> <p>Sie sind möglicherweise nicht dieselbe Person wie die Person, die das Problem erstellt hat. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Der Besitzer ist der Portfolio-Besitzer. <p>Sie sind möglicherweise nicht dieselbe Person wie die Person, die das Portfolio erstellt hat. </p></td> 
  </tr> 
  <tr> 
   <td>Dokumente</td> 
   <td>Der Eigentümer ist der Eigentümer des Dokuments (der Benutzer, der das Dokument hochgeladen hat) oder, falls es fehlt oder er nicht über den erforderlichen Zugriff verfügt, der Eigentümer des Objekts, auf dem sich das Dokument befindet.</td> 
  </tr> 
  <tr> 
   <td>Berichte und Dashboards</td> 
   <td>Der Eigentümer ist der Ersteller des Berichts oder Dashboards. </td> 
  </tr> 
  <tr> 
   <td>Kalender</td> 
   <td>Der Besitzer ist der Ersteller des Kalenders. Allen Benutzern ist standardmäßig ein Kalender zugewiesen. Sie werden als Besitzer dieses Kalenders betrachtet. </td> 
  </tr> 
  <tr> 
   <td>Filter, Ansichten und Gruppierungen</td> 
   <td>Ersteller ist der Eigentümer eines Filters, einer Ansicht oder einer Gruppierung. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Pläne</span> </td> 
   <td> <p><span>Der Eigentümer ist der Ersteller des Plans.</span> </p> <p>Dies erfordert eine zusätzliche Lizenz. </p> <p><span>Informationen zum Workfront-Szenarioplaner finden Sie unter</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Szenarioplaner - Übersicht</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Ziele</td> 
   <td> <p>Der Eigentümer ist der Benutzer, der als Eigentümer angegeben ist. Sie sind möglicherweise nicht dieselbe Person wie die Person, die das Ziel erstellt hat. </p> <p>Dies erfordert eine zusätzliche Lizenz. </p> <p>Informationen zu Workfront-Zielen finden Sie unter <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront-Ziele - Übersicht</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


