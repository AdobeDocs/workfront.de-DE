---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Herstellen einer Verbindung mit Workfront Data Connect
description: Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business-Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 10%

---

# Herstellen einer Verbindung mit Workfront Data Connect

Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business-Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.

Um Ihren Data Connect Data Lake mit einem externen Produkt zu verbinden, müssen Sie zunächst eine Verbindung erstellen, wie in [Erstellen eines Leserkontos oder einer Verbindung für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) beschrieben. Anschließend müssen Sie der Zulassungsliste alle erforderlichen IPs hinzufügen, wie unter [Hinzufügen von IPs zur Zulassungsliste](#add-ips-to-the-allowlist) unten beschrieben.

Für die meisten Produkte werden die folgenden Informationen zu Ihrem Data Lake erforderlich sein, um eine Verbindung herzustellen:

| Feldname | Wert |
|---------------|-------------|
| Server | Die URL für die Verbindung ohne den `https://`-Teil (auf der Seite **Data Connect** in Workfront*) |
| Port | `443` |
| Datenbank | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Rolle | `READER_ROLE` |
| Benutzername | Der beim Verbindungsaufbau ausgewählte Benutzername (in Workfront* auf der Seite **Data Connect**) |
| Kennwort | Das bei der ersten Snowflake-Anmeldung gewählte Kennwort* |

*Informationen darüber, wo Sie die Seite **Data Connect** mit Ihren Verbindungen finden, finden Sie unter [Erstellen eines Leserkontos oder einer Verbindung für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Sobald ein Eintrag zur IP-Zulassungsliste hinzugefügt wurde, sind alle anderen IP-Adressen nicht mehr zulässig. Stellen Sie sicher, dass Sie alle erforderlichen IP-Adressen eingegeben haben, sowohl für das Erstellungs- als auch für das Leseerlebnis Ihres Visualisierungs-Tools, bevor Sie versuchen, das Tool zu verwenden. Andernfalls wird möglicherweise ein Fehler in Bezug auf ungültige Anmeldeinformationen angezeigt.
>
>Wenn Sie keine IP-Adressen in Ihrer Zulassungsliste aufgeführt haben, aber immer noch Probleme beim Herstellen einer Verbindung mit einem BI-Tool haben, überprüfen Sie die Proxy-Serverkonfiguration für das BI-Tool.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen von IPs zur Zulassungsliste

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenverbindung**.

1. Klicken Sie auf die Registerkarte **Zulässige IPs**, und klicken Sie dann auf die Schaltfläche **IP-Adresse zu Ihrer Liste hinzufügen**.

1. Geben Sie in der **IP-Adressbeschreibung** einen Namen für die IP-Adresse ein und geben Sie die IP-Adresse (oder den CIDR-Block) für das Tool ein, das Sie in **IP-Adresse** verwenden möchten. Klicken Sie dann auf **IP zur Zulassungsliste hinzufügen**.

   ![IP-Adresse hinzufügen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Entfernen einer IP-Adresse aus der Liste der zulässigen Adressen

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke, und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bereich auf **System** > **Datenverbindung**.

1. Klicken Sie auf die Registerkarte **Zulässige IPs**, und klicken Sie dann auf das Papierkorbsymbol ![Löschen](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben der IP-Adresse, die Sie entfernen möchten.

1. Markieren Sie im eingeblendeten Fenster das Kontrollkästchen zur Bestätigung und klicken Sie dann auf **Löschen**.

## Freigeben von Daten mit Business Intelligence-Tools

Nachfolgend finden Sie eine Reihe gängiger Business Intelligence-Tools. Weitere Informationen zur Verbindung mit Ihrem Data Lake finden Sie auf den entsprechenden Dokumentations-Sites.

* Tableau
* Power BI
* Domo
* SAP HANA

## Daten in einem externen Data Warehouse speichern

Nachfolgend sind einige gängige Data Warehouses aufgeführt. Besuchen Sie deren Dokumentationsseiten, um mehr über die Verbindung zu Ihrem Data Lake zu erfahren.

* Databricks
* AWS Redshift
