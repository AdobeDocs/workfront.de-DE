---
title: Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Ein externes Suchfeld in einem benutzerdefinierten Formular ruft eine externe API auf und gibt Werte als Optionen in einem Dropdown-Feld zurück. Dieser Artikel enthält Beispiele für die Verwendung des externen Suchfelds, um dieselbe Instanz von Workfront oder eine öffentliche API aufzurufen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 13880fcb-8523-45d2-9ac6-38453e8e2391
source-git-commit: 1b3e0ab2d8ee37b7583d0b8fb0472b2fc9623da0
workflow-type: tm+mt
source-wordcount: '1237'
ht-degree: 0%

---

# Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular

Ein externes Suchfeld in einem benutzerdefinierten Formular ruft eine externe API auf und gibt Werte als Optionen in einem Dropdown-Feld zurück. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können eine oder mehrere dieser Optionen aus der Dropdown-Liste auswählen.

Dieser Artikel enthält Beispiele für die Verwendung des externen Suchfelds, um dieselbe Instanz von Workfront oder eine öffentliche API aufzurufen. Sie können auch die externe Suche verwenden, um mit einem externen System wie Jira, Salesforce oder ServiceNow zu kommunizieren.

Weitere Informationen zum Hinzufügen eines externen Suchfelds zu einem benutzerdefinierten Formular und zusätzliche Definitionen der externen Lookup-Komponenten finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Richten Sie ein externes Suchfeld für dieselbe Instanz von Workfront ein

Sie können die externe Suche verwenden, um Daten aus Ihrer Workfront-Instanz in das benutzerdefinierte Formular zu übertragen.

### Native Workfront-Feldwerte in der externen Suche verwenden

In diesem Beispiel wird gezeigt, wie die Workfront-API aufgerufen und Daten aus dem vorhandenen Feld &quot;Statusabfrage&quot;in Ihr externes Suchfeld übertragen werden.

1. Öffnen Sie das benutzerdefinierte Formular.
1. Suchen Sie auf der linken Seite des Bildschirms nach **Externer Suchvorgang** und ziehen Sie ihn in einen Bereich auf der Arbeitsfläche.
1. Geben Sie den **Titel** und den **Namen** für das Feld ein.
1. Wählen Sie das **Format** für das Feld aus.
1. Geben Sie den API-URL-Aufruf im Feld **Basis-API-URL** ein.

   * Sie können $$HOST hinzufügen, um auf dieselbe Instanz zu verweisen.
   * Sie können $$QUERY hinzufügen, um die Ergebnisse anhand der Abfrage eines anderen Felds zu filtern.

   **Beispiel**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Überprüfen Sie die **Abhängigkeiten** für die Felder, auf die dieses Suchfeld in der API verweist.

   Ein Abhängigkeitsfeld kann ein beliebiges benutzerdefiniertes oder natives Feld sein, das auf der Detailseite des Objekts vorhanden ist.

   In diesem Beispiel wird der `{DE:StatusQuery}` durch den Wert des benutzerdefinierten Felds StatusQuery ersetzt.

1. Wählen Sie die **HTTP-Methode** aus.

   Dies ist meist **Get**.

1. Geben Sie den **JSON-Pfad** ein, um die Ergebnisse aus Ihrem API-Aufruf zu erhalten.

   **Beispiel**
   `$.data[*].name`

   >[!NOTE]
   >
   >**Kopfzeileninformationen** sind für einen Aufruf an dieselbe Workfront-Instanz nicht erforderlich.

1. Klicken Sie auf **Anwenden**.

   ![Einrichten des API-Aufrufs für Workfront in benutzerdefiniertem Formular](assets/external-lookup-to-workfront.png)

   Wenn das benutzerdefinierte Formular einem Workfront-Objekt (in diesem Beispiel einem Projekt) hinzugefügt wird, sieht es ähnlich aus.

   ![Benutzerdefiniertes Formular mit externem Suchfeld](assets/external-lookup-project-status-example1.png)

   ![Externe Suchoptionen basierend auf dem Status](assets/external-lookup-project-status-example2.png)

