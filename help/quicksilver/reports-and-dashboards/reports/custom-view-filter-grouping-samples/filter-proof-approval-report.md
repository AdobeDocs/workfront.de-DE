---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Filter: Bericht zur Bestätigung der Genehmigung, um frühere Testversionen auszuschließen"
description: Sie können den Filter Aktuelle Dokumentversion verwenden, um in einem Bericht zur Bestätigung nur die aktuellen Testversionen aufzunehmen, die auf Ihre Genehmigung warten.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 0%

---

# Filter: Bericht zur Testbestätigung , um frühere Testversandversionen wegzulassen

<!--Audited: 10/2024-->

Sie können in einem Bericht zur Bestätigung des Testversands den Filter **Ist aktuelle Dokumentversion** verwenden, um nur die aktuellen Testversionen aufzunehmen, die auf Ihre Genehmigung warten.

Dies ist beispielsweise nützlich, wenn Sie aufgefordert wurden, Testsendungen mit mehreren Versionen zu genehmigen. Wenn Sie den Bericht über die Validierung des Testversands mit dem Filter Ist aktuelle Dokumentversion ausführen, listet der Bericht nur die aktuelle Version jedes Testversands auf, der auf Ihre Genehmigung wartet, wobei frühere Versionen weggelassen werden, an denen Sie nicht mehr arbeiten müssen.

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

## Filtern des Berichts zur Testbestätigung , um frühere Testversandversionen wegzulassen

Sie können einen Filter für einen Bericht zur Bestätigung des Testversands erstellen.

1. Wenn Sie bereits über einen Validierungsbericht verfügen, öffnen Sie diesen.

   Oder

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Um einen eigenen Bericht über die Genehmigung des Testversands zu erstellen, klicken Sie auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png) oben rechts oder auf das Symbol **Hauptmenü** ![](assets/lines-main-menu.png) oben links, falls verfügbar, und klicken Sie dann auf **Berichte** ![](assets/reports-in-main-menu.png).

1. Klicken Sie auf **Neuer Bericht**. Die Liste der Objekttypen wird angezeigt.
1. Klicken Sie in der Liste auf **Validierung testen** .
Die Berichterstellung wird geöffnet.
1. Klicken Sie auf **Filter** und dann auf **Filterregel hinzufügen**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Klicken Sie in das Feld **Filterregeln für Ihren Bericht festlegen** und wählen Sie dann **Testversand-Genehmigung** aus der Liste aus.
1. Klicken Sie in der Liste unter dem Objekt &quot;**Testversand der Genehmigung**&quot;auf &quot;**Ist aktuelle Dokumentversion**&quot;.
1. Wählen Sie für Ihren Filtermodifikator Gleich und dann True aus.
1. Klicken Sie links unten in Adobe Workfront auf **Speichern + Schließen** und dann im angezeigten Feld auf **Anwenden** .

   Der Bericht über die Validierung von Testsendungen zeigt nur Testsendungen an, die den aktuellen Versionen eines Dokuments zugeordnet sind, sofern Testversandgenehmigungen diesen Filterkriterien entsprechen.
