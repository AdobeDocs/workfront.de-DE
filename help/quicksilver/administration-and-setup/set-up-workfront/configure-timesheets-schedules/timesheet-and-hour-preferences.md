---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Arbeitszeittabelle und Stundeneinstellungen konfigurieren
description: Als  [!DNL Adobe Workfront]  können Sie Voreinstellungen für Arbeitszeittabellen und Stunden in festlegen [!DNL Workfront]  um festzulegen, mit welchen Elementen die Arbeitszeittabellen vorab ausgefüllt werden können und welchen Elementen Benutzer Zeit protokollieren können.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1411'
ht-degree: 0%

---

# Arbeitszeittabelle und Stundeneinstellungen konfigurieren

<!--Audited: 06/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] können Sie Voreinstellungen für Arbeitszeittabellen und Stunden in [!DNL Workfront] festlegen, mit welchen Elementen die Arbeitszeittabellen vorab ausgefüllt werden können und welchen Elementen Benutzer Zeit protokollieren können.

>[!IMPORTANT]
>
>Zusätzlich zu den Elementen, die eine Arbeitszeittabelle gemäß den in diesem Artikel beschriebenen Bedingungen vorab ausfüllen, werden standardmäßig auch die folgenden Elemente auf Arbeitszeittabellen angezeigt:
>
>* Elemente, für die Sie die Zeit im Zeitrahmen der Arbeitszeittabelle protokolliert haben
>* Elemente, die an die Arbeitszeittabelle angeheftet sind
>* Elemente, nach denen Sie suchen und die Sie manuell zur Arbeitszeittabelle hinzufügen. Manuell hinzugefügte Elemente werden standardmäßig angeheftet.
>
>Weitere Informationen finden Sie unter [Zeit protokollieren](../../../timesheets/create-and-manage-timesheets/log-time.md) und [Arbeitszeittabellen-Übersicht](/help/quicksilver/timesheets/timesheets/timesheets-overview.md).

Alle Änderungen an Arbeitszeittabellen wirken sich auf alle Arbeitszeittabellen aus, die in der Zukunft erstellt werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL-Plan]</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeitszeittabelle und Stundeneinstellungen festlegen

{{step-1-to-setup}}

1. Klicken Sie **[!UICONTROL Arbeitszeittabelle und Stunden]** > **[!UICONTROL Voreinstellungen]**.

   Die Seite Arbeitszeittabellen und Stunden-Voreinstellungen wird angezeigt.

