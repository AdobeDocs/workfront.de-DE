---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Workfront-Module
description: Sie können den Adobe Workfront Fusion Adobe Workfront-Connector verwenden, um Ihre Prozesse in Workfront zu automatisieren. Wenn Sie über eine Workfront Fusion for Work Automation and Integration-Lizenz verfügen, können Sie damit auch eine Verbindung zu Apps und Diensten von Drittanbietern herstellen.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: b84d2d41-a983-4ea3-b331-0302bfcf8a2b
source-git-commit: 0558f72fb8a7fc52d06adc0421082e20520c0b8f
workflow-type: tm+mt
source-wordcount: '5935'
ht-degree: 2%

---

# [!DNL Adobe Workfront] Module

Sie können die [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] Connector zur Automatisierung Ihrer Prozesse in [!DNL Workfront]. Wenn Sie [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] -Lizenz verwenden, können Sie damit auch eine Verbindung zu Apps und Diensten von Drittanbietern herstellen.

Die [!DNL Workfront] -Connector wird nicht mit der Anzahl der aktiven Apps angerechnet, die für Ihr Unternehmen verfügbar sind. Alle Szenarien, auch wenn sie nur die [!DNL Workfront] App verwenden, zählen Sie mit der Gesamtszenario-Anzahl Ihrer Organisation.

Weitere Informationen zu den verfügbaren Apps und Szenarien Ihrer Organisation finden Sie unter [Organisationen](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] Organisationen und Teams](../../workfront-fusion/organizations/organizations-and-teams.md).

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>


Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]

Die [!DNL Workfront] Connector verwendet OAuth 2.0 für die Verbindung mit [!DNL Workfront].

Sie können eine Verbindung zu Ihrem [!DNL Workfront] direkt in einer [!DNL Workfront Fusion] -Modul.

1. Klicken Sie in einem beliebigen Adobe Authenticator-Modul auf **Hinzufügen** neben dem Feld Verbindung .
1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Verbindungsname]</td>
        <td>
          <p>Geben Sie einen Namen für die neue Verbindung ein.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Umgebung]</td>
        <td>
          <p>Wählen Sie aus, ob eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung hergestellt werden soll.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Verbindungstyp]</td>
        <td>
          <p>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!DNL Workfront] Client-ID. Dies finden Sie im Bereich "OAuth2-Anwendungen"des Einrichtungsbereichs in Workfront. Öffnen Sie die spezifische Anwendung, mit der Sie eine Verbindung herstellen, um die Client-ID anzuzeigen.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihre [!DNL Workfront] Client-ID. Dies finden Sie im Bereich "OAuth2-Anwendungen"des Einrichtungsbereichs in Workfront. Öffnen Sie die spezifische Anwendung, mit der Sie eine Verbindung herstellen, um die Client-ID anzuzeigen.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentifizierungs-URL]</td>
        <td>Dies kann der Standardwert bleiben, oder Sie können die URL Ihrer Workfront-Instanz eingeben, gefolgt von <code>/integrations/oauth2</code>. <p>Beispiel: <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Host-Präfix]</td>
        <td>In den meisten Fällen sollte dieser Wert <code>origin</code>.
      </tr>
    </tbody>
    </table>

1. Klicks **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* Wenn keine Schaltfläche zum Anmelden bei SAML angezeigt wird, hat Ihr Unternehmen Single Sign-On (SSO) nicht aktiviert. Sie können sich mit Ihrem Benutzernamen und Passwort anmelden.
>   
>   Weitere Informationen zur einmaligen Anmeldung finden Sie unter [Übersicht über Single Sign-on [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* OAuth 2.0-Verbindungen zum [!DNL Workfront] API ist nicht mehr auf API-Schlüssel angewiesen.

## [!DNL Workfront] Module und ihre Felder

Bei der Konfiguration [!DNL Workfront] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Workfront] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

>[!NOTE]
>
>Wenn in einem Workfront-Modul nicht die aktuellsten Felder angezeigt werden, liegt dies möglicherweise an Caching-Problemen. Warten Sie eine Stunde und versuchen Sie es erneut.

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Ereignisse beobachten]**

Dieses Trigger-Modul führt ein Szenario in Echtzeit aus, wenn Objekte eines bestimmten Typs in Workfront hinzugefügt, aktualisiert oder gelöscht werden

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

1. Klicks **[!UICONTROL Hinzufügen]** rechts von der **Webhook** ankreuzen.

