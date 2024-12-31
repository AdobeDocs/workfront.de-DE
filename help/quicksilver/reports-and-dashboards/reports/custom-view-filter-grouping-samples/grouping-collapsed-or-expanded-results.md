---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Gibt an, ob die Ergebnisse einer Gruppierung im Textmodus reduziert oder erweitert werden sollen'
description: 'Gruppierung: Gibt an, ob die Ergebnisse einer Gruppierung im Textmodus reduziert oder erweitert werden sollen'
author: Nolan
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Gruppierung: Gibt an, ob die Ergebnisse einer Gruppierung im Textmodus reduziert oder erweitert werden sollen

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

Mit dem standardmäßigen Report Builder können Sie angeben, ob die Ergebnisse in einer Gruppierung in einer Liste oder einem Bericht reduziert oder erweitert angezeigt werden sollen. Die Ergebnisse in einer Gruppierung werden standardmäßig erweitert angezeigt. Informationen zum Erstellen einer Gruppierung finden Sie unter [Gruppierungen in Adobe Workfront erstellen](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Wenn Sie beim Anzeigen einer Liste Gruppierungen manuell anpassen, speichert Adobe Workfront Ihre manuellen Einstellungen, bis Sie sich abmelden. Beim erneuten Anmelden wird die Liste entsprechend dieser Einstellung angezeigt.
>* Die Ergebnisse einer Gruppierung werden immer erweitert angezeigt, nachdem über ein Diagrammelement darauf zugegriffen wurde.
>

Sie können auch im Textmodus angeben, ob eine Gruppierung erweitert oder reduziert angezeigt werden soll.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gibt an, ob die Ergebnisse einer Gruppierung im Textmodus reduziert oder erweitert werden sollen

1. Navigieren Sie zu einer Liste von Objekten.
1. Wählen Sie aus dem **Gruppierung** Dropdown-Menü **Neue Gruppierung** aus.

1. Fügen Sie eine Gruppierung hinzu und klicken Sie dann auf **In Textmodus wechseln**.

   Oder

   Wenn sich die Gruppierung bereits im Textmodus befindet, fügen Sie der Gruppierungsebene, die reduziert angezeigt werden soll, den folgenden Code hinzu:

   `group.0.iscollapsed=true`

1. (Optional) Wenn die Gruppierung erweitert angezeigt werden soll, fügen Sie der entsprechenden Gruppierungsebene den folgenden Code hinzu:

   `group.0.iscollapsed=false`

1. Klicken Sie **Fertig** und dann **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Namen der Gruppierung und klicken Sie dann auf **Gruppierung speichern**.
