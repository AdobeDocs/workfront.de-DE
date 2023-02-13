---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Importieren von Projekten in Pläne im Szenario-Planer
description: Sie können vorhandene Projekte in einen Plan importieren. Die importierten Projekte werden in Initiativen umgewandelt, und Sie können sie innerhalb des Plans so verwalten, wie Sie eine neue Initiative durchführen würden. Das ursprüngliche Projekt bleibt mit der neuen Initiative verbunden.
author: Alina
feature: Workfront Scenario Planner
exl-id: 20429bb1-c158-433b-9790-325cd577248e
source-git-commit: 844dddec944b6cfb0957eecf09c2980e9d0577cc
workflow-type: tm+mt
source-wordcount: '1699'
ht-degree: 0%

---

# Importieren von Projekten in Pläne in [!DNL Scenario Planner]

Sie können vorhandene Projekte in einen Plan importieren. Die importierten Projekte werden in Initiativen umgewandelt, und Sie können sie innerhalb des Plans so verwalten, wie Sie eine neue Initiative durchführen würden. Das ursprüngliche Projekt bleibt mit der neuen Initiative verbunden.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: add information about what happens when you import projects and where the info from projects show up;</p>
<p>- the hours/ FTE come from WorkPerDay</p>
<p>- if a task has a Duration of 0, the FTE should be 0 for that asignee but it should still come across) </p>
</div>
-->

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> Plan*</b> </p> </td> 
   <td>[!UICONTROL Business] oder höher</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> license*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen.</p> <p>Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Konfigurationen auf Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] oder höher auf die [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektberechtigungen</strong> </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im Szenario-Planer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Überlegungen zum Import von Projekten in Pläne als neue Initiativen

* Sie müssen Projekte erstellen, bevor Sie sie als neue Initiativen in einen Plan importieren können.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: no caveats for project statuses yet, mentioned in the import steps as a tip) </p>
  -->