1. Konfigurieren Sie den Webhook im **[!UICONTROL Hinzufügen eines Hooks]** angezeigt.

   Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Geben Sie einen neuen Namen für den Webhook ein.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Verbindung]</td> 
      <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Type]</td> 
      <td>Wählen Sie den Typ [!DNL Workfront] notieren, dass das Modul überwacht werden soll.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Wählen Sie aus, ob Sie den alten oder neuen Status überwachen möchten.<ul><li><p><b>[!UICONTROL Neuer Status]</b></p><p>Trigger eines Szenarios bei Datensatzänderungen <b>nach</b> einen angegebenen Wert.</p><p>Wenn beispielsweise der Status auf [!UICONTROL Neuer Status] festgelegt ist und der Filter auf [!UICONTROL Status] [!UICONTROL Entspricht] [!UICONTROL In Bearbeitung] gesetzt ist, wird der Webhook auf einen Trigger gesetzt, wenn [!UICONTROL Status] in [!UICONTROL In Bearbeitung] geändert wird, unabhängig davon, welcher Status zuvor war. </p></li><li><p><b>[!UICONTROL Alter Staat]</b></p><p>Trigger eines Szenarios bei Datensatzänderungen <b>von</b> einen angegebenen Wert.</p><p>Wenn beispielsweise der Status auf [!UICONTROL Old State] gesetzt ist und der Filter auf [!UICONTROL Status] [!UICONTROL Entspricht] [!UICONTROL In Bearbeitung] festgelegt ist, wird der Webhook auf einen Trigger angewendet, wenn ein [!UICONTROL Status], der derzeit [!UICONTROL In Bearbeitung] ist, zu einem anderen Status wechselt. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Ereignisfilter]</p> </td> 
      <td> <p>Sie können Filter festlegen, um nur Datensätze zu überwachen, die den von Ihnen ausgewählten Kriterien entsprechen.</p> <p>Geben Sie für jeden Filter das Feld, das der Filter auswerten soll, den Operator und den Wert ein, die der Filter zulassen soll. Sie können mehrere Filter verwenden, indem Sie UND-Regeln hinzufügen.</p> <p>Hinweis: Filter in vorhandenen [!DNL Workfront] Webhooks. So richten Sie verschiedene Filter für ein [!DNL Workfront] -Ereignis-Abonnements, entfernen Sie den aktuellen Webhook und erstellen Sie einen neuen.</p> <p>Weitere Informationen zu Ereignisfiltern finden Sie unter <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Ereignisabonnementfilter in [!DNL Workfront] &gt; [!UICONTROL Watch Events] -Module</a> in diesem Artikel.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Von dieser Verbindung vorgenommene Ereignisse ausschließen</td> 
      <td>Aktivieren Sie diese Option, um Ereignisse auszuschließen, die mit demselben Connector erstellt oder aktualisiert wurden, den dieses Trigger-Modul verwendet. Dies kann Situationen verhindern, in denen ein Szenario selbst Trigger hat, sodass es sich in einer Endlosschleife wiederholt.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p>Festlegen, ob das Szenario überwacht werden soll <strong>Nur neue Datensätze</strong>, <strong>[!UICONTROL Nur aktualisierte Datensätze]</strong>, <strong>[!UICONTROL Neue und aktualisierte Datensätze]</strong>oder <strong>[!DNL Deleted Records Only]</strong>.</p> <p>Hinweis: Wenn Sie <strong>[!UICONTROL Neue und aktualisierte Datensätze]</strong>, erstellt die Webhook-Erstellung zwei Ereignis-Abonnements (für dieselbe Webhook-Adresse).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Nachdem der Webhook erstellt wurde, können Sie die Adresse des Endpunkts anzeigen, an den Ereignisse gesendet werden.

Weitere Informationen finden Sie im Abschnitt . [Beispiele für Ereignis-Payloads](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) im [!DNL Workfront] Hilfeartikel [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Überwachungsfeld]**

Dieses Trigger-Modul führt ein Szenario aus, wenn ein von Ihnen angegebenes Feld aktualisiert wird. Das Modul gibt sowohl den alten als auch den neuen Wert des angegebenen Felds zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ [!DNL Workfront] notieren, dass das Modul überwacht werden soll.</p> <p>Wählen Sie beispielsweise [!UICONTROL Task] aus, wenn Sie das Szenario jedes Mal ausführen möchten, wenn ein Datensatzfeld in einer Aufgabe aktualisiert wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Wählen Sie das Feld aus, das das Modul auf Updates überwachen soll. Diese Felder spiegeln die Felder wider, die Ihre [!DNL Workfront] -Administrator hat Tracking eingerichtet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Aufzeichnen von Daten]**

Dieses Trigger-Modul führt ein Szenario aus, wenn Objekte eines bestimmten Typs hinzugefügt, aktualisiert oder beides. Das Modul gibt alle mit dem Datensatz oder den Datensätzen verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen. In der Ausgabe gibt das Modul an, ob jeder Datensatz neu oder aktualisiert ist.

Datensätze, die im angegebenen Zeitraum hinzugefügt und aktualisiert wurden, werden als neue Datensätze zurückgegeben.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Festlegen, ob das Szenario überwacht werden soll <strong>Nur neue Datensätze</strong>, <strong>[!UICONTROL Nur aktualisierte Datensätze]</strong>oder <strong>[!UICONTROL Neue und aktualisierte Datensätze]</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>(Wird angezeigt, nachdem Sie eine <strong>Filter</strong>. Wählen Sie den Typ [!DNL Workfront] notieren, dass das Modul überwacht werden soll.</p> <p>Wenn Sie beispielsweise jedes Mal, wenn ein neues Projekt erstellt wird, das Szenario starten möchten, wählen Sie [!UICONTROL Projekt]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optionaler Filter]</td> 
   <td> <p>(Erweitert) Geben Sie eine API-Code-Zeichenfolge ein, um zusätzliche Parameter oder Code zu definieren, die Ihre Kriterien verfeinern. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++


