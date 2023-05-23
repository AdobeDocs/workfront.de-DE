---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '''Filter: Validierungsbericht zum Weglassen früherer Testversionen'
description: Sie können den Filter Aktuelle Dokumentversion verwenden, um in einem Bericht zur Bestätigung nur die aktuellen Testversionen aufzunehmen, die auf Ihre Genehmigung warten.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Filter: Bericht zur Testbestätigung , um frühere Testversandversionen wegzulassen

In einem Bericht zur Testbestätigung können Sie die Variable **Ist aktuelle Dokumentversion** filtern, um nur die aktuellen Versionen von Testsendungen einzuschließen, die auf Ihre Genehmigung warten.

Dies ist beispielsweise nützlich, wenn Sie aufgefordert wurden, Testsendungen mit mehreren Versionen zu genehmigen. Wenn Sie den Bericht über die Validierung des Testversands mit dem Filter Ist aktuelle Dokumentversion ausführen, listet der Bericht nur die aktuelle Version jedes Testversands auf, der auf Ihre Genehmigung wartet, wobei frühere Versionen weggelassen werden, an denen Sie nicht mehr arbeiten müssen. 

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Filteränderung anfordern </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Filtern des Berichts zur Testbestätigung , um frühere Testversandversionen wegzulassen

1. Wenn Sie bereits über einen Validierungsbericht verfügen, öffnen Sie diesen.

   Oder

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Um einen eigenen Bericht zur Validierung des Testversands zu erstellen, klicken Sie auf das Hauptmenü ![](assets/main-menu-icon.png)Klicken Sie auf **Berichte** ![](assets/reports-in-main-menu.png). Klicken **Neuer Bericht**. Scrollen Sie in der angezeigten Liste zu und klicken Sie auf **Validierung des Testversands**. Klicken **Speichern und schließen**, geben Sie einen **Berichtsname** (optional) und klicken Sie auf **Bericht speichern**.

1. Klicken **Berichtaktionen > Bearbeiten**.
1. Klicken **Filter** Klicken Sie auf **Filterregel hinzufügen**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Klicken **Validierung des Testversands**.
1. Klicken Sie in der angezeigten Liste auf **Ist aktuelle Dokumentversion**.
1. Klicken **Speichern und schließen** Klicken Sie in der linken unteren Ecke von Adobe Workfront auf **Bericht speichern** in das Feld, das angezeigt wird.
