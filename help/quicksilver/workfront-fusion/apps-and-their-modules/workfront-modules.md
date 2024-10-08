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
source-git-commit: 3fde10cfa0428971b289a9de57cf49e24a15a0e8
workflow-type: tm+mt
source-wordcount: '6558'
ht-degree: 2%

---

# [!DNL Adobe Workfront] Module

Sie können den Connector [!DNL Adobe Workfront Fusion] [!DNL Adobe Workfront] verwenden, um Ihre Prozesse innerhalb von [!DNL Workfront] zu automatisieren. Wenn Sie über eine [!UICONTROL [!DNL Workfront Fusion] -Lizenz für Arbeitsautomatisierung und Integration] verfügen, können Sie damit auch eine Verbindung zu Drittanbieteranwendungen und -diensten herstellen.

Der Connector [!DNL Workfront] zählt nicht mit der Anzahl der aktiven Apps, die für Ihr Unternehmen verfügbar sind. Alle Szenarien, auch wenn sie nur die [!DNL Workfront] -App verwenden, werden mit der Gesamtanzahl der Szenarien Ihrer Organisation angerechnet.

Weitere Informationen zu den verfügbaren Anwendungen und Szenarien Ihrer Organisation finden Sie unter [Organisationen](../../workfront-fusion/organizations/organizations-and-teams.md#organiza2) in [[!DNL Adobe Workfront Fusion] Organisationen und Teams](../../workfront-fusion/organizations/organizations-and-teams.md).

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>


Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront] mit [!DNL Workfront Fusion] verbinden

Der [!DNL Workfront]-Connector verwendet OAuth 2.0, um eine Verbindung zu [!DNL Workfront] herzustellen.

Sie können eine Verbindung zu Ihrem [!DNL Workfront]-Konto direkt aus einem [!DNL Workfront Fusion]-Modul erstellen.

1. Klicken Sie in einem beliebigen Adobe Workfront-Modul neben dem Feld Verbindung auf **Hinzufügen** .
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
        <td>Geben Sie Ihre [!DNL Workfront] Client-ID ein. Dies finden Sie im Bereich "OAuth2-Anwendungen"des Einrichtungsbereichs in Workfront. Öffnen Sie die spezifische Anwendung, mit der Sie eine Verbindung herstellen, um die Client-ID anzuzeigen.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihre [!DNL Workfront] Client-ID ein. Dies finden Sie im Bereich "OAuth2-Anwendungen"des Einrichtungsbereichs in Workfront. Öffnen Sie die spezifische Anwendung, mit der Sie eine Verbindung herstellen, um die Client-ID anzuzeigen.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentifizierungs-URL]</td>
        <td>Dies kann der Standardwert bleiben, oder Sie können die URL Ihrer Workfront-Instanz eingeben, gefolgt von <code>/integrations/oauth2</code>. <p>Beispiel: <code>https://mydomain.my.workfront.com/integrations/oauth2</code></p></td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Host-Präfix]</td>
        <td>In den meisten Fällen sollte dieser Wert <code>origin</code> sein.
      </tr>
    </tbody>
    </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.




<!--1. Enter the name of your instance into the URL. Example: `https://<your instance>.my.workfront.com`.
1. Click **[!UICONTROL Next]**.
1. Click **[!UICONTROL SAML log in]** to create the connection and go back to the module.

   Or

   Enter your Username and Password, then click **[!UICONTROL Log in]** to create the connection and go back to the module.-->

>[!NOTE]
>
>* Wenn keine Schaltfläche zum Anmelden bei SAML angezeigt wird, hat Ihr Unternehmen Single Sign-On (SSO) nicht aktiviert. Sie können sich mit Ihrem Benutzernamen und Passwort anmelden.
>   
>   Weitere Informationen zur einmaligen Anmeldung finden Sie unter [Überblick über die einmalige Anmeldung in [!DNL Adobe Workfront]](../../administration-and-setup/add-users/single-sign-on/sso-in-workfront.md)
>   
>* OAuth 2.0-Verbindungen zur [!DNL Workfront]-API benötigen keine API-Schlüssel mehr.

## [!DNL Workfront] Module und ihre Felder

Wenn Sie [!DNL Workfront] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Workfront] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).


