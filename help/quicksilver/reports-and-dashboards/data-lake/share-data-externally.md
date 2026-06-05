---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Herstellen einer Verbindung mit Workfront Data Connect
description: Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/pPk3qt9-o3QhAajyI4eGhwe0J2tRphXDstrJxmdW8Ww
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1489
ht-degree: 4%

---

# Herstellen einer Verbindung mit Workfront Data Connect

Mit Workfront Data Connect können Sie die Workfront-Daten Ihres Unternehmens mit Business Intelligence-Tools verwenden oder in einem externen Data Warehouse speichern.

Um Ihren Data Connect Data Lake mit einem externen Produkt zu verbinden, müssen Sie zunächst eine Verbindung erstellen, wie in [Erstellen eines Leserkontos oder einer Verbindung für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) beschrieben. Anschließend müssen Sie alle erforderlichen IPs zur Zulassungsliste hinzufügen, wie in [Hinzufügen von IPs zur-](#add-ips-to-the-allowlist) unten beschrieben.

Die meisten Produkte benötigen die folgenden Informationen zu Ihrem Data Lake, um eine Verbindung herzustellen:

| Feldname | Wert |
|---------------|-------------|
| Server | Die URL für die Verbindung ohne den `https://` (auf der Seite **Data Connect** in Workfront*) |
| Port | `443` |
| Datenbank | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Schema | `WF` |
| Rolle | `READER_ROLE` |
| Benutzername | Der beim Erstellen der Verbindung gewählte Benutzername (auf der Seite **Data Connect** in Workfront*) |
| Kennwort | Das Kennwort, das bei der ersten Anmeldung bei Snowflake ausgewählt wurde* |

*Informationen dazu, wo die Seite **Data Connect** mit Ihren Verbindungen zu finden ist, finden Sie unter [Erstellen eines Leserkontos oder einer Verbindung für Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Nachdem ein Eintrag zur IP-Adresse hinzugefügt wurde, sind alle anderen IP-Adressen nicht mehr zulässig. Stellen Sie sicher, dass Sie alle erforderlichen IP-Adressen sowohl für das Erstellen als auch für das Lesen Ihres Visualisierungs-Tools eingegeben haben, bevor Sie versuchen, das Tool zu verwenden. Andernfalls kann ein Fehler bezüglich ungültiger Anmeldeinformationen auftreten.
>
>Wenn Sie keine IP-Adressen in Ihrer Zulassungsliste haben, aber immer noch Probleme haben, eine Verbindung zu einem BI-Tool herzustellen, überprüfen Sie die Proxy-Server-Konfiguration für das BI-Tool.

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
   <td> <p>Sie müssen ein Workfront-Administrator sein</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen von IPs zur Zulassungsliste

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenverbindung**.

1. Klicken Sie auf die **Zulässige IPs** und dann auf die Schaltfläche **Eine IP-Adresse zu Ihrer hinzufügen**.

1. Geben Sie in IP-Adressbeschreibung einen Namen für **IP-Adresse** und geben Sie die IP-Adresse (oder den CIDR-Block) für das Tool ein, das Sie in **IP-Adresse** verwenden möchten. Klicken Sie dann auf **IP-Adresse hinzufügen**.

   ![IP-Adresse hinzufügen](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Suchen nach Azure-IP-Bereichen für Microsoft Power BI

Der Traffic von Microsoft Power BI zu Data Connect stammt nicht von einer einzigen festen Adresse. Microsoft veröffentlicht die IP-Bereiche als CIDR-Blöcke in einer großen JSON-Datei. In diesem Abschnitt wird beschrieben, wie Sie die Blöcke für die tatsächlich verwendeten Regionen finden.

### Offizielle Microsoft-Quelle für Azure-IP-Bereiche und Service-Tags

Microsoft veröffentlicht die Liste auf der Download-Seite für [Azure IP-Bereiche und Service-Tags - Public Cloud](https://www.microsoft.com/en-us/download/details.aspx?id=56519). Laden Sie die aktuelle JSON-Datei herunter (der Dateiname ähnelt normalerweise `ServiceTags_Public_YYYYMMDD.json`). Aktualisieren Sie Ihre Datei, wenn Microsoft diese Datei aktualisiert oder Verbindungsprobleme nach einer Microsoft-Änderung auftreten.

>[!NOTE]
>
>Die JSON-Datei ist sehr groß, oft weit über 100.000 Zeilen. Das ist zu erwarten. Die benötigten Abschnitte sind klein, man muss nicht die gesamte Datei von Hand lesen.

### Power BI im Vergleich zu Power Query Online

Kunden melden manchmal &quot;Power BI&quot;, wenn der Traffic tatsächlich von Power Query-Komponenten stammt, die Microsoft in der Service-Tag-Liste als separaten Azure-Service behandelt.

| Wenn Ihre Benutzer… | Suchen Sie in der JSON nach diesem Service-Tag. |
|----------------|---------------------------------------|
| Verwenden des Power BI-Service, von in Azure gehosteten Datensätzen oder von Gateways im Cloud-Kontext | `PowerBI` (globale oder regionale Einträge wie `PowerBI.EastUS`) |
| Verwenden von Power Query Online, Cloud-Datenflüssen und ähnlichen Erlebnissen | `PowerQueryOnline` (globale oder regionale Einträge wie `PowerQueryOnline.EastUS`) |

Wenn Ihr Unternehmen beide Erlebnisse verwendet, fügen Sie CIDR-Blöcke aus `PowerBI` und `PowerQueryOnline` für dieselben Regionen hinzu. Wenn Sie nur einen hinzufügen, werden einige Benutzer möglicherweise weiterhin blockiert, während andere erfolgreich sind.

### Wählen Sie regionale Tags aus, nicht das globale Aggregat

Die JSON-Datei enthält einen einzelnen regionsübergreifenden Eintrag für `PowerBI` (und ähnlich für `PowerQueryOnline`), der viele Regionen aggregiert und Hunderte von CIDR-Blöcken sowie viele kleinere regionale Einträge wie `PowerBI.WestUS`, `PowerBI.WestUS2` und `PowerBI.WestUS3` enthalten kann. Jedes regionale Objekt listet nur die Präfixe für diese Region auf, typischerweise höchstens Dutzende von Zeilen. Es wird nicht empfohlen, den globalen Eintrag hinzuzufügen, es sei denn, Sie verfügen über eine dokumentierte Anforderung, um jede Azure-Region zuzulassen. Für die meisten Data Connect-Kunden sind regionale Einträge der richtige Standard. Fügen Sie die Regionen hinzu, in denen Ihre Power BI-Mandanten und -Benutzer tatsächlich ausgeführt werden, sowie einen kleinen Puffer für Redundanz (z. B. eine sekundäre Notfallwiederherstellungsregion, die Ihr Unternehmen verwendet).

### Regionen auswählen

Die Regionsnamen von Microsoft in der Datei sehen wie `EastUS`, `WestEurope`, `GermanyWestCentral` usw. aus. Verwenden Sie die Regionen, in denen Ihre Power BI-Kapazität und -Benutzer gehostet werden, nicht den Ort, an dem sich Ihr Büro befindet, obwohl sie häufig übereinstimmen.

| Szenario | Was zuerst hinzugefügt werden soll |
|----------|-------------------|
| Verwendung in den Vereinigten Staaten | Beginnen Sie mit den Regionen in den USA, die Sie kennen und die Ihr Mandant verwendet (Beispiele: `EastUS`, `EastUS2`, `WestUS`, `WestUS2`, `WestUS3`, `CentralUS`, `SouthCentralUS`). Sie benötigen nicht jede US-Region, es sei denn, Ihr Microsoft-Administrator bestätigt das Multi-Region-Hosting. |
| Verwendung in der Europäischen Union oder im Vereinigten Königreich | Beginnen Sie mit den Regionen, die Ihr Mandant verwendet (Beispiele: `WestEurope`, `NorthEurope`, `FranceCentral`, `GermanyWestCentral`, `SwedenCentral`, `UKSouth`). Weitere hinzufügen, wenn die Benutzer weitere Microsoft-Regionen umfassen. |
| Nutzung im asiatisch-pazifischen Raum | Fügen Sie die von Ihrem Power BI- oder Azure-Administrator bestätigten Regionen hinzu (Beispiele: `SoutheastAsia`, `EastAsia`, `AustraliaEast`). |
| Mehrere Regionen | Fügen Sie für jeden Service beide Sätze regionaler Tags (z. B. EU und USA) hinzu (`PowerBI` und `PowerQueryOnline`, wenn beide verwendet werden). |
| Unbekannter Bereich | Fragen Sie Ihren Microsoft 365- oder Power BI-Administrator, welche Azure-Regionen Ihre Power BI-Ressourcen hosten, oder überprüfen Sie Ihre Power BI Admin-Mandanteneinstellungen. Wenn Sie die Blockierung für Tests schnell aufheben müssen, fügen Sie ein bekanntes Regionspaar hinzu (z. B. `EastUS` und `WestUS`) und überwachen Sie und grenzen Sie die Liste nach der Bestätigung ein. |

### Suchen nach IP-Bereichen und Hinzufügen zur Zulassungsliste

So erfassen Sie IP-Bereiche aus Microsoft und fügen sie zu Ihrer Workfront-Zulassungsliste hinzu:

1. Öffnen Sie die Download-Seite für [Azure-IP-Bereiche und Service-Tags - Public Cloud](https://www.microsoft.com/en-us/download/details.aspx?id=56519), laden Sie die JSON-Datei für Service-Tags herunter und speichern Sie sie lokal (z. B. `Downloads\ServiceTags_Public_YYYYMMDD.json`).

1. Öffnen Sie die Datei in einem beliebigen Editor, der große JSON-Dateien gut verarbeitet, z. B. Visual Studio Code.

1. Verwenden Sie die Suchfunktion Ihres Editors (`Ctrl+F` unter Windows oder `Cmd+F` unter macOS), um JSON-Objekte zu finden, deren `"name"` einem Service-Tag entspricht, z. B. `PowerBI.EastUS` oder `PowerQueryOnline.WestEurope`. Nützliche Suchvorgänge:

   * `"name": "PowerBI.WestUS"` - Sprung nach West US Power BI.
   * `"name": "PowerQueryOnline.WestUS"` — springen Sie zu West US Power Query Online.
   * `PowerBI.` - Listet alle regionalen Power BI-Tags auf und passt dann Ihren Regionsnamen an.

1. Suchen Sie unter jedem übereinstimmenden Objekt das Array mit dem Namen `addressPrefixes`. Jede Zeichenfolge in diesem Array ist ein CIDR-Block (z. B. `20.59.79.96/27` oder ein IPv6-Präfix). Dies sind die Werte, die Sie Ihrer Workfront-Zulassungsliste hinzufügen.

1. Fügen Sie jede CIDR zur Workfront-Zulassungsliste hinzu, wie [Hinzufügen von IPs zur in diesem Artikel beschrieben](#add-ips-to-the-allowlist). Warten Sie einige Minuten für die Richtlinienübertragung, wenn Ihre Umgebung Regeln zwischenspeichert.

1. Führen Sie in Power BI oder Power Query Online eine kleine Testabfrage für Data Connect aus, um die Verbindung zu validieren. Wenn er fehlschlägt, erfassen Sie die ungefähre Zeit und fragen Sie Ihr Netzwerk-Team, ob Ablehnungen mit fehlenden Bereichen übereinstimmen. Überprüfen Sie erneut, ob Sie `PowerQueryOnline` verpasst haben, als nur `PowerBI` hinzugefügt wurde, was eine gemeinsame Lücke ist.

Wenn Ihr Microsoft-Administrator beispielsweise bestätigt, dass Ihre Power BI-Workloads West US, West US 2 und West US 3 verwenden und Ihre Benutzer sowohl Power BI als auch Power Query Online verwenden, würden Sie sechs Objekte öffnen: `PowerBI.WestUS`, `PowerBI.WestUS2`, `PowerBI.WestUS3` und die entsprechenden `PowerQueryOnline.<Region>` für jedes Objekt und dann `addressPrefixes` aus allen sechs kopieren.

### JSON-Strukturreferenz

Jeder Service-Tag-Block sieht konzeptionell wie folgt aus: Echte Dateien enthalten mehr Metadaten.

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

Das `addressPrefixes`-Array enthält die CIDR-Blöcke, die Sie Workfront hinzufügen werden. Andere Felder sind für Azure-Netzwerkszenarien vorgesehen und können hier nicht angewendet werden.

### Zulassungsliste verwalten

* Microsoft ändert IP-Bereiche im Laufe der Zeit. Wenn Microsoft eine aktualisierte JSON-Datei veröffentlicht, aktualisieren oder vergleichen Sie Ihre Zulassungsliste regelmäßig, insbesondere nach einem Verbindungsereignis.
* Wenn Ihre Umgebung IPv6 zu Snowflake unterstützt und Microsoft IPv6-Präfixe auflistet, schließen Sie diese ein, wenn Ihre Sicherheitsrichtlinie IPv6 zulässt. Stimmen Sie sich andernfalls mit Ihrem Netzwerk-Team ab.

## Eine IP-Adresse aus der Zulassungsliste entfernen

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **Setup**.

1. Klicken Sie im linken Bedienfeld auf **System** > **Datenverbindung**.

1. Klicken Sie auf die **Zulässige IPs** und klicken Sie dann auf das Papierkorbsymbol ![Löschsymbol](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) rechts neben der IP-Adresse, die Sie entfernen möchten.

1. Markieren Sie im eingeblendeten Fenster das Kontrollkästchen zur Bestätigung und klicken Sie dann auf **Löschen**.

## Freigeben von Daten mit Business Intelligence-Tools

Nachfolgend finden Sie eine Reihe gängiger Business Intelligence-Tools. Weitere Informationen zur Verbindung mit Ihrem Data Lake finden Sie auf den entsprechenden Dokumentations-Sites.

* Tableau
* Power BI
* Domo
* SAP HANA

## Speichern von Daten in einem externen Data Warehouse

Nachfolgend finden Sie eine Reihe gängiger Data Warehouses. Besuchen Sie die Dokumentations-Sites, um mehr über die Verbindung mit Ihrem Data Lake zu erfahren.

* Databricks
* AWS Redshift