### Verwenden benutzerdefinierter Feldwerte in der externen Suche

In diesem Beispiel wird gezeigt, wie Sie die Workfront-API aufrufen und Daten aus einem benutzerdefinierten Feld in Ihr externes Suchfeld übertragen. Das benutzerdefinierte Beispielfeld heißt &quot;Benutzerdefinierte Farben&quot;.

1. Öffnen Sie das benutzerdefinierte Formular.
1. Suchen Sie auf der linken Seite des Bildschirms nach **Externer Suchvorgang** und ziehen Sie ihn in einen Bereich auf der Arbeitsfläche.
1. Geben Sie den **Titel** und den **Namen** für das Feld ein.
1. Wählen Sie das **Format** für das Feld aus.
1. Geben Sie den API-URL-Aufruf im Feld **Basis-API-URL** ein.

   **Beispiel**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. Überprüfen Sie die **Abhängigkeiten** für die Felder, auf die dieses Suchfeld in der API verweist.

   Ein Abhängigkeitsfeld kann ein beliebiges benutzerdefiniertes oder natives Feld sein, das auf der Detailseite des Objekts vorhanden ist.

1. Wählen Sie die **HTTP-Methode** aus.

   Dies ist meist **Get**.

1. Geben Sie den **JSON-Pfad** ein, um die Ergebnisse aus Ihrem API-Aufruf zu erhalten.

   **Beispiel**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * &quot;parameterValues&quot;bezieht sich auf jedes benutzerdefinierte Feld in Workfront für das Objekt, auf dem Sie sich befinden.
   * In diesem Beispiel ist &quot;DE:Combo Colors&quot;das spezifische benutzerdefinierte Feld, das die Werte enthält, die Sie abrufen möchten.

   >[!NOTE]
   >
   >**Kopfzeileninformationen** sind für einen Aufruf an dieselbe Workfront-Instanz nicht erforderlich.

1. Klicken Sie auf **Anwenden**.

   Wenn das benutzerdefinierte Formular einem Workfront-Objekt hinzugefügt wird, werden alle Werte im Feld &quot;Kombinationsfarben&quot;in der Dropdown-Liste Externes Suchfeld angezeigt.

## Externes Suchfeld für eine öffentliche API einrichten

Mit der externen Suche können Sie eine externe, öffentliche API aufrufen und Daten abrufen.