1. (Optional) Geben Sie **Suchfeld „Systemzeittabellen und**&quot; den Namen einer Gruppe ein und wählen Sie diese aus, wenn sie in der Liste angezeigt wird.

   ![Nach Gruppenfeld suchen](assets/search-for-group-box-in-timesheets-preferences-page.png)

   Die Seite mit den Arbeitszeittabellen- und Stundeneinstellungen wird mit den Einstellungen für die ausgewählte Gruppe aktualisiert. Voreinstellungen auf Systemebene müssen entsperrt werden, um Einstellungen auf Gruppenebene ändern zu können. Weitere Informationen finden Sie im Abschnitt [Entsperren von Arbeitszeittabellen und Stundeneinstellungen für Gruppen](#unlock-timesheet-and-hour-preferences-for-groups) in diesem Artikel.

1. Konfigurieren Sie **[!UICONTROL Abschnitt]** Allgemeine Voreinstellungen“ eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Protokollzeit für zukünftige Daten]</td> 
      <td> <p>Ermöglicht es Benutzenden, die Zeit für zukünftige Datumsangaben im gesamten System in folgenden Bereichen zu erfassen:</p> 
       <ul> 
        <li>Alle Projekte, Aufgaben und Probleme, bei denen sie Zugriff auf die Zeitprotokollierung haben</li> 
        <li>Ihre Arbeitszeittabellen als allgemeine Zeit</li> 
       </ul> <p>Dies ist nützlich, wenn Benutzer planen, nicht im Büro zu sein und diese Zeit im Voraus protokollieren möchten.</p> <p><b>HINWEIS</b>:</p> 
       <p>Sie können nicht verhindern, dass Benutzer Zeit für Aufgaben oder Probleme protokollieren, die geschlossen oder abgebrochen wurden. Sie können nur verhindern, dass Benutzer die Zeit bei abgeschlossenen oder inaktiven Projekten protokollieren. Es wird empfohlen, in Listen von Aufgaben und Problemen Filter zu verwenden, um abgeschlossene oder abgebrochene Aufgaben von der Sichtbarkeit für Benutzer auszuschließen.</p> </td> 
     </tr>

   <tr> 
      <td role="rowheader">[!UICONTROL Aufgabengebiete manuell Stundeneinträgen zuweisen]</td> 
      <td> <p>Benutzerinnen und Benutzern erlauben, manuell ein beliebiges Aufgabengebiet auszuwählen, das in ihrem Benutzerprofil oder dem Objekt zugewiesen ist.</p> <p><b>WICHTIG</b>:  
        <ul> 
         <li>Wenn Sie diese Einstellung deaktivieren, nachdem Sie Stundeneinträgen Aufgabengebiete zugewiesen haben, müssen Benutzer die Stunden anpassen, die unter verschiedenen Rollen in der Registerkarte [!UICONTROL Stunden] des Projekts, der Aufgabe oder des Problems protokolliert sind.</li> 
         <li>Wenn dem Benutzer in seinem Profil kein Aufgabengebiet zugewiesen ist und im Dialogfeld [!UICONTROL Erweiterte Zuweisungen] eine Aufgabe als [!UICONTROL Aufgabenbesitzer] zugewiesen ist, wird dieses Aufgabengebiet angezeigt, wenn der Benutzer die Zeit bei der Aufgabe protokolliert.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Bearbeitung von Arbeitszeittabellen auf Eigentümer und Administratoren beschränken]</td> 
      <td> <p>Bearbeitung auf Arbeitszeittabellen-Besitzer und [!DNL Workfront] beschränken. Wenn diese Option deaktiviert ist, können Arbeitszeittabellen auch wie folgt bearbeitet werden:</p> 
       <ul> 
        <li> <p>Benutzer mit administrativem Zugriff auf Arbeitszeittabellen und Stunden in ihrer Zugriffsebene</p> </li> 
        <li> <p>Arbeitszeittabellen-Genehmiger, wenn „Kann Stunden bearbeiten“ in der Arbeitszeittabelle aktiviert ist</p> </li> 
        <li> <p>Der Manager des Arbeitszeittabellen-Besitzers</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Stundenbearbeitung auf Eigentümer und Administratoren beschränken]</td> 
      <td>Bearbeitung auf die Benutzenden beschränken, die die Stunden eingeben, und Administratoren [!DNL Workfront]. Diese Einstellung gilt für die Registerkarte [!UICONTROL Stunden] in einem Projekt oder einem Stundenbericht.</td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurieren **[!UICONTROL im Abschnitt „Wo Benutzer die Zeit]** können“ eine der folgenden Optionen:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Direkt bei Projekten]</td>
        <td>Ermöglicht es den Benutzern, die Zeit für das Projekt zu protokollieren (sowohl auf der Registerkarte [!UICONTROL Updates] als auch in der Arbeitszeittabelle). Wenn Benutzer die Zeit nicht auf Projektebene erfassen, sollten diese Optionen deaktiviert bleiben.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Bei abgeschlossenen Projekten]</td>
        <td>Ermöglicht Benutzern das Aufzeichnen der Zeit für ein Projekt, das als abgeschlossen markiert wurde. Wenn diese Option deaktiviert ist, können Benutzer die Zeit nicht für die Arbeit aufzeichnen, die sie an Projekten mit dem Status [!UICONTROL Abgeschlossen] abgeschlossen haben.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Für eingestellte Projekte]</td>
        <td>Wenn diese Option aktiviert ist, können Benutzer Stunden in Projekten mit dem Status [!UICONTROL Dead] protokollieren.</td>
    </tr>
   </table>