### Aktionen

<!--
* [Convert object](#convert-object) 
* [Create a record (attaching custom forms)](#create-a-record-attaching-custom-forms) 
* [Create a record](#create-a-record) 
* [Custom API Call](#custom-api-call) 
* [Delete Record](#delete-record) 
* [Download Document](#download-document) 
* [Misc Action](#misc-action) 
* [Read a Record](#read-a-record) 
* [Update Record](#update-record) 
* [Upload Document](#upload-document)
-->

+++ **[!UICONTROL Konvertierungsobjekt]**

Dieses Aktionsmodul führt eine der folgenden Konvertierungen durch:

* Problem in Projekt konvertieren
* Problem in Aufgabe konvertieren
* Aufgabe in Projekt konvertieren

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Objekttyp]</td> 
   <td> <p>Wählen Sie den Objekttyp aus, den Sie konvertieren möchten. Dies ist der Typ, den das Objekt vor der Konvertierung hat.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Convert to]</td> 
   <td>Wählen Sie das Objekt aus, in das Sie es konvertieren möchten. Dies ist der Typ, den das Objekt nach der Konvertierung hat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL &lt;object&gt; ID]</td> 
   <td> <p>Geben Sie die Kennung des Objekts ein. </p> <p>Hinweis: Bei der Eingabe der ID eines Objekts können Sie mit der Eingabe des Objektnamens beginnen und dieses dann aus der Liste auswählen. Das Modul gibt dann die entsprechende ID in das Feld ein.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Vorlagen-ID]</td> 
   <td> <p>Wenn Sie in ein Projekt konvertieren, wählen Sie die Vorlagen-ID aus, die Sie für das Projekt verwenden möchten.</p> <p>Hinweis: Bei der Eingabe der ID eines Objekts können Sie mit der Eingabe des Objektnamens beginnen und dieses dann aus der Liste auswählen. Das Modul gibt dann die entsprechende ID in das Feld ein.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Benutzerdefinierte Formulare]</td> 
   <td>Wählen Sie benutzerdefinierte Formulare aus, die Sie dem neu konvertierten Objekt hinzufügen möchten, und geben Sie dann Werte für die Felder des benutzerdefinierten Formulars ein.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Optionen]</td> 
   <td> <p>Aktivieren Sie alle Optionen, die Sie beim Konvertieren des Objekts benötigen. Je nachdem, in welches Objekt Sie konvertieren oder von welchem Objekt Sie konvertieren, sind Optionen verfügbar.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Datensatz erstellen (benutzerdefinierte Formulare anhängen)]**

Dieses Aktionsmodul erstellt ein Objekt wie ein Projekt, eine Aufgabe oder ein Problem in [!DNL Workfront]und ermöglicht das Hinzufügen eines benutzerdefinierten Formulars zum neuen Objekt. Mit dem -Modul können Sie auswählen, welche der Objektfelder im -Modul verfügbar sind.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie können dieses Modul beispielsweise verwenden, um eine Aufgabe in [!DNL Workfront] wenn ein Client eine neue Zeile in einer [!DNL Google Sheets] Liste der zu erledigenden Aufgaben.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

Stellen Sie sicher, dass Sie die Mindestanzahl der Eingabefelder angeben. Wenn Sie beispielsweise ein Problem erstellen möchten, müssen Sie im Feld Projekt-ID eine gültige ID für das übergeordnete Projekt angeben, um anzugeben, wo das Problem in Workfront leben soll. Sie können das Zuordnungsbedienfeld verwenden, um diese Informationen einem anderen Modul in Ihrem Szenario zuzuordnen, oder Sie können sie manuell eingeben, indem Sie den Namen eingeben und ihn dann aus der Liste auswählen.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ [!DNL Workfront] notieren, dass das Modul erstellt werden soll.</p> <p>Wenn Sie beispielsweise ein Projekt erstellen möchten, wählen Sie in der Dropdown-Liste die Option [!UICONTROL Projekt] aus und stellen Sie sicher, dass Sie Zugriff auf Daten (aus früheren Modulen im Szenario) haben, die das Projekt ausfüllen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td> <p>Wählen Sie die Felder aus, die für die Dateneingabe verfügbar sein sollen. Auf diese Weise können Sie diese Felder verwenden, ohne durch die Felder zu scrollen, die Sie nicht benötigen.</p> <p>Verwenden Sie für Felder in benutzerdefinierten Formularen den <b>[!UICONTROL Benutzerdefiniertes Formular anhängen]</b> -Feld.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Benutzerdefiniertes Formular anhängen]</td> 
   <td>Wählen Sie benutzerdefinierte Formulare aus, die Sie dem neuen Objekt hinzufügen möchten, und geben Sie dann Werte für diese Felder ein.</td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Bei der Eingabe der ID eines Objekts können Sie mit der Eingabe des Objektnamens beginnen und dieses dann aus der Liste auswählen. Das Modul gibt dann die entsprechende ID in das Feld ein.
>* Beim Eingeben des Texts für ein benutzerdefiniertes Feld oder ein [!UICONTROL Hinweis] -Objekt (Kommentar oder Antwort) verwenden, können Sie HTML-Tags in der [!UICONTROL Hinweis: Text] -Feld, um Rich-Text zu erstellen, z. B. fett oder kursiv gedruckten Text.
>
>  Weitere Informationen zu Rich-Text in Updates finden Sie unter [Hinzufügen einer Aktualisierung zu einem Arbeitselement](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Datensatz erstellen]**

Dieses Aktionsmodul erstellt ein Objekt wie ein Projekt, eine Aufgabe oder ein Problem in Workfront. Mit dem -Modul können Sie auswählen, welche der Objektfelder im -Modul verfügbar sind.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie können dieses Modul beispielsweise verwenden, um eine Aufgabe in [!DNL Workfront] wenn ein Client eine neue Zeile in einer Google Tabellen-Liste mit Aufgaben hinzufügt, die erledigt werden müssen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

Stellen Sie sicher, dass Sie die Mindestanzahl der Eingabefelder angeben. Wenn Sie beispielsweise ein Problem erstellen möchten, müssen Sie im Feld Projekt-ID eine gültige ID für das übergeordnete Projekt angeben, um anzugeben, wo das Problem in Workfront leben soll. Sie können das Zuordnungsbedienfeld verwenden, um diese Informationen einem anderen Modul in Ihrem Szenario zuzuordnen, oder Sie können sie manuell eingeben, indem Sie den Namen eingeben und ihn dann aus der Liste auswählen.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ [!DNL Workfront] notieren, dass das Modul erstellt werden soll.</p> <p>Wenn Sie beispielsweise ein Projekt erstellen möchten, wählen Sie in der Dropdown-Liste die Option [!UICONTROL Projekt] aus und stellen Sie sicher, dass Sie Zugriff auf Daten (aus früheren Modulen im Szenario) haben, die das Projekt ausfüllen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td>Wählen Sie die Felder aus, die für die Dateneingabe verfügbar sein sollen. Auf diese Weise können Sie diese Felder verwenden, ohne durch die Felder zu scrollen, die Sie nicht benötigen.</td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Bei der Eingabe der ID eines Objekts können Sie mit der Eingabe des Objektnamens beginnen und dieses dann aus der Liste auswählen. Das Modul gibt dann die entsprechende ID in das Feld ein.
>* Beim Eingeben des Texts für ein benutzerdefiniertes Feld oder ein [!UICONTROL Hinweis] -Objekt (Kommentar oder Antwort) verwenden, können Sie HTML-Tags in der [!UICONTROL Hinweis: Text] -Feld, um Rich-Text zu erstellen, z. B. fett oder kursiv gedruckten Text.
>
>  Weitere Informationen zu Rich-Text in Updates finden Sie unter [Hinzufügen einer Aktualisierung zu einem Arbeitselement](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Benutzerspezifischer API-Aufruf]**

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Workfront] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL Workfront] Module.