![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>* Wenn in einem Workfront-Modul nicht die aktuellsten Felder angezeigt werden, liegt dies möglicherweise an Caching-Problemen. Warten Sie eine Stunde und versuchen Sie es erneut.
>* HTTP-429-Statuscodes von Adobe Workfront sollten keine Deaktivierungen verursachen, sondern eine kurze Ausführungspause im Szenario Trigger werden.

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

<!--
* [Watch Events](#watch-events) 
* [Watch Record](#watch-record) 
* [Watch Field](#watch-field)
-->

+++ **[!UICONTROL Ereignisse ansehen]**

Dieses Trigger-Modul führt ein Szenario in Echtzeit aus, wenn Objekte eines bestimmten Typs in Workfront hinzugefügt, aktualisiert oder gelöscht werden

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

1. Klicken Sie rechts neben dem Feld **Webhook** auf **[!UICONTROL Add]**.

1. Konfigurieren Sie den Webhook im angezeigten Feld **[!UICONTROL Hook hinzufügen]** .

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
      <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Type]</td> 
      <td>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, den das Modul überwachen soll.</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL State]</td> 
      <td>Wählen Sie aus, ob Sie den alten oder neuen Status überwachen möchten.<ul><li><p><b>[!UICONTROL Neuer Status]</b></p><p>Trigger eines Szenarios, in dem der Datensatz <b>in</b> einen bestimmten Wert ändert.</p><p>Wenn beispielsweise der Status auf [!UICONTROL Neuer Status] festgelegt ist und der Filter auf [!UICONTROL Status] [!UICONTROL Entspricht] [!UICONTROL In Bearbeitung] gesetzt ist, wird der Webhook auf einen Trigger gesetzt, wenn [!UICONTROL Status] in [!UICONTROL In Bearbeitung] geändert wird, unabhängig davon, welcher Status zuvor war. </p></li><li><p><b>[!UICONTROL Alter Staat]</b></p><p>Trigger eines Szenarios, in dem der Datensatz <b>von </b> einen bestimmten Wert ändert.</p><p>Wenn beispielsweise der Status auf [!UICONTROL Old State] gesetzt ist und der Filter auf [!UICONTROL Status] [!UICONTROL Entspricht] [!UICONTROL In Bearbeitung] festgelegt ist, wird der Webhook auf einen Trigger angewendet, wenn ein [!UICONTROL Status], der derzeit [!UICONTROL In Bearbeitung] ist, zu einem anderen Status wechselt. </p></li></ul></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Ereignisfilter]</p> </td> 
      <td> <p>Sie können Filter festlegen, um nur Datensätze zu überwachen, die den von Ihnen ausgewählten Kriterien entsprechen.</p> <p>Geben Sie für jeden Filter das Feld, das der Filter auswerten soll, den Operator und den Wert ein, die der Filter zulassen soll. Sie können mehrere Filter verwenden, indem Sie UND-Regeln hinzufügen.</p> <p>Hinweis: Sie können keine Filter in vorhandenen [!DNL Workfront]-Webhooks bearbeiten. Um verschiedene Filter für [!DNL Workfront] -Ereignisabonnements einzurichten, entfernen Sie den aktuellen Webhook und erstellen Sie einen neuen.</p> <p>Weitere Informationen zu Ereignisfiltern finden Sie unter <a href="#event-subscription-filters-in-the-workfront-watch-events-modules" class="MCXref xref">Ereignisabonnementfilter in den Modulen [!DNL Workfront] &gt; [!UICONTROL Watch Events]</a> in diesem Artikel.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Von dieser Verbindung vorgenommene Ereignisse ausschließen</td> 
      <td>Aktivieren Sie diese Option, um Ereignisse auszuschließen, die mit demselben Connector erstellt oder aktualisiert wurden, den dieses Trigger-Modul verwendet. Dies kann Situationen verhindern, in denen ein Szenario selbst Trigger hat, sodass es sich in einer Endlosschleife wiederholt.<p><b>HINWEIS</b>Der Datensatztyp "Zuweisung"enthält diese Option nicht.</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Record Origin]</td> 
      <td> <p>Wählen Sie aus, ob das Szenario nur <strong>[!UICONTROL Neue Datensätze]</strong>, <strong>[!UICONTROL Nur aktualisierte Datensätze]</strong>, <strong>[!UICONTROL Neue und aktualisierte Datensätze]</strong> oder <strong>[!DNL Deleted Records Only]</strong> sehen soll.</p> <p>Hinweis: Wenn Sie "<strong>[!UICONTROL Neue und aktualisierte Datensätze]</strong>"auswählen, erstellt die Webhook-Erstellung zwei Ereignis-Abonnements (für dieselbe Webhook-Adresse).</p> </td> 
     </tr> 
    </tbody> 
   </table>

