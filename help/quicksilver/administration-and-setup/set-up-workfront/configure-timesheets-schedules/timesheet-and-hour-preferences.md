---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Konfigurieren der Voreinstellungen für das Datenblatt und die Stunde
description: Als [!DNL Adobe Workfront] Administrator können Sie in [!DNL Workfront] Voreinstellungen für Timesheets und Stunden festlegen, um zu definieren, mit welchen Elementen die Timesheets vorbelegt werden können und zu welchen Elementen Benutzer die Zeit protokollieren können.
author: Alina and Lisa
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---

# Arbeitszeittabelle und Stundeneinstellungen konfigurieren

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] -Administrator können Sie in [!DNL Workfront] Voreinstellungen für Timesheets und Stunden festlegen, um zu definieren, mit welchen Elementen die Timesheets vorbelegt werden können und zu welchen Elementen Benutzer die Zeit protokollieren können.

>[!IMPORTANT]
>
>Zusätzlich zu den Artikeln, die ein Timesheet gemäß den in diesem Artikel beschriebenen Bedingungen vorab ausfüllen, werden die folgenden Elemente standardmäßig auch auf Timesheets angezeigt:
>
>* Elemente, bei denen Sie die Zeit im Zeitrahmen des Zeitblatts protokolliert haben
>* Elemente, die auf das Zeitblatt geschrieben sind
>* Elemente, nach denen Sie suchen und die Sie manuell zum Timesheet hinzufügen. Manuell hinzugefügte Elemente werden standardmäßig fixiert.
>
>Weitere Informationen finden Sie unter [Protokollzeit](../../../timesheets/create-and-manage-timesheets/log-time.md) und [Übersicht über das Timesheet](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).

Alle Änderungen, die Sie an Timesheets vornehmen, wirken sich auf alle in der Zukunft erstellten Timesheets aus.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Aktuell:[!UICONTROL Plan]</p>
   Oder
   <p>Neu: Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
</tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Festlegen von Zeitblatt- und Stundenvoreinstellungen

{{step-1-to-setup}}

1. Klicken Sie auf **[!UICONTROL Zeitblatt &amp; Stunden]** > **[!UICONTROL Voreinstellungen]**.

   Die Seite mit den Voreinstellungen für Timesheets und Stunden wird angezeigt.