Das Modul gibt die folgenden Informationen zurück:

* **[!UICONTROL Status-Code]** (Zahl): Zeigt an, ob Ihre HTTP-Anforderung erfolgreich oder fehlgeschlagen ist. Dies sind Standardcodes, die Sie im Internet nachschlagen können.
* **[!UICONTROL Kopfzeilen]** (Objekt): Ein detaillierterer Kontext für den Antwort-/Statuscode, der nicht mit dem Ausgabetext in Verbindung steht. Nicht alle Header, die in einem Antwortheader angezeigt werden, sind Antwortheader, sodass einige möglicherweise nicht nützlich für Sie sind.

  Die Antwortheader hängen von der HTTP-Anforderung ab, die Sie beim Konfigurieren des Moduls ausgewählt haben.

* **[!UICONTROL body]** (Objekt): Je nach der HTTP-Anforderung, die Sie beim Konfigurieren des Moduls ausgewählt haben, können Sie einige Daten zurückerhalten. Diese Daten, z. B. die Daten aus einer GET-Anfrage, sind in diesem Objekt enthalten.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein<code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API-Version]</td> 
   <td>Wählen Sie die Version der [!DNL Workfront] -API, die das -Modul verwenden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu. Dadurch wird der Inhaltstyp der Anforderung bestimmt.</p> <p>Beispiel:<code> {"Content-type":"application/json"}</code></p> <p>Hinweis: Wenn Fehler auftreten und es schwierig ist, ihren Ursprung zu bestimmen, sollten Sie die Kopfzeilen basierend auf der Variablen [!DNL Workfront] Dokumentation. Wenn Ihr benutzerspezifischer API-Aufruf einen 422-HTTP-Anforderungsfehler zurückgibt, versuchen Sie, einen <code>"Content-Type":"text/plain"</code> -Kopfzeile.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> <p>Tipp: Es wird empfohlen, Informationen nicht als Abfrageparameter, sondern über den JSON-Hauptteil zu senden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Datensatz löschen]**