* Sie müssen mindestens [!UICONTROL Ansicht] Berechtigungen für die Projekte, damit sie als neue Initiative in einen Plan importiert werden können.
* Sie können dasselbe Projekt in mehrere Pläne importieren.
* Für die Projekte, die Sie importieren möchten, müssen Daten im Zeitrahmen Ihres Plans enthalten sein. Sie können keine Projekte mit einer [!UICONTROL Geplantes Abschlussdatum] vor Beginn des Plans oder [!UICONTROL Geplantes Startdatum] nach dem Ende des Plans.
* Sie können nicht mehr als 100 Projekte gleichzeitig importieren.
* Einige Projektinformationen werden ebenfalls in den Plan importiert und werden zu Initiativinformationen. Informationen darüber, welche Projektinformationen in den Plan importiert werden und zu Initiativinformationen werden, finden Sie im [Importierte Projektinformationen in den Plan](#project-information-imported-into-the-plan) in diesem Artikel.
* Änderungen an den verknüpften Projekten wirken sich nicht auf die Initiativen des Plans aus.
* Änderungen an den Initiativen im Plan wirken sich nicht automatisch auf die verknüpften Projekte aus. Änderungen der Initiative wirken sich nur dann auf die verknüpften Projekte aus, wenn Sie die Initiative aus dem Plan veröffentlichen. Informationen dazu, wie Veröffentlichungsinitiativen sich auf verknüpfte Projekte auswirken, finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
* Durch Löschen einer durch Importieren eines Projekts erstellten Initiative wird das Projekt nicht gelöscht.
* Durch das Löschen eines mit einer Initiative verknüpften Projekts wird die Initiative nicht gelöscht.

## Importierte Projektinformationen in den Plan {#project-information-imported-into-the-plan}

Wenn Sie ein Projekt in einen Plan importieren, werden auch einige Projektinformationen in den Plan importiert und zu Initiativinformationen. Die folgende Tabelle zeigt, aus welchen Projektinformationen beim Importieren eines Projekts in einen Plan Initiativinformationen werden:

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add what happens if you import a 5 year project to a 1 year plan - how does this display?) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Projektinformationen</td> 
   <td>Initiativinformationen </td> 
  </tr> 
  <tr> 
   <td>Projektname</td> 
   <td>Name der Initiative</td> 
  </tr> 
  <tr> 
   <td>Geplante Projektdaten</td> 
   <td> <p>Start- und Endmonate der Initiative.</p> <p>Beginnt oder endet ein Projekt in der Mitte eines Monats, werden die importierten Daten auf einen ganzen Monat im Plan erweitert. Wenn beispielsweise die geplanten Projektdaten der 20. März bis 5. Mai 2020 sind, dann sind die Daten der importierten Initiative März bis Mai 2020.</p> <p>Wenn das geplante Start- oder Abschlussdatum über die Dauer des Plans hinausgeht, gibt es einen visuellen Hinweis darauf, dass die importierte Initiative vor oder nach dem Plan beginnt. </p> </td> 
  </tr> 
  <tr> 
   <td>Aufgabenrollen, die Aufgaben und Problemen zugewiesen sind</td> 
   <td> <p>Aufgabengebiet für Initiative. </p> <p>Notiz:   <p>Wenn ein Benutzer während der Laufzeit des Projekts die Rollen ändert, hängen die importierten Rollen vom Status der Zuweisung beim Import des Projekts ab. Die folgenden Szenarien existieren:</p> 
     <ul> 
      <li> <p>Wenn ein Benutzer, der einer Aufgabe oder einem Problem zugewiesen wurde, seine Rolle geändert hat, nachdem er seine Zuweisung als [!UICONTROL Fertig] markiert hat, [!DNL Workfront] importiert in die Initiative die Rolle, die der Benutzer erfüllt hat, bevor er die Zuweisung als [!UICONTROL Fertig] markiert hat.</p> </li> 
      <li> <p>Wenn ein Benutzer, der einer Aufgabe oder einem Problem zugewiesen wurde, die Rolle während der Laufzeit des Projekts geändert hat, aber seine Zuweisung zu der Aufgabe oder dem Problem nicht als [!UICONTROL Fertig] markiert ist, wenn Sie das Projekt importieren, [!DNL Workfront] importiert nur die aktuelle Rolle des zugewiesenen Benutzers. </p> </li> 
     </ul> <p>Informationen zum Status einer Zuweisung finden Sie unter "Zuweisungsstatus"unter <a href="../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossar der Adobe [!DNL Workfront] Terminologie</a>. </p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projekt [!UICONTROL Geplante Stunden] im Zusammenhang mit Stellenrollen, die Aufgaben oder Problemen zugewiesen sind</td> 
   <td> <p><span>Je nachdem, ob der Plan für die Verwendung von FTEs oder Stunden eingerichtet wurde, werden die [!UICONTROL Planed Hours] aus den Aufgaben des Projekts entweder</span> [!UICONTROL Erforderliche FTEs] <span>oder [!UICONTROL Erforderliche Stunden] im Plan</span>. </p> <p>Informationen über die Einrichtung eines Plans zur Nutzung von FTEs oder Stunden finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]</a>. </p> <p>Beachten Sie Folgendes:</p> 
    <ul> 
     <li> <p>[!DNL Workfront] verwendet die Auftragsrollen, die Aufgaben und Problemen zugewiesen sind, oder die Auftragsrollen, mit denen die Benutzer, die Aufgaben oder Problemen zugewiesen sind, im Projekt verknüpft sind, und überträgt sie als "Erforderliche Auftragsrollen"in die neue Initiative. </p> </li> 
     <li> <p>Wenn der Plan für die Verwendung von FTEs eingerichtet ist, werden die Planstunden, die den Aufgaben und Problemen des Projekts zugeordnet sind, zunächst in eine FTE umgewandelt. Diese FTE wird dann der Aufgabe der Initiative übertragen. <span>Geplante Stunden sind gleichmäßig verteilt in [!DNL Workfront]. Wenn sich eine Aufgabe oder Ausgabe über mehrere Monate erstreckt, wird die für jeden Monat während der Dauer der Initiative geplante Zeitdauer in monatliche VZÄ umgerechnet und auf jeden Monat der Initiative übertragen.</span></p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><span>Wenn beispielsweise eine Aufgabe im September einer Stellenrolle für 80 geplante Stunden zugewiesen wird, zeigt die importierte Arbeitsplatzrolle im September 0,5 FTE für die Initiative an.</span> </p> </li> 
     <li> <p>[!DNL Workfront] berechnet anhand der folgenden Formel die FTE der mit der Initiative verknüpften Aufgaben "Erforderlicher Auftrag":</p> <p><code>Required Job Role FTE (initiative) = Job Role assignment Planned Hours (</code><code>from tasks and issues on the project)/ 160</code> </p> <p>Tipp: Die [!DNL Scenario Planner] geht davon aus, dass es 160 Arbeitsstunden pro Monat gibt.</p> <p>Beispiel: Wenn ein Projekt eine Dauer von 1200 Minuten hat und eine Rolle als Arbeitsplatz im Projekt mit 600 Minuten geplanter Stunden verknüpft ist, beträgt die VZÄ 0,5. Beim Import des Projekts beträgt die "Erforderliche Auftragsrolle" für die neu erstellte Initiative 0,5 für jeden Monat der Initiative. </p> </li> 
     <li>Wenn einer Aufgabe im Projekt eine berufliche Rolle zugewiesen wird, deren geplante Arbeitszeit null ist, ist die erforderliche FTE für die Stellenrolle der Initiative standardmäßig null. <!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         (NOTE: this used to be 1, not zero in Production) 
       </MadCap:conditionalText>
      --></li> 
     <li>Wenn einer Aufgabe im Projekt eine Stellenrolle mit einer [!UICONTROL Dauer] zugewiesen wird, wird die erforderliche FTE <span>oder Stunden</span> für die Stellenfunktion der Initiative standardmäßig null ist, selbst wenn die Aufgabe über geplante Stunden verfügt. </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>



