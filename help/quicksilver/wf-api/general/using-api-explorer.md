---
content-type: api
navigation-topic: general-api
title: Verwenden des API-Explorers
description: Verwenden des API-Explorers
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
TQID: https://experienceleague.adobe.com/Y-qv5r6ygRA-V7mQSM3wzjaOt58myb64Vxa7UZGsAVo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 368
ht-degree: 100%

---

# Verwenden des API-Explorers

Bei Verwendung der Adobe Workfront Core-API ist der API-Explorer ein veraltetes Referenz-Tool, das die Beziehungen zwischen unterstützten Ressourcen, Parametern und Variablen katalogisiert.

## Zugriff auf den API-Explorer:

1. Navigieren Sie in einem Webbrowser zum [API-Explorer](https://developer.adobe.com/workfront/api-explorer/)\
   ![Navigieren zum API-Explorer](assets/mceclip1-350x149.png)

1. Wählen Sie oben rechts im API-Explorer die gewünschte **API-Version** von Workfront aus. Standardmäßig wird automatisch die aktuelle Version ausgewählt
1. Das Feld **Filter** kann verwendet werden, um die Objekte nach Namen zu filtern. Dabei wird die Liste der angezeigten Objekte entsprechend gekürzt:

   ![API-Explorer-Felder](assets/mceclip2-350x147.png)

   * **Felder**: Verfügbare Felder innerhalb des angegebenen Objekts.
   * **Referenzen**: Verfügbare Referenzvariablen für das angegebene Objekt. Eine Referenz ist ein Alias für eine Variable. Nach der Initialisierung kann eine Referenz synonym mit dem Variablennamen verwendet werden. Eine Referenz verwendet initialisierten Speicher.
   * **Sammlungen**: Verfügbare Sammlungen für das Objekt. Sammlungen sind Variablen, die eine Eins-zu-viele-Beziehung zwischen dem Objekt und der Ressource darstellen.
   * **Suche**: Verfügbare Suchressourcen für das Objekt. Die Ergebnisse einer Suche basieren auf den Abfrageparametern, die von der Suchressource in der API-Anfrage angegeben werden.
   * **Aktionen**: Unterstützte Aktionen für das Objekt. Aktionen können einfache oder komplexe Prozeduren sein, die für eine Ressource oder einen Satz von Ressourcen ausgeführt werden. Eine bestimmte Aktion kann sich auch auf zugehörige Ressourcen auswirken.

1. Öffnen Sie eine Registerkarte und klicken Sie dann auf die Objekt-ID, um die entsprechenden Variablen anzuzeigen.\
   ![Anzeigen von Variablen](assets/approval-350x89.png)\
   Je nach ausgewähltem Objekt können die folgenden Variablen gelten:

   | Variable | Definition |
   |---|---|
   | Feldname | Der Name eines Feldes, das in einem Vorgang in der Workfront-API verwendet wird. |
   | Feldtyp | Die Art der Werte, die in ein bestimmtes Feld in einer Datentabelle eingegeben werden können. Mögliche Feldtypwerte sind „string“, „double“, „int“ und „dateTime“. |
   | Aufzählungstyp | Die Art der Werte, die zur Identifizierung eines Datentyps verwendet werden können. |
   | Mögliche Werte | Zulässige Werte für das Objekt. |
   | Attributtyp ObjCode | Attribute, die zum Ändern der Objektklasse verwendet werden können. |
   | URL | Der Einstiegspfad, über den Ihre Anwendung mit der Workfront-API kommunizieren kann. |
   | Argumente | Die Variablen des Objekts, die zwischen Ihrer Anwendung und Workfront übergeben werden können. |
   | Ergebnistyp | Zulässige Datentypen, die von einer Methode zurückgegeben werden können. |
