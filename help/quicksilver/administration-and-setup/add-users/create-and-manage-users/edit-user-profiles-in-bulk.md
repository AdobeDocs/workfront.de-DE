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
source-git-commit: c7b91828e5a4f961fc48e857eb63756b9b38f664
workflow-type: tm+mt
source-wordcount: '2625'
ht-degree: 0%

---

# Massenbearbeitung von Benutzerprofilen

{{highlighted-preview}}

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on editing a user's profile in the Adobe Admin Console, see the section "Edit user details" in the article [Bulk Upload Users](https://helpx.adobe.com/de/enterprise/using/bulk-upload-users.html) or contact your Adobe Admin Console Administrator.
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

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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

1. Wählen Sie mehrere Benutzer aus und klicken Sie dann auf das Symbol **Bearbeiten** ![Symbol Bearbeiten](assets/edit-icon.png).

1. Ändern Sie im Feld **Benutzer bearbeiten** die Informationen in einem der Abschnitte und klicken Sie **Änderungen speichern** <span class="preview">oder **Speichern**</span>.

### Einstellungen

* **Zeitzone**: Die Zeitzone des Benutzers.

  Informationen zur Unterstützung von Benutzern bei der Zusammenarbeit in Workfront über Zeitzonen hinweg finden Sie [Arbeiten über Zeitzonen hinweg](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

* **E-Mail** Gebietsschema: Das bevorzugte E-Mail-Gebietsschema des Benutzers. Dies wirkt sich auf das Format der Zahlen und Daten in den E-Mails aus, die von Workfront an diesen Benutzer gesendet werden.

  >[!NOTE]
  >
  >Wenn Ihr Unternehmen Adobe Unified Experience nutzt, werden die Spracheinstellungen des Benutzers in seinem Adobe-Profil gespeichert und das E-Mail-Gebietsschema wird nicht verwendet. Informationen zum Zugriff auf diese Voreinstellungen finden Sie unter [Einheitliches Adobe-Erlebnis für Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

### Benachrichtigungen

Wählen Sie die E-Mail-Benachrichtigungen aus, die für die Benutzer aktiviert werden sollen.

Sie können sowohl sofortige als auch tägliche Digest-Benachrichtigungen auswählen. Alle täglichen Digest-Benachrichtigungen werden für alle ausgewählten Benutzer irgendwann nach derselben Zeit gesendet.

Weitere Informationen finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

### Zugriff

* **Ist aktiv** / <span class="preview">**Benutzer ist aktiv**</span>: Aktivieren Sie diese Option, um anzugeben, dass die Benutzer aktiv sind. Aktive Benutzende verwenden eine Workfront-Lizenz. Durch Deaktivieren des Felds werden die Benutzenden deaktiviert und daran gehindert, sich bei Workfront anzumelden.

* **Zugriffsebene**: Wählen Sie die Zugriffsebene aus, die diesen Benutzern zugewiesen werden soll. Alle ausgewählten Benutzer verfügen über dieselbe Zugriffsebene.

  Wenn Sie Benutzenden eine Zugriffsebene zuweisen, können Sie eine Zugriffsebene zuweisen, die Ihrer eigenen Zugriffsebene entspricht oder niedriger ist. (Wenn Ihre Zugriffsebene beispielsweise „Standard“ ist, können Sie keine Administratorzugriffsebene zuweisen.)

  Sie können jedoch keine Zugriffsebene zuweisen, die standardmäßig niedriger ist als Ihre eigene Zugriffsebene, wenn der Workfront-Administrator nicht standardmäßige Berechtigungen auf der Zugriffsebene aktiviert hat, die nicht auch in Ihrer eigenen Zugriffsebene aktiviert sind.

  Wenn Sie beispielsweise über eine Standardlizenz ohne Zugriff auf das Löschen von Aufgaben verfügen, können Sie niemandem eine Light-Lizenz mit Zugriff auf das Löschen von Aufgaben zuweisen, obwohl die Light-Lizenz niedriger als die Standard-Lizenz ist. Weitere Informationen finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

  Weitere Informationen zu Zugriffsebenen finden Sie unter [Zugriff auf Adobe Workfront konfigurieren](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  >[!NOTE]
  >
  >Wenn Ihr Unternehmen das neue Zugriffsmodell (Standard/Light/Contributor) verwendet, können Sie einen Standard- oder Light-Benutzer nicht einer Contributor-Zugriffsebene zuweisen, wenn dieser Benutzer bereits das Entscheidungslimit für den Monat erreicht hat.
  >
  >Weitere Informationen zum neuen Zugriffsmodell finden Sie unter [Übersicht über neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).
  >
  >Informationen zu Entscheidungsbeschränkungen finden Sie unter [Eingeschränktes Dokument und Korrekturabzugsentscheidung für nicht bezahlte Benutzer - Übersicht](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

* **Layout-Vorlage**: Wählen Sie eine Layout-Vorlage für die Benutzer. Diese Layout-Vorlage hat Vorrang vor jeder Layout-Vorlage, die ihrer Hauptgruppe, ihrem Hauptteam oder ihrer Primären Rolle zugewiesen ist. Weitere Informationen zur Zuweisungspriorität von Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

  In der folgenden Liste wird beschrieben, wie die Liste der Vorlagen, die Sie in diesem Feld haben, von Ihrem Zugriff abhängt:

   * Als Workfront-Administrator können Sie alle Layoutvorlagen auf Systemebene und Gruppenebene sehen.
   * Als Gruppenadministrator bzw. -administratorin können Sie die Layoutvorlagen auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Vorlagen sehen.
   * Benutzende mit einer Standard- oder Plan-Lizenz, die Zugriff auf die Bearbeitung von Benutzenden haben, können nur Layoutvorlagen auf Systemebene sehen.

     Weitere Informationen zu Layout-Vorlagen auf Gruppenebene finden Sie unter [Erstellen und Ändern der Layout-Vorlagen einer Gruppe](/help/quicksilver/administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

### Organisation

* **Unternehmen**: Das Unternehmen der Benutzer. Benutzende können nur mit einer Firma verknüpft werden. Sie müssen eine Firma erstellen, bevor Sie sie mit einem Benutzer verknüpfen können. In der Liste werden nur aktive Unternehmen angezeigt. Informationen zum Erstellen von Unternehmen finden Sie unter [Erstellen und Bearbeiten von Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).
* **Home-**: Geben Sie das Home-Team für die Benutzer an. Benutzer können nur über ein Home-Team verfügen.
* **Andere Teams**: Benutzer können mehreren Teams angehören.
* **Hauptgruppe**/<span class="preview">**Aktuelle Hauptgruppe**</span>: Wählen Sie eine geeignete Gruppe aus, um die Benutzer zuzuweisen. Dadurch können Benutzer auf Objekte zugreifen, die für die Gruppe freigegeben sind. Sie können Layout-Vorlagen auch für eine Hauptgruppe freigeben.

  Dies ist ein Pflichtfeld. Jeder Benutzer muss einer Hauptgruppe zugeordnet sein. Wenn Sie keine Hauptgruppe auswählen, wird diese als Hauptgruppe zugewiesen.

  Sie können eine Gruppe nur dann einem Benutzer zuweisen, wenn einer der folgenden Punkte zutrifft:

   * Sie sind ein Workfront-Administrator
   * Sie sind der Administrator der Gruppe
   * Die Gruppe ist öffentlich

* **Andere Gruppen**: Benutzer können mehreren Gruppen angehören. Eine Gruppe kann einem Benutzer nur zugewiesen werden, wenn Sie Workfront-Administrator sind, Administrator der Gruppe sind oder die Gruppe öffentlich ist.

  >[!IMPORTANT]
  >
  >Das Hinzufügen eines Benutzers zu mehr als 100 Gruppen kann in jedem Bereich von Workfront, der die Liste der Gruppen lädt, zu Leistungsproblemen führen.

  Weitere Informationen zu öffentlichen Gruppen finden Sie unter [Erstellen einer Gruppe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

  Weitere Informationen zu Gruppen finden Sie unter [Gruppen - Übersicht](/help/quicksilver/administration-and-setup/manage-groups/groups-overview/groups.md).

### Ressourcenplanung

* **Arbeitszeit**: Gibt den Prozentsatz der Vollzeitäquivalenzzeit (VZÄ) an, die die Benutzer für die tatsächliche Arbeit zur Verfügung haben, ohne Gemeinkosten. Arbeitszeit muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. So würde beispielsweise eine Verfügbarkeit von 20 % für die tatsächliche Arbeit 0,2 betragen.

  Der Standardwert des Feldes ist 1. Dies bedeutet, dass ein Benutzer sein gesamtes FTE für die tatsächliche, projektbezogene Arbeit verwendet.

  Anhand dieser Zahl berechnet das System die Verfügbarkeit des Nutzers für die tatsächliche, projektbezogene Arbeit.

  Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter [Erstellen eines Zeitplans](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  Zeitplanausnahmen und Ausfallzeiten können sich ebenfalls auf die Kapazität des Benutzers auswirken.

  Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich. Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  >[!TIP]
  >
  >Legen Sie den Wert für Arbeitszeit auf 1 fest, um anzugeben, dass der Benutzer für projektbezogene Arbeit bis zum gesamten Vollzeitäquivalent verfügbar ist.

* **Deaktivierung planen** / <span class="preview">**Deaktivierungsdatum festlegen**</span>: Aktivieren Sie dieses Kontrollkästchen / <span class="preview">klicken Sie auf diese Schaltfläche</span>, wenn Sie diese Benutzer planen möchten, zu einem bestimmten Datum und zu einer bestimmten Uhrzeit deaktiviert zu werden.
* **Geplantes Deaktivierungsdatum** / <span class="preview">**Deaktivierungsdatum**</span>: Das Datum und die Uhrzeit, zu der die Benutzer deaktiviert werden. Informationen zum Planen von Benutzern für die Deaktivierung finden Sie unter [Planen von Benutzern für die ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#schedule-users-for-deactivation)) in [Deaktivieren oder Reaktivieren von Benutzern](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
* **Primäre Rolle**: Dies ist das primäre Aufgabengebiet, das die Benutzerinnen und Benutzer in Workfront erfüllen können. Jede Aufgabe und jedes Problem, der/dem die Benutzenden zugewiesen sind, wird ebenfalls diesem Aufgabengebiet zugewiesen. Aufgabengebiete sind im Ressourcen-Management von entscheidender Bedeutung. Sie können dieses Feld nur aktualisieren, wenn Sie über eine Standard- oder Planlizenz mit administrativem Benutzerzugriff verfügen oder wenn Sie ein Workfront-Administrator sind. Weitere Informationen zum Einrichten von Benutzern mit administrativem Benutzerzugriff finden Sie unter [Gewähren des Zugriffs für Benutzer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

  In der Liste werden nur aktive Aufgabengebiete angezeigt.

* (Bedingt) Wenn Sie eine **Primäre Rolle ausgewählt haben** wird das Feld **Prozentsatz der FTE-Verfügbarkeit** angezeigt. Geben Sie an, wie viel Prozent der Zeit in den Zeitplänen der Benutzer diesem Aufgabengebiet zugewiesen sind. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die Primäre Funktion ist 100 %.
* **Andere Rollen**: Benutzer können in Workfront über mehrere Aufgabengebiete verfügen. Aufgabengebiete sind im Ressourcen-Management von entscheidender Bedeutung. Es gibt keine Begrenzung dafür, wie viele Aufgabengebiete ein Benutzer erfüllen kann. Wir empfehlen jedoch, einer zu großen Anzahl von Aufgabengebieten nicht einen Benutzer zuzuweisen, da die Ressourcenverwaltung für diese Benutzer möglicherweise zu komplex wird.

  In der Liste werden nur aktive Aufgabengebiete angezeigt. Weitere Informationen zu Aufgabengebieten finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

  Sie können dieses Feld nur aktualisieren, wenn Sie über eine Standard- oder Planlizenz mit administrativem Benutzerzugriff verfügen oder wenn Sie ein Workfront-Administrator sind.

  Weitere Informationen zum Einrichten von Benutzern mit administrativem Benutzerzugriff finden Sie unter [Gewähren des Zugriffs für Benutzer](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

* (Bedingt) Wenn Sie eine oder mehrere Rollen **Sonstige Rollen** ausgewählt haben, wird für **jeweilige Rolle das Feld** Prozentsatz der FTE-Verfügbarkeit“ angezeigt. Geben Sie an, welcher Prozentsatz der Zeit in den Zeitplänen der Benutzer den einzelnen Aufgabengebieten zugewiesen ist. Der Standardwert für den Prozentsatz der FTE-Verfügbarkeit für die anderen Funktionen ist 0 %.

  Wenn für andere Funktionen eine FTE-Verfügbarkeit von 0 % verfügbar ist, werden sie nicht im Ressourcenplaner angezeigt, es sei denn, die Benutzer sind Aufgaben in diesen Rollen zugewiesen.

  Die Summe aller **Prozentsätze der FTE-Verfügbarkeit** für alle Rollen muss 100 % betragen. Jeder Prozentsatz der FTE-Verfügbarkeit berechnet die verfügbaren Stunden für jede Rolle pro Benutzer im Ressourcenplaner. Die verfügbaren Stunden für jede Rolle pro Benutzer hängen von der verfügbaren Zeit für den Benutzer ab.

  Die verfügbare Zeit für den Benutzer wird von Workfront abhängig von der Methode berechnet, die vom Workfront-Administrator zur Berechnung des FTE in den Voreinstellungen für das Ressourcenmanagement ausgewählt wurde.

  Informationen zur Berechnung der Verfügbarkeit für den Benutzer finden Sie unter [Übersicht über die Berechnung von Stunden und VZÄ für Benutzer und Funktionen im Ressourcenplaner](/help/quicksilver/resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md).

  Informationen zum Konfigurieren der Voreinstellungen für die Ressourcenverwaltung finden Sie [Konfigurieren der Voreinstellungen für die ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)).

* **Zeitplan**: Ordnen Sie den Benutzern einen Zeitplan zu. Der Zeitplan der Benutzer berechnet die Zeitleiste der Aufgaben, denen die Benutzer zugewiesen sind.

  Sie müssen einen Zeitplan erstellen, bevor Sie ihn Benutzern zuordnen können. Weitere Informationen zum Erstellen von Zeitplänen finden Sie unter [Erstellen eines Zeitplans](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

  >[!IMPORTANT]
  >
  >Workfront verwendet den Zeitplan eines Benutzers nur, wenn die Einstellung **Ressourcenverfügbarkeit berechnen mit** auf &quot;**des Benutzers“** ist. Weitere Informationen darüber, wie sich diese Einstellung auf den für die Ressourcenverwaltung verwendeten Zeitplan auswirkt, finden Sie [Konfigurieren der Voreinstellungen für die ](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)&quot;.

* **Arbeitszeittabellen-**: Verknüpfen Sie die Benutzer mit einem Arbeitszeittabellen-Profil, um sicherzustellen, dass Arbeitszeittabellen automatisch generiert werden.

  Die Liste der Profile, die in diesem Feld verfügbar sind, hängt von Ihrem Zugriff ab:

   * Als Workfront-Administrator können Sie alle Arbeitszeittabellen-Profile auf Systemebene und Gruppenebene anzeigen.
   * Als Gruppenadministrator können Sie Arbeitszeittabellen-Profile auf Systemebene sowie die mit den von Ihnen verwalteten Gruppen verknüpften Profile anzeigen.
   * Benutzende mit einer Standard- oder Plan-Lizenz, die Zugriff haben, um Benutzende zu bearbeiten, können nur Arbeitszeittabellen-Profile auf Systemebene sehen. Weitere Informationen zu Arbeitszeittabellen-Profilen auf Gruppenebene finden Sie unter [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](/help/quicksilver/timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Standardstundentyp**: Wählen Sie den Standardstundentyp für die Benutzer aus. Dies ist der Stundentyp, der standardmäßig verwendet wird, wenn Benutzer die Zeit erfassen.
* **Verfügbare Stundentypen**: Wählen Sie die Stundentypen aus, die für die Benutzer verfügbar sein sollen. Diese Stundentypen sind überall in Workfront sichtbar, wo Benutzende die Zeit protokollieren können. Benutzer können nur die Stundentypen sehen, die auf Projekt- sowie auf Benutzerebene aktiviert sind. Weitere Informationen dazu, welche Stundentypen Benutzern zur Verfügung stehen, finden Sie unter [Festlegen von Stundentypen und Verfügbarkeit](/help/quicksilver/timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).
* **FTE**: Dies ist das Vollzeitäquivalent der Benutzer. Workfront verwendet diese Zahl, um die Verfügbarkeit der Benutzer auf der Grundlage des Standardzeitplans nur dann zu berechnen, wenn die Ressourcenverwaltungseinstellungen auf Systemebene auf den Standardzeitplan eingestellt sind.

  Das FTE gibt an, wie viel Zeit die Benutzer bei der Arbeit verbringen können. Dazu gehören Gemeinkosten sowie die Zeit, die mit der Projektarbeit verbracht wird. Beispielsweise wird die Zeit, die in Meetings oder Schulungen verbracht wird, ebenfalls in das VZÄ einbezogen.

  Der FTE muss eine Dezimalzahl bis 1 sein und darf nicht 0 sein. Wenn beispielsweise der FTE-Wert 0,5 beträgt und der Standardzeitplan in Workfront 40 Stunden beträgt, stehen die Benutzenden 20 Stunden pro Woche zur Verfügung.

  Der Standardwert des Felds ist 1.

  Zeitplanausnahmen, Ausfallzeiten und der Wert der Arbeitszeit können sich auf die Verfügbarkeit der Benutzer auswirken.

  Workfront berechnet die Verfügbarkeit eines Benutzers abhängig von den Voreinstellungen für die Ressourcenverwaltung in Ihrem Setup-Bereich.

  Wenn die Voreinstellungen für das Ressourcen-Management auf Systemebene auf den Zeitplan des Benutzers festgelegt sind, wird der hier angegebene Wert ignoriert und der Benutzer wird gemäß den Angaben in seinem Zeitplan als verfügbar betrachtet.

  Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

  Weitere Informationen zum Erstellen von Zeitplänen in Workfront finden Sie unter [Erstellen eines Zeitplans](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

* **Ressourcenpools**: Verknüpfen Sie die Benutzer mit Ressourcenpools.

  >[!NOTE]
  >
  >In diesem Feld werden nur die Ressourcenpools angezeigt, die für alle ausgewählten Benutzer gelten. Wenn die ausgewählten Benutzer keine freigegebenen Ressourcenpools haben, ist dieses Feld leer. Wenn dieses Feld leer ist, überschreiben die hier angegebenen Ressourcenpools ihre einzelnen Ressourcenpools.

  Weitere Informationen zu Ressourcenpools finden Sie unter [Ressourcenpools mit Benutzern verknüpfen](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/associate-resource-pools-with-users.md).

* **Kostensatz**: Der Betrag der Kosten pro Stunde für den Benutzer.

  Klicken Sie für gültige Datumssätze auf &quot;**hinzufügen**. Geben Sie den Wert des Kostensatzes für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Kostensatz 1 hat kein Startdatum und der letzte Kostensatz hat kein Enddatum.

  Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Kostensatz 1 kein Enddatum hat und Sie Kostensatz 2 mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem Kostensatz 1 das Enddatum 30. April 2023 hinzugefügt, sodass keine Lücken entstehen.

* **Abrechnungssatz**: Der Abrechnungsbetrag pro Stunde für den Benutzer.

  Klicken Sie für Abrechnungssätze mit Gültigkeitsdatum auf **Abrechnungssatz hinzufügen**. Geben Sie den Wert des Abrechnungssatzes für den Zeitraum ein und weisen Sie gegebenenfalls ein Start- und Enddatum zu. Abrechnungssatz 1 hat kein Startdatum und der letzte Abrechnungssatz hat kein Enddatum.

  Einige Daten werden automatisch hinzugefügt. Wenn beispielsweise Abrechnungssatz 1 kein Enddatum hat und Sie eine Sekunde mit dem Startdatum 1. Mai 2023 hinzufügen, wird dem Abrechnungssatz 1 ein Enddatum vom 30. April 2023 hinzugefügt, sodass keine Lücken bestehen.

### Benutzerdefinierte Formulare

Verknüpfen Sie ein vorhandenes benutzerdefiniertes Formular mit den Benutzern. Sie müssen ein benutzerdefiniertes Formular erstellen, bevor Sie es mit einem Benutzer verknüpfen können. In der Liste werden nur aktive benutzerdefinierte Formulare angezeigt. Felder, auf die Sie keinen Zugriff haben, werden nicht in einem einzelnen benutzerdefinierten Formular angezeigt.

>[!NOTE]
>
>Erweiterte benutzerdefinierte Formularfunktionen wie externe Suchfelder und native Workfront-Felder sind nur verfügbar, wenn Sie den Benutzerdatensatz auf der Detailseite öffnen, nicht im Dialogfeld „Benutzer bearbeiten“. (Klicken Sie in der Benutzerliste auf den Benutzernamen, um die Details zu öffnen.)

Sie können optional die Option **Benutzerdefinierte Ausdrücke neu berechnen** auswählen, um sicherzustellen, dass alle berechneten benutzerdefinierten Felder in benutzerdefinierten Formularen, die an die ausgewählten Benutzer angehängt sind, auf dem neuesten Stand sind.

Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Kommentar

Geben Sie den Kommentar ein, den Sie den Benutzern und dem Bereich Aktualisierungen ihrer Benutzerprofile senden möchten.

<!--
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Preferences</td> 
      <td> 
       <ul> 
        <li><b>Time Zone:</b> The users' time zone.</li> 
        <li><b>Locale</b>: The users' preferred locale. This affects the format of numbers and dates in the emails that come from Workfront.</li> 
        <li><b>Send work I assign to myself to my Working On tab</b>: This setting refers to a deprecated feature that has been removed from Workfront.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notifications</td> 
      <td>Select the email notifications which should be enabled for the new user.<p>You can select instant as well as daily digest notifications. All the daily digest notifications are delivered sometime after the same time for all the users selected. For more information, see <a href="../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md" class="MCXref xref">Configure event notifications for everyone in the system</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Access</td> 
      <td> 
       <ul> 
        <li><b>Is Active:</b> Select this field to indicate whether the users are active. Active users use a Workfront license. Deselecting the field deactivates the users.</li> 
        <li> 
        <p><b>Access Level:</b> Select the access level to assign to these users. All users selected will have the same access level.
        </p> 
        <p>When you assign an access level to users, you can assign a level equal to or less than your own access level. (For example, if your access level is Planner, you cannot assign the Administrator access level.) </p>
        <p>However, you cannot assign an access level that is lower than your own if the Workfront administrator has enabled permissions on the access level that are not also enabled in your own (via the Fine-Tune settings, as described in <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>).</p> 
        <p>For more information about access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md" class="MCXref xref">Configure access to Adobe Workfront</a>.</p> 
         </li> 
        <li> 
        <p><b>Layout Template</b>: Choose a layout template for the users. The layout template assigned to the users will take precedence over any layout template assigned to their Home Group, Home Team or primary job role. For more information about the assignment priority of layout template, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p> 
        <p><b>NOTE</b>:  The list of layout templates you have available in this field depends on your access:
          <ul>
           <li>As a Workfront administrator, you can see all system-level and group-level layout templates.</li>
           <li>As a group administrator, you can see system-level layout templates, as well as those associated with the groups that you manage.</li>
           <li><p>As a user with a Planner license and access to edit users, you can see only system-level layout templates. </p>
           <p>For information about group-level layout templates, see <a href="../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
           </li>
          </ul></p> 
          </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Organization</td> 
      <td> 
       <ul> 
        <li><b>Company</b>: The company of the users. Users can be associated only with one company. You must create a company before you can associate it with a user. Only active companies display in the list. For information about creating companies, see Understanding and Managing Companies.</li> 
        <li><b>Home Team</b>: Specify the home team for the users. Users can only have one home team. </li> 
        <li><b>Other Teams</b>: Users can belong to multiple teams. </li> 
        <li> <p><b>Home Group:</b> Select an appropriate group to assign the users as their Home Group. This gives the user the ability to access objects that are shared with the group.</p> <p><b>NOTE</b>:  This is a required field. You cannot have users not associated with a Home Group.</p> <p>You can assign a group to users only in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li>The group is public.</li> 
         </ul> </li> 
        <li> <p><b>Other Groups</b>: Users can belong to multiple groups. You can assign a group to a user only  in the following situations:</p> 
         <ul> 
          <li>You are a Workfront administrator.</li> 
          <li>You are the administrator of that group.</li> 
          <li> <p>The group is public. </p> 
          <p>For more information about public groups, see <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md" class="MCXref xref">Create a group</a>.</p> 
          <p>For more information about groups, see <a href="../../../administration-and-setup/manage-groups/groups-overview/groups.md" class="MCXref xref">Groups overview</a>.</p> 
          </li> 
         </ul> 
         </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resource Planning</td> 
      <td> 
       <ul> 
      
      <li>
       <b>Work Time</b>: Represents the percentage of the Full Time Equivalent (FTE) time that the user is available for actual work, not including overhead. Work Time must be a decimal number up to 1, and it cannot be 0. For example, a 20% availability for actual work would be 0.2.

      The field's default is 1, indicating that a user spends their entire FTE on actual, project-related work. 

      The system uses this number to calculate the availability of the user for actual, project-related work. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.

      Schedule exceptions and time off might also affect the user capacity. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area. For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      <b>TIP</b>

      Set the Work Time value to  1 to indicate that the user is available for project-related work their entire full-time equivalent.
      </li> 

      <li><b>Schedule Deactivation</b>: Check this box if you want to schedule users to be deactivated after a period of time.</li> 
       <li><b>Scheduled Deactivation Date</b>: The date after which the users become deactivated. For more information about scheduling users for deactivation, see the section <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md#scheduling-users-for-deactivation" class="MCXref xref">Schedule users for deactivation</a> in <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</li> 
       <li> <p><b>Primary Role</b>: This is the primary job role that a user has in Workfront. Every task and issue that the users are assigned to is also assigned to this job role, by default. Job roles are essential in resource management. For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a></p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li>(Conditional) If you selected a <b>Primary Role</b>, the <b>Percentage of FTE Availability</b> field displays. Specify what percentage of time of the users' schedules is allocated to this job role. The default value for the Percentage of FTE Availability for the Primary Role is 100%.</li> 
       <li> <p><b>Other Roles</b>: Users can have multiple job roles in Workfront. Job roles are essential in resource management. There is no limit for how many job roles a user can fulfill. However, we recommend to not assign one user to an excessively large number of job roles, because resource management might become too complex for these users.</p> <p>For more information about job roles, see <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">Create and manage job roles</a>.</p> <p>You can update this field only if you have a Plan license with administrative user access, or if you are a Workfront administrator. For more information about setting up users with administrative user access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Grant access to users</a>.</p> </li> 
       <li> <p>(Conditional) If you selected one or multiple <b>Other Roles</b>, the <b>Percentage of FTE Availability</b> field displays for each role. Specify what percentage of time of the users' schedules is allocated to each job role. The default value for the Percentage of FTE Availability for the Other Roles is 0%.</p> <p><b>NOTE</b>:  
       <ul> 
       <li>If Other Roles have a 0% FTE Availability, they do not display in the Resource Planner, unless the users are assigned to tasks in these roles.</li> 
       <li> <p>The sum of all Percentages of FTE Availability for all roles must equal 100%. Each Percentage of FTE Availability calculates the Available Hours for each role per user in the Resource Planner. The Available Hours for each role per user depends on the available time for the user.</p> <p>The available time for the user is calculated by Workfront depending on the method that has been selected by the Workfront administrator to calculate the FTE in the Resource Management Preferences.</p> <p>For more information about calculating availability for the user, see <a href="../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> <p>For more information about configuring Resource Management preferences, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       </ul> </p> </li> 
       <li> <p><b>Schedule</b>: Associate a schedule with the users. The schedule of the users calculates the timeline of the tasks the users are assigned to.</p> <p>A Workfront administrator or a group administrator must create a schedule before it can be associated with users.</p> <p>Select a system-level or a group schedule to assign it to the selected users.</p> <p>For more information about system-level and group schedules, see <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Create a schedule</a>.</p> <p><b>IMPORTANT</b>: Workfront uses the schedule of a user only when the Calculate Resource Availability Using setting is set to The User's Schedule. For information about how the Calculate Resource Availability Using setting affects which schedule is used for Resource Management, see <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md" class="MCXref xref">Configure Resource Management preferences</a>.</p> </li> 
       <li> <p><b>Timesheet Profile</b>: Associate a Timesheet Profile with the users. This ensures that timesheets generate automatically for the users.</p> 
       <p><b>NOTE</b>:  
       <ul> 
       <li>The list of timesheet profiles you have available in this field depends on your access:
       <ul>
       <li>As a Workfront administrator, you can see all system-level and group-level timesheet profiles.</li>
       <li><p>As a group administrator, you can see system-level timesheet profiles, as well as those associated with the groups that you manage.</p></li>
       <li><p>As a user with a Planner license and access to edit users, you can see only system-level timesheet profiles.</p></li>
       </ul></li> 
       <li>If you are a group administrator, all of the users you are editing must be members of a group that you administer.</li> 
       </ul> </p> </li> 
       <li><b>Default Hour Type</b>: Select the default hour type for the users. This is the hour type that is used by default when the users log time.</li> 
       <li> <p><b>Available Hour Types</b>: Select the hour types that should be available to the user. These hour types are visible everywhere in Workfront where the users can log time. A user can only see the hour types that are enabled at the project level as well as the user level.</p> 
       <p>For more information about what hour types are available to users, see <a href="../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md" class="MCXref xref">Define hour types and availability</a>.</p> 
       </li> 
       <li> <b>FTE</b>: This is the Full Time Equivalent of the user. Workfront uses this number to calculate the availability of the user based on the Default Schedule only when the Resource Management Preferences at the system level are set to The Default Schedule. 

      <p>The FTE indicates the amount of time that the user can spend at work. This includes overhead, as well as time spent on project work. For example, time that is spent in meetings, or training is also included in the FTE.</p> 

      The FTE must be a decimal number up to 1, and it cannot be 0. For example, if the FTE value is 0.5 and the Default Schedule in Workfront is 40 hours, the user is available for 20 hours a week. 

      The field's default is 1.

      Schedule exceptions, time off might, and the value of Work Time may affect the availability of the user. 

      Workfront calculates a user's availability depending on the Resource Management preferences in your Setup area.

      If the Resource Management Preferences at the system level are set to The User's Schedule, the value you specify here is ignored and the user is considered to be available according to what is specified in their schedule. 

      For more information, see <a href="../../set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">Configure Resource Management preferences</a>. 

      For more information about creating schedules in Workfront, see <a href="../../set-up-workfront/configure-timesheets-schedules/create-schedules.md">Create a schedule</a>.
      </li> 
       <li> <p><b>Resource Pools</b>: Associate the users with resource pools.</p> <p><b>NOTE</b>:  Only the resource pools that are common to all the users selected appear in this field. If the users selected have no shared resource pools, this field is empty. If this field is empty, the resource pools you specify here will overwrite their individual resource pools.</p> 
       <p>For more information about resource pools, see <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Resource pools overview </a>.</p> </li> 
       <li><b>Cost Per Hour</b>: The amount of cost per hour for the user. </li> 
       <li><b>Billing Per Hour</b>: The amount of billing per hour for the user.</li> 
       <li><b>Custom Forms</b>: Associate an existing user custom form with the users. You must create a custom form before you can associate it with a user. Only active custom forms display in the list. For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>.</li> 
       <li><b>Comment</b>: Enter a comment in the field provided. All users selected will receive an in-app notification as well as an email notification with your comment. The comment shows in the Updates tab of the users' profile.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
-->