Nachdem der Webhook erstellt wurde, können Sie die Adresse des Endpunkts anzeigen, an den Ereignisse gesendet werden.

Weitere Informationen finden Sie im Abschnitt [Beispiele für Ereignis-Payloads](../../wf-api/general/event-subs-api.md#examples-of-event-payloads) im [!DNL Workfront] Hilfeartikel [Ereignis-Abonnement-API](../../wf-api/general/event-subs-api.md).

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

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
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, den das Modul überwachen soll.</p> <p>Wählen Sie beispielsweise [!UICONTROL Task] aus, wenn Sie das Szenario jedes Mal ausführen möchten, wenn ein Datensatzfeld in einer Aufgabe aktualisiert wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td>Wählen Sie das Feld aus, das das Modul auf Updates überwachen soll. Diese Felder spiegeln die Felder wider, die Ihr [!DNL Workfront]-Administrator für das Tracking eingerichtet hat.</td> 
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

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

+++

+++ **[!UICONTROL Aufzeichnen von Datensätzen ansehen]**

Dieses Trigger-Modul führt ein Szenario aus, wenn Objekte eines bestimmten Typs hinzugefügt, aktualisiert oder beides. Das Modul gibt alle mit dem Datensatz oder den Datensätzen verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen. In der Ausgabe gibt das Modul an, ob jeder Datensatz neu oder aktualisiert ist.

Datensätze, die im angegebenen Zeitraum hinzugefügt und aktualisiert wurden, werden als neue Datensätze zurückgegeben.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Wählen Sie aus, ob das Szenario nur <strong>[!UICONTROL Neue Datensätze]</strong>, <strong>[!UICONTROL Nur aktualisierte Datensätze]</strong> oder <strong>[!UICONTROL Neue und aktualisierte Datensätze]</strong> sehen soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>(Wird angezeigt, nachdem Sie einen <strong>Filter</strong> ausgewählt haben.) Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, den das Modul überwachen soll.</p> <p>Wenn Sie beispielsweise jedes Mal, wenn ein neues Projekt erstellt wird, das Szenario starten möchten, wählen Sie [!UICONTROL Projekt]</p> </td> 
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

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

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

+++ **[!UICONTROL Objekt konvertieren]**

Dieses Aktionsmodul führt eine der folgenden Konvertierungen durch:

* Problem in Projekt konvertieren
* Problem in Aufgabe konvertieren
* Aufgabe in Projekt konvertieren

>[!NOTE]
>
>Ab Juli 2024 können beim Konvertieren eines Objekts benutzerdefinierte Formulare einbezogen werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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
   <td>[!UICONTROL &lt;Objekt&gt; ID]</td> 
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
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Native Felder kopieren]</td> 
   <td> <p>Aktivieren Sie diese Option, um alle nativen Felder vom ursprünglichen Objekt in das neue Objekt zu kopieren.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Benutzerdefinierte Formulare kopieren]</td> 
   <td> <p>Aktivieren Sie diese Option, um alle nativen Felder vom ursprünglichen Objekt in das neue Objekt zu kopieren.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Erstellen eines Datensatzes (Anhängen benutzerdefinierter Formulare)]**

