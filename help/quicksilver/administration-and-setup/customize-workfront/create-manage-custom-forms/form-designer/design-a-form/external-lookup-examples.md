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
source-git-commit: 3838e355c16275b9e10fb92497f1698ac99c4fa4
workflow-type: tm+mt
source-wordcount: '1414'
ht-degree: 0%

---

# Beispiele für das externe Suchfeld in einem benutzerdefinierten Formular

Ein externes Suchfeld in einem benutzerdefinierten Formular ruft eine externe API auf und gibt Werte als Optionen in einem Dropdown-Feld zurück. Benutzer, die mit dem Objekt arbeiten, an das das benutzerdefinierte Formular angehängt ist, können eine oder mehrere dieser Optionen aus der Dropdown-Liste auswählen.

Dieser Artikel enthält Beispiele für die Verwendung des externen Suchfelds, um dieselbe Instanz von Workfront oder eine öffentliche API aufzurufen. Sie können die externe Suche auch verwenden, um mit einem externen System wie Jira, Salesforce oder ServiceNow zu kommunizieren.

Weitere Informationen zum Hinzufügen eines externen Suchfelds zu einem benutzerdefinierten Formular und zusätzliche Definitionen der externen Suchkomponenten finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Administrativer Zugriff auf benutzerdefinierte Formulare</p> </td> 
  </tr>  
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einrichten eines externen Suchfelds für dieselbe Instanz von Workfront

Sie können die externe Suche verwenden, um Daten aus Ihrer Workfront-Instanz in das benutzerdefinierte Formular zu übertragen.

<!--When someone accesses the field in the custom form, they will only see in the list of options what they have permissions to see in Workfront. For example, if you are showing a list of projects, the user would only see projects that are shared with them.-->

### Verwenden von nativen Workfront-Feldwerten in der externen Suche

Dieses Beispiel zeigt, wie die Workfront-API aufgerufen und eine Liste von Projekten in einem externen Suchfeld aufgefüllt wird, das anhand des Werts des benutzerdefinierten Felds „Statusabfrage“ und eines Suchbegriffs über $$QUERY nach Status gefiltert wird.

1. Öffnen Sie das benutzerdefinierte Formular.
1. Suchen Sie auf der linken Seite des Bildschirms nach **Externe Suche** und ziehen Sie sie in einen Abschnitt auf der Arbeitsfläche.
1. Geben Sie die **Bezeichnung** und **Name** für das Feld ein.
1. Wählen Sie das **Format** für das Feld aus.
1. Geben Sie den API-Aufruf in das Feld **Basis-API** URL ein.

   * Verwenden Sie $$HOST, um auf dieselbe Instanz von Workfront zu verweisen, in der sich das benutzerdefinierte Formular befindet.
   * Verwenden Sie $$QUERY , um die Ergebnisse basierend auf der Benutzereingabe dynamisch zu filtern.

   **Beispiel-API-Aufruf**
   `$$HOST/attask/api/v15.0/project/search?status={DE:Status Query}&description=$$QUERY`

1. Überprüfen Sie die **Abhängigkeiten** für die Felder, auf die im API-Aufruf verwiesen wird.

   Ein Abhängigkeitsfeld kann jedes benutzerdefinierte oder native Feld sein, das für das Objekt verfügbar ist. Wenn Sie z. B. ein benutzerdefiniertes Formular für Gruppen erstellen, das ein externes Suchfeld enthält, können Abhängigkeitsfelder alle in einer Gruppe verfügbaren Felder enthalten.

   In diesem Beispiel wird `{DE:Status Query}` dynamisch durch den Wert des benutzerdefinierten Felds „Statusabfrage“ für die aktuelle Gruppe ersetzt. Wenn das Formular also an Gruppe A angehängt ist, wird `{DE:Status Query}` durch den Wert ersetzt, der im Feld „Statusabfrage“ für diese Gruppe festgelegt ist.

1. Wählen Sie die **HTTP-Methode**.

   Dies wird höchstwahrscheinlich &quot;**&quot;**.

1. Geben Sie den **JSON-Pfad** ein, um die Ergebnisse aus Ihrem API-Aufruf abzurufen.

   **Beispiel**
   `$.data[*].name`

   >[!NOTE]
   >
   >**Header**-Informationen sind für einen Aufruf derselben Workfront-Instanz nicht erforderlich.

1. Klicken Sie auf **Übernehmen**.

   ![Einrichtung eines API-Aufrufs an Workfront in benutzerdefinierter Form](assets/external-lookup-to-workfront.png)

   Wenn das benutzerdefinierte Formular einem Workfront-Objekt (in diesem Beispiel einem Projekt) hinzugefügt wird, sieht es in etwa wie folgt aus.

   ![Benutzerdefiniertes Formular mit externem Suchfeld](assets/external-lookup-project-status-example1.png)

   ![Externe Suchoptionen basierend auf dem Status](assets/external-lookup-project-status-example2.png)