Dieses Aktionsmodul löscht ein Objekt, z. B. ein Projekt, eine Aufgabe oder ein Problem in Workfront.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Löschvorgang erzwingen]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass der Datensatz gelöscht wird, auch wenn die [!DNL Workfront] Die Benutzeroberfläche fordert eine Bestätigung des Löschvorgangs an.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Eindeutige Angabe [!DNL Workfront] Kennung des Datensatzes, den das Modul löschen soll.</p> <p>Um die ID abzurufen, öffnen Sie die [!DNL Workfront] -Objekt in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ [!DNL Workfront] notieren, dass das Modul gelöscht werden soll.</td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>Wir empfehlen die folgende Szenario-Konfiguration, um zu verhindern, dass Datensätze aufgrund asynchroner Vorgänge nicht gelöscht werden.
>
>1. Den Datensatz synchron löschen.
>1. Fügen Sie dem Modul Datensatz löschen die Fehlerbehandlung hinzu, um den Fehler zu ignorieren, der durch das 40-Sekunden-Timeout verursacht wurde.


+++

+++ **[!UICONTROL Dokument herunterladen]**

Dieses Aktionsmodul lädt ein Dokument aus Workfront herunter.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt den Inhalt, den Dateinamen, die Dateierweiterung und die Dateigröße des Dokuments zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dokument-ID]</td> 
   <td> <p>Zuordnung oder manuelle Eingabe der eindeutigen [!DNL Workfront] ID des Dokuments, das Sie vom Modul herunterladen möchten.</p> <p>Um die ID abzurufen, öffnen Sie die [!DNL Workfront] -Objekt in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Verschiedene Aktionen]**

Mit diesem Aktionsmodul können Sie Aktionen für die API ausführen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ [!DNL Workfront] -Datensatz, mit dem das -Modul interagieren soll.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Aktion]</td> 
   <td> <p>Wählen Sie die Aktion aus, die das Modul ausführen soll.</p> <p>Je nach ausgewähltem [!UICONTROL Record Type] und [!UICONTROL Action] müssen Sie möglicherweise zusätzliche Felder ausfüllen. Einige Kombinationen dieser beiden Einstellungen erfordern möglicherweise nur eine Datensatz-ID, während andere (z. B. Projekt für die <strong>[!UICONTROL Record Type]</strong> und [!UICONTROL Anlagenvorlage] für die <strong>[!UICONTROL Aktion]</strong>) zusätzliche Informationen benötigen (z. B. eine Objekt-ID und eine Vorlagen-ID).</p> <p>Weitere Informationen zu einzelnen Feldern finden Sie unter <a href="http://developer.workfront.com/">Workfront-Entwicklerdokumentation</a>. <p><strong>Hinweis</strong>: Die Entwicklerdokumentations-Site enthält Informationen nur über API-Version 14, enthält aber trotzdem wertvolle Informationen für API-Aufrufe. </p> 
    <ol> 
     <li value="1"> <p>Wählen Sie im linken Navigationsbereich des [!DNL Workfront] Seite mit Entwicklerdokumentation. Die folgenden Typen haben eigene Seiten:</p> 
      <ul> 
       <li> <p>[!UICONTROL Projekte]</p> </li> 
       <li> <p>[!UICONTROL Aufgaben]</p> </li> 
       <li> <p>[!UICONTROL Probleme]</p> </li> 
       <li> <p>[!UICONTROL Benutzer]</p> </li> 
       <li> <p>[!UICONTROL Dokumente]</p> </li> 
      </ul> <p>Wählen Sie für alle anderen Datensatztypen die Option <b>[!UICONTROL Andere Objekte und Endpunkte]</b>und suchen Sie den Datensatztyp auf den alphabetisch sortierten Seiten.</p> </li> 
     <li value="2"> <p>Suchen Sie auf der Seite des entsprechenden Datensatztyps (Strg-F oder Befehl-F) nach der Aktion.</p> </li> 
     <li value="3"> <p>Zeigen Sie Beschreibungen für verfügbare Felder unter der ausgewählten Aktion an.</p> </li> 
    </ol> <p>Hinweis:  <p>Beim Erstellen eines Testversands durch die [!DNL Workfront] [!UICONTROL Misc Action]-Modul verwenden, wird empfohlen, einen Testversand ohne erweiterte Optionen zu erstellen und dann den Testversand mithilfe des [!DNL Workfront Proof] SOAP-API.</p> <p>Weitere Informationen zum Erstellen eines Testversands mit dem [!DNL Workfront] API (die dieses Modul verwendet), siehe <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Erweiterte Testversandoptionen bei der Erstellung eines Testversands über die [!DNL Adobe Workfront] API</a></p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Eindeutige Eingabe oder Zuordnung [!DNL Workfront] Kennung des Datensatzes, mit dem das Modul interagieren soll.<p>Um die ID abzurufen, öffnen Sie die [!DNL Workfront] -Objekt in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Datensatz lesen]**

