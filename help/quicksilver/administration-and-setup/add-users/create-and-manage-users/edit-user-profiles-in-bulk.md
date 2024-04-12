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
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '2247'
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

Sie können Benutzerkonten stapelweise bearbeiten. Bei der Massenbearbeitung von Benutzern werden nur die Felder, die Sie spezifisch auswählen, mit den gleichen Informationen für alle ausgewählten Benutzer aktualisiert. Alle anderen Felder, die Sie nicht ausgewählt lassen, bleiben für jeden einzelnen Benutzer gleich, auch wenn sie für jeden Benutzer unterschiedlich sind.

>[!NOTE]
>
>* Sie können den Abschnitt &quot;Persönliche Informationen&quot;der Benutzerprofile nicht stapelweise bearbeiten, da diese Informationen für jeden Benutzer eindeutig sein müssen.
>* Um Genauigkeit der Daten und optimale Leistung zu gewährleisten, empfehlen wir, maximal 2000 Benutzer gleichzeitig für eine Massenbearbeitung auszuwählen.
>

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsebene des Systemadministrators. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p><b>Benutzer</b> -Einstellung in Ihrer Zugriffsstufe konfiguriert auf <b>Bearbeiten</b> Zugriff, mit <b>Erstellen</b> und mindestens eines der beiden <b>Benutzeradministrator</b> Optionen aktiviert unter <b>Optimieren Ihrer Einstellungen</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Wenn Benutzer <b>Admin (Gruppenbenutzer)</b> aktiviert ist, müssen Sie ein Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</p> <p>Weitere Informationen zum <b>Benutzer</b> auf einer Zugriffsebene festzulegen, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Stapelweises Bearbeiten von Benutzerkonten

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Benutzer** ![](assets/users-icon-in-main-menu.png).

1. Wählen Sie mehr als einen Benutzer aus und klicken Sie dann auf das Symbol Bearbeiten . ![](assets/edit-icon.png).