In diesem Beispiel wird gezeigt, wie eine -API von Ländern (z. B. <https://api.first.org/data/v1/countries>) aufgerufen wird, damit Sie nicht alle Ländernamen in den Dropdown-Optionen hartcodieren müssen.

1. Öffnen Sie das benutzerdefinierte Formular.
1. Suchen Sie auf der linken Seite des Bildschirms nach **Externer Suchvorgang** und ziehen Sie ihn in einen Bereich auf der Arbeitsfläche.
1. Geben Sie den **Titel** und den **Namen** für das Feld ein.
1. Wählen Sie das **Format** für das Feld aus.
1. Geben Sie den API-URL-Aufruf im Feld **Basis-API-URL** ein.

   * Sie können $$QUERY hinzufügen, um die Abfragefilterung für Ihre Endbenutzer zu implementieren.

   **Beispiele**
Listet alle Länder auf: <https://api.first.org/data/v1/countries>

   Ermöglicht dem Benutzer die Suche nach einem beliebigen Land im Dropdown-Feld: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Ermöglicht dem Benutzer die Suche nach einem Land in einer Region: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Die verfügbaren Regionen werden in Workfront in einem separaten benutzerdefinierten Feld definiert.
   * Wenn der Benutzer eine Region im Formular auswählt, zeigt das externe Suchfeld nur die Länder in dieser Region an (das Land, in dem sich die Region befindet, die in der API definiert ist). Der Benutzer kann auch nach einem Land in der ausgewählten Region suchen.

1. Überprüfen Sie die **Abhängigkeiten** für die Felder, auf die dieses Suchfeld in der API verweist.

   Ein Abhängigkeitsfeld kann ein beliebiges benutzerdefiniertes oder natives Feld sein, das auf der Detailseite des Objekts vorhanden ist.

   In diesem Beispiel wird der `{DE:Region}` durch den Wert des benutzerdefinierten Felds Region ersetzt.

1. Wählen Sie die **HTTP-Methode** aus.

   Dies ist meist **Get**.

1. Geben Sie den **JSON-Pfad** ein, um die Ergebnisse aus Ihrem API-Aufruf zu erhalten.

   Diese Option ermöglicht das Extrahieren von Daten aus der JSON-Datei, die von der API-URL zurückgegeben wird. Es dient dazu, festzulegen, welche Werte aus dem JSON-Bereich in den Dropdown-Optionen angezeigt werden.

   **Beispiel**
   `$.data[*].country`

1. (Optional) Klicken Sie auf **Kopfzeile hinzufügen** und geben Sie das Schlüssel-Wert-Paar ein oder fügen Sie es ein, das für die Authentifizierung mit der API erforderlich ist.

   >[!NOTE]
   >
   >Die Felder &quot;Kopfzeile&quot;sind kein sicherer Ort zum Speichern von Anmeldeinformationen. Achten Sie darauf, was Sie eingeben und speichern.

1. (Optional) Wählen Sie &quot;**Dropdown mit Mehrfachauswahl**&quot;aus, damit der Benutzer mehr als einen Wert in der Dropdown-Liste auswählen kann.

1. Klicken Sie auf **Anwenden**.

   ![Einrichtung des API-Aufrufs für die öffentliche API in benutzerdefiniertem Formular](assets/external-lookup-to-api-for-countries.png)

   Wenn das benutzerdefinierte Formular einem Workfront-Objekt (in diesem Beispiel einem Projekt) hinzugefügt wird, sieht es ähnlich aus.

   ![Benutzerdefiniertes Formular mit externem Suchfeld](assets/external-lookup-countries-example1.png)

   ![Externe Suchoptionen für ein Land basierend auf Region](assets/external-lookup-countries-example2.png)

## Zusätzliche Anwendungsfälle für externe Suchfelder

Es gibt viele weitere Anwendungsfälle zum Erstellen einer externen Suche.

**Anwendungsfall:** Ersetzen Sie typeahead-Felder, da sie Probleme mit der Berichterstellung verursachen können.
**Lösung:** Verwenden Sie einen API-Aufruf für vorhandene Objekte im System.

Beispiel einer Basis-API-URL für Vorlagen, um ein typeahead -Feld zu ersetzen:
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**Anwendungsfall:** Erstellen Sie Dropdown-Felder mit weiteren Funktionen (z. B. ist eine Zeilenumbruch im Feld Externes Suchfeld vorhanden).
**Lösung:** Verwenden Sie einen API-Aufruf für vorhandene Objekte im System oder erstellen Sie ein neues Objekt und verwenden Sie einen API-Aufruf für dieses Objekt.

**Anwendungsfall:** Definieren Sie eine Möglichkeit für Benutzer, ihre eigenen Felder außerhalb des benutzerdefinierten Formularbereichs zu verwalten. Richten Sie das externe Suchfeld ein und Sie können Benutzern die Objekte des Felds zuweisen. Diese Option eignet sich gut für Felder und Teams mit hoher Wartung.
**Lösung:** Erstellen Sie ein neues Objekt und verwenden Sie einen API-Aufruf für dieses Objekt.

**Anwendungsfall:** Integration mit Objekten außerhalb von Workfront. Beispielsweise beim Zugriff auf ein anderes System, um den Namen jedes Benutzers abzurufen, anstatt in einem typeahead -Feld eingeschränkt zu sein.
**Lösung:** Webhook-/Fusion-Automatisierung zur Verbindung mit anderen Systemen.

