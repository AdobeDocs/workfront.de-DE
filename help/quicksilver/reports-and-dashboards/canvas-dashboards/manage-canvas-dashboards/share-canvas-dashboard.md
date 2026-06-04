---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Freigeben eines Arbeitsflächen-Dashboards
description: Sie können ein Arbeitsflächen-Dashboard für andere Adobe Workfront-Benutzende freigeben, damit diese es anzeigen oder bearbeiten können.
author: Courtney
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Aujcry4UfvcMotGau6-o2cjiH1wdG5V4-ytBzgvu9aI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 522
ht-degree: 10%

---

# Freigeben eines Arbeitsflächen-Dashboards

>[!IMPORTANT]
>
>Die Funktion Canvas-Dashboards ist derzeit nur für Benutzer verfügbar, die an der Beta-Phase teilnehmen. Teile der Funktion sind in dieser Phase möglicherweise nicht vollständig oder funktionieren nicht wie vorgesehen. Bitte senden Sie Feedback zu Ihrem Erlebnis, indem Sie die Anweisungen im Abschnitt [Feedback geben](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) im Artikel Beta-Übersicht für Canvas-Dashboards befolgen.<br>
>Wenn Sie Feedback zu einem möglichen Fehler oder einem technischen Problem haben, senden Sie bitte ein Ticket an den Workfront-Support. Weitere Informationen finden Sie unter [Kundensupport kontaktieren](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Beachten Sie, dass diese Beta-Version bei den folgenden Cloud-Anbietern nicht verfügbar ist:
>
>* Eigene Schlüssel für Amazon Web Services mitbringen
>* Azure
>* Google Cloud Platform

Sie können ein Arbeitsflächen-Dashboard für andere Adobe Workfront-Benutzende freigeben, damit diese es anzeigen oder bearbeiten können.

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
<p>Standard </p> 
<p>Abo</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationen der Zugriffsebene</p></td> 
   <td><p>Anzeigen des Zugriffs auf Berichte, Dashboards und Kalender</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td><p>Anzeigen von Berechtigungen für das Dashboard zur Freigabe des Dashboards</p>
   <p>Verwalten von Berechtigungen für das Dashboard zum Zuweisen von Dashboard-Berechtigungen</p>
  </td> 
  </tr>
</tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Überlegungen zur Freigabe von Dashboards

* Dashboards können für Benutzende, Teams, Gruppen, Aufgabengebiete oder Unternehmensressourcen freigegeben werden.

* Standardmäßig verfügt der Ersteller eines Dashboards über Verwaltungsberechtigungen für das Dashboard.

* Systemadministratoren und Benutzer mit der Berechtigung „Verwalten“ können Zugriff auf ein Dashboard gewähren, anzeigen oder verwalten.

* Benutzende mit der Berechtigung Anzeigen für ein Dashboard können Ansichtszugriff auf ein Dashboard gewähren.

* Bei der Freigabe eines Dashboards erben die Ressourcen, für die es freigegeben ist, die Berechtigungen für die im Dashboard angezeigten Berichte.

* Wenn ein Dashboard über eine Layout-Vorlage verteilt wird, wird allen Ressourcen, die der Layout-Vorlage zugewiesen sind, eine automatische Ansichtsberechtigung für das Dashboard (und dessen Berichte) gewährt.

* Wenn ein Bericht in einem Dashboard mit der Option Als Benutzer ausführen konfiguriert ist, sehen alle Viewer Daten, die auf den Berechtigungen der ausgewählten Benutzenden und nicht auf ihren eigenen basieren. Das bedeutet, dass Betrachterinnen und Betrachter möglicherweise Daten sehen, auf die sie normalerweise keinen Zugriff haben. Wenn einige Berichte in einem Dashboard die Funktion „Als Benutzer ausführen“ verwenden und andere nicht, werden den Betrachtern möglicherweise inkonsistente Daten in allen Berichten angezeigt.


## Freigeben eines Arbeitsflächen-Dashboards


{{step1-to-dashboards}}

1. Klicken Sie im linken Bedienfeld auf **Arbeitsflächen-Dashboards**.

1. Wählen Sie auf **Seite &quot;** Dashboards“ das Dashboard aus, das Sie freigeben möchten.

1. Klicken Sie oben rechts auf der Seite auf die Schaltfläche **Freigeben**. Das **Dashboard-Freigabe** wird angezeigt.

   ![Freigabe-Schaltfläche](assets/share-button.png)

1. Beginnen Sie im Feld **Zugriff erteilen an** mit der Eingabe des Namens eines bestimmten Benutzers, Teams, einer bestimmten Rolle, einer Gruppe oder eines Unternehmens, für den bzw. die Sie das Arbeitsflächen-Dashboard freigeben möchten, und wählen Sie ihn aus, wenn er in der Dropdown-Liste angezeigt wird.

1. (Optional) Um den Zugriff einer Ressource auf das Dashboard zu bearbeiten, klicken Sie auf **Anzeigen** neben ihrem Namen und wählen Sie dann **Verwalten** in der angezeigten Dropdown-Liste aus.

   >[!NOTE]
   >
   > Wenn Benutzenden die Bearbeitungsberechtigungen für ein Dashboard nicht über ihre Zugriffsebene zugewiesen wurden, können ihnen keine Verwaltungsberechtigungen für ein Dashboard zugewiesen werden.

1. Wiederholen Sie die Schritte 5 bis 6 für jede Ressource, für die Sie das Dashboard freigeben möchten.

1. Klicken Sie auf die **Freigeben**. Die Empfänger erhalten eine E-Mail-Benachrichtigung, die sie darüber informiert, dass das Dashboard für sie freigegeben wurde, auf das sie jetzt unter **Dashboards** > **Arbeitsflächen-Dashboards** > **Freigegebene Dashboards** zugreifen können.

   >[!NOTE]
   >
   > Es können individuelle Benutzervoreinstellungen und Systemausschlüsse für E-Mail-Benachrichtigungen gelten. <br>
   > Benachrichtigungen werden nur gesendet, wenn sie direkt für einen Benutzer freigegeben werden. Bei der Freigabe für Gruppen, Rollen, Unternehmen und Teams werden keine E-Mail-Benachrichtigungen generiert.<br>
   > Berechtigungen, die von einer Layout-Vorlage übernommen werden, generieren keine E-Mail-Benachrichtigung über den Zugriff auf das Dashboard.