## Importieren von Projekten in einen Plan

>[!IMPORTANT]
>
>Nach dem Import von Projekten in einen Plan werden sie zu Initiativen für den Plan. Obwohl die beiden Elemente verknüpft sind, existieren sie als unabhängige Entitäten und beeinflussen sich bei der Aktualisierung nicht automatisch gegenseitig.
>
>Folgendes geschieht:
>
>* Änderungen am Projekt wirken sich nicht auf die Initiative aus, nachdem Sie das Projekt in den Plan importiert haben. Diese Änderungen umfassen Änderungen an den Zuordnungen von Stellenrollen.
>
>  <!--
>  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change if projects will ever affect initiatives automatically) </p>>
>  -->
>
>* Änderungen der Initiative wirken sich auf die Informationen im [!DNL Scenario Planner] nur dann auf dem Projekt angezeigt werden, wenn Sie die Initiative im entsprechenden Projekt veröffentlichen. Andernfalls haben sie keine Auswirkungen auf die [!UICONTROL Geplante Stunden] Informationen zu den Aufgaben und Problemen des Projekts.
>
>  Informationen dazu, wie Veröffentlichungsinitiativen sich auf verknüpfte Projekte auswirken, finden Sie unter  [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im Szenario-Planer](../scenario-planner/publish-scenarios-update-projects.md).

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Workfront]Klicken Sie auf [!DNL Scenarios] , um auf die [!DNL Scenario Planner].

1. Klicken Sie auf den Namen eines Plans, aus dem Sie Projekte importieren möchten.
1. Klicken **[!UICONTROL Neue Initiative]** Klicken Sie auf **[!UICONTROL Projekte importieren]**.

   Die [!UICONTROL Projekte importieren] angezeigt. Projekte mit Datumsangaben im Zeitrahmen Ihres Plans werden in einer Liste angezeigt.

   ![](assets/project-import-ui-projects-selected-350x72.png)

   >[!TIP]
   >
   >Projekte mit einem beliebigen Status werden in der Liste angezeigt.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the status of the projects in the import projects UI might change; right now it's ALL statuses)</p>
   -->