1. (Optional) Beginnen Sie im Suchfeld **Voreinstellungen für Systemzeiten und Voreinstellungen** mit der Eingabe des Namens einer Gruppe und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

   ![](assets/search-for-group-box-in-timesheets-preferences-page.png)

   Auf der Seite &quot;Timesheet- und Stundeneinstellungen&quot;werden die Voreinstellungen für die ausgewählte Gruppe aktualisiert. Die Voreinstellungen auf Systemebene müssen entsperrt sein, damit Sie die Voreinstellungen auf Gruppenebene ändern können. Weitere Informationen finden Sie im Abschnitt [Zeitblatt- und Stundeneinstellungen für Gruppen entsperren](#unlock-timesheet-and-hour-preferences-for-groups) in diesem Artikel.

1. Konfigurieren Sie im Abschnitt **[!UICONTROL Allgemeine Voreinstellungen]** eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Protokollzeit für zukünftige Daten]</td> 
      <td> <p>Ermöglicht Benutzern, die Zeit für zukünftige Daten im gesamten System zu protokollieren in:</p> 
       <ul> 
        <li>Alle Projekte, Aufgaben und Probleme, auf die sie Zugriff auf die Protokollzeit haben</li> 
        <li>Ihre Timesheets als "Allgemeine Zeit"</li> 
       </ul> <p>Dies ist nützlich, wenn Benutzer planen, außerhalb des Büros zu sein, und diese Zeit vorher protokollieren möchten.</p> <p><b>NOTE</b>:</p> 
       <p>Sie können Benutzer nicht daran hindern, die Zeit für Aufgaben oder Probleme zu protokollieren, die geschlossen oder abgebrochen werden. Sie können Benutzer nur daran hindern, die Zeit für komplette oder tote Projekte zu protokollieren. Es wird empfohlen, Filter in Listen mit Aufgaben und Problemen zu verwenden, um auszuschließen, dass abgeschlossene oder abgebrochene Aufgaben für Benutzer nicht sichtbar sind.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Manuelles Zuweisen von Auftragsrollen zu Stundeneinträgen]</td> 
      <td> <p>Benutzern die manuelle Auswahl von Aufgaben ermöglichen, die in ihrem Benutzerprofil zugewiesen oder dem Objekt zugewiesen sind.</p> <p><b>WICHTIG</b>:  
        <ul> 
         <li>Wenn Sie diese Einstellung deaktivieren, nachdem Sie Stundeneinträgen Auftragsrollen zugewiesen haben, müssen die Benutzer die Stunden anpassen, die auf der Registerkarte [!UICONTROL Hours] des Projekts, der Aufgabe oder des Problems unter verschiedenen Rollen protokolliert wurden.</li> 
         <li>Wenn dem Benutzer in seinem Profil keine Auftragsrolle zugewiesen ist und im Dialogfeld [!UICONTROL Erweiterte Zuweisungen] eine Aufgabe als [!UICONTROL Aufgabenbesitzer] zugewiesen ist, wird diese Auftragsrolle angezeigt, wenn der Benutzer die Zeit für die Aufgabe angibt.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Eingrenzen der Bearbeitung von Zeitblättern an Eigentümer und Administratoren]</td> 
      <td> <p>Beschränken Sie die Bearbeitung auf die Inhaber von Zeitblättern und die Administratoren von [!DNL Workfront]. Wenn diese Option deaktiviert ist, können Timesheets auch wie folgt bearbeitet werden:</p> 
       <ul> 
        <li> <p>Benutzer mit administrativem Zugriff auf Timesheets und Stunden in ihrer Zugriffsebene</p> </li> 
        <li> <p>Timesheet-Genehmiger, wenn auf dem Timesheet "Kann Stunden bearbeiten"aktiviert ist</p> </li> 
        <li> <p>Manager des Timesheet-Eigentümers</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Eingeschränkte Stundenbearbeitung für Eigentümer und Administratoren]</td> 
      <td>Beschränken Sie die Bearbeitung auf den Benutzer, der die Stunden eingibt, und auf [!DNL Workfront] Administratoren. Diese Einstellung gilt für die Registerkarte [!UICONTROL Hours] in einem Projekt oder in einem Stundenbericht.</td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurieren Sie im Abschnitt &quot;**[!UICONTROL Wo Benutzer die Zeit protokollieren können]**&quot;eine der folgenden Optionen:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Direkt über Projekte]</td>
        <td>Ermöglicht Benutzern die Protokollierung der Zeit im Projekt (sowohl auf der Registerkarte [!UICONTROL Updates] als auch auf dem Timesheet). Wenn Benutzer keine Zeit auf Projektebene aufzeichnen, sollten diese Optionen deaktiviert bleiben.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Bei abgeschlossenen Projekten]</td>
        <td>Ermöglicht Benutzern das Aufzeichnen der Zeit für ein Projekt, das als abgeschlossen gekennzeichnet wurde. Wenn diese Option deaktiviert ist, können Benutzer die Zeit für die Arbeit, die sie an Projekten abgeschlossen haben, nicht im Status [!UICONTROL Abgeschlossen] aufzeichnen.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Über verstorbene Projekte]</td>
        <td>Wenn diese Option aktiviert ist, können Benutzer Stunden für Projekte mit dem Status [!UICONTROL Dead] protokollieren.</td>
    </tr>
   </table>

