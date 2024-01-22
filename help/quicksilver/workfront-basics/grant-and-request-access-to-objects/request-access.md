---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Zugriff auf Objekte anfordern
description: Die Sichtbarkeit der Objekte in Adobe Workfront hängt von Ihrem Zugriff auf diesen Objekttyp sowie von Ihren Berechtigungen für einzelne Objekte ab.
author: Alina
feature: Get Started with Workfront
exl-id: ad1c525c-42a8-4fb7-a2cd-7792e1c280ab
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 0%

---

# Zugriff auf Objekte anfordern

Die Sichtbarkeit der Objekte in Adobe Workfront hängt von Ihrem Zugriff auf diesen Objekttyp sowie von Ihren Berechtigungen für einzelne Objekte ab.

>[!NOTE]
>
>In diesem Artikel wird beschrieben, wie Sie Berechtigungen für alle Objekte mit Ausnahme von Plänen im Adobe Workfront-Szenario-Planer anfordern können. Informationen zum Anfordern des Zugangs zu Plänen finden Sie unter [Anfordern des Zugriffs auf einen Plan im Szenario-Planer](../../scenario-planner/request-access-to-plan.md). Dies erfordert eine zusätzliche Lizenz.

Ihr Workfront-Administrator konfiguriert Ihren Zugriff auf einen Objekttyp in Ihrer Zugriffsebene. Weitere Informationen finden Sie unter [Wie Zugriffsebenen und Berechtigungen zusammenarbeiten](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Wenn Sie Berechtigungen für bestimmte Objekte in Workfront benötigen, können Sie den Zugriff darauf anfordern. Anstatt E-Mails an den Workfront-Administrator oder Objekteigentümer zu senden, um Ihre Anforderungen zu erläutern, können Sie innerhalb von Workfront zusätzlichen Zugriff (oder Berechtigungen) anfordern.

Sie können den anfänglichen Zugriff auf Objekte anfordern, wenn jemand eine Verknüpfung mit dem Objekt für Sie freigegeben hat, oder Sie können zusätzlichen Zugriff auf Objekte anfordern, die Sie zumindest anzeigen.

Sie können beispielsweise über Ansichtsberechtigungen für ein Projekt verfügen, müssen diesem Projekt jedoch Aufgaben hinzufügen. In diesem Fall können Sie Beitragsberechtigungen für das Projekt anfordern.

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access or higher to the objects you request permissions to</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Sie müssen über Folgendes verfügen, um Objekte freizugeben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Anzeigen des Zugriffs oder höher auf Objekte, für die Sie Berechtigungen anfordern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Grundlegendes zu standardmäßigen Freigaberegeln

Die folgenden standardmäßigen Freigaberegeln werden automatisch wirksam, da sie in Ihrem Workfront-System als Standardoptionen eingerichtet sind.

* Benutzer, die einer Aufgabe oder einem Problem zugewiesen sind, haben Contribute-Zugriff darauf.
* Projekt-, Portfolio- und Programmmanager haben Zugriff auf die Objekte, deren Inhaber sie sind.
* Benutzer, die in einer Konversation enthalten sind, haben Ansichtszugriff auf das Objekt, an dem die Konversation stattfindet.
* Als Genehmiger zugewiesene Benutzer haben Zugriff auf Ansicht auf das Objekt, das auf die Genehmigung wartet.
* Beim Freigeben eines Dashboards werden alle Berichte im Dashboard auch für dieselben Benutzer freigegeben.
* Objekteigentümer können den Zugriff auf ein Objekt nicht über ihren Zugriff auf dieses Objekt hinaus erweitern, wie vom Administrator definiert.

## Zugriffsberechtigung anfordern

Sie können den anfänglichen Zugriff auf Objekte anfordern, auf die Sie derzeit keinen Zugriff haben, oder Sie können zusätzlichen Zugriff auf Objekte anfordern, auf die Sie nur eingeschränkten Zugriff haben.

* [Erlangen Sie Zugriff](#request-initial-access)
* [Zusätzlichen Zugriff anfordern](#request-additional-access)

### Erlangen Sie Zugriff  {#request-initial-access}

Wenn Sie noch keinen Zugriff auf ein Objekt haben und über einen Link zu diesem Objekt navigieren, wird ein Bildschirm angezeigt, der Sie darüber informiert, dass Sie keinen Zugriff auf die Informationen haben.

So fordern Sie den anfänglichen Zugriff auf ein Objekt an:

1. Klicks **Zugriff anfordern**.\
   Die **Zugriff anfordern** angezeigt.

1. (Bedingt) Wenn mehr als ein Benutzer über den entsprechenden Zugriff verfügt, um Ihnen zusätzlichen Zugriff zu gewähren, wird neben dem Namen des Benutzers ein Dropdown-Pfeil angezeigt.
1. Wählen Sie den Benutzer aus der Dropdown-Liste aus, der Ihre Zugriffsanfrage erhalten soll.\
   In der Dropdown-Liste werden nur zehn Benutzer angezeigt. Die Liste ist alphabetisch sortiert.\
   Weitere Informationen zur Reihenfolge der in diesem Dropdown-Menü aufgeführten Benutzer finden Sie unter  [Hierarchie der Dropdown-Menüs &quot;Zugriff anfordern&quot;und &quot;Zugriff anfordern&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Wählen Sie aus der Dropdown-Liste den gewünschten Zugriffstyp aus.
1. (Optional) Im **P.S.** geben Sie dem Benutzer einen Hinweis dazu an, warum Sie zusätzlichen Zugriff benötigen.

   ![](assets/request-access-dialog-350x314.png)

Wenn Sie keine Zugriffsberechtigung für ein Objekt haben und versuchen, über einen Link auf dieses Objekt zuzugreifen, wird ein Bildschirm angezeigt, in dem Sie informiert werden, dass Sie sich an den Workfront-Administrator wenden können.

Wenn Sie beispielsweise keinen Portfoliozugriff haben, aber einen Link zu einem Portfolio erhalten haben, wird die folgende Meldung angezeigt:\
![](assets/permission-request-initial2-350x96.png)

### Zusätzlichen Zugriff anfordern {#request-additional-access}

So fordern Sie zusätzlichen Zugriff auf ein Objekt an, auf das Sie bereits eingeschränkten Zugriff haben:

1. Markieren Sie das Objekt, für das Sie zusätzlichen Zugriff anfordern möchten.

1. Klicken Sie auf **Mehr** Menü rechts neben dem Projektnamen und klicken Sie auf **Mehr Zugriff anfordern**.

   ![](assets/request-access-in-project-350x201.png)

1. (Bedingt) Wenn mehr als ein Benutzer über den entsprechenden Zugriff verfügt, um Ihnen zusätzlichen Zugriff zu gewähren, wird neben dem Namen des Benutzers ein Dropdown-Pfeil angezeigt.
1. Wählen Sie den Benutzer aus der Dropdown-Liste aus, der Ihre Zugriffsanfrage erhalten soll.\
   In der Dropdown-Liste werden nur zehn Benutzer angezeigt. Die Liste ist alphabetisch sortiert.\
   Weitere Informationen zur Reihenfolge der in diesem Dropdown-Menü aufgeführten Benutzer finden Sie unter  [Hierarchie der Dropdown-Menüs &quot;Zugriff anfordern&quot;und &quot;Zugriff anfordern&quot;](#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus).

1. Wählen Sie aus der Dropdown-Liste die Zugriffsstufe aus, die Sie anfordern.
1. (Optional) Im **P.S.** geben Sie einen Hinweis dazu an, warum Sie zusätzlichen Zugriff benötigen.
1. Klicks **Zugriff anfordern**.\
   ![](assets/request-access-dialog-350x314.png)

## Hierarchie der Dropdown-Menüs &quot;Zugriff anfordern&quot;und &quot;Zugriff anfordern&quot; {#hierarchy-of-the-request-access-and-request-more-access-drop-down-menus}

* [Machen Sie sich mit der Hierarchie der Benutzer vertraut, die in den Dropdownmenüs Zugriff anfordern und Mehr Zugriff anfordern aufgeführt sind.](#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus)
* [Grundlegendes zum Eigentümer eines Objekts](#understand-the-owner-of-an-object)

### Machen Sie sich mit der Hierarchie der Benutzer vertraut, die in den Dropdownmenüs Zugriff anfordern und Mehr Zugriff anfordern aufgeführt sind. {#understand-the-hierarchy-of-users-listed-in-the-request-access-and-request-more-access-drop-down-menus}

Beim Ausfüllen der Listen &quot;Zugriff anfordern&quot;oder &quot;Mehr Zugriff anfordern&quot;für Objekte wählt Workfront eine Liste mit bis zu zehn Benutzern aus, die wie unten beschrieben verschiedene Rollen bei der Freigabe des Objekts erfüllen. Diese Benutzer können dem Benutzer, der das Objekt anfordert, Zugriff auf das Objekt gewähren.\
Die resultierende Liste wird dann nach ihrem Namen in aufsteigender alphabetischer Reihenfolge sortiert.\
Workfront zeigt bis zu 10 Benutzer in den Listen &quot;Zugriff anfordern&quot;und &quot;Mehr Zugriff anfordern&quot;an.

Die Reihenfolge der Benutzer in den Dropdown-Menüs &quot;Zugriff anfordern&quot;oder &quot;Mehr Zugriff anfordern&quot;wird durch die folgenden Regeln bestimmt:

* Der erste Benutzer in der Liste ist das Objekt &quot;owner&quot;, wie unter [Grundlegendes zum Eigentümer eines Objekts](#understand-the-owner-of-an-object).
* Anschließend wird die Liste mit Benutzern gefüllt, für die das Objekt einzeln freigegeben ist. Sie werden in alphabetischer Reihenfolge aufgelistet.
* Anschließend wird die Liste mit Benutzern gefüllt, die den erforderlichen Zugriff durch die Freigabe für ihre Teams, Gruppen oder Unternehmen erhalten. Sie werden in alphabetischer Reihenfolge aufgelistet.
* Wenn die Liste leer ist, werden die Workfront-Administratoren hinzugefügt, sodass immer jemand zum Anfordern des Zugriffs verfügbar ist. Sie werden in alphabetischer Reihenfolge aufgelistet.
* Jeder Benutzer in der Liste muss über den angeforderten Zugriff auf das Objekt und Zugriff zum Freigeben des Objekts verfügen.

### Grundlegendes zum Eigentümer eines Objekts {#understand-the-owner-of-an-object}

Der Eigentümer eines Objekts wird wie folgt definiert:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Objekt</strong> </th> 
   <th><strong>Definition des Eigentümers des Objekts</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Projekte</td> 
   <td>Der Eigentümer ist der Projekteigentümer oder, falls er fehlt oder nicht über den erforderlichen Zugriff verfügt, der Eigentümer des übergeordneten Portfolios. <p>Sie sind möglicherweise nicht dieselbe Person wie der Projektersteller. </p></td> 
  </tr> 
  <tr> 
   <td>Aufgaben</td> 
   <td>Der Eigentümer ist der Primäre Bevollmächtigte oder, falls er fehlt oder nicht über den erforderlichen Zugriff verfügt, der Eigentümer des Projekts, auf dem sich die Aufgabe befindet, wie oben definiert. <p>Sie sind möglicherweise nicht dieselbe Person wie der Ersteller der Aufgabe. </p></td> 
  </tr> 
  <tr> 
   <td>Probleme</td> 
   <td> <p>Der Eigentümer ist der Primäre Ansprechpartner für das Problem oder, falls es fehlt oder er keinen erforderlichen Zugriff hat, der Eigentümer des Projekts, in dem das Problem liegt, wie oben definiert. </p> <p>Sie sind möglicherweise nicht dieselbe Person wie der Ersteller des Problems. </p> </td> 
  </tr> 
  <tr> 
   <td>Portfolios</td> 
   <td>Der Eigentümer ist der Eigentümer des Portfolios. <p>Sie sind möglicherweise nicht dieselbe Person wie der Ersteller des Portfolios. </p></td> 
  </tr> 
  <tr> 
   <td>Dokumente</td> 
   <td>Der Eigentümer ist der Eigentümer des Dokuments (der Benutzer, der das Dokument hochgeladen hat) oder, wenn es fehlt oder er keinen erforderlichen Zugriff hat, der Eigentümer des Objekts, in dem sich das Dokument befindet.</td> 
  </tr> 
  <tr> 
   <td>Berichte und Dashboards</td> 
   <td>Der Inhaber ist der Ersteller, der Bericht oder das Dashboard. </td> 
  </tr> 
  <tr> 
   <td>Kalender</td> 
   <td>Der Eigentümer ist der Ersteller des Kalenders. Allen Benutzern ist standardmäßig ein Kalender zugewiesen. Sie werden als Eigentümer dieses Kalenders betrachtet. </td> 
  </tr> 
  <tr> 
   <td>Filter, Ansichten und Gruppierungen</td> 
   <td>Der Eigentümer eines Filters, einer Ansicht oder einer Gruppierung ist der Ersteller. </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td><span>Pläne</span> </td> 
   <td> <p><span>Der Eigentümer ist der Ersteller des Plans.</span> </p> <p>Dies erfordert eine zusätzliche Lizenz. </p> <p><span>Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter</span> <a href="../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">Übersicht über den Szenario-Planer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
   <td>Ziele</td> 
   <td> <p>Der Eigentümer ist der Benutzer, der als Inhaber bezeichnet wurde. Sie sind möglicherweise nicht dieselbe Person wie der Ersteller des Ziels. </p> <p>Dies erfordert eine zusätzliche Lizenz. </p> <p>Weitere Informationen zu Workfront-Zielen finden Sie unter <a href="../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Übersicht über Adobe Workfront-Ziele</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>


