---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Herstellen einer Verbindung mit Workfront Data Connect
description: Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# Herstellen einer Verbindung mit Workfront Data Connect

Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.

Um Ihren Data Connect Data Lake mit einem externen Produkt zu verbinden, müssen Sie zunächst eine Verbindung erstellen, wie in [Erstellen eines Leserkontos oder einer Verbindung für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) beschrieben. Anschließend müssen Sie alle erforderlichen IPs zur Zulassungsliste auf die Zulassungsliste setzte hinzufügen, wie in [Hinzufügen von IPs zur-](#add-ips-to-the-allowlist) unten beschrieben.

Die meisten Produkte benötigen die folgenden Informationen zu Ihrem Data Lake, um eine Verbindung herzustellen:

| Feldname | Wert |
|---------------|-------------|
| Server | Die URL für die Verbindung ohne den `https://` (auf der Seite **Data Connect** in Workfront*) |
| Port | `443` |
| Datenbank | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Funktion | `READER_ROLE` |
| Benutzername | Der beim Erstellen der Verbindung gewählte Benutzername (auf der Seite **Data Connect** in Workfront*) |
| Kennwort | Das Kennwort, das bei der ersten Anmeldung bei Snowflake ausgewählt wurde* |

*Informationen dazu, wo die Seite **Data Connect** mit Ihren Verbindungen zu finden ist, finden Sie unter [Erstellen eines Leserkontos oder einer Verbindung für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Auf die Zulassungsliste setzen Nachdem ein Eintrag zur IP-Adresse hinzugefügt wurde, sind alle anderen IP-Adressen nicht mehr zulässig. Stellen Sie sicher, dass Sie alle erforderlichen IP-Adressen sowohl für das Erstellen als auch für das Lesen Ihres Visualisierungs-Tools eingegeben haben, bevor Sie versuchen, das Tool zu verwenden. Andernfalls kann ein Fehler bezüglich ungültiger Anmeldeinformationen auftreten.
>
>Wenn Sie keine IP-Adressen in Ihrer Zulassungsliste haben, aber immer noch Probleme haben, eine Verbindung zu einem BI-Tool herzustellen, überprüfen Sie die Proxy-Server-Konfiguration für das BI-Tool.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td><p>In den folgenden Plänen enthalten:</p>
    <ul>
        <li><p>Ultimativ</p></li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>Workfront Data Connect ist nicht für veraltete Workfront-Pläne verfügbar.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen von IPs zur Zulassungsliste

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenverbindung**.

1. Auf die Zulassungsliste setzen Klicken Sie auf die **Zulässige IPs** und dann auf die Schaltfläche **Eine IP-Adresse zu Ihrer hinzufügen**.

1. Auf die Zulassungsliste setzen Geben Sie in IP-Adressbeschreibung einen Namen für **IP-Adresse** und geben Sie die IP-Adresse (oder den CIDR-Block) für das Tool ein, das Sie in **IP-Adresse** verwenden möchten. Klicken Sie dann auf **IP-Adresse hinzufügen**.

   ![IP-Adresse hinzufügen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Eine IP-Adresse aus der Zulassungsliste entfernen

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenverbindung**.

1. Klicken Sie auf die **Zulässige IPs** und klicken Sie dann auf das Papierkorbsymbol ![Löschsymbol](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben der IP-Adresse, die Sie entfernen möchten.

1. Markieren Sie im eingeblendeten Fenster das Kontrollkästchen zur Bestätigung und klicken Sie dann auf **Löschen**.

## Freigeben von Daten mit Business Intelligence-Tools

Nachfolgend finden Sie eine Reihe gängiger Business Intelligence-Tools. Weitere Informationen zur Verbindung mit Ihrem Data Lake finden Sie auf den entsprechenden Dokumentations-Sites.

* Tableau
* Power BI
* Domo
* SAP HANA

## Speichern von Daten in einem externen Data Warehouse

Nachfolgend finden Sie eine Reihe gängiger Data Warehouses. Besuchen Sie die Dokumentations-Sites, um mehr über die Verbindung mit Ihrem Data Lake zu erfahren.

* Datenblöcke
* AWS Redshift
