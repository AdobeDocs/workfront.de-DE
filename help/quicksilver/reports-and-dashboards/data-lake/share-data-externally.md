---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Herstellen einer Verbindung zu Workfront Data Connect
description: Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 7b50876f1be16473704eddeb3157dacfacd96e90
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 1%

---

# Herstellen einer Verbindung zu Workfront Data Connect

Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.

Um Ihren Data Connect Data Lake mit einem externen Produkt zu verbinden, müssen Sie zunächst eine Verbindung wie in [Erstellen eines Leserkontos oder einer Verbindung für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) beschrieben herstellen. Anschließend müssen Sie alle erforderlichen IPs zur Zulassungsliste hinzufügen, wie unten unter [IPs zur Zulassungsliste hinzufügen](#add-ips-to-the-allowlist) beschrieben.

Die meisten Produkte benötigen die folgenden Informationen über Ihren Data Lake, um eine Verbindung herzustellen:

| Feldname | Wert |
|---------------|-------------|
| Server | Die URL für die Verbindung ohne den `https://` -Teil (auf der Seite **Datenverbindung** in Workfront* zu finden) |
| Port | `443` |
| Datenbank | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Funktion | `READER_ROLE` |
| Benutzername | Der beim Erstellen der Verbindung ausgewählte Benutzername (auf der Seite **Data Connect** in Workfront* zu finden) |
| Kennwort | Das bei der ersten Snowflake-Anmeldung ausgewählte Kennwort* |

*Informationen darüber, wo Sie die Seite **Datenverbindung** mit Ihren Verbindungen finden, finden Sie unter [Erstellen eines Leserkontos oder einer Verbindung für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Nachdem ein Eintrag zur IP-Zulassungsliste hinzugefügt wurde, sind alle anderen IP-Adressen nicht mehr zulässig. Stellen Sie sicher, dass Sie alle erforderlichen IP-Adressen - sowohl für die Erstellung als auch für die Lektüre Ihres Visualisierungs-Tools - eingegeben haben, bevor Sie versuchen, das Tool zu verwenden. Andernfalls kann es zu einem Fehler bezüglich ungültiger Anmeldedaten kommen.
>
>Wenn keine IP-Adressen in Ihrer Zulassungsliste enthalten sind, aber dennoch Probleme beim Herstellen einer Verbindung zu einem BI-Tool auftreten, überprüfen Sie die Proxyserverkonfiguration für das BI-Tool.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td><p>In den folgenden Plänen enthalten:</p>
    <ul>
        <li>Ultimativ</li> 
    </ul>    
   <p>Kann als Zusatzprodukt zu den folgenden Plänen erworben werden:</p> 
    <ul>
        <li>Auswählen</li> 
        <li>Erstklassig</li>
    </ul> 
    <p>Workfront Data Connect ist nicht für ältere Workfront-Pläne verfügbar.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen von IPs zur Zulassungsliste

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bereich auf **System** > **Data Connect**.

1. Klicken Sie auf die Registerkarte **Zulässige IP-Adressen** und dann auf die Schaltfläche **IP-Adresse zu Ihrer Zulassungsliste hinzufügen** .

1. Geben Sie in **IP-Adressbeschreibung** einen Namen für die IP-Adresse ein, geben Sie die IP-Adresse (oder den CIDR-Block) für das Tool ein, das Sie in **IP-Adresse** verwenden möchten, und klicken Sie dann auf **IP zu Zulassungsliste hinzufügen**.

   ![IP-Adresse hinzufügen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Entfernen einer IP-Adresse aus der Zulassungsliste

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bereich auf **System** > **Data Connect**.

1. Klicken Sie auf die Registerkarte **Zulässige IP-Adressen** und dann auf das Papierkorbsymbol ![Löschsymbol](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben der IP-Adresse, die Sie entfernen möchten.

1. Aktivieren Sie im sich öffnenden Fenster das Kontrollkästchen zur Bestätigung und klicken Sie auf **Löschen**.

## Datenfreigabe mit Business Intelligence-Tools

Unten finden Sie eine Reihe häufig verwendeter Business Intelligence-Tools. Besuchen Sie die entsprechenden Dokumentations-Sites, um mehr über die Verbindung mit Ihrem Data Lake zu erfahren.

* Tableau
* Power BI
* Domo
* SAP HANA

## Daten in einem externen Data Warehouse speichern

Nachfolgend finden Sie eine Reihe gemeinsamer Data Warehouse-Aktivitäten. Besuchen Sie die entsprechenden Dokumentations-Sites, um mehr über die Verbindung mit Ihrem Data Lake zu erfahren.

* Datenricks
* AWS Redshift