1. Konfigurieren **[!UICONTROL im Abschnitt]** vorab ausfüllen eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Arbeit, die innerhalb von] &lt;Anzahl der Wochen&gt; [!UICONTROL des Arbeitsbereichs der Arbeitszeittabelle] liegt</td> 
      <td> <p>Definiert die Anzahl der Wochen vor und nach dem Datumsbereich der Arbeitszeittabelle, die dem Benutzer zugewiesene Daten von Aufgaben und Problemen enthält.</p> 
      <p>Die Standardeinstellung ist 1 Woche, und Sie können diesen Bereich auf 4 Wochen erweitern.</p> 
      <p>Das bedeutet, dass die Arbeitszeittabelle vorab mit Aufgaben und Problemen ausgefüllt wird, deren Termine zwischen vier Wochen vor dem Datumsbereich der Arbeitszeittabelle und bis zu vier Wochen nach dem Datumsbereich der Arbeitszeittabelle liegen, wenn Sie für Ihren Bereich 4 Wochen auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!Abgeschlossene UICONTROL-Aufgaben und -Probleme]</td> 
      <td>Wenn einer einzelnen Aufgabe normalerweise mehrere Ressourcen zugewiesen sind, empfehlen wir diese Einstellung. Wenn also eine Ressource die Zeit für einen Vorgang aufzeichnet und ihn als abgeschlossen markiert, können die anderen Ressourcen, die dem Vorgang zugewiesen sind, den Vorgang oder das Problem weiterhin in ihrer Arbeitszeittabelle finden, um ihre Stunden aufzuzeichnen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aufgaben und Probleme, für die im Datumsbereich der Arbeitszeittabelle geplante Termine liegen]</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält die Arbeitszeittabelle Aufgaben und Probleme, die entweder ein geplantes Startdatum oder ein Abschlussdatum haben, das in den Datumsbereich der Arbeitszeittabelle fällt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Aufgaben mit möglichen Terminen im Datumsbereich der Arbeitszeittabelle]</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält die Arbeitszeittabelle Aufgaben mit einem voraussichtlichen Start- oder Abschlussdatum, die innerhalb des Zeitrahmens des Projekts liegen, auch wenn das geplante Datum des Problems oder der Aufgabe außerhalb des Datumsbereichs der Arbeitszeittabelle liegt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Geben **[!UICONTROL im Abschnitt „Gelöschte Projekte, Aufgaben und]**&quot; Folgendes an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> Beim Löschen von Projekten</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Protokollierte Zeit beibehalten, die Arbeitszeittabellen bereits als allgemeine Zeit hinzugefügt wurde]</strong>: Wenn dieses Projekt zu einem späteren Zeitpunkt wiederhergestellt wird, verbleibt die Zeit in der Arbeitszeittabelle.</li> 
        <li><strong>[!UICONTROL Protokollierte Zeit löschen]</strong>: Wenn dieses Projekt zu einem späteren Zeitpunkt wiederhergestellt wird, wird bereits protokollierte Zeit im Projekt wiederhergestellt.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beim Löschen von Aufgaben oder Problemen</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Beliebige protokollierte Zeit in das Projekt verschieben]</strong> in dem sich die Aufgabe oder das Problem befindet: Wenn diese Aufgabe oder dieses Problem zu einem späteren Zeitpunkt wiederhergestellt wird, bleibt die Zeit im Projekt.<br></li> 
        <li> <p><strong>[!UICONTROL Protokollierte Zeit löschen]</strong>: Wenn diese Aufgabe oder dieses Problem zu einem späteren Zeitpunkt wiederhergestellt wird, wird protokollierte Zeit in der Aufgabe oder dem Problem wiederhergestellt.</p> <p>Detailliertere Informationen zu diesen Optionen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL configure impact] für Stunden, an denen ein Objekt gelöscht und wiederhergestellt wird</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Arbeitszeittabelle und Stundeneinstellungen für Gruppen entsperren

Gruppen in Ihrer Organisation benötigen möglicherweise Arbeitszeittabellen oder Stundeneinstellungen, die für ihre spezifischen Workflows anders konfiguriert sind. Sie können die Voreinstellungen für alle Gruppen im gesamten Unternehmen entsperren, damit sie sie selbst konfigurieren können.

Wenn eine Voreinstellung entsperrt wird und ein Gruppenadministrator sie ändert, wirkt sich dies auf Arbeitszeittabellen-Besitzer aus, wenn die Gruppe ihre Hauptgruppe ist.

Informationen zum Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen durch Gruppenadmins für eine Gruppe finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundeneinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Nachdem ein [!DNL Workfront] eine Voreinstellung auf Systemebene entsperrt hat, kann sie jeder Gruppenadministrator konfigurieren und dann sperren, um sicherzustellen, dass alle Benutzer in seiner Gruppe und den Untergruppen unten dieselbe Konfiguration verwenden. Dies geschieht parallel zu der Möglichkeit, dass ein [!DNL Workfront]-Administrator eine Voreinstellung für alle im System konfigurieren und sperren muss. Weitere Informationen finden Sie unter [Sperren oder Entsperren einer Gruppenarbeitszeittabelle und Stundenvoreinstellung](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

So entsperren Sie eine Projektvoreinstellung, damit Gruppen sie konfigurieren können:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **[!UICONTROL Arbeitszeittabellen und Stunden]** und dann auf **[!UICONTROL Voreinstellungen]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Gruppenadministratoren eine Voreinstellung für ihre Gruppen konfigurieren können, klicken Sie auf den Umschalter **Entsperren** (![-Umschalter](assets/unlock-toggle-button.png), um ihn zu entsperren .
   * Wenn Sie möchten, dass alle Gruppen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass es sich um einen gesperrten Umschalter handelt ![Voreinstellung gesperrt](assets/locked-preference-toggle.png) (dies ist die Standardeinstellung).

     >[!IMPORTANT]
     >
     >Es wird empfohlen, mit den Administratoren und Benutzern in Gruppen im gesamten System zu kommunizieren, um sicherzustellen, dass alle Anforderungen in der Art und Weise berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren.
     >
     >Wenn Sie ihn sperren, wird die entsprechende Konfiguration von allen Gruppen im System übernommen. Und wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Konfigurationen, die Gruppenadministratoren möglicherweise vorgenommen haben.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
