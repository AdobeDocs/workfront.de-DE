---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Anzeigen von Fortschritt und Status eines Testversands in [!DNL Workfront Proof]
description: Der Fortschritt des Testversands gibt an, welche Arbeit an einem Testversand von dem Zeitpunkt an, an den Sie den Testversand an die Validierungsverantwortlichen senden, bis zu dem Zeitpunkt, an dem sie über den Testversand entscheiden.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 8fd85595-1403-490e-9d52-2ba5b01457b7
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Anzeigen von Fortschritt und Status eines Testversands in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

## Grundlegendes zum Testfortschritt

Der Fortschritt des Testversands gibt an, welche Arbeit an einem Testversand von dem Zeitpunkt an, an den Sie den Testversand an die Validierungsverantwortlichen senden, bis zu dem Zeitpunkt, an dem sie über den Testversand entscheiden.

* [Fortschrittssymbole](#progress-icons)
* [Stufen der Beweisaufnahme](#levels-of-proof-progress)

### Fortschrittssymbole {#progress-icons}

Die Fortschrittssymbole S, O, C und D werden in der Fortschrittsleiste angezeigt und zeigen den Fortschritt des Testversands an.

![proof_edit_existing_progress.png](assets/proof-edit-existing-progress-350x78.png)

Sie geben die folgenden Informationen zu einem Testversand an:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Fortschrittssymbol</strong> </p> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt="proof_progress_sent_icon.png"> </p> </td> 
   <td> <p><strong>Gesendet</strong>. Der Testversand wurde den Validierungsverantwortlichen übermittelt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-opened-icon.png" alt="proof_progress_opened_icon.png"> </p> <p> </p> </td> 
   <td> <p><strong>Geöffnet</strong>. Ein Validierer hat die Seite Testversand-Details geöffnet oder den Testversand selbst im Testversand-Viewer geöffnet.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-comment-icon.png" alt="proof_progress_comment_icon.png"> </p> </td> 
   <td> <p><strong>Kommentare</strong>. Überprüfer (Benutzer, die Kommentare abgeben können) haben sich zu dem Testversand geäußert.</p> <p>Wenn für den Testversand keine Validierungsverantwortlichen bestimmt wurden, wird dieses Symbol nicht angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt="proof_progress_decision_icon.png"> </p> </td> 
   <td> <p><strong>Entscheidung</strong>. Ein Prüfer hat eine Entscheidung über den Testversand getroffen.</p> <p>Wenn keine Genehmiger (Entscheidungsträger) für den Testversand bestimmt sind, wird dieses Symbol nicht angezeigt. </p> </td> 
  </tr> 
 </tbody> 
</table>

Diese Symbole können in den folgenden Farben angezeigt werden, um bestimmte Informationen über den Fortschritt des Testversands anzuzeigen:

* **Grün**. Abgeschlossen.
* **White**. Nicht abgeschlossen.
* **Orange**. Nicht vollständig und die Frist beträgt weniger als 24 Stunden.
* **Rot**. Nicht abgeschlossen und die Frist verstrichen.

### Stufen der Beweisaufnahme {#levels-of-proof-progress}

Workfront Proof verwendet die Fortschrittssymbole, um den Fortschritt eines Testversands auf den folgenden Ebenen zu verfolgen:

* Für jeden Validierer, basierend auf der Aktivität dieser Person auf dem Testversand.
* Für jede Phase, basierend auf dem Fortschritt der Validierer auf der Bühne, der am meisten im Testprozess zurückliegt. Weitere Informationen finden Sie unter [Übersicht über automatisierte Workflow-Phasen](../../../review-and-approve-work/proofing/proofing-overview/stages.md).
* Für den Testversand, basierend auf dem Fortschritt der Phase (Gruppe der Validierungsverantwortlichen), die am meisten hinter dem Testprozess zurückliegt.

Ein Beispiel dafür, wie [!DNL Workfront Proof] den Fortschritt anhand des Validierers oder der Phase ermittelt, die am meisten hinterherhinkt, finden Sie unter der Annahme, dass drei Validierungsverantwortliche für einen Testversand eine Entscheidung treffen müssen. Wenn zwei von ihnen ihre Entscheidung getroffen haben, der dritte jedoch nicht, zeigt der Fortschrittsbalken für den Nachweis aufgrund der noch ausstehenden Entscheidung nicht, dass die D grün ist.

Wenn die Einstellung [!UICONTROL Primärer Entscheidungsträger] für einen Testversand ausgewählt ist und der primäre Entscheidungsträger eine Entscheidung sendet, wird die ID in der Fortschrittsleiste für Testsendungen für alle Prüfer grün, da keine anderen Entscheidungen erforderlich sind.

Wenn die Einstellung [!UICONTROL Nur eine Entscheidung erforderlich] für einen Testversand ausgewählt ist und ein Validierer eine Entscheidung sendet, wird die ID in der Fortschrittsleiste für den Testversand für alle Validierer grün, da keine anderen Entscheidungen erforderlich sind.

## Wissenswertes zum Teststatus

Der Status des Testversands zeigt den Status der Entscheidungen an, die für den Testversand erforderlich sind.

![proof_edit_existing_status.png](assets/proof-edit-existing-status-350x78.png)\
Die Standardstatusoptionen sind:

* Ausstehend
* Genehmigt
* Genehmigt mit Änderungen
* Erforderliche Änderungen
* Nicht relevant

Wenn benutzerdefinierte Entscheidungen in Ihrem Konto konfiguriert sind, spiegeln die Statusoptionen Ihre benutzerdefinierten Entscheidungseinstellungen wider.

Der Status des Testversands wird durch den Teilnehmer &quot;Schlimmster Fall&quot; bestimmt. Angenommen, es gibt drei Entscheidungen über den Testversand: zwei haben den Status **Akzeptiert** und eine hat den Status **Abgelehnt**. Die Entscheidung &quot;Schlimmster Fall&quot;der Zurückweisung regelt die anderen Entscheidungen und den Gesamtstatus des Testversands wird als **Abgelehnt** angezeigt.

## Anzeigen von Fortschritt und Status {#viewing-progress-and-status}

Sie können Fortschritt und Status für Testsendungen, Bühnen und Prüfer auf jeder Phase anzeigen.

* [Testzusammenfassung](#proof-summary)
* [Menü &quot;Staging-Aktionen&quot;](#stage-actions-menu)
* [Im Abschnitt [!UICONTROL Zusammenfassung] können Sie auch auf die Aktionsmenüs der Prüfer zugreifen, sofern Sie über Bearbeitungsrechte für den Testversand verfügen. Weitere Informationen finden Sie unter Profile für Testberechtigungen in Workfront Proof und Verwalten von Proof-Rollen in Workfront Proof . Das Menü &quot;[!UICONTROL Prüferaktionen]&quot;(1) wird angezeigt, wenn Sie den Mauszeiger über die Details des Prüfers bewegen. Dort können Sie:](#in-the-summary-section-you-can-also-access-the-reviewer-actions-menus-provided-you-have-edit-rights-on-the-proof-for-more-information-see-proof-permissions-profiles-in-workfront-proof-and-manage-proof-roles-in-workfront-proof-the-reviewer-actions-menu-1-appears-when-you-hover-over-the-reviewer-s-details-and-allows-you-to)
* [Menü &quot;Proof Actions&quot;](#proof-actions-menu)

### Testzusammenfassung {#proof-summary}

Jeder Testversand im Ordner verfügt über eine erweiterbare Zusammenfassung, mit der Sie die Details des Testversands schnell anzeigen und bearbeiten können.

So erweitern oder reduzieren Sie die Zusammenfassung:

1. Klicken Sie im Dashboard oder in einer beliebigen Listenansicht auf den Pfeil links neben dem Testversand.

![Summary_expand.png](assets/summary-expandable-350x68.png)

Die Zusammenfassung enthält Folgendes:

* Workflow (2)
* Version 3
* Ordner (4)
* Bundesland (5)\
   ![summary_2.png](assets/summary-2-350x160.png)

In der Zusammenfassung können Sie die folgenden Details Ihres Testversands anzeigen und bearbeiten:

* Fortschritte bei der Überprüfung (1)
* Fortschritt der einzelnen Phasen (2)
* Für die Phase festgelegter Termin (3)
* Reviewer-Details:

   * Anzahl der Stellungnahmen und Antworten der einzelnen Prüfer (4)
   * Fortschritt der einzelnen Prüfer (5)
   * Entscheidung (wenn eine Entscheidung eine elektronische Signatur enthält, wird neben der Entscheidung ein Symbol angezeigt, auf dem diese angegeben wird.) Absatz 6
   * Rolle bei der Beweisaufnahme (7)
   * Einstellungen für E-Mail-Warnhinweise (8)

>[!NOTE]
>
>Ihre Fähigkeit, die Details des Testversands zu bearbeiten, hängt von Ihren Berechtigungen für den Testversand ab (siehe [Profile für Testversandberechtigungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) und [Rollen verwalten in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![summary_details_3.png](assets/summary-details-3-350x160.png)

### Menü [!UICONTROL Staging-Aktionen]  {#stage-actions-menu}

Jede Workflow-Phase verfügt über ein eigenes Menü, über das Sie Massenaktionen für die validierungsverantwortlichen Benutzer in dieser Phase durchführen können.

Das Menü [!UICONTROL Staging-Aktionen] wird angezeigt, wenn Sie den Mauszeiger über den Abschnitt &quot;Staging&quot;(1) bewegen, und ermöglicht Ihnen Folgendes:

* [!UICONTROL Nachricht für alle ] (2)
* [!UICONTROL Share] (3)
* [!UICONTROL Löschphase] (4)

>[!NOTE]
>
>Die Verfügbarkeit dieser Optionen hängt von Ihren Berechtigungen für den Testversand ab (siehe [Profile für Testversandberechtigungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) und [Rollen in Testsendungen verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![Stage_actions_menu.png](assets/stage-actions-menu-350x161.png)

Im Abschnitt Zusammenfassung können Sie auch auf die Aktionsmenüs der validierungsverantwortlichen Benutzer zugreifen, sofern Sie über Bearbeitungsrechte für den Testversand verfügen. Weitere Informationen finden Sie unter [Proof Permissions Profiles in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) und [Proof Roles in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) verwalten . Das Menü mit den Reviewer-Aktionen (1) wird angezeigt, wenn Sie den Mauszeiger über die Details des Reviewers bewegen. Dort können Sie:

* Nachricht an den Validierer senden (2)
* Details des Validierers bearbeiten (3) - ermöglicht die Bearbeitung des Anzeigenamens, der Rolle des Testversands und der E-Mail-Warnung für diesen Validierer.
* Machen Sie sie zum Inhaber des Testversands (4)
* Machen Sie sie zum wichtigsten Entscheidungsträger (5)
* Aus dem Testversand entfernen (6)

>[!NOTE]
>
>Die Sichtbarkeit dieser Optionen hängt von Ihren Berechtigungen für den Testversand ab (siehe [Profile für Testversandberechtigungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) und [Rollen in Testsendungen verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

![reviewer_actions_menu.png](assets/reviewer-actions-menu-350x135.png)

### Menü &quot;Proof Actions&quot; {#proof-actions-menu}

Jeder Testversand verfügt außerdem über ein Menü (1), mit dem Sie die folgenden Aktionen durchführen können:

* Sie können auf die Seite mit Details zum Testversand (2) zugreifen.
* Testversand mit anderen Personen teilen (3)
* Nachricht an die validierungsverantwortlichen Benutzer senden (4)
* Erstellen einer neuen Testversion (5)
* Testversand kopieren (6)
* Originaldatei herunterladen (7)
* Freigeben von Testversand-Links (8)
* Kommentare drucken (9)
* Anfordern einer Excel-Zusammenfassung des Testversands (10)
* Testversand sperren (11)
* Testversand löschen (12)

![Proof_actions_menu_1_.png](assets/proof-actions-menu--1--350x158.png)

>[!NOTE]
>
>Die Verfügbarkeit dieser Optionen hängt von Ihren Berechtigungen für den Testversand ab (siehe [Profile für Testversandberechtigungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) und [Rollen in Testsendungen verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md)).

Informationen zum Anzeigen des Testversands-Fortschritts und -Status innerhalb von [!DNL Workfront] finden Sie unter [Anzeigen von Fortschritt und Status](#viewing-progress-and-status).

Informationen zum Anzeigen des Fortschritts und Status im Viewer für die Desktop-Prüfung finden Sie unter [Überprüfen eines Workflows im Testversand-Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-workflow.md).
