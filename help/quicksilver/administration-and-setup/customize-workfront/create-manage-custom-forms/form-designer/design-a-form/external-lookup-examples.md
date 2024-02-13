---
title: Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Ein Feld "Externe Suche"in einem benutzerdefinierten Formular ruft eine externe API auf und gibt Werte als Optionen in einem Dropdown-Feld zurück. In diesem Artikel finden Sie Beispiele für die Verwendung des Felds Externe Suche , um dieselbe Instanz von Workfront oder eine öffentliche API aufzurufen.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: a082f010dbd78235aaad41a80d87d772ca77ff89
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular

Ein Feld &quot;Externe Suche&quot;in einem benutzerdefinierten Formular ruft eine externe API auf und gibt Werte als Optionen in einem Dropdown-Feld zurück. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können eine oder mehrere dieser Optionen aus der Dropdown-Liste auswählen.

In diesem Artikel finden Sie Beispiele für die Verwendung des Felds Externe Suche , um dieselbe Instanz von Workfront oder eine öffentliche API aufzurufen. Sie können auch die externe Suche verwenden, um mit einem externen System wie Jira, Salesforce oder ServiceNow zu kommunizieren.

Weitere Informationen zum Hinzufügen eines externen Suchfelds zu einem benutzerdefinierten Formular sowie zusätzliche Definitionen der externen Lookup-Komponenten finden Sie unter [Formular mit dem Formularentwickler erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Einrichten eines externen Suchfelds für dieselbe Instanz von Workfront

Sie können die externe Suche verwenden, um Daten aus Ihrer Workfront-Instanz in das benutzerdefinierte Formular zu übertragen.

In diesem Beispiel wird gezeigt, wie die Workfront-API aufgerufen und Daten aus dem vorhandenen Feld &quot;Statusabfrage&quot;in das Feld &quot;Externe Suche&quot;übertragen werden.

1. Öffnen Sie das benutzerdefinierte Formular.
1. Suchen Sie auf der linken Bildschirmseite nach **Externe Suche** und ziehen Sie es in einen Bereich auf der Arbeitsfläche.
1. Geben Sie die **Titel** und **Name** für das Feld.
1. Wählen Sie die **Format** für das Feld.
1. Geben Sie den API-URL-Aufruf im **Basis-API-URL** -Feld.

   * Sie können $$HOST hinzufügen, um auf dieselbe Instanz zu verweisen.
   * Sie können $$QUERY hinzufügen, um die Ergebnisse anhand der Abfrage eines anderen Felds zu filtern.

   **Beispiel**
   `$$HOST/attask/api/v15.0/project/search?status={DE:StatusQuery}&$$QUERY`

1. Überprüfen Sie die **Abhängigkeiten** für die Felder, auf die dieses Suchfeld in der API verweist.

   Ein Abhängigkeitsfeld kann ein beliebiges benutzerdefiniertes oder natives Feld sein, das auf der Detailseite des Objekts vorhanden ist.

   In diesem Beispiel wird die `{DE:StatusQuery}` wird durch den Wert des benutzerdefinierten Felds StatusQuery ersetzt.

1. Wählen Sie die **HTTP-Methode**.

   Dies wird höchstwahrscheinlich **Get**.

1. Geben Sie die **JSON-Pfad** , um die Ergebnisse aus Ihrem API-Aufruf zu erhalten.

   **Beispiel**
   `$.data[*].name`

   >[!NOTE]
   >
   >**Kopfzeile** -Informationen sind für einen Aufruf an dieselbe Workfront-Instanz nicht erforderlich.

1. Klicks **Anwenden**.

   ![Einrichten des API-Aufrufs für Workfront in benutzerdefiniertem Formular](assets/external-lookup-to-workfront.png)

   Wenn das benutzerdefinierte Formular einem Workfront-Objekt (in diesem Beispiel einem Projekt) hinzugefügt wird, sieht es ähnlich aus.

   ![Benutzerdefiniertes Formular mit externem Suchfeld](assets/external-lookup-project-status-example1.png)

   ![Externe Suchoptionen basierend auf dem Status](assets/external-lookup-project-status-example2.png)

## Externes Suchfeld für eine öffentliche API einrichten

Mit der externen Suche können Sie eine externe, öffentliche API aufrufen und Daten abrufen.

In diesem Beispiel wird gezeigt, wie eine -API von Ländern aufgerufen wird (z. B. <https://api.first.org/data/v1/countries>), damit Sie nicht alle Ländernamen in den Dropdown-Optionen hartcodieren müssen.

1. Öffnen Sie das benutzerdefinierte Formular.
1. Suchen Sie auf der linken Bildschirmseite nach **Externe Suche** und ziehen Sie es in einen Bereich auf der Arbeitsfläche.
1. Geben Sie die **Titel** und **Name** für das Feld.
1. Wählen Sie die **Format** für das Feld.
1. Geben Sie den API-URL-Aufruf im **Basis-API-URL** -Feld.

   * Sie können $$QUERY hinzufügen, um die Abfragefilterung für Ihre Endbenutzer zu implementieren.

   **Beispiele**
Listet alle Länder auf: <https://api.first.org/data/v1/countries>

   Ermöglicht dem Benutzer die Suche nach einem beliebigen Land im Dropdown-Feld: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Ermöglicht dem Benutzer die Suche nach einem Land in einer Region: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Die verfügbaren Regionen werden in Workfront in einem separaten benutzerdefinierten Feld definiert.
   * Wenn der Benutzer eine Region im Formular auswählt, zeigt das Feld &quot;Externe Suche&quot;nur die Länder in dieser Region an (das Land, in dem sich die Region befindet, die in der API definiert ist). Der Benutzer kann auch nach einem Land in der ausgewählten Region suchen.

1. Überprüfen Sie die **Abhängigkeiten** für die Felder, auf die dieses Suchfeld in der API verweist.

   Ein Abhängigkeitsfeld kann ein beliebiges benutzerdefiniertes oder natives Feld sein, das auf der Detailseite des Objekts vorhanden ist.

   In diesem Beispiel wird die `{DE:Region}` durch den Wert des benutzerdefinierten Felds Region ersetzt.

1. Wählen Sie die **HTTP-Methode**.

   Dies wird höchstwahrscheinlich **Get**.

1. Geben Sie die **JSON-Pfad** , um die Ergebnisse aus Ihrem API-Aufruf zu erhalten.

   Diese Option ermöglicht das Extrahieren von Daten aus der JSON-Datei, die von der API-URL zurückgegeben wird. Es dient dazu, festzulegen, welche Werte aus dem JSON-Bereich in den Dropdown-Optionen angezeigt werden.

   **Beispiel**
   `$.data[*].country`

1. (Optional) Klicken Sie auf **Kopfzeile hinzufügen** und geben Sie das Schlüssel-Wert-Paar ein oder fügen Sie es ein, das für die Authentifizierung mit der API erforderlich ist.

   >[!NOTE]
   >
   >Die Felder &quot;Kopfzeile&quot;sind kein sicherer Ort zum Speichern von Anmeldeinformationen. Achten Sie darauf, was Sie eingeben und speichern.

1. (Optional) Wählen Sie **Dropdown für mehrere Auswahlen** , damit der Benutzer mehr als einen Wert in der Dropdown-Liste auswählen kann.

1. Klicks **Anwenden**.

   ![Einrichten des API-Aufrufs für die öffentliche API im benutzerdefinierten Formular](assets/external-lookup-to-api-for-countries.png)

   Wenn das benutzerdefinierte Formular einem Workfront-Objekt (in diesem Beispiel einem Projekt) hinzugefügt wird, sieht es ähnlich aus.

   ![Benutzerdefiniertes Formular mit externem Suchfeld](assets/external-lookup-countries-example1.png)

   ![Externe Suchoptionen für ein Land basierend auf einer Region](assets/external-lookup-countries-example2.png)