1. (Optional) Klicken Sie auf die **[!UICONTROL Filtersymbol]** ![](assets/filter-nwepng.png)und wählen Sie einen verfügbaren Filter aus der Liste aus, um die Anzahl der Projekte in Ihrer Liste zu reduzieren. Standardmäßig wird die Projektliste durch den aktuell ausgewählten Projektfilter des Benutzers in einer Projektliste gefiltert.

1. (Optional) Klicken Sie auf die **[!UICONTROL Suchsymbol]** ![](assets/search-icon.png) und fügen Sie einen Suchbegriff hinzu, der in einem beliebigen Feld auf dem Bildschirm angezeigt wird. Die Elemente, die das Suchwort enthalten, werden automatisch in der Liste angezeigt und alle Elemente werden ausgeblendet.

1. (Bedingt) Klicken Sie auf die **[!UICONTROL X-Symbol]** , um die Suche zu entfernen und alle Projekte anzuzeigen.
1. Wählen Sie bis zu 100 Projekte aus und klicken Sie auf **[!UICONTROL Import]**.

   Die Projekte werden als neue Initiativen importiert.

   Beachten Sie Folgendes:

   * Ein Projektsymbol ![](assets/project-icon-sp.png) rechts neben dem Namen der Initiative angezeigt.
   * Überschreitet die Zeitleiste des Projekts die Dauer des Plans, endet der Balken der Initiative mit einem deutlichen Rand auf der linken Seite (wenn das Startdatum vor dem Datum des Plans liegt) oder auf der rechten Seite (wenn das Enddatum nach dem Datum des Plans liegt).

      ![](assets/project-bar-earlier-than-the-plan-start-date-350x39.png)

   * Die Anzahl der Monate und der Stellenrollen wurde aktualisiert und entspricht nun denen des Projekts.
   >[!TIP]
   >
   >Die mit den Stellenrollen verbundenen Kosten werden auf der Ebene der Initiative aktualisiert und nicht aus dem Projekt importiert.

1. Klicken Sie auf die Leiste, die die neue Initiative darstellt, um den Bereich für die Details der Initiative auf der rechten Seite zu öffnen.

   ![](assets/initiative-duration-with-project-duration-details-panel-350x292.png)

   Im **[!UICONTROL Dauer der Initiative]** -Bereich die folgenden Informationen überprüfen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Projektdauer]</td> 
      <td>Dies ist die Dauer der Initiative in Monaten. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative]</td> 
      <td>Beginn und Ende der Initiative. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Projekt]</td> 
      <td> <p>Das [!UICONTROL geplante Startdatum] und das [!UICONTROL Abschlussdatum] des verknüpften Projekts.</p> <p>Tipp: Wenn die Informationen zum [!UICONTROL Projekt] fehlen, wurde das Projekt gelöscht.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Bearbeiten Sie den Namen der Initiative. Standardmäßig stimmt sie mit dem Namen des Projekts überein.
1. (Optional) Führen Sie einen der folgenden Schritte aus:

   * Aktualisierung der Vorgangsrollen in der **[!UICONTROL Erforderliche Vorgangsrollen]** Abschnitt
   * Aktualisieren Sie die **[!UICONTROL Feste Kosten]** im **[!UICONTROL Kosten]** Abschnitt

   * Klicken **[!UICONTROL Verfügbare Vorgangsrollen aktualisieren]** oder **[!UICONTROL Verfügbares Budget aktualisieren]** die Beilegung von Konflikten zwischen der neuen Initiative und anderen Initiativen des Plans.

1. (Bedingt) Klicken Sie auf **[!UICONTROL Anwenden]** , um Änderungen an Ihrer Initiative zu speichern.
1. Klicken **[!UICONTROL Plan speichern]** , um die Änderungen an Ihrem Plan zu speichern.
1. (Optional) Um die Änderungen, die Sie an der Initiative vornehmen, wieder in das Projekt zu aktualisieren, aus dem sie importiert wurde, veröffentlichen Sie das Projekt aus dem Plan. Weitere Informationen zu Veröffentlichungsplänen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
1. (Optional) Klicken Sie auf das Projektsymbol, um auf das verknüpfte Projekt zuzugreifen.

   ![](assets/project-icon-on-initiative-highlighted-350x49.png)