Dieses Aktionsmodul erstellt ein Objekt wie ein Projekt, eine Aufgabe oder ein Problem in [!DNL Workfront] und ermöglicht das Hinzufügen eines benutzerdefinierten Formulars zum neuen Objekt. Mit dem -Modul können Sie auswählen, welche der Objektfelder im -Modul verfügbar sind.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie können dieses Modul beispielsweise verwenden, um eine Aufgabe in [!DNL Workfront] zu erstellen, wenn ein Client eine neue Zeile in einer Liste mit Aufgaben vom Typ [!DNL Google Sheets] hinzufügt, die ausgeführt werden müssen.

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
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, den das Modul erstellen soll.</p> <p>Wenn Sie beispielsweise ein Projekt erstellen möchten, wählen Sie in der Dropdown-Liste die Option [!UICONTROL Projekt] aus und stellen Sie sicher, dass Sie Zugriff auf Daten (aus früheren Modulen im Szenario) haben, die das Projekt ausfüllen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td> <p>Wählen Sie die Felder aus, die für die Dateneingabe verfügbar sein sollen. Auf diese Weise können Sie diese Felder verwenden, ohne durch die Felder zu scrollen, die Sie nicht benötigen.</p> <p>Verwenden Sie für Felder in benutzerdefinierten Formularen das Feld "<b>[!UICONTROL Benutzerdefiniertes Formular anhängen]</b>".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Benutzerdefiniertes Formular anhängen]</td> 
   <td>Wählen Sie benutzerdefinierte Formulare aus, die Sie dem neuen Objekt hinzufügen möchten, und geben Sie dann Werte für diese Felder ein.</td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

>[!NOTE]
>
>* Bei der Eingabe der ID eines Objekts können Sie mit der Eingabe des Objektnamens beginnen und dieses dann aus der Liste auswählen. Das Modul gibt dann die entsprechende ID in das Feld ein.
>* Bei der Eingabe des Texts für ein benutzerdefiniertes Feld oder ein [!UICONTROL Hinweis] -Objekt (Kommentar oder Antwort) können Sie HTML-Tags im Feld [!UICONTROL Hinweistext] verwenden, um Rich-Text zu erstellen, z. B. fett oder kursiv gedruckten Text.
>
>  Weitere Informationen zu Rich-Text-Updates finden Sie unter [Hinzufügen einer Aktualisierung zu einem Arbeitselement](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Arbeit aktualisieren](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Datensatz erstellen]**

Dieses Aktionsmodul erstellt ein Objekt wie ein Projekt, eine Aufgabe oder ein Problem in Workfront. Mit dem -Modul können Sie auswählen, welche der Objektfelder im -Modul verfügbar sind.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie können dieses Modul beispielsweise verwenden, um eine Aufgabe in [!DNL Workfront] zu erstellen, wenn ein Client eine neue Zeile in einer Google Tabellen-Liste mit Aufgaben hinzufügt, die ausgeführt werden müssen.

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
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, den das Modul erstellen soll.</p> <p>Wenn Sie beispielsweise ein Projekt erstellen möchten, wählen Sie in der Dropdown-Liste die Option [!UICONTROL Projekt] aus und stellen Sie sicher, dass Sie Zugriff auf Daten (aus früheren Modulen im Szenario) haben, die das Projekt ausfüllen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td>Wählen Sie die Felder aus, die für die Dateneingabe verfügbar sein sollen. Auf diese Weise können Sie diese Felder verwenden, ohne durch die Felder zu scrollen, die Sie nicht benötigen.</td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

>[!NOTE]
>
>* Bei der Eingabe der ID eines Objekts können Sie mit der Eingabe des Objektnamens beginnen und dieses dann aus der Liste auswählen. Das Modul gibt dann die entsprechende ID in das Feld ein.
>* Bei der Eingabe des Texts für ein benutzerdefiniertes Feld oder ein [!UICONTROL Hinweis] -Objekt (Kommentar oder Antwort) können Sie HTML-Tags im Feld [!UICONTROL Hinweistext] verwenden, um Rich-Text zu erstellen, z. B. fett oder kursiv gedruckten Text.
>
>  Weitere Informationen zu Rich-Text-Updates finden Sie unter [Hinzufügen einer Aktualisierung zu einem Arbeitselement](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Arbeit aktualisieren](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Benutzerspezifischer API-Aufruf]**

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Workfront] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Workfront] -Modulen nicht ausgeführt werden kann.

Das Modul gibt die folgenden Informationen zurück:

* **[!UICONTROL Status-Code]** (Zahl): Zeigt an, ob Ihre HTTP-Anforderung erfolgreich oder fehlgeschlagen ist. Dies sind Standardcodes, die Sie im Internet nachschlagen können.
* **[!UICONTROL Kopfzeilen]** (Objekt): Ein detaillierterer Kontext für den Antwort-/Statuscode, der sich nicht auf den Ausgabetext bezieht. Nicht alle Header, die in einem Antwortheader angezeigt werden, sind Antwortheader, sodass einige möglicherweise nicht nützlich für Sie sind.

  Die Antwortheader hängen von der HTTP-Anforderung ab, die Sie beim Konfigurieren des Moduls ausgewählt haben.

