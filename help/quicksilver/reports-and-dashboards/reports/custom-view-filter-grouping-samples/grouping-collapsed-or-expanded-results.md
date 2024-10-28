---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Geben Sie an, ob die Ergebnisse einer Gruppierung mithilfe des Textmodus reduziert oder erweitert werden sollen.'
description: 'Gruppierung: Geben Sie an, ob die Ergebnisse einer Gruppierung im Textmodus reduziert oder erweitert werden sollen.'
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

Mithilfe des standardmäßigen ReportBuilder können Sie angeben, ob die Ergebnisse in einer Gruppierung in einer Liste oder in einem Bericht ausgeblendet oder erweitert werden sollen. Die Ergebnisse einer Gruppierung werden standardmäßig erweitert. Informationen zum Erstellen einer Gruppierung finden Sie unter [Erstellen von Gruppierungen in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* Wenn Sie Gruppierungen bei der Anzeige einer Liste manuell anpassen, behält sich Adobe Workfront Ihre manuellen Voreinstellungen vor, bis Sie sich abmelden. Wenn Sie sich wieder anmelden, wird die Liste entsprechend dieser Einstellung angezeigt.
>* Die Ergebnisse einer Gruppierung werden immer erweitert, nachdem sie über ein Diagrammelement aufgerufen wurden.
>

Sie können auch angeben, ob eine Gruppierung mithilfe des Textmodus erweitert oder reduziert angezeigt werden soll.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gibt an, ob die Ergebnisse einer Gruppierung mithilfe des Textmodus reduziert oder erweitert werden sollen

1. Navigieren Sie zu einer Liste von Objekten.
1. Wählen Sie aus dem Dropdownmenü **Gruppierung** die Option **Neue Gruppierung** aus.

1. Fügen Sie eine Gruppierung hinzu und klicken Sie dann auf **In den Textmodus wechseln**.

   Oder

   Wenn sich die Gruppierung bereits im Textmodus befindet, fügen Sie den folgenden Code zur Gruppierungsebene hinzu, die ausgeblendet angezeigt werden soll:

   `group.0.iscollapsed=true`

1. (Optional) Wenn die Gruppierung erweitert werden soll, fügen Sie den folgenden Code zur entsprechenden Gruppierungsebene hinzu:

   `group.0.iscollapsed=false`

1. Klicken Sie auf **Fertig** und dann auf **Gruppierung speichern**.
1. (optional) Aktualisieren Sie den Namen der Gruppierung und klicken Sie dann auf **Gruppierung speichern**.