Dieses Aktionsmodul ruft Daten aus einem einzelnen Datensatz ab.

Sie geben die Kennung des Datensatzes an. Sie können auch angeben, welche zugehörigen Datensätze das Modul lesen soll.

Wenn der Datensatz, den das Modul liest, beispielsweise ein Projekt ist, können Sie festlegen, dass die Aufgaben des Projekts gelesen werden sollen.

Das Modul gibt ein Array von Daten aus den Standardfeldern für die angegebene Ausgabe zurück.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Verbindung]</td>

<td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>

<td>Wählen Sie die [!DNL Workfront] -Objekttyp, den das Modul lesen soll.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Ausgaben]</td>

<td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Referenzen]</td>
   <td>Wählen Sie beliebige Referenzfelder aus, die Sie in die Ausgabe aufnehmen möchten.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Sammlungen]</td>
   <td>Wählen Sie beliebige Referenzfelder aus, die Sie in die Ausgabe aufnehmen möchten.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL ID]</td>
   <td> <p>Eindeutige Angabe [!DNL Workfront] Kennung des Datensatzes, den das Modul lesen soll.</p> <p>Um die ID abzurufen, öffnen Sie die [!DNL Workfront] -Objekt in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++

+++ **[!UICONTROL Datensatz aktualisieren]**

Dieses Aktionsmodul aktualisiert ein Objekt, z. B. ein Projekt, eine Aufgabe oder ein Problem. Mit dem -Modul können Sie auswählen, welche der Objektfelder im -Modul verfügbar sind.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die ID des Objekts und aller zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Eindeutige Angabe [!DNL Workfront] Kennung des Datensatzes, den das Modul aktualisieren soll.</p> <p>Um die ID abzurufen, öffnen Sie die [!DNL Workfront] -Objekt in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Wählen Sie den Typ [!DNL Workfront] notieren, dass das Modul aktualisiert werden soll.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Wählen Sie die Felder aus, die für die Dateneingabe verfügbar sein sollen. Auf diese Weise können Sie diese Felder verwenden, ohne durch die Felder zu scrollen, die Sie nicht benötigen.</td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

>[!NOTE]
>
>* Bei der Eingabe der ID eines Objekts können Sie mit der Eingabe des Objektnamens beginnen und dieses dann aus der Liste auswählen. Das Modul gibt dann die entsprechende ID in das Feld ein.
>* Beim Eingeben des Texts für ein benutzerdefiniertes Feld oder ein [!UICONTROL Hinweis] -Objekt (Kommentar oder Antwort) verwenden, können Sie HTML-Tags in der [!UICONTROL Hinweis: Text] -Feld, um Rich-Text zu erstellen, z. B. fett oder kursiv gedruckten Text.
>
>  Weitere Informationen zu Rich-Text in Updates finden Sie unter [Hinzufügen einer Aktualisierung zu einem Arbeitselement](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Update der Arbeit](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Dokument hochladen]**

Dieses Aktionsmodul lädt ein Dokument in ein [!DNL Workfront] -Objekt, z. B. ein Projekt, eine Aufgabe oder ein Problem.

Sie geben den Speicherort für das Dokument, die Datei, die Sie hochladen möchten, und einen optionalen neuen Namen für die Datei an.

Das Modul gibt die ID des Dokuments sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Eindeutige Angabe [!DNL Workfront] Kennung des Datensatzes, in den Sie das Dokument hochladen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verwandter Datensatztyp]</td> 
   <td>Wählen Sie den Typ [!DNL Workfront] notieren, wo das Modul das Dokument hochladen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++

### Suchvorgänge