* **[!UICONTROL Hauptteil]** (Objekt): Je nach der HTTP-Anforderung, die Sie beim Konfigurieren des Moduls ausgewählt haben, erhalten Sie möglicherweise einige Daten zurück. Diese Daten, z. B. die Daten aus einer GET-Anfrage, sind in diesem Objekt enthalten.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code> https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</code> ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API-Version]</td> 
   <td>Wählen Sie die Version der [!DNL Workfront]-API aus, die das Modul verwenden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu. Dadurch wird der Inhaltstyp der Anforderung bestimmt.</p> <p>Beispiel:<code> {"Content-type":"application/json"}</code></p> <p>Hinweis: Wenn Fehler auftreten und es schwierig ist, ihren Ursprung zu bestimmen, sollten Sie die Kopfzeilen auf Grundlage der [!DNL Workfront] -Dokumentation ändern. Wenn Ihr benutzerspezifischer API-Aufruf einen 422-HTTP-Anforderungsfehler zurückgibt, versuchen Sie, einen <code>"Content-Type":"text/plain"</code> -Header zu verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> <p>Tipp: Es wird empfohlen, Informationen nicht als Abfrageparameter, sondern über den JSON-Hauptteil zu senden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

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
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Löschvorgang erzwingen]</td> 
   <td>Aktivieren Sie diese Option, um sicherzustellen, dass der Datensatz gelöscht wird, auch wenn die Benutzeroberfläche von [!DNL Workfront] eine Bestätigung des Löschvorgangs anfordert.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>ID</td> 
   <td> <p>Geben Sie die eindeutige [!DNL Workfront]-ID des Datensatzes ein, den das Modul löschen soll.</p> <p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Workfront] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, den das Modul löschen soll.</td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

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
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dokument-ID]</td> 
   <td> <p>Ordnen Sie die eindeutige [!DNL Workfront]-ID des Dokuments zu, das das Modul herunterladen soll, oder geben Sie sie manuell ein.</p> <p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Workfront] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

+++

+++ **[!UICONTROL Falsche Aktion]**

Mit diesem Aktionsmodul können Sie Aktionen für die API ausführen.

>[!NOTE]
>
>Ab Juli 2024 enthält die Aktion `convertToProject` das Feld `copyCategories`. Wenn der Wert auf &quot;`TRUE`&quot; gesetzt wird, werden alle benutzerdefinierten Formulare in das Projekt aufgenommen, in das das Problem konvertiert wird.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, mit dem das Modul interagieren soll.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Aktion]</td> 
   <td> <p>Wählen Sie die Aktion aus, die das Modul ausführen soll.</p> <p>Je nach ausgewähltem [!UICONTROL Record Type] und [!UICONTROL Action] müssen Sie möglicherweise zusätzliche Felder ausfüllen. Einige Kombinationen dieser beiden Einstellungen erfordern möglicherweise nur eine Datensatz-ID, während andere (z. B. Projekt für den <strong>[!UICONTROL Record Type]</strong> und [!UICONTROL Attach Template] für die <strong>[!UICONTROL Action]</strong>) zusätzliche Informationen benötigen (z. B. eine Objekt-ID und eine Vorlagen-ID).</p> <p>Weitere Informationen zu einzelnen Feldern finden Sie in der <a href="http://developer.workfront.com/">Workfront-Entwicklerdokumentation</a>. <p><strong>Hinweis</strong>: Die Entwicklerdokumentations-Site enthält Informationen nur über API-Version 14, enthält aber trotzdem wertvolle Informationen für API-Aufrufe. </p> 
    <ol> 
     <li value="1"> <p>Wählen Sie im linken Navigationsbereich auf der Seite mit der Entwicklerdokumentation die Art des Datensatzes aus. [!DNL Workfront] Die folgenden Typen haben eigene Seiten:</p> 
      <ul> 
       <li> <p>[!UICONTROL Projekte]</p> </li> 
       <li> <p>[!UICONTROL Aufgaben]</p> </li> 
       <li> <p>[!UICONTROL Probleme]</p> </li> 
       <li> <p>[!UICONTROL Benutzer]</p> </li> 
       <li> <p>[!UICONTROL Dokumente]</p> </li> 
      </ul> <p>Wählen Sie für alle anderen Datensatztypen <b>[!UICONTROL Sonstige Objekte und Endpunkte]</b> aus und suchen Sie den Datensatztyp auf den alphabetisch sortierten Seiten.</p> </li> 
     <li value="2"> <p>Suchen Sie auf der Seite des entsprechenden Datensatztyps (Strg-F oder Befehl-F) nach der Aktion.</p> </li> 
     <li value="3"> <p>Zeigen Sie Beschreibungen für verfügbare Felder unter der ausgewählten Aktion an.</p> </li> 
    </ol> <p>Hinweis:  <p>Beim Erstellen eines Testversands mithilfe des Moduls [!DNL Workfront] [!UICONTROL Misc Action] empfiehlt es sich, einen Testversand ohne erweiterte Optionen zu erstellen und den Testversand dann mithilfe der SOAP API [!DNL Workfront Proof] zu aktualisieren.</p> <p>Weitere Informationen zum Erstellen eines Testversands mit der [!DNL Workfront]-API (die dieses Modul verwendet) finden Sie unter <a href="../../wf-api/tips-tricks-and-troubleshooting/api-create-proof-options-json.md" class="MCXref xref">Erweiterte Testoptionen beim Erstellen eines Testversands über die [!DNL Adobe Workfront]-API hinzufügen</a> .</p> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Workfront]-ID des Datensatzes ein oder ordnen Sie sie zu, mit dem das Modul interagieren soll.<p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Workfront] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p></td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

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