### Verwenden benutzerdefinierter Feldwerte in der externen Suche

Dieses Beispiel zeigt, wie Sie die Workfront-API aufrufen und Daten aus einem benutzerdefinierten Feld in Ihr externes Suchfeld einfügen. Das benutzerdefinierte Beispielfeld heißt „Benutzerdefinierte Farben“.

1. Öffnen Sie das benutzerdefinierte Formular.
1. Suchen Sie auf der linken Seite des Bildschirms nach **Externe Suche** und ziehen Sie sie in einen Abschnitt auf der Arbeitsfläche.
1. Geben Sie die **Bezeichnung** und **Name** für das Feld ein.
1. Wählen Sie das **Format** für das Feld aus.
1. Geben Sie den API-URL-Aufruf in das Feld **Basis-API** URL ein.

   **Beispiel**
   `$$HOST/attask/api/v18.0/PORT/search?ID={portfolioID}&fields=parameterValues`

1. Überprüfen Sie **Abhängigkeiten** für die Felder, auf die dieses Suchfeld in der API verweist.

   Ein Abhängigkeitsfeld kann jedes benutzerdefinierte oder native Feld sein, das auf der Detailseite des -Objekts vorhanden ist.

1. Wählen Sie die **HTTP-Methode**.

   Dies wird höchstwahrscheinlich &quot;**&quot;**.

1. Geben Sie den **JSON-Pfad** ein, um die Ergebnisse aus Ihrem API-Aufruf abzurufen.

   **Beispiel**
   `$.data[*].parameterValues.["DE:Combo Colors"]`

   * „parameterValues“ bezieht sich auf jedes benutzerdefinierte Feld in Workfront für das Objekt, an dem Sie sich befinden.
   * In diesem Beispiel ist „DE:ComboColors“ das spezifische benutzerdefinierte Feld, das die abzurufenden Werte enthält.

   >[!NOTE]
   >
   >**Header**-Informationen sind für einen Aufruf derselben Workfront-Instanz nicht erforderlich.

1. Klicken Sie auf **Übernehmen**.

   Wenn das benutzerdefinierte Formular zu einem Workfront-Objekt hinzugefügt wird, werden alle Werte im Feld „Kombinationsfarben“ in der Dropdown-Liste Externes Suchfeld angezeigt.

## Einrichten eines externen Suchfelds für die Workfront Planning-API

In der Workfront Planning-API ist ein Endpunkt verfügbar, mit dem Datensätze nach Datensatztyp-ID über die Get-Methode gesucht werden können. Sie können diesen Endpunkt verwenden, um Planungsdatensätze in externen Suchfeldern zu referenzieren.

* **Basis-API-URL:** `$$HOST/maestro/api/v1/records/search?recordTypeId={recordTypeID}`
* **HTTP-Methode:** GET
* **JSON-Pfad:** `$.records[*].data.{fieldID}`

  **{fieldID}** ist das Feld, das im benutzerdefinierten Formular für Endbenutzer in den externen Suchergebnissen angezeigt werden soll.

Weitere Informationen finden Sie unter [Workfront Planning API](/help/quicksilver/planning/general/planning-api-basics.md).

## Einrichten eines externen Suchfelds für eine öffentliche API

Mit der externen Suche können Sie eine externe, öffentliche API aufrufen und Daten abrufen.

