---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Cut-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Cvent verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: c95b9764-29a5-4d8c-8e6d-68a3969129e0
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1059'
ht-degree: 1%

---

# [!DNL Cvent] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Cvent] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Cvent] -Module zu verwenden, müssen Sie über ein [!DNL Cvent] -Konto verfügen.

## API-Informationen für das Ausschließen

Der Cvent-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> V200611.ASMX </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.7.14</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Cvent] mit [!DNL Adobe Workfront Fusion] verbinden {#connect-cvent-to-adobe-workfront-fusion}

>[!NOTE]
>
>Die [!DNL Cvent] -Module funktionieren über eine [!UICONTROL SOAP] -API. Um eine Verbindung zu [!DNL Cvent] zu erstellen, müssen Sie Folgendes sicherstellen:
>
>* Sie haben [!UICONTROL SOAP] Zugriff auf die [!DNL Cvent] -API.
>* Die [!DNL Workfront Fusion] IP-Adressen wurden der Zulassungsliste Ihres Unternehmens hinzugefügt.
>
>  Eine Liste der [!DNL Workfront Fusion] IP-Adressen finden Sie unter [IP-Adressen für den Zugriff auf [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md) .


Sie können eine Verbindung zu Ihrem [!DNL Cvent]-Konto direkt aus einem [!DNL Cvent]-Modul erstellen.

1. Klicken Sie in einem beliebigen [!DNL Cvent]-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Wählen Sie die Region aus, mit der Sie eine Verbindung herstellen möchten.

   * [!UICONTROL Nordamerika]
   * [!UICONTROL Europa]
   * [!UICONTROL Sandbox]

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Cvent] Module und ihre Felder

Wenn Sie [!DNL Cvent] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Cvent] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Aktionen

* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#create-meeting-request)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Einladung registrieren]](#register-invitee)
* [[!UICONTROL Einladung hinzufügen]](#add-invitee)
* [[!UICONTROL Kontakt löschen]](#delete-contact)
* [[!UICONTROL Kontakt aktualisieren]](#update-contact)
* [[!UICONTROL Erstellen einer Sitzungsanforderung]](#create-meeting-request)

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Cvent] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Cvent] -Modulen nicht ausgeführt werden kann.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

Das Modul gibt den Status-Code zusammen mit den Kopfzeilen und dem Text des API-Aufrufs zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Cvent]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Vorgang</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Textkörper (XML)</td> 
   <td> <p>Geben Sie den Hauptteil des API-Aufrufs ein oder ordnen Sie ihn zu. Dies darf nur die XML-Datei enthalten. Das Modul enthält automatisch Authentifizierungskopfzeilen. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest Informationen zu einem bestimmten Datensatz.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Cvent]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record Type]</p> </td> 
   <td>Wählen Sie den Elementtyp des Datensatzes aus, den Sie lesen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kontakt] / [!UICONTROL Ereignis] / [!UICONTROL Einladungs-ID]</td> 
   <td> <p>Geben Sie die ID des Elements ein, das Sie lesen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten. Die Felder sind je nach ausgewähltem Elementtyp verfügbar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einladung registrieren]

Dieses Aktionsmodul registriert eine Einladung für ein Ereignis.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Cvent]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Einladungs-ID</p> </td> 
   <td> <p>Geben Sie die ID der Einladung ein oder ordnen Sie sie zu, die Sie für ein Ereignis registrieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ereignis-ID</td> 
   <td> <p>Geben Sie die ID des Ereignisses ein oder ordnen Sie sie zu, für das Sie die Einladung registrieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einladung hinzufügen]

Dieses Aktionsmodul lädt einen Kontakt zu einer Veranstaltung ein.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Cvent]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kontakt-ID]</p> </td> 
   <td> <p>Geben Sie die Kennung des Kontakts ein, den Sie einem Ereignis hinzufügen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td> <p>Geben Sie die ID des Ereignisses ein oder ordnen Sie sie zu, dem Sie den Kontakt hinzufügen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kontakt löschen]

Dieses Aktionsmodul löscht einen einzelnen Kontakt in Cvent.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Cvent]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kontakt-ID]</td> 
   <td> <p>Geben Sie die Kennung des Kontakts ein, den Sie löschen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kontakt aktualisieren]

Dieses Aktionsmodul aktualisiert einen bestehenden Kontakt mit seiner Kennung.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Cvent]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kontakt-ID]</p> </td> 
   <td> <p>Geben Sie die Kennung des Kontakts ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder]</td> 
   <td> <p>Wählen Sie die Felder aus, für die Sie Informationen eingeben möchten, und geben Sie dann die gewünschten Werte für diese Felder ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Felder]</td> 
   <td> <p>Wählen Sie die Felder aus, für die Sie Informationen eingeben möchten, und geben Sie dann die gewünschten Werte für diese Felder ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen einer Sitzungsanforderung]

Dieses Aktionsmodul fügt Ihrem -Konto eine Sitzungsanfrage hinzu.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Cvent]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Formular-ID]</p> </td> 
   <td> <p>Geben Sie die Kennung des Formulars ein, das Sie zur Erstellung der neuen Sitzungsanforderung verwenden möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder für Meeting-Anfragen]</td> 
   <td> <p>Wählen Sie die Felder aus, für die Sie Informationen eingeben möchten, und geben Sie dann die gewünschten Werte für diese Felder ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignisanforderungsfelder]</td> 
   <td> <p>Wählen Sie die Ereignisanforderungsfelder aus, für die Sie Informationen eingeben möchten, und geben Sie dann die gewünschten Werte für diese Felder ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL RFP-Anforderungsfelder]</td> 
   <td> <p>Wählen Sie die Anforderung für die Vorschlagsfelder aus, für die Sie Informationen eingeben möchten, und geben Sie dann die gewünschten Werte für diese Felder ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

#### [!UICONTROL Listeneinträge]

Dieses Suchmodul ruft Informationen zu allen Datensätzen eines bestimmten Typs ab.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Cvent]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-cvent-to-adobe-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Cvent] mit [!DNL Adobe Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Record Type]</p> </td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie auflisten möchten.</p> 
    <ul> 
     <li> <p>Alle Ereignisse aus Ihrem [!DNL Cvent]-Konto</p> </li> 
     <li> <p>Alle Sitzungen für ein Ereignis</p> </li> 
     <li> <p>Alle Einladungen für eine Veranstaltung</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td> <p>Wenn Sie Einladungen oder Sitzungen auflisten, geben Sie die ID des Ereignisses ein, mit dem diese Einladungen oder Sitzungen verknüpft sind, oder ordnen Sie diese zu.</p> </td> 
  </tr> 
 </tbody> 
</table>
