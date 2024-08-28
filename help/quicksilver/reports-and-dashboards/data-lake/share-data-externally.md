---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Herstellen einer Verbindung zum Workfront Data Lake
description: Mit Workfront Data Lake können Sie die Workfront-Daten Ihres Unternehmens mit beliebten Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 1%

---

# Herstellen einer Verbindung zu Workfront Data Connect

Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.

Um Ihren Data Connect Data Lake mit einem externen Produkt zu verbinden, müssen Sie zunächst alle erforderlichen IPs zur Zulassungsliste hinzufügen, wie unten unter [Hinzufügen von IPs zur Zulassungsliste hinzufügen](#add-ips-to-the-allowlist) beschrieben. Darüber hinaus benötigen die meisten Produkte zusätzliche Informationen über Ihren Data Lake, um eine Verbindung herzustellen:

| Feldname | Wert |
|---------------|-------------|
| Server | Die URL für die Verbindung ohne den `https://` -Teil (auf der Seite **Datenzugriff** in Workfront* zu finden) |
| Port | `443` |
| Datenbank | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Funktion | `READER_ROLE` |
| Benutzername | Der beim Erstellen der Verbindung ausgewählte Benutzername (auf der Seite **Datenzugriff** in Workfront* zu finden) |
| Kennwort | Das bei der ersten Snowflake-Anmeldung ausgewählte Kennwort* |

*Informationen darüber, wo Sie die Seite &quot;**Datenzugriff**&quot; finden, auf der Ihre Data Connect-Verbindungen enthalten sind, finden Sie unter [Erstellen eines Leserkontos (Dienstkonto) für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Nachdem ein Eintrag zur IP-Zulassungsliste hinzugefügt wurde, sind alle anderen IP-Adressen nicht mehr zulässig. Stellen Sie sicher, dass Sie alle erforderlichen IP-Adressen - sowohl für die Erstellung als auch für die Lektüre Ihres Visualisierungs-Tools - eingegeben haben, bevor Sie versuchen, das Tool zu verwenden. Andernfalls kann es zu einem Fehler bezüglich ungültiger Anmeldedaten kommen.
>
>Wenn keine IP-Adressen in Ihrer Zulassungsliste enthalten sind, aber dennoch Probleme beim Herstellen einer Verbindung zu einem BI-Tool auftreten, überprüfen Sie die Proxyserverkonfiguration für das BI-Tool.

## Hinzufügen von IPs zur Zulassungsliste

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicken Sie auf die Registerkarte **Zulässige IP-Adressen** und dann auf die Schaltfläche **IP-Adresse zu Ihrer Zulassungsliste hinzufügen** .

1. Geben Sie in **IP-Adressbeschreibung** einen Namen für die IP-Adresse ein, geben Sie die IP-Adresse (oder den CIDR-Block) für das Tool ein, das Sie in **IP-Adresse** verwenden möchten, und klicken Sie dann auf **IP zu Zulassungsliste hinzufügen**.

   ![IP-Adresse hinzufügen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Entfernen einer IP-Adresse aus der Zulassungsliste

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bereich auf **System** > **Datenzugriff**.

1. Klicken Sie auf die Registerkarte **Zulässige IP-Adressen** und dann auf das Papierkorbsymbol ![Löschsymbol](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben der IP-Adresse, die Sie entfernen möchten.

1. Aktivieren Sie im sich öffnenden Fenster das Kontrollkästchen zur Bestätigung und klicken Sie auf **Löschen**.

## Datenfreigabe mit Business Intelligence-Tools

Unten finden Sie eine Reihe häufig verwendeter Business Intelligence-Tools. Über die Links gelangen Sie zur Dokumentations-Site des Dienstes, um mehr über die Verbindung mit Ihrem Data Lake zu erfahren.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Daten in einem externen Data Warehouse speichern

Unten finden Sie eine Reihe gemeinsamer Data Warehouse-Informationen. Über die Links gelangen Sie auf die Dokumentations-Site jedes Dienstes, auf der Sie mehr über die Anbindung an Ihren Data Lake erfahren.

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
