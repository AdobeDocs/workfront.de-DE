---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: Massenbearbeitung von Benutzerprofilen
description: Als Adobe Workfront-Administrator können Sie Benutzerkonten stapelweise bearbeiten.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cb709b2f-659e-4110-81ac-a1ef967d534c
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '2212'
ht-degree: 0%

---

# Massenbearbeitung von Benutzerprofilen

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
-->

Sie können Benutzerkonten stapelweise bearbeiten. Bei der Massenbearbeitung werden nur die Felder, die Sie auswählen, mit denselben Informationen für alle ausgewählten Benutzer aktualisiert. Alle anderen Felder, die Sie nicht ausgewählt lassen, bleiben für jeden einzelnen Benutzer gleich, auch wenn sie für jeden Benutzer unterschiedlich sind.

>[!NOTE]
>
>* Sie können den Abschnitt „Persönliche Informationen“ der Benutzerprofile nicht stapelweise bearbeiten, da diese Informationen für jeden Benutzer eindeutig sein müssen.
>* Um die Genauigkeit der Daten und eine optimale Leistung zu gewährleisten, empfehlen wir, nicht mehr als 2.000 Benutzer gleichzeitig für eine Massenbearbeitung auszuwählen.
>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p><p>Oder</p><p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. </li> 
     <li> <p><b>Benutzer</b> Einstellung in Ihrer Zugriffsebene konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens einer der beiden <b>Benutzeradmin</b> Optionen unter <b>Optimieren Sie Ihre Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn diese beiden Optionen <b>Benutzeradministrator (Gruppenbenutzer)) aktiviert </b>, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Massenbearbeitung von Benutzerkonten

{{step-1-to-users}}

1. Wählen Sie mehrere Benutzer aus und klicken Sie dann auf das Symbol Bearbeiten ![Symbol Bearbeiten](assets/edit-icon.png).

