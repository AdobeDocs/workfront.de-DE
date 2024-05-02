---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Organisationsrollen in [!DNL Adobe Workfront Fusion]
description: Dieser Artikel enthält Informationen über den Zugriff und die Berechtigungen der Rollen in [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 0370fa9d-6680-4724-a431-8df884ce4f9a
source-git-commit: cb093fcecd5defd9dbdbb955ad5158d4a794f005
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 1%

---

# Organisations- und Teamrollen in [!DNL Adobe Workfront Fusion]

In diesem Artikel werden der Zugriff und die Funktionalität beschrieben, die den verschiedenen Team- und Organisationsrollen in [!DNL Workfront Fusion].

>[!NOTE]
>
>Die Organisationsrollen unterscheiden sich von den Teamrollen in [!DNL Workfront Fusion]. Weitere Informationen zu Organisations- und Teamrollen finden Sie unter [Organisationen und Teams](../organizations/organizations-and-teams.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
   <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
    <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> 
     <p>Sie müssen [!DNL Workfront Fusion] Administrator für Ihre Organisation.</p>
     <p>Sie müssen [!DNL Workfront Fusion] Administrator für Ihr Team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Organisationsrollen

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p>[!UICONTROL Inhaber]</p> </th> 
   <th> <p>[!UICONTROL Admin]</p> </th> 
   <th> <p>[!UICONTROL Mitglied]</p> </th> 
   <th> <p>[!UICONTROL Accountant]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Zugriff auf alle Teams</p> </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Organisation bearbeiten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Verwalten von Organisationsbenutzern</p> </td> 
   <td>✓ </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Organisation anzeigen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Process payments</p> </td> 
    <td>✓ </td> 
    <td>✓ </td> 
    <td> </td> 
    <td> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>List payments</p> </td> 
    <td>✓ </td> 
    <td>✓ </td> 
    <td> </td> 
    <td> </td> 
   </tr>
  --> 
  <tr> 
   <td> <p>Team hinzufügen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr>

</tbody> 
</table>


## Teamrollen

### Szenarios

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Admin]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Mitglied]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Überwachung]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Operator]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p style="text-align: left;">Verwalten unvollständiger Ausführungen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Unvollständige Ausführungen auflisten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Szenarien hinzufügen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Löschen von Szenarien</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Szenarien bearbeiten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Ausführungsverlauf des Durchsuchen-Szenarios</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Empfangsszenario-Benachrichtigungen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Status zurücksetzen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Listen-Szenarien</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Bearbeiten des Szenario-Schedulers</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Start-Szenarien</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Stoppszenarien</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Szenarien manuell ausführen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Szenarien anzeigen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   </tr> 
 </tbody> 
</table>

### Verbindungen

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Admin]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Mitglied]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Überwachung]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Operator]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p style="text-align: left;">Verbindungen hinzufügen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Verbindungen löschen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Verbindungen bearbeiten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Listen-Verbindungen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

### Webhooks

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Admin]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Mitglied]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Überwachung]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Operator]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p style="text-align: left;">Webhooks hinzufügen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Webhooks löschen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Webhooks bearbeiten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Webhooks auflisten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

### Datenspeicher

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Admin]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Mitglied]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Überwachung]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Operator]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p style="text-align: left;">Hinzufügen von Datenspeichern</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Datenspeicher löschen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Datenspeicher bearbeiten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Datenspeicher auflisten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Datenspeicher durchsuchen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

### Datenstrukturen

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Admin]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Mitglied]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Überwachung]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Operator]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p style="text-align: left;">Hinzufügen von Datenstrukturen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Datenstrukturen löschen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Datenstrukturen bearbeiten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Auflisten von Datenstrukturen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

### Schlüssel

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Admin]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Mitglied]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Überwachung]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Operator]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p style="text-align: left;">Schlüssel hinzufügen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Schlüssel löschen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Schlüssel bearbeiten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Listenschlüssel</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

### Vorlagen

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Admin]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Mitglied]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Überwachung]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Operator]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p style="text-align: left;">Vorlagen hinzufügen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Vorlagen löschen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Vorlagen bearbeiten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Vorlagen auflisten</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Vorlagen anzeigen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>

### Teams

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Admin]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Mitglied]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Überwachung]</p> </th> 
   <th> <p style="text-align: left;">[!UICONTROL Operator]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p style="text-align: left;">Teams hinzufügen</p> </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Löschen von Teams</p> </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Team-Benutzer hinzufügen und bearbeiten</p> </td> 
   <td>✓ </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p style="text-align: left;">Teams anzeigen</p> </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
   <td>✓ </td> 
  </tr> 
 </tbody> 
</table>




