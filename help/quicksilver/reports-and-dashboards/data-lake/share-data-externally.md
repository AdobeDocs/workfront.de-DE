---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: Herstellen einer Verbindung zum Workfront Data Lake
description: Mit Workfront Data Lake können Sie die Workfront-Daten Ihres Unternehmens mit beliebten Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# Herstellen einer Verbindung zum Workfront Data Lake

Mit Workfront Data Lake können Sie die Workfront-Daten Ihres Unternehmens mit Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.

Um Ihre Workfront Data Lake-Daten mit einem externen Produkt zu verbinden, müssen Sie zunächst erforderliche IPs zur Zulassungsliste hinzufügen, wie unter [Hinzufügen von IPs zur Zulassungsliste](#add-ips-to-the-allowlist) unten. Darüber hinaus benötigen die meisten Produkte zusätzliche Informationen über Ihren Data Lake, um eine Verbindung herzustellen:

| Feldname | Wert |
|---------------|-------------|
| Server | Die URL für die Verbindung ohne `https://` -Teil (gefunden in der **Datenzugriff** Seite in Workfront*) |
| Port | `443` |
| Datenbank | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Funktion | `READER_ROLE` |
| Benutzername | Der beim Erstellen der Verbindung ausgewählte Benutzername (befindet sich auf der **Datenzugriff** Seite in Workfront*) |
| Kennwort | Das bei der ersten Snowflake-Anmeldung ausgewählte Kennwort* |

*Informationen darüber, wo Sie die **Datenzugriff** Seite, die Ihre Data Lake-Verbindungen enthält, siehe [Erstellen eines Leserkontos (Dienstkontos) für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Nachdem ein Eintrag zur IP-Zulassungsliste hinzugefügt wurde, sind alle anderen IP-Adressen nicht mehr zulässig. Stellen Sie sicher, dass Sie alle erforderlichen IP-Adressen - sowohl für die Erstellung als auch für die Lektüre Ihres Visualisierungs-Tools - eingegeben haben, bevor Sie versuchen, das Tool zu verwenden. Andernfalls kann es zu einem Fehler bezüglich ungültiger Anmeldedaten kommen.

## Hinzufügen von IPs zur Zulassungsliste

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **Einrichtung**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicken Sie auf **Zulässige IPs** und klicken Sie auf die **Hinzufügen einer IP-Adresse zu Ihrer Zulassungsliste** Schaltfläche.

1. Geben Sie einen Namen für die IP-Adresse in **Beschreibung der IP-Adresse** und geben Sie die IP-Adresse für das Tool ein, das Sie in verwenden möchten **IP-Adresse** Klicken Sie auf **Hinzufügen von IP-Adresse zur Zulassungsliste**.

   ![IP-Adresse hinzufügen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Entfernen einer IP-Adresse aus der Zulassungsliste

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **Einrichtung**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicken Sie auf **Zulässige IPs** Registerkarte und dann auf das Papierkorbsymbol ![Löschsymbol](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben der IP-Adresse, die Sie entfernen möchten.

1. Markieren Sie im sich öffnenden Fenster das zu validierende Kästchen und klicken Sie auf **Löschen**.

## Datenfreigabe mit Business Intelligence-Tools

Unten finden Sie eine Reihe häufig verwendeter Business Intelligence-Tools. Über die Links gelangen Sie zur Dokumentations-Site des Dienstes, um mehr über die Verbindung mit Ihrem Data Lake zu erfahren.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Daten in einem externen Data Warehouse speichern

Unten finden Sie eine Reihe gemeinsamer Data Warehouse-Informationen. Über die Links gelangen Sie auf die Dokumentations-Site jedes Dienstes, auf der Sie mehr über die Anbindung an Ihren Data Lake erfahren.

* [Datenricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
