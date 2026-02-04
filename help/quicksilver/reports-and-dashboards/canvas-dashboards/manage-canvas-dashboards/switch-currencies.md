---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Verwenden von Währungsfeldern in Dashboards der Arbeitsfläche
description: Sie können die Währungsfelder in einem Arbeitsflächen-Dashboard verwenden.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---


# Verwenden von Währungsfeldern in Dashboards der Arbeitsfläche

>[!IMPORTANT]
>
>Die Funktion Canvas-Dashboards ist derzeit nur für Benutzer verfügbar, die an der Beta-Phase teilnehmen. Teile der Funktion sind in dieser Phase möglicherweise nicht vollständig oder funktionieren nicht wie vorgesehen. Bitte senden Sie Feedback zu Ihrem Erlebnis, indem Sie die Anweisungen im Abschnitt [Feedback geben](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) im Artikel Beta-Übersicht für Canvas-Dashboards befolgen.<br>
>Wenn Sie Feedback zu einem möglichen Fehler oder einem technischen Problem haben, senden Sie bitte ein Ticket an den Workfront-Support. Weitere Informationen finden Sie unter [Kundensupport kontaktieren](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Beachten Sie, dass diese Beta-Version bei den folgenden Cloud-Anbietern nicht verfügbar ist:
>
>* Eigene Schlüssel für Amazon Web Services mitbringen
>* Azure
>* Google Cloud Platform

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebig </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td> 
<p>Standard</p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td> 
   <td><p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p>
   <p>Zugriff auf Finanzdaten anzeigen</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td><p>Berechtigungen für das Dashboard verwalten</p>
  </td> 
  </tr> 
</tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Voraussetzungen

1. Sie müssen mehrere Währungstypen in Ihrer Workfront-Instanz eingerichtet haben, um die in diesem Artikel beschriebenen Funktionen verwenden zu können. Weitere Informationen finden Sie [Einrichten von Wechselkursen](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   >[!IMPORTANT]
   >
   >Die in diesem Artikel beschriebene Funktion gilt nur für Felder in nativer Währung. Die Unterstützung für benutzerdefinierte Währungsfelder wird bald verfügbar sein.


## Festlegen einer Standardwährung für ein Arbeitsflächen-Dashboard

Beim Erstellen eines Arbeitsflächen-Dashboards können Sie eine Standardwährung für das Dashboard festlegen. Diese Währung wird verwendet, um alle Felder in der nativen Währung in Berichten im Dashboard anzuzeigen, es sei denn, das Währungsfeld ist auf Berichtsebene gesperrt.

1. Klicken Sie im linken Bedienfeld auf **Arbeitsflächen-Dashboards**.

1. Klicken Sie **oben** auf „Neues Dashboard“.

1. Im Feld **Dashboard erstellen**

1. Geben Sie Folgendes an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Name</strong></td>
      <td><p>Geben Sie einen Namen für Ihr Dashboard ein. Es wird empfohlen, nur UTF-8-Zeichen zu verwenden, um Kompatibilitätsprobleme zu vermeiden.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beschreibung (optional)</strong></td>
      <td>Eine Beschreibung Ihres Dashboards eingeben.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Währung</strong></td>
      <td>Wählen Sie den Standardwährungstyp für das Dashboard aus. <br>
      <br>Benutzer können beim Filtern des Dashboards zwischen verschiedenen Währungstypen wechseln.</td>
     </tr>
    </tbody>
   </table>


## Wechseln zwischen Währungen auf einem Arbeitsflächen-Dashboard

Sie können auf Dashboard-Ebene zwischen verschiedenen Währungstypen wechseln. Berichte, die Währungsfelder enthalten, werden entsprechend dem ausgewählten Währungstyp aktualisiert.

Währungsfelder können auf Berichtsebene gesperrt werden. Wenn ein Währungsfeld gesperrt ist, ändert sich der Währungstyp für diesen Bericht nicht, wenn Sie den Währungstyp für das Dashboard ändern.

So ändern Sie den Währungstyp für das Dashboard:

1. Klicken Sie auf das Dropdown-Menü Währung in der oberen rechten Ecke der Detailseite des Dashboards.
1. Wählen Sie den gewünschten Währungstyp aus der Liste aus.

   ![Währungs-Dropdown ändern](assets/filter-by-currency.png)


## Einschränkungen

In der folgenden Tabelle sind Einschränkungen aufgeführt, wenn Währungen im Bereich „Wechselkurse“ unter „Setup“ definiert sind.

<table> 
<tr>
<td></td>
<td>Benutzer können</td>
<td>Benutzer können nicht</td>
</tr>
<tr> 
<td>Eine einheitliche Währung ist definiert</td>
<td>
<ul>
<li>Verwenden von Feldern in nativen Währungen in Arbeitsflächen-Diagrammen, KPIs und Tabellenberichten</li>
<li>Verwenden benutzerdefinierter Währungsfelder in Arbeitsflächen-Diagramm-, KPI- und Diagrammberichten</li>
</ul>
</td>
<td>
<ul>
<li>Weisen Sie dem Dashboard eine Standardwährung zu (bei der Erstellung oder bei der Bearbeitung des Dashboards)</li>
<li>Den Umschalter für die Währung auf Dashboard-Ebene anzeigen und verwenden</li>
<li>Sperren einer bestimmten Währung zur Anzeige in einem Arbeitsflächendiagramm, einem KPI oder einem Tabellenbericht</li>
<li>Verwenden von Planning-Währungsfeldern in Arbeitsflächendiagrammen, KPIs und Tabellenberichten</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>Mehrere Währungen sind definiert</td>
<td>
<ul>
  <li>Verwenden von Feldern in nativen Währungen in Arbeitsflächen-Diagrammen, KPIs und Tabellenberichten</li>
  <li>Festlegen einer Standardwährung für das Dashboard (bei der Erstellung oder beim Bearbeiten des Dashboards)</li>
  <li>Den Umschalter für die Währung auf Dashboard-Ebene anzeigen und verwenden</li>
  <li>Eine bestimmte Währung für die Ansicht in einem Arbeitsflächen-Diagramm, KPI oder Tabellenbericht sperren, um die Voreinstellung zum Umschalten der Dashboard-Währung zu ignorieren</li>
</ul>
</td>
<td><ul>
  <li>Verwenden benutzerdefinierter Datenwährungsfelder in Arbeitsflächen-Diagrammen, KPIs und Tabellenberichten</li>
  <li>Verwenden von Planning-Währungsfeldern in Arbeitsflächendiagrammen, KPIs und Tabellenberichten</li>
</ul>
</td>
</tr></table>