<!--
* [Read Related Records](#read-related-records) 
* [Search](#search)
-->

+++ **[!UICONTROL Verwandte Aufzeichnungen lesen]**

Dieses Suchmodul liest Datensätze, die mit der von Ihnen angegebenen Suchabfrage übereinstimmen, in einem bestimmten übergeordneten Objekt.

Sie geben an, welche Felder in die Ausgabe aufgenommen werden sollen. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des übergeordneten Datensatzes (Workfront-Objekt) aus, dessen verknüpfte Datensätze Sie lesen möchten.</p> <p>Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] für jede [!DNL Workfront] Modul</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Übergeordnete Datensatz-ID von [!UICONTROL]</td> 
   <td> <p>Geben Sie die Kennung des übergeordneten Datensatzes ein oder ordnen Sie ihn zu, dessen verknüpfte Datensätze Sie lesen möchten.</p> <p>Um die ID abzurufen, öffnen Sie die [!DNL Workfront] -Objekt in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sammlungen]</td> 
   <td>Wählen Sie den Typ des untergeordneten Datensatzes aus oder ordnen Sie ihn zu, den das Modul lesen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Suche]**

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Workfront] die mit der angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Workfront] App auf [!DNL Workfront Fusion], siehe <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ [!DNL Workfront] -Datensatz, nach dem das -Modul suchen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ergebnissatz]</td> 
   <td>Wählen Sie eine Option aus, um anzugeben, ob das Modul das erste Ergebnis erhalten soll, das Ihren Suchkriterien entspricht, oder alle Ergebnisse, die dem Ergebnis entsprechen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximal]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suchkriterien]</td> 
   <td> <p>Geben Sie das Feld, nach dem Sie suchen möchten, den Operator, den Sie in Ihrer Abfrage verwenden möchten, und den Wert ein, nach dem Sie im Feld suchen.</p> <p>Hinweis: Verwenden Sie <code>username </code>in Ihren Suchkriterien. Einschließlich <code>username </code>in einer API-Abfrage zu [!DNL Workfront] meldet den Benutzer in Workfront an und die Suche wird nicht erfolgreich durchgeführt.</p> <p>Hinweis: <code>In</code> und <code>NotIn</code>mit Arrays verwendet werden. Die Eingaben sollten im Array-Format erfolgen.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Felder aus, die Sie in die Ausgabe dieses Moduls aufnehmen möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Referenzen]</td> 
   <td>Wählen Sie beliebige Referenzfelder aus, die Sie in die Suche einbeziehen möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sammlungen]</td> 
   <td>Wählen Sie alle Sammlungen aus, die Sie der Suche hinzufügen möchten.</td> 
  </tr> 
 </tbody> 
</table>

Eine Liste der [!DNL Workfront] Objekttypen, für die dieses Modul verwendet werden kann, in [[!DNL Workfront] für jede [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module).

+++

## [!DNL Workfront] für jede [!DNL Workfront] Modul

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Für jede [!DNL Workfront] Trigger-Modul**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Überwachungsdatensatz]</th> 
   <th>[!UICONTROL Überwachungsfeld]</th> 
   <th>[!UICONTROL Überwachungsereignisse]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Genehmigungsprozess</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Zuweisung</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ausgangsbasis</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> Rechnungsnachweis </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Abrechnungssatz</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Firma</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dashboard</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokument</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokumentenordner</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dokumentanforderung</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Dokumentversion</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ausgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ausgabentyp</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Stunde</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Stundentyp</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Wiederholung</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgabengebiet</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Journaleintrag</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Meilenstein</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Meilensteinpfad</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Notiz</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Notiz-Tag</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programm</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projektbenutzer</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Korrekturabzug-Genehmigung</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Reservierte Zeit* </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bericht</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Risiko</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risikotyp</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Schritt-Genehmiger</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Vorlage</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Vorlagenaufgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Arbeitszeittabelle</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Aktualisieren</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Für jede [!DNL Workfront] Aktionsmodul**

>[!NOTE]
>
>Die [!UICONTROL Dokument herunterladen] -Modul nicht in dieser Tabelle enthalten ist, da [!DNL Workfront] -Objekttypen sind nicht Teil ihrer Konfiguration.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Datensatz erstellen]</th> 
   <th>[!UICONTROL Datensatz aktualisieren]</th> 
   <th>[!UICONTROL Datensatz löschen]</th> 
   <th>[!UICONTROL Dokument hochladen]</th> 
   <th>[!UICONTROL Datensatz lesen]</th> 
   <th>[!UICONTROL Benutzerdefinierter API-Aufruf]</th> 
   <th>[!UICONTROL Misc Action]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Genehmigungsprozess</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Zuweisung</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Rechnungsnachweis</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Abrechnungssatz</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Firma</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokument</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokumentenordner</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokumentversion</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ausgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ausgabentyp</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Stunde</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Stundentyp</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Wiederholung</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgabengebiet</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Journaleintrag</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Meilenstein</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Meilensteinpfad</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Notiz</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Notiz-Tag</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programm</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projektbenutzer</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Reservierte Zeit* </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risiko</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risikotyp</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Schritt-Genehmiger</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Vorlage</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Vorlagenaufgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Arbeitszeittabelle</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Aktualisieren</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**Für jede [!DNL Workfront] Suchmodul**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>[!UICONTROL Suche]</th> 
   <th>[!UICONTROL Verwandte Aufzeichnungen lesen]</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Genehmigungsprozess</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Zuweisung</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Rechnungsnachweis</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Abrechnungssatz</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Firma</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokument</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokumentenordner</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Dokumentversion</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ausgabe</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ausgabentyp</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Gruppe</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Stunde</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Stundentyp</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Problem</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Wiederholung</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgabengebiet</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Journaleintrag</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Meilenstein</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Meilensteinpfad</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Notiz</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Notiz-Tag</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Portfolio</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Programm</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projekt</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Projektbenutzer</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Reservierte Zeit* </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risiko</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Risikotyp</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Schritt-Genehmiger</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aufgabe</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Team</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Vorlage</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Vorlagenaufgabe</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Arbeitszeittabelle</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Benutzerin oder Benutzer</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Benutzerdelegierung</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