<td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>

<td>Wählen Sie den Objekttyp [!DNL Workfront] aus, den das Modul lesen soll.</td> 
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
   <td> <p>Geben Sie die eindeutige [!DNL Workfront]-ID des Datensatzes ein, den das Modul lesen soll.</p> <p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Workfront] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

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
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Geben Sie die eindeutige [!DNL Workfront]-ID des Datensatzes ein, den das Modul aktualisieren soll.</p> <p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Workfront] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
  </tr> 
  <tr> 
   <td>[!DNL Record Type]</td> 
   <td> <p>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, den das Modul aktualisieren soll.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!DNL Select fields to map]</td> 
   <td>Wählen Sie die Felder aus, die für die Dateneingabe verfügbar sein sollen. Auf diese Weise können Sie diese Felder verwenden, ohne durch die Felder zu scrollen, die Sie nicht benötigen.</td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

>[!NOTE]
>
>* Bei der Eingabe der ID eines Objekts können Sie mit der Eingabe des Objektnamens beginnen und dieses dann aus der Liste auswählen. Das Modul gibt dann die entsprechende ID in das Feld ein.
>* Bei der Eingabe des Texts für ein benutzerdefiniertes Feld oder ein [!UICONTROL Hinweis] -Objekt (Kommentar oder Antwort) können Sie HTML-Tags im Feld [!UICONTROL Hinweistext] verwenden, um Rich-Text zu erstellen, z. B. fett oder kursiv gedruckten Text.
>
>  Weitere Informationen zu Rich-Text-Updates finden Sie unter [Hinzufügen einer Aktualisierung zu einem Arbeitselement](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) in [Arbeit aktualisieren](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
>

+++

+++ **[!UICONTROL Dokument hochladen]**

Dieses Aktionsmodul lädt ein Dokument in ein [!DNL Workfront] -Objekt hoch, z. B. ein Projekt, eine Aufgabe oder ein Problem. Dieses Modul lädt das Dokument in Teilen hoch, wodurch der Upload-Prozess für Workfront reibungsloser abläuft.

Sie geben den Speicherort für das Dokument, die Datei, die Sie hochladen möchten, und einen optionalen neuen Namen für die Datei an.

Das Modul gibt die ID des Dokuments sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Workfront]-ID des Datensatzes ein, in den Sie das Dokument hochladen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verwandter Datensatztyp]</td> 
   <td>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, in den das Modul das Dokument hochladen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner-ID]</td> 
   <td>Je nach Typ des zugehörigen Datensatzes müssen Sie möglicherweise eine Ordner-ID eingeben oder zuordnen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

+++

+++ **[!UICONTROL Dokument hochladen (veraltet)]**

