---
title: Verwalten von Datensätzen im Planungsabschnitt von Adobe Workfront-Objekten
description: Sie können die Workfront-Planungsdatensätze, die mit Adobe Workfront-Objekten verbunden sind, im Planungsabschnitt eines Workfront-Objekts im linken Bereich anzeigen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '1828'
ht-degree: 0%

---


<!--add also Group and Company when they are available-->

# Verwalten von Datensatzverbindungen aus Workfront-Objekten

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

{{planning-important-intro}}

Sie können Workfront-Planungsdatensätze in Workfront in den folgenden Bereichen der mit ihnen verbundenen Objekte anzeigen:

* Der Abschnitt Planung eines Workfront-Objekts: Zeigt alle mit einem Objekt verbundenen Datensatztypen und die entsprechenden verbundenen Datensätze an.
* Benutzerdefiniertes Feld für Planning-Verbindung: Zeigt einen Datensatztyp, die entsprechenden verbundenen Datensätze und bis zu 7 Suchfelder der verbundenen Datensätze an.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
Oder
<li><p>Beliebiger Workflow und beliebiges Planungspaket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte, Programme und Portfolios</p>  
   <p>Es gibt keine Zugriffsebenen-Konfiguration für Workfront Planning. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <p>Zeigen Sie in Workfront Berechtigungen oder höhere Berechtigungen für ein Projekt, ein Portfolio oder ein Programm an</a> </p> 
   <p>In Workfront Planning:</p>
   <ul><li>Anzeigen von Berechtigungen für einen Arbeitsbereich und Datensatztyp zum Anzeigen verbundener Datensätze </li>
   Oder
   <li> Beitragen von oder höhere Berechtigungen zu einem Arbeitsbereich und Datensatztyp, um Datensätze zu verbinden oder zu trennen</a></li></ul> 
   <p>Systemadministratoren haben Berechtigungen für alle Workfront Planning-Arbeitsbereiche, einschließlich der nicht erstellten</p> 
  </td>
  </tr>   
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--Old:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Products</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront Planning<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any of the following Workfront plans:</p>
<ul><li>Select</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>Workfront Planning is not available for legacy Workfront plans</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td>
   <td>
<p>Any</p>
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront platform</p></td>
   <td>
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>View or higher access to Projects, Programs, and Portfolios</p>  
   <p>There is no access level configuration for Workfront Planning. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td>
   <p>In Workfront, View or higher permissions to a project, portfolio, or program</a> </p> 
   <p>In Workfront Planning:
   <ul><li>
   View permissions to a workspace and record type to view any connected records </li>
   or
   <li> Contribute or higher permissions to a workspace and record type  to connect or disconnect records</a></li></ul> </p>  
   <p>System Administrators have permissions to all Workfront Planning workspaces, including the ones they did not create</p> 
  </td>
  </tr>
 </tbody>
</table>-->


## Verwalten von Datensätzen im Abschnitt Planung

Sie können den Abschnitt Planung eines Workfront-Objekts verwenden, um alle Datensatztypen und deren jeweilige Datensätze anzuzeigen, die mit dem Workfront-Objekt verbunden sind.
Der Abschnitt Planung ist für die folgenden Workfront-Objekte verfügbar:

* Projekt
* Portfolio
* Programm
<!--* Group
* Company-->

### Überlegungen zum Planungsabschnitt von Workfront-Objekten

Beachten Sie Folgendes, wenn Sie Workfront-Planungsdatensätze im Planungsabschnitt eines Workfront-Objekts anzeigen:

* Workfront Planning-Datensatztypen müssen zunächst mit Workfront-Objekttypen verbunden werden.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Einträge verbinden](/help/quicksilver/planning/records/connect-records.md)
* Sie können den Planungsabschnitt über ein Workfront-Objekt anzeigen, selbst wenn keine Datensätze mit dem Workfront-Objekt verknüpft sind.
* <span class="preview">Ein Datensatztyp wird nur dann im Bereich Planung eines Workfront-Objekts angezeigt, wenn Sie beim Erstellen der Verbindung zwischen zwei Datensatztypen das entsprechende Feld in der Einstellung Verknüpfter Datensatztyp erstellen aktivieren.</span>

  Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