1. Ändern Sie **angezeigten** „Benutzer bearbeiten“ eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Einstellungen</td> 
      <td> 
       <ul> 
        <li><b>Zeitzone:</b> Die Zeitzone der Benutzer.</li> 
        <li><b>Locale</b>: Das bevorzugte Gebietsschema der Benutzer. Dies wirkt sich auf das Format der Zahlen und Daten in den E-Mails aus, die von Workfront stammen.</li> 
        <li><b>Arbeit, die ich mir selbst zuweise, an meine Registerkarte „Arbeiten an“ senden</b>: Diese Einstellung bezieht sich auf eine veraltete Funktion, die aus Workfront entfernt wurde.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benachrichtigungen</td> 
      <td>Wählen Sie die E-Mail-Benachrichtigungen aus, die für den neuen Benutzer aktiviert werden sollen.<p>Sie können sowohl sofortige als auch tägliche Digest-Benachrichtigungen auswählen. Alle täglichen Digest-Benachrichtigungen werden für alle ausgewählten Benutzer irgendwann nach der gleichen Zeit zugestellt. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zugriff</td> 
      <td> 
       <ul> 
        <li><b>Ist Aktiv</b> Wählen Sie dieses Feld aus, um anzugeben, ob die Benutzer aktiv sind. Aktive Benutzende verwenden eine Workfront-Lizenz. Durch Deaktivieren des Felds werden die Benutzer deaktiviert.</li> 
        <li> 
        <p><b>Zugriffsebene:</b> Wählen Sie die Zugriffsebene aus, die Sie diesen Benutzern zuweisen möchten. Alle ausgewählten Benutzer haben dieselbe Zugriffsebene.
        </p> 
        <p>Wenn Sie Benutzenden eine Zugriffsebene zuweisen, können Sie eine Zugriffsebene zuweisen, die gleich oder kleiner als Ihre eigene Zugriffsebene ist. (Wenn Ihre Zugriffsebene beispielsweise „Planer“ ist, können Sie keine Administratorzugriffsebene zuweisen.) </p>
        <p>Sie können jedoch keine Zugriffsebene zuweisen, die niedriger ist als Ihre eigene, wenn der Workfront-Administrator Berechtigungen auf der Zugriffsebene aktiviert hat, die nicht auch in Ihren eigenen aktiviert sind (über die Feinabstimmungseinstellungen, wie in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern von benutzerdefinierten Zugriffsebenen</a> beschrieben).</p> 
        <p>Weitere Informationen zu Zugriffsebenen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Zugriff auf Adobe Workfront konfigurieren</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout-Vorlage</b>: Wählen Sie eine Layout-Vorlage für die Benutzer. Die den Benutzern zugewiesene Layout-Vorlage hat Vorrang vor jeder Layout-Vorlage, die ihrer Hauptgruppe, ihrem Home-Team oder ihrem primären Aufgabengebiet zugewiesen ist. Weitere Informationen zur Zuweisungspriorität der Layout-Vorlage finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layout-Vorlagen</a>.</p> 
        <p><b>HINWEIS</b>: Die Liste der Layout-Vorlagen, die in diesem Feld verfügbar sind, hängt von Ihrem Zugriff ab:
          <ul>
           <li>Als Workfront-Administrator können Sie alle Layoutvorlagen auf Systemebene und Gruppenebene sehen.</li>
           <li>Als Gruppenadministrator bzw. -administratorin können Sie Layoutvorlagen auf Systemebene sowie die Vorlagen sehen, die mit den von Ihnen verwalteten Gruppen verknüpft sind.</li>
           <li><p>Benutzende mit einer Planner-Lizenz und Zugriff auf die Bearbeitung von Benutzenden können nur Layoutvorlagen auf Systemebene sehen. </p>
           <p>Weitere Informationen zu Layout-Vorlagen auf Gruppenebene finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layout-Vorlagen</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation</td> 
      <td> 
       <ul> 
        <li><b>Unternehmen</b>: Das Unternehmen der Benutzer. Benutzende können nur mit einer Firma verknüpft werden. Sie müssen eine Firma erstellen, bevor Sie sie mit einem Benutzer verknüpfen können. In der Liste werden nur aktive Unternehmen angezeigt. Informationen zum Erstellen von Unternehmen finden Sie unter Grundlagen und Verwalten von Unternehmen .</li> 
        <li><b>Home-</b>: Geben Sie das Home-Team für die Benutzer an. Benutzer können nur über ein Home-Team verfügen. </li> 
        <li><b>Andere Teams</b>: Benutzer können mehreren Teams angehören. </li> 
        <li> <p><b>Hauptgruppe: </b> Sie eine geeignete Gruppe aus, um die Benutzer ihrer Hauptgruppe zuzuweisen. Dadurch kann der Benutzer auf Objekte zugreifen, die für die Gruppe freigegeben sind.</p> <p><b>HINWEIS</b>: Dies ist ein Pflichtfeld. Es können keine Benutzer einer Hauptgruppe zugeordnet sein.</p> <p>Eine Gruppe kann Benutzenden nur in den folgenden Situationen zugewiesen werden:</p> 
         <ul> 
          <li>Sie sind ein Workfront-Administrator.</li> 
          <li>Sie sind der Administrator dieser Gruppe.</li> 
          <li>Die Gruppe ist öffentlich.</li> 
         </ul> </li> 
        <li> <p><b>Andere Gruppen</b>: Benutzer können mehreren Gruppen angehören. Eine Gruppe kann einem Benutzer nur in den folgenden Situationen zugewiesen werden:</p> 
         <ul> 
          <li>Sie sind ein Workfront-Administrator.</li> 
          <li>Sie sind der Administrator dieser Gruppe.</li> 
          <li> <p>Die Gruppe ist öffentlich. </p> 
          <p>Weitere Informationen zu öffentlichen Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Erstellen einer Gruppe</a>.</p> 
          <p>Weitere Informationen zu Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppen - Übersicht</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ressourcenplanung</td> 
      <td> 
       <ul>

   <li>
       <b>Arbeitszeit</b>: Gibt den Prozentsatz der Vollzeitäquivalenzzeit (VZÄ) an, die der Benutzer für die tatsächliche Arbeit zur Verfügung hat, ohne Gemeinkosten. Arbeitszeit muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. So würde beispielsweise eine Verfügbarkeit von 20 % für die tatsächliche Arbeit 0,2 betragen.

   Der Standardwert des Feldes ist 1. Dies bedeutet, dass ein Benutzer sein gesamtes FTE für die tatsächliche, projektbezogene Arbeit verwendet.

   Anhand dieser Zahl berechnet das System die Verfügbarkeit des Nutzers für die tatsächliche, projektbezogene Arbeit.

   Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>.

   Zeitplanausnahmen und Ausfallzeiten können sich auch auf die Benutzerkapazität auswirken.

   Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich. Weitere Informationen finden Sie unter <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.

   <b>TIPP</b>

   Legen Sie den Wert für Arbeitszeit auf 1 fest, um anzugeben, dass der Benutzer für projektbezogene Arbeit bis zum gesamten Vollzeitäquivalent verfügbar ist.
   </li>

   <li><b>Deaktivierung planen</b>: Aktivieren Sie dieses Kontrollkästchen, um festzulegen, dass Benutzer nach einem bestimmten Zeitraum deaktiviert werden sollen.</li> 
       <li><b>Geplantes Deaktivierungsdatum</b>: Das Datum, nach dem die Benutzer deaktiviert werden. Weitere Informationen zum Planen von Benutzern für die Deaktivierung finden Sie im Abschnitt <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planen von Benutzern für die Deaktivierung</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deaktivieren oder Reaktivieren von </a>.</li> 
       <li> <p><b>Primäre Rolle</b>: Dies ist das primäre Aufgabengebiet, das eine Benutzerin oder ein Benutzer in Workfront hat. Alle Aufgaben und Probleme, denen die Benutzer zugewiesen sind, sind standardmäßig auch diesem Aufgabengebiet zugewiesen. Aufgabengebiete sind im Ressourcen-Management von entscheidender Bedeutung. Weitere Informationen zu Aufgabengebieten finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a></p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planlizenz mit administrativem Benutzerzugriff verfügen oder wenn Sie ein Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit administrativem Benutzerzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </li> 
       <li>(Bedingt) Wenn Sie eine <b>Primäre Rolle ausgewählt haben</b> wird das Feld <b>Prozentsatz der FTE-Verfügbarkeit</b> angezeigt. Geben Sie an, wie viel Prozent der Zeit in den Zeitplänen der Benutzer diesem Aufgabengebiet zugewiesen sind. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die Primäre Funktion ist 100 %.</li> 
       <li> <p><b>Andere Rollen</b>: Benutzer können in Workfront über mehrere Aufgabengebiete verfügen. Aufgabengebiete sind im Ressourcen-Management von entscheidender Bedeutung. Es gibt keine Begrenzung dafür, wie viele Aufgabengebiete ein Benutzer erfüllen kann. Wir empfehlen jedoch, einer zu großen Anzahl von Aufgabengebieten nicht einen Benutzer zuzuweisen, da die Ressourcenverwaltung für diese Benutzer möglicherweise zu komplex wird.</p> <p>Weitere Informationen zu Aufgabengebieten finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Aufgabengebieten</a>.</p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planlizenz mit administrativem Benutzerzugriff verfügen oder wenn Sie ein Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit administrativem Benutzerzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </li> 
       <li> <p>(Bedingt) Wenn Sie eine oder mehrere Rollen <b>Sonstige Rollen</b> ausgewählt haben, wird für </b> jeweilige Rolle das Feld <b>Prozentsatz der FTE-Verfügbarkeit“ angezeigt. Geben Sie an, welcher Prozentsatz der Zeit in den Zeitplänen der Benutzer den einzelnen Aufgabengebieten zugewiesen ist. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die anderen Funktionen ist 0 %.</p> <p><b>HINWEIS</b>:  
       <ul> 
       <li>Wenn für andere Funktionen eine FTE-Verfügbarkeit von 0 % verfügbar ist, werden sie nicht im Ressourcenplaner angezeigt, es sei denn, die Benutzer sind Aufgaben in diesen Rollen zugewiesen.</li> 
       <li> <p>Die Summe aller Prozentsätze der FTE-Verfügbarkeit für alle Funktionen muss 100 % betragen. Jeder Prozentsatz der FTE-Verfügbarkeit berechnet die verfügbaren Stunden für jede Rolle pro Benutzer im Ressourcenplaner. Die verfügbaren Stunden für jede Rolle pro Benutzer hängen von der verfügbaren Zeit für den Benutzer ab.</p> <p>Die verfügbare Zeit für den Benutzer wird von Workfront abhängig von der Methode berechnet, die vom Workfront-Administrator zur Berechnung des FTE in den Voreinstellungen für das Ressourcenmanagement ausgewählt wurde.</p> <p>Weitere Informationen zur Berechnung der Verfügbarkeit für den Benutzer finden Sie unter <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung von Stunden und VZÄ für Benutzer und Funktionen im Ressourcenplaner</a>.</p> <p>Weitere Informationen zum Konfigurieren der Voreinstellungen für das Ressourcen-Management finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurieren der Voreinstellungen für das Ressourcen-Management</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Zeitplan</b>: Ordnen Sie den Benutzern einen Zeitplan zu. Der Zeitplan der Benutzer berechnet die Zeitleiste der Aufgaben, denen die Benutzer zugewiesen sind.</p> <p>Ein Workfront-Administrator oder ein Gruppenadministrator muss einen Zeitplan erstellen, bevor er mit Benutzenden verknüpft werden kann.</p> <p>Wählen Sie einen Zeitplan auf Systemebene oder eine Gruppierung aus, um ihn den ausgewählten Benutzern zuzuweisen.</p> <p>Weitere Informationen zu Zeitplänen für das System und Gruppen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Erstellen eines Zeitplans</a>.</p> <p><b>WICHTIG</b>: Workfront verwendet den Zeitplan eines Benutzers nur, wenn die Einstellung Ressourcenverfügbarkeit mithilfe von berechnen auf den Zeitplan des Benutzers festgelegt ist. Weitere Informationen dazu, wie sich die Einstellung Ressourcenverfügbarkeit mithilfe von berechnen auf den für die Ressourcenverwaltung verwendeten Zeitplan auswirkt, finden Sie <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Konfigurieren der Voreinstellungen für die Ressourcenverwaltung</a>.</p> </li> 
       <li> <p><b>Arbeitszeittabellen-Profil</b>: Ordnen Sie den Benutzern ein Arbeitszeittabellen-Profil zu. Dadurch wird sichergestellt, dass Arbeitszeittabellen automatisch für die Benutzer generiert werden.</p> 
       <p><b>HINWEIS</b>:  
       <ul> 
       <li>Die Liste der Arbeitszeittabellen-Profile, die in diesem Feld verfügbar sind, hängt von Ihrem Zugriff ab:
       <ul>
       <li>Als Workfront-Administrator können Sie alle Arbeitszeittabellen-Profile auf Systemebene und Gruppenebene anzeigen.</li>
       <li><p>Als Gruppenadministrator können Sie Arbeitszeittabellen-Profile auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Profile anzeigen.</p></li>
       <li><p>Benutzende mit einer Planner-Lizenz und Zugriff auf die Bearbeitung von Benutzenden können nur Arbeitszeittabellen-Profile auf Systemebene anzeigen.</p></li>
       </ul></li> 
       <li>Wenn Sie Gruppenadministrator sind, müssen alle Benutzer, die Sie bearbeiten, Mitglieder einer Gruppe sein, die Sie verwalten.</li> 
       </ul> </p> </li> 
       <li><b>Standardstundentyp</b>: Wählen Sie den Standardstundentyp für die Benutzer aus. Dies ist der Stundentyp, der standardmäßig verwendet wird, wenn Benutzer die Zeit erfassen.</li> 
       <li> <p><b>Verfügbare Stundentypen</b>: Wählen Sie die Stundentypen aus, die für den Benutzer verfügbar sein sollen. Diese Stundentypen sind überall in Workfront sichtbar, wo Benutzende die Zeit protokollieren können. Ein Benutzer kann nur die Stundentypen sehen, die sowohl auf Projekt- als auch auf Benutzerebene aktiviert sind.</p> 
       <p>Weitere Informationen dazu, welche Stundentypen Benutzern zur Verfügung stehen, finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Festlegen von Stundentypen und Verfügbarkeit</a>.</p> 
       </li> 
       <li> <b>FTE</b>: Dies ist das Vollzeitäquivalent des Benutzers. Workfront verwendet diese Zahl, um die Verfügbarkeit der Benutzerin bzw. des Benutzers auf der Grundlage des Standardzeitplans nur dann zu berechnen, wenn die Ressourcenverwaltungseinstellungen auf Systemebene auf den Standardzeitplan eingestellt sind.

   <p>Das FTE gibt an, wie viel Zeit der Benutzer bei der Arbeit verbringen kann. Dazu gehören Gemeinkosten sowie die Zeit, die mit der Projektarbeit verbracht wird. Beispielsweise wird die Zeit, die in Meetings oder Schulungen verbracht wird, ebenfalls in das VZÄ einbezogen.</p>

   Der FTE muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. Wenn beispielsweise der FTE-Wert 0,5 beträgt und der Standardzeitplan in Workfront 40 Stunden beträgt, ist die Benutzerin bzw. der Benutzer 20 Stunden pro Woche verfügbar.

   Der Standardwert des Felds ist 1.

   Zeitplanausnahmen, Ausfallzeiten und der Wert der Arbeitszeit können sich auf die Verfügbarkeit der Benutzenden auswirken.

   Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich.

   Wenn die Voreinstellungen für das Ressourcen-Management auf Systemebene auf den Zeitplan des Benutzers festgelegt sind, wird der hier angegebene Wert ignoriert und der Benutzer wird gemäß den Angaben in seinem Zeitplan als verfügbar betrachtet.

   Weitere Informationen finden Sie unter <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.

   Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Erstellen eines Zeitplans</a>.
   </li> 
       <li> <p><b>Ressourcenpools</b>: Verknüpfen Sie die Benutzer mit Ressourcenpools.</p> <p><b>HINWEIS</b>: In diesem Feld werden nur die Ressourcenpools angezeigt, die allen ausgewählten Benutzern gemeinsam sind. Wenn die ausgewählten Benutzer keine freigegebenen Ressourcenpools haben, ist dieses Feld leer. Wenn dieses Feld leer ist, überschreiben die hier angegebenen Ressourcenpools ihre einzelnen Ressourcenpools.</p> 
       <p>Weitere Informationen zu Ressourcenpools finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Ressourcenpools - Übersicht </a>.</p> </li> 
       <li><b>Kosten pro Stunde</b>: Der Betrag der Kosten pro Stunde für den Benutzer. </li> 
       <li><b>Abrechnung pro Stunde</b>: Der Abrechnungsbetrag pro Stunde für den Benutzer.</li> 
       <li><b>Benutzerdefinierte Forms</b>: Verknüpfen Sie die Benutzer mit einem vorhandenen benutzerdefinierten Benutzerformular. Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Erstellen eines benutzerdefinierten Formulars</a>.</li> 
       <li><b>Kommentar</b>: Geben Sie einen Kommentar in das bereitgestellte Feld ein. Alle ausgewählten Benutzer erhalten eine In-App-Benachrichtigung sowie eine E-Mail-Benachrichtigung mit Ihrem Kommentar. Der Kommentar wird auf der Registerkarte Aktualisierungen des Benutzerprofils angezeigt.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wählen Sie im Abschnitt **Benutzerdefinierte Forms** die Option **Benutzerdefinierte Ausdrücke neu berechnen** aus, um sicherzustellen, dass alle berechneten benutzerdefinierten Felder in benutzerdefinierten Formularen, die an die ausgewählten Benutzenden angehängt sind, auf dem neuesten Stand sind.

1. Klicken Sie auf **Änderungen speichern**.