1. Konfigurieren Sie im Abschnitt **[!UICONTROL Vorfüllen von Timesheets]** eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Arbeit, die innerhalb von] &lt;Anzahl der Wochen&gt; [!UICONTROL Arbeitsumfang des Zeitplans]</td> 
      <td> <p>Definiert die Anzahl der Wochen vor und nach dem Datumsbereich des Zeitblatts, das Datum der dem Benutzer zugewiesenen Aufgaben und Probleme enthält.</p> 
      <p>Die Standardeinstellung ist 1 Woche, und Sie können diesen Bereich auf 4 Wochen erweitern.</p> 
      <p>Das bedeutet, dass das Timesheet mit Aufgaben und Problemen vorausgefüllt ist, die zwischen vier Wochen vor dem Datumsbereich des Zeitblatts und bis zu vier Wochen nach dem Datumsbereich des Zeitblatts liegen, wenn Sie für Ihren Bereich vier Wochen auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aufgaben und abgeschlossene Probleme]</td> 
      <td>Wenn normalerweise mehrere Ressourcen einer einzelnen Aufgabe zugewiesen sind, empfehlen wir diese Einstellung. Das bedeutet, dass die anderen Ressourcen, die der Aufgabe zugewiesen sind, die Aufgabe bzw. das Problem in ihrem Timesheet finden können, um ihre Stunden aufzuzeichnen, wenn eine Ressource die Zeit für die Aufgabe aufzeichnet und sie als abgeschlossen kennzeichnet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aufgaben und Probleme, bei denen im Datumsbereich des Datenblatts geplante Daten angegeben sind]</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält das Timesheet Aufgaben und Probleme mit einem geplanten Startdatum oder einem geplanten Abschlussdatum, das in den Datumsbereich des Zeitblatts fällt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Aufgaben, bei denen im Datumsbereich des Datenblatts die geplanten Daten angegeben sind]</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält das Timesheet Aufgaben mit einem geplanten Startdatum oder Abschlussdatum, die innerhalb des Zeitrahmens des Projekts liegen, selbst wenn das geplante Datum des Problems oder der Aufgabe außerhalb des Zeitblatt-Datumsbereichs liegt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Geben Sie im Abschnitt **[!UICONTROL Gelöschte Projekte, Aufgaben und Probleme]** Folgendes an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> Beim Löschen von Projekten</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Behalten Sie die bereits zu Timesheets hinzugefügte Protokollzeit als allgemeine Zeit bei]</strong>: Wenn dieses Projekt zu einem späteren Zeitpunkt wiederhergestellt wird, bleibt die Zeit auf dem Timesheet.</li> 
        <li><strong>[!UICONTROL Beliebige Zeit löschen]</strong>: Wenn dieses Projekt später wiederhergestellt wird, wird die bereits protokollierte Zeit wieder in das Projekt eingefügt.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beim Löschen von Aufgaben oder Problemen</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Verschieben Sie eine protokollierte Zeit in das Projekt]</strong>, in dem sich die Aufgabe oder das Problem befindet: Wenn diese Aufgabe oder dieses Problem später wiederhergestellt wird, bleibt die Zeit im Projekt.<br></li> 
        <li> <p><strong>[!UICONTROL Beliebige Zeit löschen]</strong>: Wenn diese Aufgabe oder dieses Problem später wiederhergestellt wird, wird die protokollierte Zeit für die Aufgabe oder das Problem wiederhergestellt.</p> <p>Weitere Informationen zu diesen Optionen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Auswirkungen konfigurieren] für Stunden, in denen ein Objekt gelöscht und wiederhergestellt wird</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Zeitblatt- und Stundenvoreinstellungen für Gruppen entsperren

Gruppen in Ihrer Organisation benötigen möglicherweise Timesheets oder Stundenvoreinstellungen, die für ihre individuellen Workflows unterschiedlich konfiguriert sind. Sie können die Voreinstellungen für alle Gruppen in der Organisation entsperren, damit sie sie selbst konfigurieren können.

Wenn eine Voreinstellung entsperrt ist und ein Gruppenadministrator sie ändert, wirkt sich dies auf die Inhaber von Zeitblättern aus, wenn es sich bei der Gruppe um ihre Startseite handelt.

Informationen dazu, wie ein Gruppenadministrator die Voreinstellungen für das Zeitblatt und die Stunde für eine Gruppe konfiguriert, finden Sie unter [Konfigurieren von Voreinstellungen für Zeitblätter und Stunden für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Nachdem ein [!DNL Workfront] -Administrator eine Voreinstellung auf Systemebene entsperrt hat, kann jeder Gruppenadministrator sie konfigurieren und sie dann sperren, um sicherzustellen, dass alle Mitglieder ihrer Gruppe und der unten stehenden Untergruppen dieselbe Konfiguration verwenden. Dies entspricht der Möglichkeit, dass ein [!DNL Workfront] -Administrator eine Voreinstellung für alle Benutzer im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Vorgabe zum Sperren oder Entsperren eines Gruppen-Timesheets und einer Stunde](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

So entsperren Sie eine Projektvoreinstellung, damit Gruppen sie konfigurieren können:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Timesheets und Stunden]** und klicken Sie dann auf **[!UICONTROL Voreinstellungen]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Gruppenadministratoren eine Voreinstellung für ihre Gruppen konfigurieren können, klicken Sie auf den Umschalter **Entsperren** , um sie zu entsperren.![](assets/unlock-toggle-button.png)
   * Wenn Sie möchten, dass alle Gruppen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass der Umschalter &quot;![](assets/locked-preference-toggle.png)&quot;ist (dies ist die Standardeinstellung).

     >[!IMPORTANT]
     >
     >Es wird empfohlen, mit den Administratoren und Benutzern in Gruppen im gesamten System zu kommunizieren, um sicherzustellen, dass alle Anforderungen so berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren.
     >
     >Wenn Sie sie sperren, wird Ihre Konfiguration für sie von allen Gruppen im System übernommen. Wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Einstellungen, die von Gruppenadministratoren vorgenommen wurden.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