Dieses Beispiel zeigt, wie Sie eine API von Ländern aufrufen (z. B. <https://api.first.org/data/v1/countries>), damit Sie nicht alle Ländernamen in den Dropdown-Optionen hart codieren müssen.

1. Öffnen Sie das benutzerdefinierte Formular.
1. Suchen Sie auf der linken Seite des Bildschirms nach **Externe Suche** und ziehen Sie sie in einen Abschnitt auf der Arbeitsfläche.
1. Geben Sie die **Bezeichnung** und **Name** für das Feld ein.
1. Wählen Sie das **Format** für das Feld aus.
1. Geben Sie den API-URL-Aufruf in das Feld **Basis-API** URL ein.

   * Sie können $$QUERY hinzufügen, um die Abfragefilterung für Ihre Endbenutzer zu implementieren.

   **Beispiele**
Listet alle Länder auf: <https://api.first.org/data/v1/countries>

   Ermöglicht dem Benutzer, im Dropdown-Feld nach einem beliebigen Land zu suchen: <https://api.first.org/data/v1/countries?q=$$QUERY>

   Ermöglicht die Suche nach einem Land in einer Region: <https://api.first.org/data/v1/countries?region={DE:Region}&q=$$QUERY>

   * Die verfügbaren Regionen werden in Workfront in einem separaten benutzerdefinierten Feld definiert.
   * Wenn Benutzende im Formular eine Region auswählen, zeigt das Feld Externe Suche nur die Länder in dieser Region an (welches Land sich in welcher Region befindet, wird in der API definiert). Der Benutzer kann auch in der ausgewählten Region nach einem Land suchen.

1. Überprüfen Sie **Abhängigkeiten** für die Felder, auf die dieses Suchfeld in der API verweist.

   Ein Abhängigkeitsfeld kann jedes benutzerdefinierte oder native Feld sein, das auf der Detailseite des -Objekts vorhanden ist.

   In diesem Beispiel wird der `{DE:Region}` durch den Wert des benutzerdefinierten Felds Region ersetzt.

1. Wählen Sie die **HTTP-Methode**.

   Dies wird höchstwahrscheinlich &quot;**&quot;**.

1. Geben Sie den **JSON-Pfad** ein, um die Ergebnisse aus Ihrem API-Aufruf abzurufen.

   Diese Option ermöglicht das Extrahieren von Daten aus der von der API-URL zurückgegebenen JSON. Sie dient als Möglichkeit, festzulegen, welche Werte aus dem JSON-Code in den Dropdown-Optionen angezeigt werden.

   **Beispiel**
   `$.data[*].country`

1. (Optional) Klicken Sie auf **Kopfzeile hinzufügen** und geben Sie das Schlüssel-Wert-Paar ein, das für die Authentifizierung mit der API erforderlich ist, oder fügen Sie es ein.

   >[!NOTE]
   >
   >Die Header-Felder sind kein sicherer Ort zum Speichern von Anmeldeinformationen, und Sie sollten darauf achten, was Sie eingeben und speichern.

1. (Optional) Wählen Sie **Mehrfachauswahl-Dropdown** aus, damit Benutzende mehr als einen Wert im Dropdown-Menü auswählen können.

1. Klicken Sie auf **Übernehmen**.

   ![Einrichtung eines API-Aufrufs an eine öffentliche API in benutzerdefinierter Form](assets/external-lookup-to-api-for-countries.png)

   Wenn das benutzerdefinierte Formular einem Workfront-Objekt (in diesem Beispiel einem Projekt) hinzugefügt wird, sieht es in etwa wie folgt aus.

   ![Benutzerdefiniertes Formular mit externem Suchfeld](assets/external-lookup-countries-example1.png)

   ![Externe Suchoptionen für ein Land basierend auf einer Region](assets/external-lookup-countries-example2.png)

## Zusätzliche Anwendungsfälle für externe Suchfelder

Es gibt viele weitere Anwendungsfälle für die Erstellung einer externen Suche.

**Anwendungsfall:** Ersetzen Sie Felder mit automatischer Textvervollständigung, da sie Probleme beim Reporting verursachen können.
**Lösung** Verwenden Sie einen API-Aufruf an vorhandene Objekte im System.

Beispiel-Basis-API-URL für Vorlagen, um ein Feld mit automatischer Textvervollständigung zu ersetzen:
`$$HOST/attask/api/v17.0/tmpl/search?isActive=true&name_Sort=asc`

**Anwendungsfall:** Dropdown-Felder mit mehr Funktionen erstellen (z. B. Zeilenumbruch im externen Suchfeld).
**Lösung** Verwenden Sie einen API-Aufruf an vorhandene Objekte im System oder erstellen Sie ein neues Objekt und verwenden Sie einen API-Aufruf an dieses Objekt.

**Anwendungsfall:** Definieren Sie eine Möglichkeit für Benutzende, ihre eigenen Felder außerhalb des Bereichs für benutzerdefinierte Formulare zu verwalten. Richten Sie das externe Suchfeld ein, und Sie können den Objekten, aus denen das Feld besteht, Benutzer zuweisen. Diese Option eignet sich gut für Felder und Teams mit hoher Wartung.
**Lösung:** Erstellen Sie ein neues Objekt und verwenden Sie einen API-Aufruf an dieses Objekt.

**Anwendungsfall:** Integration mit Objekten außerhalb von Workfront. Beispielsweise den Zugriff auf ein anderes System, um den Namen jedes Benutzers abzurufen, anstatt in einem Feld mit automatischer Textvervollständigung eingeschränkt zu werden.
**Lösung:** Webhook/Fusion-Automatisierung zur Verbindung mit anderen Systemen.

