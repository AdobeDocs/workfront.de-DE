---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Zeitblatt- und Stundenvoreinstellungen konfigurieren
description: Als [!DNL Adobe Workfront] Administrator können Sie die Voreinstellungen für Timesheets und Stunden in [!DNL Workfront] um zu definieren, mit welchen Elementen die Timesheets vorbelegt werden können und zu welchen Elementen Benutzer die Zeit protokollieren können.
author: Courtney and Alina
feature: System Setup and Administration
role: Admin
exl-id: 8cc49dc2-b23f-4899-85dd-bd53d5242dbe
source-git-commit: 3b0a82381d1c33d897b123a597df21ba54cc2565
workflow-type: tm+mt
source-wordcount: '1310'
ht-degree: 1%

---

# Zeitblatt- und Stundenvoreinstellungen konfigurieren

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Als [!DNL Adobe Workfront] Administrator können Sie die Voreinstellungen für Timesheets und Stunden in [!DNL Workfront] um zu definieren, mit welchen Elementen die Timesheets vorbelegt werden können und zu welchen Elementen Benutzer die Zeit protokollieren können.

Alle Änderungen an Timesheets wirken sich auf alle in der Zukunft erstellten Timesheets aus.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator.</p> <p><b>NOTIZ</b>

Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
 </tbody> 
</table>

## Festlegen von Zeitblatt- und Stundenvoreinstellungen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken **[!UICONTROL Datenblatt und Stunden]** > **[!UICONTROL Voreinstellungen]**.

1. Auf der angezeigten Seite wird im **[!UICONTROL Allgemeine Voreinstellungen]** konfigurieren Sie eine der folgenden Optionen:

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
       </ul> <p>Dies ist nützlich, wenn Benutzer planen, außerhalb des Büros zu sein, und diese Zeit vorher protokollieren möchten.</p> <p><b>NOTE</b>: Sie können Benutzer nicht daran hindern, die Zeit für Aufgaben oder Probleme zu protokollieren, die geschlossen oder abgebrochen werden. Sie können Benutzer nur daran hindern, die Zeit für komplette oder tote Projekte zu protokollieren. Es wird empfohlen, Filter in Listen mit Aufgaben und Problemen zu verwenden, um auszuschließen, dass abgeschlossene oder abgebrochene Aufgaben für Benutzer nicht sichtbar sind.</p> </td> 
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
      <td role="rowheader">[!UICONTROL Einschränken der Bearbeitung von Zeitblättern auf Eigentümer und Administratoren]</td> 
      <td> <p>Beschränken Sie die Bearbeitung auf Timesheet-Eigentümer und [!DNL Workfront] Administratoren. Wenn diese Option deaktiviert ist, können Timesheets auch wie folgt bearbeitet werden:</p> 
       <ul> 
        <li> <p>Benutzer mit administrativem Zugriff auf Timesheets und Stunden in ihrer Zugriffsebene</p> </li> 
        <li> <p>Timesheet-Genehmiger, wenn auf dem Timesheet "Kann Stunden bearbeiten"aktiviert ist</p> </li> 
        <li> <p>Manager des Timesheet-Eigentümers</p> </li> 
       </ul> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Beschränkung der Stundenbearbeitung auf Inhaber und Administratoren]</td> 
      <td>Beschränken Sie die Bearbeitung auf den Benutzer, der die Stunden eingibt, und [!DNL Workfront] Administratoren. Diese Einstellung gilt für die Registerkarte [!UICONTROL Hours] in einem Projekt oder in einem Stundenbericht.</td> 
     </tr> 
    </tbody> 
   </table>

