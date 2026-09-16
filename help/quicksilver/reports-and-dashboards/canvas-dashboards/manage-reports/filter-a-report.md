---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtern eines Berichts in einem Arbeitsflächen-Dashboard
description: Fügen Sie einen Filter für einen Bericht hinzu oder bearbeiten Sie ihn, um zu steuern, welche Daten in einem Arbeitsflächen-Dashboard angezeigt werden.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 15%
---
# Filtern eines Berichts in einem Arbeitsflächen-Dashboard

>[!IMPORTANT]
>
>Die Funktion Canvas-Dashboards ist derzeit nur für Benutzer verfügbar, die an der Beta-Phase teilnehmen. Teile der Funktion sind in dieser Phase möglicherweise nicht vollständig oder funktionieren nicht wie vorgesehen. Bitte senden Sie Feedback zu Ihrem Erlebnis, indem Sie die Anweisungen im Abschnitt [Feedback geben](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) im Artikel Beta-Übersicht für Arbeitsflächen-Dashboards befolgen.<br>
>Wenn Sie Feedback zu einem möglichen Fehler oder einem technischen Problem haben, senden Sie bitte ein Ticket an den Workfront-Support. Weitere Informationen finden Sie unter [Kontaktieren des Kunden-Supports](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Beachten Sie, dass diese Beta-Version bei den folgenden Cloud-Anbietern nicht verfügbar ist:
>
>* Eigene Schlüssel für Amazon Web Services mitbringen
>* Azure
>* Google Cloud Platform

Sie können einen Bericht filtern, um zu steuern, welche Daten angezeigt werden, sowohl während der Erstellung des Berichts als auch jederzeit danach. Die Filteroptionen und das Verhalten sind in beiden Fällen identisch.

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
<p>Abo</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td> 
   <td><p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p>
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td><p>Berechtigungen für das Dashboard verwalten</p>
  </td> 
  </tr>
</tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Voraussetzungen

Sie müssen über einen Bericht in einem Dashboard verfügen oder einen erstellen, bevor Sie ihn filtern können. Weitere Informationen finden Sie unter [Erstellen eines Arbeitsflächen-Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Hinzufügen oder Bearbeiten eines Berichtsfilters

So fügen Sie einen Filter für einen Bericht hinzu oder bearbeiten ihn:

1. Öffnen Sie das Filterbedienfeld des Berichts:

   * Wenn Sie einen Bericht erstellen, klicken Sie auf das Symbol **Filter** im linken Bereich des Dialogfelds **Konfigurieren**.
   * Wenn Sie einen vorhandenen Bericht bearbeiten, klicken Sie auf das Symbol **Mehr** oben rechts, wählen Sie **Bearbeiten** aus und klicken Sie dann im Dialogfeld **Konfigurieren** auf das Bedienfeld **Filter**.

1. Klicken Sie **Filter bearbeiten**.

1. Klicken Sie **Bedingung hinzufügen** und definieren Sie dann die Bedingung:

   * Klicken Sie **Feld auswählen** und wählen Sie dann das Feld aus, nach dem Sie filtern möchten.
   * Wählen Sie den Modifikator, der definiert, welche Art von Bedingung das Feld erfüllen muss.
   * Geben Sie den Wert ein, anhand dessen ausgewertet werden soll, oder wählen Sie ihn aus, wenn der Modifikator einen erfordert.

   ![Bedingung hinzufügen](assets/add-condition.png)

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Bedingungen hinzuzufügen.

1. (Optional) Klicken Sie auf **Filtergruppe hinzufügen**, um einen weiteren Satz von Filterkriterien hinzuzufügen. Der Standardoperator zwischen den Sätzen ist UND. Klicken Sie auf den Operator, um ihn in ODER zu ändern.

>[!NOTE]
>
>Eine vollständige Liste der Felder, Operatoren, Platzhalter und speziellen Filterregeln finden Sie unter [Berichtsfilterreferenz für Arbeitsflächen-Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

1. Klicken Sie auf **Speichern**.
