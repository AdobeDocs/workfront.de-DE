---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filter: Bericht zu Korrekturabzugsgenehmigungen zum Auslassen früherer Korrekturabzugsversionen'
description: In einem Bericht zu Korrekturabzugsgenehmigungen können Sie den Filter Ist aktuelle Dokumentversion verwenden, um nur die aktuellen Versionen von Korrekturabzügen einzubeziehen, die auf Ihre Genehmigung warten.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Filter: Bericht zu Korrekturabzugsgenehmigungen , um frühere Korrekturabzugsversionen wegzulassen

<!--Audited: 10/2024-->

In einem Bericht zu Korrekturabzugsgenehmigungen können Sie den Filter **Ist aktuelle Dokumentversion** verwenden, um nur die aktuellen Versionen von Korrekturabzügen einzubeziehen, die auf Ihre Genehmigung warten.

Dies ist beispielsweise nützlich, wenn Sie aufgefordert wurden, Korrekturabzüge zu genehmigen, die mehrere Versionen haben. Wenn Sie den Bericht zu Korrekturabzugsgenehmigungen mit dem Filter Ist aktuelle Dokumentversion ausführen, listet der Bericht nur die aktuelle Version jedes Korrekturabzugs auf, der auf Ihre Genehmigung wartet, wobei frühere Versionen weggelassen werden, an denen Sie nicht mehr arbeiten müssen.

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
   <td> 
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtern Sie den Bericht zu Korrekturabzugsgenehmigungen, um frühere Korrekturabzugsversionen wegzulassen.

Sie können einen Filter für einen Bericht zu Korrekturabzugsgenehmigungen erstellen.

1. Wenn Sie bereits über einen Bericht zu Korrekturabzugsgenehmigungen verfügen, öffnen Sie ihn.

   Oder

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Um einen eigenen Bericht zu Korrekturabzugsgenehmigungen zu erstellen, klicken Sie auf das Symbol **Hauptmenü** (Symbol ![ Hauptmenü](assets/main-menu-icon.png) in der oberen rechten Ecke oder auf das Symbol **Hauptmenü** ![Hauptmenüzeilen](assets/lines-main-menu.png) in der oberen linken Ecke, falls verfügbar, und klicken Sie dann auf **Berichte** ![Berichte](assets/reports-in-main-menu.png).

1. Klicken Sie **Neuer Bericht**. Die Liste der Objekttypen wird angezeigt.
1. Klicken Sie **der Liste**Korrekturabzug-Genehmigung“.
Report Builder wird geöffnet.
1. Klicken Sie **Filter** und anschließend auf **Filterregel hinzufügen**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Klicken Sie in das **Filterregeln für Ihren Bericht festlegen** und wählen Sie dann **Korrekturabzugsgenehmigung** aus der Liste aus.
1. Klicken Sie **Ist aktuelle Dokumentversion** in der Liste unter dem Objekt **Korrekturabzugsgenehmigung**.
1. Wählen Sie für Ihren Filtermodifikator Gleich und dann Wahr aus.
1. Klicken Sie **Speichern + Schließen** in der linken unteren Ecke von Adobe Workfront und klicken Sie dann in **angezeigten** auf „Anwenden“.

   Der Bericht zu Korrekturabzugs-Genehmigungen zeigt nur Korrekturabzüge an, die mit den aktuellen Versionen eines Dokuments verknüpft sind, wenn Genehmigungen von Korrekturabzügen diesen Filterkriterien entsprechen.