1. Im **[!UICONTROL Wo Benutzer die Zeit protokollieren können]** konfigurieren Sie eine der folgenden Optionen:

   <table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Direkte Projektprotokollierung]</td>
        <td>Ermöglicht Benutzern die Protokollierung der Zeit im Projekt (sowohl auf der Registerkarte [!UICONTROL Updates] als auch auf dem Timesheet). Wenn Benutzer keine Zeit auf Projektebene aufzeichnen, sollten diese Optionen deaktiviert bleiben.</td>
    </tr>
    <tr>
        <td>Zeit für abgeschlossene Projekte protokollieren</td>
        <td>Ermöglicht Benutzern das Aufzeichnen der Zeit für ein Projekt, das als abgeschlossen gekennzeichnet wurde. Wenn diese Option deaktiviert ist, können Benutzer die Zeit für die Arbeit, die sie an Projekten abgeschlossen haben, nicht im Status [!UICONTROL Abgeschlossen] aufzeichnen.</td>
    </tr>
    <tr>
        <td>Zeit für eingestellte Projekte protokollieren</td>
        <td>Wenn diese Option aktiviert ist, können Benutzer Stunden für Projekte mit dem Status [!UICONTROL Dead] protokollieren.</td>
    </tr>
   </table>

1. Im **[!UICONTROL Vorfüllen von Zeitleisten]** konfigurieren Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Arbeit, die sich innerhalb von befindet] &lt;number of="" weeks=""&gt; [!UICONTROL des Arbeitsbereichs des Zeitplans]</td> 
      <td> <p>Definiert die Anzahl der Wochen vor und nach dem Datumsbereich des Zeitblatts, das Datum der dem Benutzer zugewiesenen Aufgaben und Probleme enthält. Die Standardeinstellung ist 1 Woche, und Sie können diesen Bereich auf 4 Wochen erweitern. Das bedeutet, dass das Timesheet mit Aufgaben und Problemen vorausgefüllt ist, die zwischen vier Wochen vor dem Datumsbereich des Zeitblatts und bis zu vier Wochen nach dem Datumsbereich des Zeitblatts liegen, wenn Sie für Ihren Bereich vier Wochen auswählen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aufgaben und Probleme, die abgeschlossen wurden]</td> 
      <td>Wenn normalerweise mehrere Ressourcen einer einzelnen Aufgabe zugewiesen sind, empfehlen wir diese Einstellung. Das bedeutet, dass die anderen Ressourcen, die der Aufgabe zugewiesen sind, die Aufgabe bzw. das Problem in ihrem Timesheet finden können, um ihre Stunden aufzuzeichnen, wenn eine Ressource die Zeit für die Aufgabe aufzeichnet und sie als abgeschlossen kennzeichnet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Aufgaben und Probleme, bei denen im Datumsbereich des Datenblatts die geplanten Daten eingetragen sind]</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält das Timesheet Aufgaben und Probleme mit einem geplanten Startdatum oder einem geplanten Abschlussdatum, das in den Datumsbereich des Zeitblatts fällt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> [!UICONTROL Aufgaben, bei denen im Datumsbereich des Datenblatts die geplanten Daten angegeben sind]</td> 
      <td> <p>Wenn diese Option aktiviert ist, enthält das Timesheet Aufgaben mit einem geplanten Startdatum oder Abschlussdatum, die innerhalb des Zeitrahmens des Projekts liegen, selbst wenn das geplante Datum des Problems oder der Aufgabe außerhalb des Zeitblatt-Datumsbereichs liegt.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Im **[!UICONTROL Gelöschte Projekte, Aufgaben und Probleme]** geben Sie Folgendes an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beim Löschen von Projekten]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Behalten Sie die bereits zu Timesheets hinzugefügte protokollierte Zeit als allgemeine Zeit bei.]</strong>: Wenn dieses Projekt zu einem späteren Zeitpunkt wiederhergestellt wird, verbleibt die Zeit auf dem Timesheet.</li> 
        <li><strong>[!UICONTROL Beliebige Zeit löschen]</strong>: Wenn dieses Projekt später wiederhergestellt wird, wird die bereits protokollierte Zeit für das Projekt wiederhergestellt.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Beim Löschen von Aufgaben oder Problemen]</td> 
      <td> 
       <ul> 
        <li><strong>[!UICONTROL Verschieben einer beliebigen protokollierten Zeit in das Projekt, in dem sich die Aufgabe oder das Problem befindet]</strong>: Wenn diese Aufgabe oder dieses Problem später wiederhergestellt wird, bleibt die Zeit im Projekt.<br></li> 
        <li> <p><strong>[!UICONTROL Beliebige Zeit löschen]</strong>: Wenn diese Aufgabe oder dieses Problem später wiederhergestellt wird, wird die protokollierte Zeit für die Aufgabe oder das Problem wiederhergestellt.</p> <p>Weitere Informationen zu diesen Optionen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/manage-deleted-items/configure-how-hours-affected-when-obj-deleted-restored.md" class="MCXref xref">[!UICONTROL Konfigurationseffekt] für Stunden, in denen ein Objekt gelöscht und wiederhergestellt wird</a>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

