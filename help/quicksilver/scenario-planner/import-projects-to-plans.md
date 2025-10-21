---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Projekte in Pläne im Szenario-Planer importieren
description: Sie können vorhandene Projekte in einen Plan importieren. Die importierten Projekte werden in Initiativen umgewandelt, und Sie können sie innerhalb des Plans so verwalten, wie Sie es für eine neue Initiative tun würden. Das ursprüngliche Projekt bleibt mit der neuen Initiative verknüpft.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---

# Projekte in Pläne im [!DNL Scenario Planner] importieren

Sie können vorhandene Projekte in einen Plan importieren. Die importierten Projekte werden in Initiativen umgewandelt, und Sie können sie innerhalb des Plans so verwalten, wie Sie es für eine neue Initiative tun würden. Das ursprüngliche Projekt bleibt mit der neuen Initiative verknüpft.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Packstück</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>NOTIZ</b></p>
<p>Wenden Sie sich an Ihren Workfront-Support-Mitarbeiter, wenn Sie ein anderes Workfront-Paket haben.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Lizenz</p> </td> 
   <td> <p>[!UICONTROL light] oder höher</p> 
   <p>[!UICONTROL Überprüfung] oder höher</p> </td> 
  </tr> 
    <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf [!DNL Scenario Planner]</p> <p>Zugriff auf Projekte anzeigen oder höher.</p></td> 
  </tr> 
  <tr> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für einen Plan</p> <p>Zeigen Sie Berechtigungen für Projekte an oder erhöhen Sie diese.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zum Zugriff auf den Szenario-Planer finden Sie unter [Zugriff für die Verwendung des erforderlich [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen für Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> <p>View or higher access to Projects.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>View or higher permissions to projects.</p><p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements to Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Überlegungen zum Importieren von Projekten in Pläne als neue Initiativen

* Sie müssen Projekte erstellen, bevor Sie sie als neue Initiativen in einen Plan importieren können.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Sie müssen mindestens über [!UICONTROL Ansicht]-Berechtigungen für die Projekte verfügen, um sie als neue Initiative in einen Plan importieren zu können.
* Sie können dasselbe Projekt in mehrere Pläne importieren.
* Die Projekte, die Sie importieren möchten, müssen Datumsangaben im Zeitrahmen Ihres Plans enthalten. Sie können keine Projekte importieren[!UICONTROL &#x200B; deren geplantes Abschlussdatum vor dem Start des Plans &#x200B;] oder deren [!UICONTROL geplantes Startdatum] nach dem Ende des Plans liegt.
* Sie können nicht mehr als 100 Projekte gleichzeitig importieren.
* Einige Projektinformationen werden ebenfalls in den Plan importiert und werden zu Initiativinformationen. Informationen darüber, welche Projektinformationen in den Plan importiert werden und zu Initiativinformationen werden, finden Sie [&#x200B; Abschnitt „Projektinformationen in den Plan &#x200B;](#project-information-imported-into-the-plan)&quot; in diesem Artikel.
* Änderungen an den verknüpften Projekten wirken sich nicht auf die Initiativen des Plans aus.
* Änderungen an den Initiativen im Plan wirken sich nicht automatisch auf die Änderungen an den verknüpften Projekten aus. Änderungen an der Initiative wirken sich nur dann auf die verknüpften Projekte aus, wenn Sie die Initiative im Plan veröffentlichen. Informationen darüber, wie sich Veröffentlichungsinitiativen auf die verknüpften Projekte auswirken, finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* Beim Löschen einer Initiative, die durch den Import eines Projekts erstellt wurde, wird das Projekt nicht gelöscht.
* Wenn Sie ein mit einer Initiative verknüpftes Projekt löschen, wird die Initiative nicht gelöscht.

## In den Plan importierte Projektinformationen {#project-information-imported-into-the-plan}

Wenn Sie ein Projekt in einen Plan importieren, werden einige Projektinformationen ebenfalls in den Plan importiert und werden zu Initiativinformationen. Die folgende Tabelle zeigt, welche Projektinformationen zu Initiativinformationen werden, wenn Sie ein Projekt in einen Plan importieren:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Projektinformationen</td> 
   <td>Informationen zur Initiative </td> 
  </tr> 
  <tr> 
   <td>Projektname</td> 
   <td>Name der Initiative</td> 
  </tr> 
  <tr> 
   <td>Geplante Projektdaten</td> 
   <td> <p>Beginn und Ende der Initiative.</p> <p>Wenn ein Projekt in der Mitte eines Monats beginnt oder endet, werden die importierten Daten erweitert, um einen ganzen Monat im Plan abzudecken. Wenn die geplanten Projektdaten beispielsweise der 20. März bis 5. Mai 2020 sind, lauten die Daten der importierten Initiative März bis Mai 2020.</p> <p>Wenn das geplante Start- oder Abschlussdatum nach der Laufzeit des Plans liegt, gibt es einen visuellen Hinweis darauf, dass die importierte Initiative vor dem Plan beginnt oder nach diesem endet. </p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabengebiete zugewiesen zu Aufgaben und Problemen</td> 
   <td> <p>Aufgabengebiete der Initiative. </p> <p>Hinweis:   <p>Wenn ein(e) Benutzende(r) die Rollen während der Laufzeit des Projekts ändert, hängen die Rollen, die importiert werden, vom Status der Zuweisung beim Importieren des Projekts ab. Die folgenden Szenarien sind vorhanden:</p> 
     <ul> 
      <li> <p>Wenn ein(e) Benutzende(r), der/die einer Aufgabe oder einem Problem zugewiesen wurde, seine/ihre Rolle geändert hat, nachdem er/sie seine/ihre Zuweisung als [!UICONTROL Done] markiert hat, importiert [!DNL Workfront] die Rolle, die der/die Benutzende erfüllt hat, bevor er/sie die Zuweisung als [!UICONTROL Done] markiert hat.</p> </li> 
      <li> <p>Wenn ein(e) Benutzende(r), der/die einer Aufgabe oder einem Problem zugewiesen wurde, die Rolle während der Lebensdauer des Projekts geändert hat, aber seine/ihre Zuweisung zu der Aufgabe oder dem Problem beim Importieren des Projekts nicht als [!UICONTROL Done] markiert ist, importiert [!DNL Workfront] nur die aktuelle Rolle des/r zugewiesenen Benutzenden. </p> </li> 
     </ul> <p>Informationen zum Status eines Arbeitsauftrags finden Sie unter „Arbeitsauftragsstatus“ in <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossar der [!DNL Workfront] Terminologie von Adobe</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt [!UICONTROL Geplante Stunden] mit Aufgabengebieten verknüpft, die Aufgaben oder Problemen zugewiesen sind</td> 
   <td> <p><span>Je nachdem, ob der Plan für die Verwendung von FTEs oder Stunden eingerichtet ist, werden die [!UICONTROL Geplante Stunden] aus den Aufgaben für das Projekt entweder </span> [!UICONTROL Erforderliche FTEs] <span>oder [!UICONTROL Erforderliche Stunden] im Plan</span>. </p> <p>Informationen zum Einrichten eines Plans für die Verwendung von FTEs oder Stunden finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]</a>. </p> <p>Beachten Sie Folgendes:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] verwendet die Aufgabengebiete, die Aufgaben und Problemen zugewiesen sind, oder die Aufgabengebiete, mit denen die Benutzer im Projekt Aufgaben oder Problemen verknüpft sind, und überträgt sie nach Bedarf auf die neue Initiative. </p> </li> 
     <li> <p>Wenn der Plan für die Verwendung von FTEs eingerichtet ist, werden die geplanten Stunden, die den Aufgabengebieten für die Aufgaben und Probleme des Projekts zugeordnet sind, zunächst in FTEs konvertiert. Dieses VZÄ wird dann dem Aufgabengebiet der Initiative zugewiesen. <span>Die geplanten Stunden sind gleichmäßig auf [!DNL Workfront] verteilt. Wenn eine Aufgabe oder ein Problem mehrere Monate umfasst, wird die Anzahl der geplanten Stunden für jeden Monat während der Dauer der Initiative in monatliche VZÄ umgerechnet und auf jeden Monat der Initiative übertragen.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><span>Beispiel: Wenn eine Aufgabe im September einem Aufgabengebiet für 80 geplante Stunden zugewiesen wird, zeigt das importierte Aufgabengebiet im September 0,5 VZÄ für die Initiative an.</span> </p> </li> 
     <li> <p>[!DNL Workfront] Berechnet das FTE der erforderlichen Aufgabengebiete, die mit der Initiative verknüpft sind, nach folgender Formel:</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Tipp: Die [!DNL Scenario Planner] geht davon aus, dass ein Monat 160 Arbeitsstunden hat.</p> <p>Wenn beispielsweise ein Projekt eine Dauer von 1200 Minuten hat und ein Aufgabengebiet im Projekt mit 600 Minuten der geplanten Stunden verknüpft ist, beträgt ihr VZÄ 0,5. Beim Importieren des Projekts beträgt der erforderliche Aufgabengebiets-VZÄ der neu erstellten Initiative 0,5 für jeden Monat der Initiative. </p> </li> 
     <li>Wenn einer Aufgabe im Projekt ein Aufgabengebiet mit null geplanten Stunden zugewiesen wird, ist der erforderliche VZÄ für das Aufgabengebiet der Initiative standardmäßig null. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Wenn einer Aufgabe im Projekt mit einer Dauer von null  ein Aufgabengebiet zugewiesen wird, ist der erforderliche VZÄ (<span> Stunden) </span> Aufgabengebiet der Initiative standardmäßig null, auch wenn die Aufgabe über geplante Stunden verfügt. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Projekte in einen Plan importieren

>[!IMPORTANT]
>
>Nachdem Projekte in einen Plan importiert wurden, werden sie zu Initiativen im Plan. Obwohl die beiden Elemente verknüpft sind, existieren sie als unabhängige Entitäten und beeinflussen sich beim Aktualisieren nicht automatisch gegenseitig.
>
>Folgendes geschieht:
>
>* Änderungen am Projekt wirken sich nach dem Import des Projekts in den Plan nicht mehr auf die Initiative aus. Zu diesen Änderungen gehören Änderungen an den Zuweisungen für Aufgabengebiete.
>* Änderungen an der Initiative wirken sich nur dann auf die Informationen im [!DNL Scenario Planner] Bereich des Projekts aus, wenn Sie die Initiative im entsprechenden Projekt veröffentlichen. Andernfalls wirken sie sich nicht auf die [!UICONTROL Geplante Stunden] Informationen zu den Aufgaben und Problemen des Projekts aus.
>
>  Informationen darüber, wie sich Veröffentlichungsinitiativen auf die verknüpften Projekte auswirken, finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen im Szenario-Planer](../scenario-planner/publish-scenarios-update-projects.md).

{{step1-to-scenario-planner}}

1. Klicken Sie auf den Namen eines Plans, in den Sie Projekte importieren möchten.
1. Klicken Sie auf **[!UICONTROL Neue Initiative]** und dann auf **[!UICONTROL Projekte importieren]**.

   Das [!UICONTROL Projekte importieren] wird angezeigt. Projekte, deren Termine im Zeitrahmen Ihres Plans enthalten sind, werden in einer Liste angezeigt.

   ![Projekte importieren](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Projekte mit beliebigem Status werden in der Liste angezeigt.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Optional) Klicken Sie auf **[!UICONTROL Filtersymbol]** ![Filtersymbol](assets/filter-nwepng.png) und wählen Sie einen verfügbaren Filter aus der Liste aus, um die Anzahl der Projekte in Ihrer Liste zu reduzieren. Standardmäßig wird die Liste der Projekte nach dem aktuell ausgewählten Projektfilter der Benutzerin bzw. des Benutzers in einer Projektliste gefiltert.

1. (Optional) Klicken Sie auf **[!UICONTROL Suchsymbol]** ![Suchsymbol](assets/search-icon.png) und fügen Sie ein Keyword hinzu, das in einem beliebigen Feld auf dem Bildschirm angezeigt wird. Die Elemente, die das Suchwort enthalten, werden automatisch in der Liste angezeigt und alle Elemente sind ausgeblendet.

1. (Bedingt) Klicken Sie auf das Symbol **[!UICONTROL X]**, um die Suche zu entfernen und alle Projekte anzuzeigen.
1. Wählen Sie bis zu 100 Projekte aus und klicken Sie auf **[!UICONTROL Importieren]**.

   Die Projekte werden als neue Initiativen importiert.

   Beachten Sie Folgendes:

   * Rechts neben dem Namen ![&#x200B; Initiative wird &#x200B;](assets/project-icon-sp.png) Projektsymbol (Projektsymbol) angezeigt.
   * Wenn der Projektzeitplan die Dauer des Plans überschreitet, endet der Balken der Initiative mit einem spitzen Rand nach links (wenn das Startdatum vor dem Datum des Plans liegt) oder nach rechts (wenn das Enddatum nach dem Datum des Plans liegt).

     ![Projektleiste vor dem Startdatum](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * Die Anzahl der Monate und Aufgabengebiete wurde aktualisiert, damit sie denen des Projekts entsprechen.

   >[!TIP]
   >
   >Die mit den Aufgabengebieten verbundenen Kosten werden auf Initiativebene aktualisiert und nicht aus dem Projekt importiert.

1. Klicken Sie auf die Leiste für die neue Initiative, um das Bedienfeld mit den Details der Initiative auf der rechten Seite zu öffnen.

   ![Dauer der Initiative](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   Überprüfen Sie **[!UICONTROL Bereich „Dauer]** Initiative“ die folgenden Informationen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Dauer]</td> 
      <td>Dies ist die Dauer der Initiative in Monaten. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>Start- und Enddatum der Initiative. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL -Projekt]</td> 
      <td> <p>Der [!UICONTROL Geplanter Start] und die [!UICONTROL Abschlussdaten] des verknüpften Projekts.</p> <p>Tipp: Wenn die [!UICONTROL Project]-Informationen fehlen, wurde das Projekt gelöscht.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Bearbeiten Sie den Namen der Initiative. Standardmäßig entspricht dies dem Namen des Projekts.
1. (Optional) Führen Sie einen der folgenden Schritte aus:

   * Aktualisieren Sie Aufgabengebiete im Abschnitt **[!UICONTROL Erforderliche]**)
   * Aktualisieren Sie **[!UICONTROL Fixkosten]** im Abschnitt **[!UICONTROL Kosten]**

   * Klicken Sie auf **[!UICONTROL Verfügbare Aufgabengebiete aktualisieren]** oder **[!UICONTROL Verfügbares Budget aktualisieren]**, um Konflikte zwischen der neuen Initiative und anderen Initiativen im Plan zu lösen.

1. (Bedingt) Klicken Sie auf **[!UICONTROL Anwenden]**, um Änderungen an Ihrer Initiative zu speichern.
1. Klicken Sie **[!UICONTROL Plan speichern]**, um die Änderungen an Ihrem Plan zu speichern.
1. (Optional) Um die Änderungen an der Initiative in dem Projekt zu aktualisieren, aus dem sie importiert wurde, veröffentlichen Sie das Projekt aus dem Plan. Informationen zu Veröffentlichungsplänen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Optional) Klicken Sie auf das Projektsymbol, um auf das verknüpfte Projekt zuzugreifen.

   ![Projektsymbol auf Initiative](assets/project-icon-on-initiative-highlighted-350x49.png)