1. Im **Benutzer bearbeiten** ändern Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Einstellungen</td> 
      <td> 
       <ul> 
        <li><b>Zeitzone:</b> Die Zeitzone des Benutzers.</li> 
        <li><b>Gebietsschema</b>: Das bevorzugte Gebietsschema der Benutzer. Dies wirkt sich auf das Zahlenformat und das Datumsformat der aus Workfront stammenden E-Mails aus.</li> 
        <li><b>Versand der Arbeit, die ich mir auf die Registerkarte "Arbeit an"zuweise</b>: Aktivieren Sie diese Option, wenn alles, was die Benutzer sich selbst zuweisen, direkt auf ihrer Registerkarte "Arbeiten am"angezeigt werden soll. Standardmäßig werden alle einem Benutzer zugewiesenen Elemente auf der Registerkarte "Arbeitsanforderung"aufgelistet.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benachrichtigungen</td> 
      <td>Wählen Sie die E-Mail-Benachrichtigungen aus, die für den neuen Benutzer aktiviert werden sollen.<p>Sie können sowohl die sofortige als auch die tägliche Digest-Benachrichtigung auswählen. Alle täglichen Digest-Benachrichtigungen werden für alle ausgewählten Benutzer nach derselben Zeit bereitgestellt. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zugriff</td> 
      <td> 
       <ul> 
        <li><b>Ist aktiv:</b> Wählen Sie dieses Feld aus, um anzugeben, ob die Benutzer aktiv sind. Aktive Benutzer verwenden eine Workfront-Lizenz. Wenn Sie das Feld deaktivieren, werden die Benutzer deaktiviert.</li> 
        <li> 
        <p><b>Zugriffsebene:</b> Wählen Sie die Zugriffsebene aus, die diesen Benutzern zugewiesen werden soll. Alle ausgewählten Benutzer haben dieselbe Zugriffsstufe.
        </p> 
        <p>Wenn Sie Benutzern eine Zugriffsebene zuweisen, können Sie eine Ebene zuweisen, die Ihrer eigenen Zugriffsebene entspricht oder darunter liegt. (Wenn Ihre Zugriffsebene beispielsweise "Planer"lautet, können Sie die Zugriffsebene "Administrator"nicht zuweisen.) </p>
        <p>Sie können jedoch keine Zugriffsstufe zuweisen, die kleiner als Ihre ist, wenn der Workfront-Administrator Berechtigungen für die Zugriffsstufe aktiviert hat, die nicht auch in Ihrer eigenen aktiviert sind (über die Einstellungen für die Feinabstimmung, wie hier beschrieben: <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>).</p> 
        <p>Weitere Informationen zu Zugriffsebenen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Zugriff auf Adobe Workfront konfigurieren</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout-Vorlage</b>: Wählen Sie eine Layoutvorlage für die Benutzer aus. Die den Benutzern zugewiesene Layoutvorlage hat Vorrang vor allen Layoutvorlagen, die ihrer Startseite, Startseite oder Hauptauftragsrolle zugewiesen sind. Weitere Informationen zur Zuweisungspriorität von Layoutvorlagen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layoutvorlagen</a>.</p> 
        <p><b>NOTE</b>: Die Liste der in diesem Feld verfügbaren Layoutvorlagen hängt von Ihrem Zugriff ab:
          <ul>
           <li>Als Workfront-Administrator können Sie alle Layoutvorlagen auf System- und Gruppenebene sehen.</li>
           <li>Als Gruppenadministrator können Sie Layout-Vorlagen auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Vorlagen sehen.</li>
           <li><p>Als Benutzer mit einer Planner-Lizenz und Zugriff zur Bearbeitung von Benutzern können Sie nur Layoutvorlagen auf Systemebene sehen. </p>
           <p>Weitere Informationen zu Layout-Vorlagen auf Gruppenebene finden Sie unter <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Erstellen und Verwalten von Layoutvorlagen</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organisation</td> 
      <td> 
       <ul> 
        <li><b>Firma</b>: Das Unternehmen der Benutzer. Benutzer können nur mit einem Unternehmen verknüpft werden. Sie müssen ein Unternehmen erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive Unternehmen angezeigt. Informationen zum Erstellen von Unternehmen finden Sie unter Verstehen und Verwalten von Unternehmen.</li> 
        <li><b>Startseite</b>: Geben Sie das Startseiten-Team für die Benutzer an. Benutzer können nur ein Home-Team haben. </li> 
        <li><b>Sonstige Teams</b>: Benutzer können mehreren Teams angehören. </li> 
        <li> <p><b>Startseite:</b> Wählen Sie eine entsprechende Gruppe aus, um die Benutzer als ihre Startseite zuzuweisen. Dadurch erhält der Benutzer die Möglichkeit, auf Objekte zuzugreifen, die für die Gruppe freigegeben sind.</p> <p><b>NOTE</b>: Dies ist ein erforderliches Feld. Benutzer, die keiner Startseite zugeordnet sind, können nicht hinzugefügt werden.</p> <p>Sie können Benutzern eine Gruppe nur in den folgenden Situationen zuweisen:</p> 
         <ul> 
          <li>Sie sind Workfront-Administrator.</li> 
          <li>Sie sind der Administrator dieser Gruppe.</li> 
          <li>Die Gruppe ist öffentlich.</li> 
         </ul> </li> 
        <li> <p><b>Andere Gruppen</b>: Benutzer können mehreren Gruppen angehören. Sie können einem Benutzer eine Gruppe nur in den folgenden Situationen zuweisen:</p> 
         <ul> 
          <li>Sie sind Workfront-Administrator.</li> 
          <li>Sie sind der Administrator dieser Gruppe.</li> 
          <li> <p>Die Gruppe ist öffentlich. </p> 
          <p>Weitere Informationen zu öffentlichen Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Gruppe erstellen</a>.</p> 
          <p>Weitere Informationen zu Gruppen finden Sie unter <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Gruppenübersicht</a>.</p> 
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
       <b>Arbeitszeit</b>: Stellt den Prozentsatz der Vollzeitäquivalenzzeit (FTE) dar, zu dem der Benutzer für die tatsächliche Arbeit verfügbar ist, ohne dass der Overhead eingeschlossen ist. Die Arbeitszeit muss eine Dezimalzahl von bis zu 1 sein, und sie darf nicht 0 sein. Eine Verfügbarkeit von 20 % für tatsächliche Arbeit wäre beispielsweise 0,2.

   Der Standardwert des Felds ist 1, was bedeutet, dass ein Benutzer seine gesamte FTE für tatsächliche, projektbezogene Arbeiten ausgibt.

   Das System verwendet diese Zahl, um die Verfügbarkeit des Benutzers für tatsächliche, projektbezogene Arbeiten zu berechnen.

   Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Zeitplan erstellen</a>.

   Eine Planung von Ausnahmen und Zeitüberschreitungen kann sich auch auf die Benutzerkapazität auswirken.

   Workfront berechnet die Verfügbarkeit eines Benutzers entsprechend den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich. Weitere Informationen finden Sie unter <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.

   <b>TIPP</b>

   Setzen Sie den Wert für die Arbeitszeit auf 1, um anzugeben, dass der Benutzer für projektbezogene Arbeiten in seiner gesamten Vollzeitäquivalenz verfügbar ist.
   </li>

   <li><b>Deaktivierung planen</b>: Aktivieren Sie dieses Kontrollkästchen, wenn Sie planen möchten, dass Benutzer nach einem bestimmten Zeitraum deaktiviert werden.</li> 
       <li><b>Geplantes Deaktivierungsdatum</b>: Das Datum, nach dem die Benutzer deaktiviert werden. Weitere Informationen zum Planen der Deaktivierung von Benutzern finden Sie im Abschnitt . <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Planen von Benutzern für die Deaktivierung</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Benutzer deaktivieren oder reaktivieren</a>.</li> 
       <li> <p><b>Primäre Rolle</b>: Dies ist die primäre Aufgabenrolle, die ein Benutzer in Workfront hat. Jede Aufgabe und jedes Problem, denen die Benutzer zugewiesen sind, wird standardmäßig ebenfalls dieser Auftragsrolle zugewiesen. Arbeitsplatzrollen sind im Ressourcenmanagement von entscheidender Bedeutung. Weitere Informationen zu Auftragsrollen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Vorgangsrollen</a></p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planungslizenz mit Administratorzugriff verfügen oder wenn Sie Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
       <li>(Bedingt) Wenn Sie eine <b>Primäre Rolle</b>, die <b>Prozentsatz der VZÄ-Verfügbarkeit</b> angezeigt. Geben Sie an, welcher Prozentsatz der Zeit der Zeitpläne der Benutzer dieser Auftragsrolle zugeordnet ist. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die Primäre Rolle beträgt 100 %.</li> 
       <li> <p><b>Sonstige Rollen</b>: Benutzer können in Workfront über mehrere Vorgangsrollen verfügen. Arbeitsplatzrollen sind im Ressourcenmanagement von entscheidender Bedeutung. Es gibt keine Beschränkung dafür, wie viele Jobrollen ein Benutzer erfüllen kann. Es wird jedoch empfohlen, keinen Benutzer einer zu großen Anzahl von Vorgängen zuzuweisen, da die Ressourcenverwaltung für diese Benutzer zu komplex werden kann.</p> <p>Weitere Informationen zu Auftragsrollen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Erstellen und Verwalten von Vorgangsrollen</a>.</p> <p>Sie können dieses Feld nur aktualisieren, wenn Sie über eine Planungslizenz mit Administratorzugriff verfügen oder wenn Sie Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit Administratorzugriff finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
       <li> <p>(Bedingt) Wenn Sie eine oder mehrere <b>Sonstige Rollen</b>, die <b>Prozentsatz der VZÄ-Verfügbarkeit</b> für jede Rolle angezeigt. Geben Sie an, welcher Prozentsatz der Zeit der Zeitpläne der Benutzer den einzelnen Auftragsrollen zugeordnet wird. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die anderen Rollen beträgt 0 %.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>Wenn "Andere Rollen"eine FTE-Verfügbarkeit von 0 % haben, werden sie nicht im Ressourcen-Planer angezeigt, es sei denn, die Benutzer sind Aufgaben in diesen Rollen zugewiesen.</li> 
       <li> <p>Die Summe aller Prozentsätze der FTE-Verfügbarkeit für alle Rollen muss 100 % betragen. Jeder Prozentsatz der FTE-Verfügbarkeit berechnet die verfügbaren Stunden für jede Rolle pro Benutzer im Resource Planer. Die verfügbaren Stunden für jede Rolle pro Benutzer hängen von der verfügbaren Zeit des Benutzers ab.</p> <p>Die verfügbare Zeit für den Benutzer wird von Workfront entsprechend der Methode berechnet, die der Workfront-Administrator unter "Voreinstellungen für die Ressourcenverwaltung"zur Berechnung der FTE ausgewählt hat.</p> <p>Weitere Informationen zur Berechnung der Verfügbarkeit für den Benutzer finden Sie unter <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Übersicht über die Berechnung der Stunden und der FTE für Benutzer und Rollen im Resource Planer</a>.</p> <p>Weitere Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Zeitplan</b>: Verknüpfen Sie den Benutzern einen Zeitplan. Der Zeitplan der Benutzer berechnet die Zeitleiste der Aufgaben, denen die Benutzer zugewiesen sind.</p> <p>Ein Workfront-Administrator oder ein Gruppenadministrator muss einen Zeitplan erstellen, bevor er Benutzern zugeordnet werden kann.</p> <p>Wählen Sie einen Plan auf Systemebene oder Gruppe aus, um ihn den ausgewählten Benutzern zuzuweisen.</p> <p>Weitere Informationen zu Zeitplänen auf Systemebene und Gruppen finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a>.</p> <p><b>WICHTIG</b>: Workfront verwendet den Zeitplan eines Benutzers nur, wenn die Einstellung "Ressourcenverfügbarkeit berechnen mit"auf den Zeitplan des Benutzers gesetzt ist. Informationen dazu, wie sich die Einstellung "Ressourcenverfügbarkeit berechnen mit"darauf auswirkt, welcher Zeitplan für die Ressourcenverwaltung verwendet wird, finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.</p> </li> 
       <li> <p><b>Datenblatt-Profil</b>: Verknüpfen Sie den Benutzern ein Timesheet-Profil. Dadurch wird sichergestellt, dass Timesheets automatisch für die Benutzer generiert werden.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>Die Liste der in diesem Feld verfügbaren Timesheet-Profile hängt von Ihrem Zugriff ab:
       <ul>
       <li>Als Workfront-Administrator können Sie alle auf System- und Gruppenebene erstellten Zeitleistenprofile sehen.</li>
       <li><p>Als Gruppenadministrator können Sie auf Systemebene die Profile des Zeitplans sowie die Profile sehen, die mit den von Ihnen verwalteten Gruppen verknüpft sind.</p></li>
       <li><p>Als Benutzer mit einer Planner-Lizenz und Zugriff zur Bearbeitung von Benutzern können Sie nur Timesheet-Profile auf Systemebene sehen.</p></li>
       </ul></li> 
       <li>Wenn Sie Gruppenadministrator sind, müssen alle Benutzer, die Sie bearbeiten, Mitglieder einer Gruppe sein, die Sie verwalten.</li> 
       </ul> </p> </li> 
       <li><b>Standardstündentyp</b>: Wählen Sie den Standardstundentyp für die Benutzer aus. Dies ist der Stundentyp, der standardmäßig bei der Protokollzeit der Benutzer verwendet wird.</li> 
       <li> <p><b>Verfügbare Stundentypen</b>: Wählen Sie die für den Benutzer verfügbaren Stundentypen aus. Diese Stundentypen sind überall in Workfront sichtbar, wo die Benutzer die Zeit protokollieren können. Ein Benutzer kann nur die Stunden-Typen sehen, die auf Projektebene und auf Benutzerebene aktiviert sind.</p> 
       <p>Weitere Informationen darüber, welche Stundentypen Benutzern zur Verfügung stehen, finden Sie unter <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Festlegen von Stundentypen und Verfügbarkeit für Timesheets</a>.</p> 
       </li> 
       <li> <b>FTE</b>: Dies ist das Vollzeitäquivalent des Benutzers. Workfront verwendet diese Zahl, um die Verfügbarkeit des Benutzers anhand des Standardzeitplans nur zu berechnen, wenn die Voreinstellungen für die Ressourcenverwaltung auf Systemebene auf den Standardzeitplan gesetzt sind.

   <p>Die FTE gibt die Zeit an, die der Benutzer bei der Arbeit verbringen kann. Dazu gehören Gemeinkosten sowie die Zeit, die für die Projektarbeit benötigt wird. Beispielsweise wird auch die in Sitzungen verbrachte Zeit oder Schulungen in die VZÄ einbezogen.</p>

   Die VZÄ muss eine Dezimalzahl von bis zu 1 haben und darf nicht 0 sein. Wenn der FTE-Wert beispielsweise 0,5 beträgt und der Standardzeitplan in Workfront 40 Stunden beträgt, ist der Benutzer 20 Stunden pro Woche verfügbar.

   Der Standardwert des Felds ist 1.

   Planen Sie Ausnahmen, eine Zeitüberschreitung und den Wert der Arbeitszeit können sich auf die Verfügbarkeit des Benutzers auswirken.

   Workfront berechnet die Verfügbarkeit eines Benutzers entsprechend den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich.

   Wenn die Voreinstellungen für die Ressourcenverwaltung auf Systemebene auf den Zeitplan des Benutzers gesetzt sind, wird der hier angegebene Wert ignoriert und der Benutzer gilt als gemäß den Angaben in seinem Zeitplan verfügbar.

   Weitere Informationen finden Sie unter <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Voreinstellungen für die Ressourcenverwaltung konfigurieren</a>.

   Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Zeitplan erstellen</a>.
   </li> 
       <li> <p><b>Ressourcenpools</b>: Verknüpfen Sie die Benutzer mit Ressourcen-Pools.</p> <p><b>NOTE</b>: In diesem Feld werden nur die Ressourcen-Pools angezeigt, die für alle ausgewählten Benutzer gültig sind. Wenn die ausgewählten Benutzer keine gemeinsamen Ressourcen-Pools haben, ist dieses Feld leer. Wenn dieses Feld leer ist, überschreiben die Ressourcen-Pools, die Sie hier angeben, ihre einzelnen Ressourcen-Pools.</p> 
       <p>Weitere Informationen zu Ressourcen-Pools finden Sie unter <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Ressourcen-Pools - Übersicht </a>.</p> </li> 
       <li><b>Kosten pro Stunde</b>: Die Kosten pro Stunde für den Benutzer. </li> 
       <li><b>Abrechnung pro Stunde</b>: Die Höhe der Abrechnung pro Stunde für den Benutzer.</li> 
       <li><b>Benutzerdefinierte Forms</b>: Verknüpfen Sie ein vorhandenes benutzerdefiniertes Formular mit den Benutzern. Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>.</li> 
       <li><b>Kommentar</b>: Geben Sie einen Kommentar in das angegebene Feld ein. Alle ausgewählten Benutzer erhalten eine In-App-Benachrichtigung sowie eine E-Mail-Benachrichtigung mit Ihrem Kommentar. Der Kommentar wird im Tab Aktualisierungen des Benutzerprofils angezeigt.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Im **Benutzerdefinierte Forms** auswählen, wählen Sie die **Benutzerdefinierte Ausdrücke neu berechnen** , um sicherzustellen, dass alle berechneten benutzerdefinierten Felder in benutzerdefinierten Formularen, die an die ausgewählten Benutzer angehängt sind, auf dem neuesten Stand sind.

1. Klicken Sie auf **Änderungen speichern**.