Dieses Aktionsmodul lädt ein Dokument in ein [!DNL Workfront] -Objekt hoch, z. B. ein Projekt, eine Aufgabe oder ein Problem. Das gesamte Dokument wird gleichzeitig hochgeladen.

Sie geben den Speicherort für das Dokument, die Datei, die Sie hochladen möchten, und einen optionalen neuen Namen für die Datei an.

Das Modul gibt die ID des Dokuments sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Related Record ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Workfront]-ID des Datensatzes ein, in den Sie das Dokument hochladen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verwandter Datensatztyp]</td> 
   <td>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, in den das Modul das Dokument hochladen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner-ID]</td> 
   <td>Je nach Typ des zugehörigen Datensatzes müssen Sie möglicherweise eine Ordner-ID eingeben oder zuordnen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

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
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des übergeordneten Datensatzes (Workfront-Objekt) aus, dessen verknüpfte Datensätze Sie lesen möchten.</p> <p>Eine Liste der [!DNL Workfront] -Objekttypen, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul</a> verfügbaren <a href="#object-types-available-for-each-workfront-search-module" class="MCXref xref">[!DNL Workfront] Objekttypen verwenden können, finden Sie in diesem Artikel.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Übergeordnete Datensatz-ID von [!UICONTROL]</td> 
   <td> <p>Geben Sie die Kennung des übergeordneten Datensatzes ein oder ordnen Sie ihn zu, dessen verknüpfte Datensätze Sie lesen möchten.</p> <p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Workfront] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach "ID=". Beispiel: https://my.workfront.com/project/view?ID=<i>5e43010c03286a2a555e1d0a75d6a86e</i></p> </td> 
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

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Workfront], die mit der von Ihnen angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, nach dem das Modul suchen soll.</p> </td> 
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
   <td>[!UICONTROL Suchkriterienfelder]</td> 
   <td> <p>Wählen Sie die Felder aus, die Sie für Ihre Suchkriterien verwenden möchten. Diese Felder stehen dann im Dropdown-Menü Suchkriterien zur Verfügung.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suchkriterien]</td> 
   <td> <p>Geben Sie das Feld, nach dem Sie suchen möchten, den Operator, den Sie in Ihrer Abfrage verwenden möchten, und den Wert ein, nach dem Sie im Feld suchen.</p> <p>Hinweis: Verwenden Sie nicht <code>username </code>in Ihren Suchkriterien. Wenn Sie <code>username </code> in eine API-Abfrage zu [!DNL Workfront] einschließen, wird der Benutzer in Workfront protokolliert und die Suche wird nicht erfolgreich durchgeführt.</p> <p>Hinweis: <code>In</code> und <code>NotIn</code>funktionieren mit Arrays. Die Eingaben sollten im Array-Format erfolgen.</p></td> 
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
+++

+++ **[!UICONTROL Suche (veraltet)]**

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Workfront], die mit der von Ihnen angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ von [!DNL Workfront] Datensatz aus, nach dem das Modul suchen soll.</p> </td> 
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
   <td> <p>Geben Sie das Feld, nach dem Sie suchen möchten, den Operator, den Sie in Ihrer Abfrage verwenden möchten, und den Wert ein, nach dem Sie im Feld suchen.</p> <p>Hinweis: Verwenden Sie nicht <code>username </code>in Ihren Suchkriterien. Wenn Sie <code>username </code> in eine API-Abfrage zu [!DNL Workfront] einschließen, wird der Benutzer in Workfront protokolliert und die Suche wird nicht erfolgreich durchgeführt.</p> <p>Hinweis: <code>In</code> und <code>NotIn</code>funktionieren mit Arrays. Die Eingaben sollten im Array-Format erfolgen.</p></td> 
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