### Verwalten von Datensatzverbindungen über den Abschnitt Planung

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps, der mit einem Workfront-Projekt, -Portfolio oder -Programm verbunden ist.
1. Wechseln Sie zu einem verbundenen Datensatzfeld, das über eine Verbindung mit einem Workfront-Objekt verfügt, entweder in der Tabellenansicht oder auf der Detailseite eines Datensatzes. Weitere Informationen finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).
1. Klicken Sie auf den Namen eines Workfront-Objekts im Feld Verbundener Datensatz .
Die Seite des -Objekts wird in Workfront geöffnet.

   >[!NOTE]
   >
   >  Wenn Sie wissen, dass ein Workfront-Objekt bereits mit einem Planning-Datensatz verbunden ist, können Sie vom Workfront-Objekt zum Planning-Abschnitt navigieren.

1. Klicken **im linken** auf „Planung“.

   >[!NOTE]
   >
   >   Ihr Workfront- oder Gruppenadministrator muss der Layoutvorlage den Abschnitt Planung hinzufügen, bevor sie für ein Workfront-Projekt, -Portfolio oder -Programm angezeigt wird.

   Der Abschnitt Planung wird mit den folgenden Informationen angezeigt:

   * Die verbundenen Datensätze werden auf einzelnen Karten mit den folgenden Informationen angezeigt:
      * Name des Datensatzes
      * Die Miniaturansicht des Datensatzes
      * Der Name des verbundenen Datensatzfelds, wie er in Workfront Planning angezeigt wird.
   * Datensätze werden unter ihrem jeweiligen Arbeitsbereich und Datensatztyp angezeigt.

   ![Planungsabschnitt zum Projekt](assets/planning-section-on-project.png)

1. (Optional) Klicken Sie auf **Alle Verbindungen anzeigen** um alle verbundenen Datensatztypen anzuzeigen, einschließlich der Typen ohne verbundene Datensätze. Standardmäßig werden Datensatztypen ohne verbundene Datensätze nicht angezeigt.
1. Klicken Sie auf eine Datensatzkarte, um weitere Informationen zum Datensatz anzuzeigen. Das Datensatzvorschau-Feld wird angezeigt.
1. (Optional) Beginnen Sie mit der Bearbeitung von Feldern im Vorschaufeld des Datensatzes. Ihre Änderungen werden automatisch gespeichert.
1. (Optional) Klicken Sie auf **In einer neuen Registerkarte öffnen** Symbol ![Details in einer neuen Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) in der oberen rechten Ecke des Vorschaufelds, um die Detailseite des Datensatzes zu öffnen. Die Detailseite des Datensatzes wird in Workfront Planning geöffnet.
1. (Optional) Bewegen Sie den Mauszeiger über eine Datensatzkarte und klicken Sie dann auf das Symbol zum Trennen des Datensatzes **-** und anschließend auf **Trennen**.
Folgendes geschieht:
   * Der Datensatz ist nicht mehr mit dem Workfront-Objekt verbunden.
   * Das Workfront-Objekt wird auch aus dem verknüpften Feld des Datensatzes aus Workfront Planning entfernt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden ebenfalls gelöscht.
1. Klicken Sie **Verbinden**, um weitere Datensätze für die verbundenen Datensatztypen zu verbinden.

   Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).