Es wird empfohlen, die Markierung zu verdoppeln, um sicherzustellen, dass dies so funktioniert, wie Sie es erwarten.

+++

## Ereignisabonnementfilter in [!DNL Workfront] > [!UICONTROL Ereignisse beobachten] Module

>[!NOTE]
>
>Wir empfehlen dringend die Verwendung von Ereignisabonnementfiltern in Ihren [!UICONTROL Ereignisse beobachten] Module.

Die [!DNL Workfront] [!UICONTROL Ereignisse beobachten] Trigger von Modulen, die auf einem Webhook basieren, der ein Ereignisabonnement im [!DNL Workfront] API. Das Ereignisabonnement ist ein Satz von Daten, die bestimmen, welche Ereignisse an den Webhook gesendet werden. Wenn Sie beispielsweise eine [!UICONTROL Ereignisse beobachten] -Modul, das auf Probleme überwacht, sendet das Ereignisabonnement nur Ereignisse, die sich auf Probleme beziehen.

Mithilfe von Ereignisabonnementfiltern können Fusion-Benutzer Ereignisabonnements erstellen, die für ihre Anwendungsfälle besser geeignet sind. Sie können beispielsweise ein Ereignisabonnement im [!DNL Workfront] API, um nur Probleme zu senden, die sich in einem bestimmten Projekt befinden, und sicherzustellen, dass die [!UICONTROL Ereignisse beobachten] -Modul wird nur für Probleme in diesem Projekt Trigger. Die Möglichkeit, schmalere Trigger zu erstellen, verbessert das Szenario-Design, indem die Anzahl irrelevanter Trigger verringert wird.

Dies unterscheidet sich von der Einrichtung eines Filters im [!DNL Workfront Fusion] Szenario. Ohne einen Abonnementfilter für Ereignisse erhält Ihr Webhook alle Ereignisse im Zusammenhang mit dem ausgewählten Objekttyp. Die meisten dieser Ereignisse wären für das Szenario irrelevant und müssen herausgefiltert werden, bevor das Szenario fortgesetzt werden kann.

Die folgenden Operatoren sind im Filter Workfront > Ereignisse überwachen verfügbar:

* Ist gleich
* Ungleich
* Größer als
* Kleiner als
* Größer oder gleich
* Kleiner oder gleich
* Enthält
* Vorhanden
   * Dieser Operator benötigt keinen Wert und das Wertefeld fehlt.
* Nicht vorhanden
   * Dieser Operator benötigt keinen Wert und das Wertefeld fehlt.
* Geändert
   * Dieser Operator benötigt keinen Wert und das Wertefeld fehlt.
   * Dieser Operator ignoriert das Feld Status .
   * Bei Verwendung von `Changed`auswählen **Nur aktualisierte Ereignisse** im **Ursprung des Datensatzes** -Feld.

>[!IMPORTANT]
>
>Filter in vorhandenen [!DNL Workfront] Webhooks. So richten Sie verschiedene Filter für ein [!DNL Workfront] -Ereignis-Abonnements, entfernen Sie den aktuellen Webhook und erstellen Sie einen neuen.

>[!INFO]
>
>**Beispiel:** Betrachten Sie ein Szenario, das neue Probleme verarbeitet, die einem bestimmten Benutzer, Ana, zugewiesen sind.
>
>### Filtern von Ereignissen mithilfe eines Ereignisabonnementfilters (empfohlen)
>
>Mithilfe des Ereignisfilters können Sie den Webhook so einrichten, dass das Szenario Trigger wird, wenn ein Problem bei der Erstellung des Problems Ana zugewiesen wird. Ana hat die Benutzer-ID b378489d8f7cd3cee0539260720a84b7.
>
>![](assets/event-filter-watch-events-350x277.png)
>
>Wenn an einem Tag 100 Probleme erstellt werden, aber nur zwei davon Ana zugewiesen sind, wird das Szenario zweimal ausgeführt.
>
>### Filtern von Ereignissen innerhalb des Szenarios (nicht empfohlen)
>
>Um Ereignisse so zu filtern, dass nur die der Analytics zugewiesenen Probleme verarbeitet werden, können Sie einen Filter nach der [!UICONTROL Ereignisse beobachten] -Modul.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Wenn 100 Probleme an einem Tag erstellt werden, aber nur zwei davon Ana zugewiesen sind, wird das Szenario 100-mal ausgeführt. 98 der Ausführungen würden am Filter anhalten, aber das Trigger-Modul verbraucht weiterhin Daten und führt Vorgänge in allen Ausführungen durch.

Weitere Informationen zu Ereignisanmeldungen finden Sie unter [Häufig gestellte Fragen - Ereignisabos](../../wf-api/general/event-subs-faq.md).

Weitere Informationen zu Webhooks finden Sie unter [Sofortige Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Weitere Informationen zu Filtern in Szenarien finden Sie unter [Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

