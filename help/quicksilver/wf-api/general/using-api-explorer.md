---
content-type: api
navigation-topic: general-api
title: Verwenden des API-Explorers
description: Verwenden des API-Explorers
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 1%

---


# Verwenden des API-Explorers

Bei Verwendung der Adobe Workfront Core API ist der API Explorer ein veraltetes Referenztool, das die Beziehungen zwischen unterstützten Ressourcen, Parametern und Variablen katalogisiert.

## Zugriff auf den API Explorer:

1. Navigieren Sie mit einem Webbrowser zum [API-Explorer](https://developer.adobe.com/workfront/api-explorer/)\
   ![](assets/mceclip1-350x149.png)

1. Wählen Sie oben rechts im API Explorer das gewünschte Workfront **API-Version** aus. Standardmäßig wird automatisch die neueste Version ausgewählt
1. Das Feld **Filter** kann verwendet werden, um die Objekte nach Namen zu filtern, und kürzt die Liste der angezeigten Objekte entsprechend:

   ![](assets/mceclip2-350x147.png)

   * **Fields**: Verfügbare Felder innerhalb des angegebenen Objekts.
   * **References**: Verfügbare Referenzvariablen für das angegebene Objekt. Ein Verweis ist ein Alias für eine Variable. Nach der Initialisierung kann eine Referenz synonym mit dem Variablennamen verwendet werden. Eine Referenz verwendet initialisierten Speicher.
   * **Sammlungen**: Verfügbare Sammlungen für das Objekt. Sammlungen sind Variablen, die eine Eins-zu-viele-Beziehung zwischen dem -Objekt und der Ressource darstellen.
   * **Suche**: Verfügbare Suchressourcen für das Objekt. Die Ergebnisse einer Suche basieren auf den Abfrageparametern, die von der Suchressource in der API-Anfrage angegeben werden.
   * **Aktionen**: Unterstützte Aktionen für das Objekt. Aktionen können einfache oder komplexe Prozeduren sein, die für eine Ressource oder einen Satz von Ressourcen ausgeführt werden. Eine bestimmte Aktion kann sich auch auf zugehörige Ressourcen auswirken.

1. Öffnen Sie eine Registerkarte und klicken Sie dann auf die Objekt-ID, um die entsprechenden Variablen anzuzeigen.\
   ![](assets/approval-350x89.png)\
   Je nach ausgewähltem Objekt können die folgenden Variablen zutreffen:

   | Variable | Definition |
   |---|---|
   | Feldname | Der Name eines Felds, das in einem Vorgang innerhalb der Workfront-API verwendet wird. |
   | Feldtyp | Die Art der Werte, die in ein bestimmtes Feld in einer Datentabelle eingegeben werden können. Mögliche Feldtypwerte sind „String“, „Double“, „int“ und „dateTime“. |
   | Aufzählungstyp | Die Art der Werte, die zur Identifizierung eines Datentyps verwendet werden können. |
   | Mögliche Werte | Zulässige Werte für das Objekt. |
   | Attributtyp ObjCode | Attribute, die zum Ändern der Objektklasse verwendet werden können. |
   | URL | Der Einstiegspfad, über den Ihre App mit der Workfront-API kommunizieren kann. |
   | Argumente | Die Variablen des -Objekts, die zwischen Ihrer Anwendung und Workfront übergeben werden können. |
   | Ergebnistyp | Zulässige Datentypen, die von einer Methode zurückgegeben werden können. |