## Zeitblatt- und Stundenvoreinstellungen für Gruppen entsperren

Gruppen in Ihrer Organisation benötigen möglicherweise ein Timesheet oder eine andere Stundenvoreinstellung, die für ihre individuellen Workflows unterschiedlich konfiguriert ist. Sie können die Voreinstellung für alle Gruppen in der Organisation freigeben, damit sie sie selbst konfigurieren können.

Wenn eine Voreinstellung entsperrt ist und ein Gruppenadministrator sie ändert, wirkt sich dies auf die Inhaber von Zeitblättern aus, wenn es sich bei der Gruppe um ihre Startseite handelt.

Informationen dazu, wie ein Gruppenadministrator die Voreinstellungen für das Arbeitsblatt und die Stunde für eine Gruppe konfiguriert, finden Sie unter [Konfigurieren von Zeitblatt- und Stundeneinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

>[!NOTE]
>
>Nach [!DNL Workfront] Administrator entsperrt eine Voreinstellung auf Systemebene, kann jeder Gruppenadministrator sie konfigurieren und dann sperren, um sicherzustellen, dass alle Mitglieder ihrer Gruppe und der Untergruppen unten dieselbe Konfiguration verwenden. Dies entspricht der Fähigkeit, dass ein [!DNL Workfront] -Administrator muss eine Voreinstellung für alle Benutzer im System konfigurieren und sperren. Weitere Informationen finden Sie unter [Voreinstellung für Zeitblatt und Stunde einer Gruppe sperren oder entsperren](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-timesheet-hour-preference.md).

So entsperren Sie eine Projektvoreinstellung, damit Gruppen sie konfigurieren können:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe] Workfront, und klicken Sie dann auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **[!UICONTROL Timesheets und Stunden]** Klicken Sie auf **[!UICONTROL Voreinstellungen]**.

1. Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie möchten, dass Gruppenadministratoren eine Voreinstellung für ihre Gruppen konfigurieren können, entsperren Sie sie. ![](assets/unlock-toggle-button.png).
   * Wenn Sie möchten, dass alle Gruppen Ihre Konfiguration für eine Voreinstellung verwenden, stellen Sie sicher, dass sie gesperrt ist (dies ist die Standardeinstellung).

      >[!IMPORTANT]
      >
      >Es wird empfohlen, mit den Administratoren und Benutzern in Gruppen im gesamten System zu kommunizieren, um sicherzustellen, dass alle Anforderungen so berücksichtigt werden, wie Sie eine gesperrte Voreinstellung konfigurieren. Wenn Sie sie sperren, wird Ihre Konfiguration für sie von allen Gruppen im System übernommen. Wenn die Voreinstellung für einen beliebigen Zeitraum entsperrt wurde, ersetzt Ihre Konfiguration die Einstellungen, die von Gruppenadministratoren vorgenommen wurden.

1. Klicken Sie auf **[!UICONTROL Speichern]**.