Sehen Sie sich eine Liste der [!DNL Workfront] -Objekttypen an, für die Sie dieses Modul in den für jedes [!DNL Workfront] Modul](#workfront-object-types-available-for-each-workfront-module) verfügbaren [[!DNL Workfront] Objekttypen verwenden können.

+++

## [!DNL Workfront] Objekttypen, die für jedes [!DNL Workfront]-Modul verfügbar sind

<!-- [Object types available for each Workfront trigger module](#object-types-available-for-each-workfront-trigger-module) 
* [Object types available for each Workfront action module](#object-types-available-for-each-workfront-action-module) 
* [Object types available for each Workfront search module](#object-types-available-for-each-workfront-search-module)-->

+++**Objekttypen, die für jedes [!DNL Workfront] Trigger-Modul verfügbar sind**

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
   <td> Abrechnungseintrag </td> 
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

+++**Objekttypen, die für jedes [!DNL Workfront] Aktionsmodul verfügbar sind**

>[!NOTE]
>
>Das Modul [!UICONTROL Dokument herunterladen] ist nicht in dieser Tabelle enthalten, da [!DNL Workfront] -Objekttypen nicht Teil der Konfiguration sind.

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
   <td>Ausgangsbasis</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
   <tr> 
   <td>Abrechnungseintrag</td> 
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
   <td> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Wechselkurs</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
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
   <td>Externes Dokument</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
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
   <td> </td> 
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

+++**Objekttypen, die für jedes [!DNL Workfront] Suchmodul verfügbar sind**

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
   <td>Abrechnungseintrag</td> 
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

## Ereignisabonnementfilter in den Modulen [!DNL Workfront] > [!UICONTROL Ereignisse ansehen]

>[!NOTE]
>
>Wir empfehlen dringend die Verwendung von Ereignisabonnementfiltern in Ihren [!UICONTROL Überwachungsereignissen] -Modulen.

Das Modul [!DNL Workfront] [!UICONTROL Ereignisse beobachten] ermöglicht Trigger-Szenarien, die auf einem Webhook basieren, der ein Ereignisabonnement in der [!DNL Workfront] -API erstellt. Das Ereignisabonnement ist ein Satz von Daten, die bestimmen, welche Ereignisse an den Webhook gesendet werden. Wenn Sie beispielsweise ein Modul [!UICONTROL Ereignisse überwachen] einrichten, das auf Probleme überwacht, sendet das Ereignisabonnement nur Ereignisse, die sich auf Probleme beziehen.

Mithilfe von Ereignisabonnementfiltern können Fusion-Benutzer Ereignisabonnements erstellen, die für ihre Anwendungsfälle besser geeignet sind. Sie können beispielsweise ein Ereignisabonnement in der API [!DNL Workfront] einrichten, um nur Probleme zu senden, die sich in einem bestimmten Projekt befinden, an den Webhook zu senden, sodass das Modul [!UICONTROL Überwachungsereignisse] nur für Probleme in diesem Projekt Trigger wird. Die Möglichkeit, schmalere Trigger zu erstellen, verbessert das Szenario-Design, indem die Anzahl irrelevanter Trigger verringert wird.

Dies unterscheidet sich vom Einrichten eines Filters im [!DNL Workfront Fusion] -Szenario. Ohne einen Abonnementfilter für Ereignisse erhält Ihr Webhook alle Ereignisse im Zusammenhang mit dem ausgewählten Objekttyp. Die meisten dieser Ereignisse wären für das Szenario irrelevant und müssen herausgefiltert werden, bevor das Szenario fortgesetzt werden kann.

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
   * Wählen Sie bei Verwendung von &quot;`Changed`&quot;im Feld **Record Origin** die Option **Nur aktualisierte Ereignisse** aus.

>[!IMPORTANT]
>
>Filter in vorhandenen [!DNL Workfront]-Webhooks können nicht bearbeitet werden. Um verschiedene Filter für [!DNL Workfront] -Ereignisabonnements einzurichten, entfernen Sie den aktuellen Webhook und erstellen Sie einen neuen.

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
>Um Ereignisse so zu filtern, dass nur angesehene Probleme verarbeitet werden, können Sie einen Filter nach dem Modul [!UICONTROL Ereignisse überwachen] erstellen.
>
>![](assets/watch-events-non-event-filter-350x206.png)
>
>Wenn 100 Probleme an einem Tag erstellt werden, aber nur zwei davon Ana zugewiesen sind, wird das Szenario 100-mal ausgeführt. 98 der Ausführungen würden am Filter anhalten, aber das Trigger-Modul verbraucht weiterhin Daten und führt Vorgänge in allen Ausführungen durch.

Weitere Informationen zu Ereignisabonnements finden Sie unter [FAQs - Ereignisabonnements](../../wf-api/general/event-subs-faq.md).

Weitere Informationen zu Webhooks finden Sie unter [Instant Trigger (Webhooks) in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)

Weitere Informationen zu Filtern in Szenarien finden Sie unter [Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md).