1. (Optional) Wenn Sie einen Datensatz für die Verbindung nicht finden können und Sie ihn hinzufügen möchten, klicken Sie auf **+ Hinzufügen**, um einen neuen Datensatz hinzuzufügen. Weitere Informationen finden Sie im Abschnitt „Erstellen von Datensätzen, während Sie sie mit anderen Datensätzen verbinden“ im Artikel [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

   Folgendes geschieht:

   * Die Datensätze werden sofort mit dem Workfront-Objekt verbunden und im Abschnitt Planung angezeigt.
   * Das Workfront-Objekt wird dem verbundenen Feld des Workfront-Planungsdatensatzes hinzugefügt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden in Workfront Planning ausgefüllt.

## Verwalten von Datensätzen im Verbindungs-Feldtyp „Planung“

Sie können ein benutzerdefiniertes Feld für Planning-Verbindungen in einem Workfront-Objekt verwenden, um einen Datensatztyp und die entsprechenden Datensätze anzuzeigen, die mit dem Workfront-Objekt verbunden sind.

Sie können steuern, welche Planning-Datensatztypen für das Workfront-Objekt angezeigt werden, wenn Sie benutzerdefinierte Felder für die Planning-Verbindung erstellen.

* Das Feld Planning-Verbindung zeigt Planungsdatensätze an, nachdem eine Verbindung hergestellt wurde und wenn das Feld für die folgenden Workfront-Objekte an Formulare angehängt wird:

   * Projekt
   * Portfolio
   * Programm
   * Gruppe
   * Firma

Weitere Informationen finden Sie unter [Formular erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Überlegungen zum Planungs-Verbindungs-Feldtyp

Beachten Sie Folgendes, wenn Sie Workfront-Planungsdatensätze über ein Feld für die Planning-Verbindung eines Workfront-Objekts anzeigen:

* Ein Feld für die Planning-Verbindung wird im benutzerdefinierten Formular eines Workfront-Objekts wie folgt angezeigt, nachdem Planning-Datensätze mit dem Workfront-Objekt verknüpft wurden:

   * Wenn nur das primäre Feld des verbundenen Datensatzes ausgewählt ist, wird das Feld Planning-Verbindung als Feld mit mehreren Werten angezeigt, wenn die Verbindung die Verknüpfung mehrerer Datensätze zulässt. Weitere Informationen finden Sie unter [Übersicht über Datensatztypen verbinden](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
   * Wenn Ihr Workfront- oder Gruppenadministrator bzw. Ihre Gruppenadministratorin zusätzliche Suchfelder aus dem verbundenen Datensatz im benutzerdefinierten Formular hinzugefügt hat, wird das Feld „Planning-Verbindung“ als Tabelle angezeigt. Für das Feld Verbindung planen können bis zu 7 Felder ausgewählt werden. Die Tabellenansicht ist schreibgeschützt.

* Es kann nur ein Datensatztyp mit einem Planning-Verbindungsfeld verknüpft werden. Die Anzahl der Planning-Verbindungsfelder in einem Formular ist unbegrenzt.
* Sie müssen über die richtigen Zugriffsrechte und Berechtigungen für das Objekt, den Datensatz und Workfront Planning verfügen, um ein benutzerdefiniertes Formular mit einem benutzerdefinierten Feld für die Planning-Verbindung an ein Workfront-Objekt anzuhängen.
* Sie müssen Beitragsberechtigungen für einen Arbeitsbereich in Workfront Planning besitzen, um Datensätze mit dem Feld Planning-Verbindung eines Workfront-Objekts verbinden oder trennen zu können.
* Workfront Planning-Datensatztypen müssen zunächst mit Workfront-Objekttypen verbunden werden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md). Dadurch können die Workfront-Planungsdatensätze von Workfront aus aufgerufen werden.
* Sie können Datensätze nur für Objekte, die Workfront Planning-Verbindungen aufweisen können, mit dem Feld Planning-Verbindung eines Workfront-Objekts verbinden oder davon trennen.

  Beispielsweise können Sie möglicherweise ein benutzerdefiniertes Formular mit einem Feld für eine Planning-Verbindung an Aufgaben anhängen, Sie können jedoch keine Workfront Planning-Objekte mit Aufgaben verbinden.
* Ein Planning-Verbindungsfeld kann nicht bearbeitet werden, wenn Workfront-Objekte stapelweise bearbeitet werden.
* <span class="preview">Ein Datensatztyp wird in einem benutzerdefinierten Feld von Planning-Verbindung eines Workfront-Objekts nur angezeigt, wenn Sie beim Erstellen der Verbindung zwischen zwei Datensatztypen die Einstellung Entsprechendes Feld erstellen in der Einstellung Verknüpfter Datensatztyp aktivieren.</span>

  Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

### Verwalten von Datensatzverbindungen über den Feldtyp Planungsverbindung

1. Wechseln Sie zu einem der folgenden Objekttypen, die mit einem Workfront Planning-Datensatztyp verbunden wurden:

   * Projekt
   * Portfolio
   * Programm
   * Firma
   * Gruppe

1. Klicken Sie im linken Bedienfeld auf **&lt; Objekt**> Details.
1. (Bedingt) Fügen Sie ein benutzerdefiniertes Formular mit mindestens einem Planning-Verbindungsfeld für das ausgewählte Objekt hinzu, wenn kein solches Feld vorhanden ist.

   >[!NOTE]
   >
   >Ihr Workfront- oder Gruppenadministrator muss zunächst das Formular erstellen und ein Feld für die Planning-Verbindung hinzufügen, bevor Sie es einem Objekt hinzufügen können.


1. Klicken Sie in das Feld, um verbundene Datensätze hinzuzufügen, und klicken Sie dann auf den nach unten zeigenden Pfeil innerhalb des Felds, um Datensätze aus der Liste auszuwählen.

   ![Planen eines Verbindungsfelds in einem Projekt mit geöffneter Datensatzliste](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Sie können keine Datensätze zu Planning-Verbindungsfeldern hinzufügen, die mit anderen Workfront-Objekten als dem Objekt verknüpft sind, das Sie beim Konfigurieren des Felds ausgewählt haben.
   >
   >Sie können beispielsweise keine Datensätze zu einem Planning-Verbindungsfeld hinzufügen, das für eine Portfolio-Verbindung aus dem benutzerdefinierten Formular eines Projekts erstellt wurde.
   >
   >Es gibt einen Hinweis darauf, dass das Objekt des Felds und das ausgewählte Objekt nicht übereinstimmen.
   >
   >![Warnung: Nicht unterstütztes Objekt-Planungs-Verbindungsfeld im Formular](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Klicken Sie auf eine Stelle außerhalb der Liste, um sie zu schließen.

   Folgendes geschieht:

   * Die Datensätze werden sofort mit dem Workfront-Objekt verbunden und im Feld Planning-Verbindung sowie im Abschnitt Planning des Workfront-Objekts angezeigt.
   * Das Workfront-Objekt wird dem verbundenen Feld des Workfront-Planungsdatensatzes hinzugefügt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden in Workfront Planning ausgefüllt.
   * Wenn Ihr Workfront- oder Gruppen-Administrator beim Erstellen des benutzerdefinierten Formulars Datensatzsuchfelder hinzugefügt hat, werden die Suchfelder des Datensatzes automatisch in einer Tabellenansicht ausgefüllt. Die Tabellenansicht im Feld Planning-Verbindung ist schreibgeschützt.

     ![Planen eines Verbindungsfelds mit einer Tabelle im benutzerdefinierten Formular „Projektdetails“](assets/planning-connection-field-with-table-on-project-details-custom-form.png)

     >[!NOTE]
     >
     >Die Tabellenansicht wird nur angezeigt, wenn dem Feld Planning-Verbindungen im benutzerdefinierten Formular Suchfelder hinzugefügt wurden.


1. (Optional) Klicken Sie auf den Namen eines Datensatzes oder bewegen Sie den Mauszeiger über den Namen des Datensatzes in der Tabelle und klicken Sie dann auf das Symbol **Datensatz öffnen** ![Symbol „Datensatz öffnen“ im benutzerdefinierten Formular „Planning-Verbindung](assets/open-record-icon-on-planning-connection-custom-form.png) im Feld „Planning-Verbindung“, um den Datensatz in Workfront Planning zu öffnen.
Das Vorschaufeld mit den Details der Workfront-Planungsdatensätze wird geöffnet.
1. Überprüfen oder bearbeiten Sie Informationen zum Datensatz oder klicken Sie auf das Symbol **In neuer Registerkarte öffnen** ![Datensatz in neuer Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png), um die Seite mit den Datensatzdetails zu öffnen.

1. (Optional) Klicken Sie im benutzerdefinierten Formular in Workfront auf das Symbol **Entfernen** ![Symbol Entfernen](assets/remove-icon.png) in einem Datensatz, um ihn aus dem Feld „Planning-Verbindung“ zu entfernen und vom Workfront-Objekt zu trennen.
Das Workfront-Objekt wird vom Planungsdatensatz getrennt und alle Suchinformationen aus Workfront werden aus dem Datensatz entfernt.

1. Klicken Sie **Änderungen speichern**, um das benutzerdefinierte Formular und alle anderen Änderungen zu speichern, die Sie am Workfront-Objekt vorgenommen haben.
