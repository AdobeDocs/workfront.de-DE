---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Erstellen und Verwalten von automatisierten Workflow-Vorlagen
description: Wenn als Adobe Workfront-Administrator der Prozess zur Inhaltsüberprüfung Ihres Unternehmens häufig wiederholt wird oder Inhalte häufig von denselben Personen geprüft werden, können Sie automatisierte Workflow-Vorlagen erstellen, die diese Reviewer mit von Ihnen angegebenen Korrekturabzugsrollen und Benachrichtigungseinstellungen enthalten. Eine automatisierte Workflow-Vorlage kann mit nur einem oder zwei Validierungsverantwortlichen einfach oder komplex mit vielen Phasen und Abhängigkeiten sein.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: 7a2cfddf4683b5b49121bbe3987498297b963ffa
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# Erstellen und Verwalten von automatisierten Workflow-Vorlagen

<!-- Audited: 2/2024 -->

Wenn als Adobe Workfront-Administrator der Prozess zur Inhaltsüberprüfung Ihres Unternehmens häufig wiederholt wird oder Inhalte häufig von denselben Personen geprüft werden, können Sie automatisierte Workflow-Vorlagen erstellen, die diese Reviewer mit von Ihnen angegebenen Korrekturabzugsrollen und Benachrichtigungseinstellungen enthalten. Eine automatisierte Workflow-Vorlage kann mit nur einem oder zwei Validierungsverantwortlichen einfach oder komplex mit vielen Phasen und Abhängigkeiten sein.

Automatisierte Workflow-Vorlagen erleichtern die Erstellung eines Korrekturabzugs mit einem automatisierten Workflow. Wenn ein(e) Benutzende(r) einen Korrekturabzug erstellt, wählt er/sie einfach die gewünschte Vorlage aus.

Sie können jede automatisierte Workflow-Vorlage jederzeit ändern, Reviewer und Phasen hinzufügen oder entfernen. Und Korrekturabzug-Ersteller, die die Vorlage verwenden, können Prüfer für den Korrekturabzug hinzufügen oder entfernen.

Beachten Sie bei der Verwendung einer automatisierten Workflow-Vorlage Folgendes:

1. Die Einstellungen einer automatisierten Workflow-Vorlage bestimmen, was Sie mit dem automatisierten Workflow für einen Korrekturabzug tun können. Wenn zum Beispiel die Schaltfläche Schritt hinzufügen in der Vorlage deaktiviert ist, wird sie nicht angezeigt, wenn Sie mit den Einstellungen des automatisierten Workflows für den Korrekturabzug arbeiten.
1. Wenn eine Person zu einem Schritt in einer automatisierten Workflow-Vorlage hinzugefügt wird, aber auch bereits als Prüferin bzw. Prüfer im Korrekturabzug vorhanden ist, wird sie durch Anwenden der Vorlage von dem Schritt entfernt. Wenn Sie keinen weiteren Validierungsverantwortlichen zum Schritt hinzufügen, werden Sie in einer Meldung aufgefordert, einen hinzuzufügen.
1. Ihre Möglichkeit, eine Vorlage für einen automatisierten Workflow zu ändern, hängt von den Vorlageneinstellungen ab, die vom Workfront-Administrator konfiguriert wurden, wie in beschrieben. Wenn die Möglichkeit, die Vorlage zu ändern, deaktiviert ist, kann nur der Besitzer der Vorlage sie ändern.

Informationen zu automatisierten Workflows finden Sie unter [Automatisierter Workflow - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Neu: Beliebig</p><p>Aktuell: Pro oder höher</p><p>Legacy: Premium oder Select</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p><p>Aktuell: Arbeit oder Plan</p> <p>Legacy: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>In Ihrem Profil für Korrekturabzugsberechtigungen muss „Administrator“ ausgewählt sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer automatisierten Workflow-Vorlage

{{step1-to-proofing}}

1. Klicken Sie **linken** auf „Workflows“.
1. Klicken Sie auf der **Workflow**-Registerkarte auf **Neu** > **Neue Vorlage**.

1. Geben **im Abschnitt** die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vorlagenname</td> 
      <td>(Erforderlich) Geben Sie einen Namen für Ihre Vorlage ein. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inhaber der Vorlage</td> 
      <td>Sie können den Workfront-Administrator oder den Workfront Proof-Administrator auswählen, der die Vorlage verwalten soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorlagengruppe</td> 
      <td> <p> Wenn die automatisierten Workflows Ihres Unternehmens in Gruppen unterteilt sind, können Sie den Namen der Gruppe auswählen. Weitere Informationen <a href="#create-automated-workflow-template-groups" class="MCXref xref"> Sie unter „Erstellen automatisierter Workflow</a>Vorlagengruppen“ weiter unten in diesem Artikel.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Zeitzonen-Vorlage </td> 
      <td> <p>Die Standardzeitzone für die Vorlage ist die Zeitzone, in der Sie arbeiten. Wenn die Zeitzone der Ersteller und Prüfer von Korrekturabzügen, die die Vorlage verwenden werden, unterschiedlich ist, können Sie sie hier ändern, um sicherzustellen, dass die Staging-Fristen für diese Benutzer zur richtigen Zeit festgelegt werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">zulassen</td> 
      <td> <p>Sie können die Staging-Aktivitäten auswählen, die Sie der Person, die einen Testversand erstellt, zur Verfügung stellen möchten, indem Sie die Vorlage verwenden.</p> 
      <p><b>WARNUNG</b>: Wenn Sie die Optionen Phase hinzufügen und Personen zu Phasen hinzufügen nicht auswählen, können weder der Vorlagenbesitzer noch der Besitzer eines Korrekturabzugs, der diese Vorlage verwendet, einen Schritt hinzufügen oder den Korrekturabzug freigeben. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Konfigurieren Sie **Abschnitt** Phasen“ jede Phase der automatisierten Workflow-Vorlage.

   Sie können mehrere Phasen hinzufügen und zwischen ihnen erstellen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Der Name des Stadiums wird im Diagramm Automatisierter Workflow oben im Workflow-Abschnitt, auf der Seite mit den Korrekturabzugsdetails und in den E-Mail-Benachrichtigungen angezeigt, die an die Validierungsverantwortlichen gesendet werden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Phase aktivieren</td> 
      <td> <p>Geben Sie an, ob der Schritt automatisch oder manuell aktiviert werden soll. Im ersten Schritt können Sie "<strong> Korrekturabzugs-Erstellung</strong>, <strong>An einem bestimmten Datum und zu einer bestimmten Uhrzeit</strong> oder <strong>Manuell</strong> auswählen.</p> <p>Die anderen Optionen werden verfügbar, wenn Sie ein zweites Stadium hinzufügen, da Sie dafür ein übergeordnetes Stadium auswählen müssen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deadline calculated from</td> 
      <td> <p>Geben Sie an, wie die Frist berechnet werden soll:</p> 
       <ul> 
        <li> <p><strong>Testversand-Erstellung</strong>: Wählen Sie in der Dropdown-Liste unter <strong>Frist (+ Werktage)</strong> die Anzahl der Werktage aus, die Sie zum Erstellungsdatum des Testversands hinzufügen möchten, um automatisch eine Frist für den Testversand festzulegen.</p> </li> 
        <li><strong>Wenn die Phase beginnt</strong>: Wählen Sie in der Dropdown-Liste unter <strong>Frist (+ Werktage)</strong> die Anzahl der Werktage aus, die Sie zum Aktivierungsdatum der Phase hinzufügen möchten, um automatisch eine Frist für den Korrekturabzug festzulegen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schleusenbühne</td> 
      <td>Geben Sie an, ob die Phase für Kommentare gesperrt werden soll. Die Optionen bestehen darin, eine Phase manuell oder automatisch zu sperren, entweder beim Start der nächsten Phase oder wenn alle Entscheidungen auf der übergeordneten Phase getroffen werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Primärer Entscheidungsträger</td> 
      <td> <p>Die verfügbaren Entscheidungsträger werden erst dann in der Liste angezeigt, nachdem Sie die Reviewer zur Phase hinzugefügt haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur eine Entscheidung erforderlich</td> 
      <td>Der Überprüfungsprozess für die Phase wird abgeschlossen, sobald einer der Entscheidungsträger seine Entscheidung vorlegt. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurieren der Testversandeinstellungen in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Private Bühne</td> 
      <td>Blendet Kommentare und Entscheidungen aus für Personen aus, die nicht zur Phase hinzugefügt wurden oder keine Workfront-Administratoren sind. Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Automatisierter Workflow - Übersicht</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schritt nicht löschen lassen</td> 
      <td> <p>Macht die Phase obligatorisch.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Wenn die Korrekturabzüge, die diese Vorlage verwenden werden, immer an dieselben Personen in der Phase gesendet werden, fügen Sie sie hier hinzu, damit Benutzer sie nicht jedes Mal hinzufügen müssen, wenn sie einen Korrekturabzug erstellen.

   Wählen Sie auf den Testsendungen **die Rollen der einzelnen Personen aus** für die diese Vorlage verwendet wird, und wählen Sie die **E-Mail-Benachrichtigungen**, die der/die Benutzende bei der Arbeit an Testsendungen erhalten soll, die diese Vorlage verwenden.

   Informationen zu Rollen für einen Korrekturabzug finden Sie unter [Standard-Proofing-Rollen konfigurieren](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Informationen zu E-Mail-Warnhinweisen für Korrekturabzüge finden Sie im Abschnitt [Konfigurieren von Standardeinstellungen für Korrekturabzüge für ](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) im Artikel [Konfigurieren von E-Mail-Benachrichtigungseinstellungen in Workfront Proof](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Jeder Benutzer kann nur zu einem Schritt hinzugefügt werden. Sie können beliebig viele Benutzer zu einem Schritt hinzufügen.

   >[!TIP]
   >
   >Sie können Reviewer-Namen per Drag-and-Drop zwischen Phasen auf das Phasen-Diagramm ziehen. Verfügbare Stadien sind blau hervorgehoben.

1. Wiederholen Sie die beiden vorherigen Schritte für alle weiteren Schritte, die Sie der Vorlage hinzufügen möchten.

   Oben im Abschnitt **Workflow** wird ein Diagramm des automatisierten Workflows angezeigt, den Sie einrichten. Wenn Sie weitere Stadien hinzufügen, werden diese im Diagramm mit Zeilen angezeigt, die die Abhängigkeiten zwischen ihnen anzeigen. Sie können auf eine Phase im Diagramm klicken, um die Einstellungen für diese Phase anzuzeigen.

   Wenn Sie das Diagramm nicht sehen müssen, können Sie auf &quot;**&quot;**.

1. Klicken Sie im Abschnitt **Vorlage freigeben für** auf eine Option (wenn die Vorlage noch nicht für die gesamte Organisation freigegeben ist), um anzugeben, wer sie verwenden kann.

   Standardmäßig werden neue automatisierte Workflow-Vorlagen für alle Personen in Ihrer Organisation freigegeben.

1. Klicken Sie auf **Erstellen**.

## Ändern einer automatisierten Workflow-Vorlage

Als Workfront Proof-Administrator können Sie eine Vorlage für einen automatisierten Workflow ändern. Ihre Änderungen werden automatisch gespeichert, sobald Sie sie vornehmen.

{{step1-to-proofing}}

1. Klicken Sie **linken** auf „Workflows“.
1. Klicken Sie in **angezeigten** „Workflow-Vorlagen“ auf die Vorlage, die Sie ändern möchten.
1. Geben **im Abschnitt** die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vorlagenname</td> 
      <td>(Erforderlich) Geben Sie einen Namen für Ihre Vorlage ein. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inhaber der Vorlage</td> 
      <td>Sie können den Workfront-Administrator oder den Workfront Proof-Administrator auswählen, der die Vorlage verwalten soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorlagengruppe</td> 
      <td> <p> Wenn die automatisierten Workflows Ihres Unternehmens in Gruppen unterteilt sind, können Sie den Namen der Gruppe auswählen. Weitere Informationen <a href="#create-automated-workflow-template-groups" class="MCXref xref"> Sie unter „Erstellen automatisierter Workflow</a>Vorlagengruppen“ weiter unten in diesem Artikel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeitzonen-Vorlage </td> 
      <td> <p>Die Standardzeitzone für die Vorlage ist die Zeitzone, in der Sie arbeiten. Wenn die Zeitzone der Ersteller und Prüfer von Korrekturabzügen, die die Vorlage verwenden werden, unterschiedlich ist, können Sie sie hier ändern, um sicherzustellen, dass die Staging-Fristen für diese Benutzer zur richtigen Zeit festgelegt werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">zulassen</td> 
      <td> <p>Wählen Sie die Staging-Aktivitäten aus, die denjenigen Benutzern zur Verfügung stehen sollen, die Korrekturabzüge mithilfe der Vorlage erstellen. </p> <p><b>WARNUNG</b>: Wenn Sie die Optionen Phase hinzufügen und Personen zu Phasen hinzufügen nicht auswählen, können weder der Vorlagenbesitzer noch der Besitzer eines Korrekturabzugs, der diese Vorlage verwendet, einen Schritt hinzufügen oder den Korrekturabzug freigeben.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Ändern **im Abschnitt „Workflow** den Namen eines beliebigen Schritts und erweitern Sie seine Einstellungen, ![](assets/arrow-button.png) alle erforderlichen Änderungen vorzunehmen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Deadline calculated from</td> 
      <td> <p>Geben Sie an, wie die Frist berechnet werden soll:</p> 
       <ul> 
        <li> <p><strong>Frist berechnet aus der Erstellung eines Korrekturabzugs</strong>: Wählen Sie in der Dropdown-Liste <strong>Frist für die Phase festlegen</strong> die Anzahl der Werktage aus, die Sie zum Erstellungsdatum des Korrekturabzugs hinzufügen möchten, um automatisch eine Frist für den Korrekturabzug festzulegen.</p> </li> 
        <li><strong>Frist berechnet aus Staging-Aktivierung</strong>: Wählen Sie in der Dropdown-Liste <strong>Staging-Frist festlegen</strong> die Anzahl der Werktage aus, die Sie zum Staging-Aktivierungsdatum hinzufügen möchten, um automatisch eine Frist für den Korrekturabzug festzulegen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Phase aktivieren</td> 
      <td> <p>Geben Sie an, ob der Schritt automatisch oder manuell aktiviert werden soll. Im ersten Schritt können Sie "<strong> Korrekturabzugs-Erstellung</strong>, <strong>An einem bestimmten Datum und zu einer bestimmten Uhrzeit</strong> oder <strong>Manuell</strong> auswählen.</p> <p>Die anderen Optionen werden verfügbar, wenn Sie ein zweites Stadium hinzufügen, da Sie dafür ein übergeordnetes Stadium auswählen müssen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Schleusenbühne</td> 
      <td>Geben Sie an, ob die Phase für Kommentare gesperrt werden soll. Die Optionen bestehen darin, eine Phase manuell oder automatisch zu sperren, entweder beim Start der nächsten Phase oder wenn alle Entscheidungen auf der übergeordneten Phase getroffen werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidung</td> 
      <td>Beendet die Phase, wenn einer der Entscheidungsträger seine Entscheidung zum ersten Mal einreicht. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurieren der Testversandeinstellungen in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">DATENSCHUTZ</td> 
      <td>Blendet Kommentare und Entscheidungen aus für Personen aus, die nicht zur Phase hinzugefügt werden oder die nicht Supervisoren und höher im Konto sind. Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Automatisierter Workflow - Übersicht</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Staging-Löschung</td> 
      <td>Macht die Phase obligatorisch.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mehr <img src="assets/more-icon.png"></td> 
      <td>Fügen Sie Reviewer zur Phase hinzu oder löschen Sie die Phase.<p>Wenn jeder Korrekturabzug in einem bestimmten Schritt an dieselben Personen gesendet wird, können Sie seinen Namen hier angeben, damit Sie ihn nicht jedes Mal hinzufügen müssen, wenn Sie einen Korrekturabzug erstellen. Geben Sie den Namen eines Benutzers ein, den Sie der Phase hinzufügen möchten, wählen Sie ihn aus und fügen Sie dann <strong>Rolle</strong> zu den Einstellungen für den Korrekturabzug und <strong>E-Mail</strong>Warnungen hinzu, die Sie für den Benutzer verwenden möchten. Informationen zu Proofing-Rollen finden Sie <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Konfigurieren von Standard-Proofing-Rollen</a>. Informationen zu E-Mail-Warnhinweisen für Korrekturabzüge finden Sie im Abschnitt <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Konfigurieren von Standardeinstellungen für Korrekturabzüge für </a> im Artikel <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">Konfigurieren von E-Mail-Benachrichtigungseinstellungen in Workfront Proof</a>.</p><p>Sie können beliebig viele Benutzer zu einem Schritt hinzufügen</p><p>Tipp: Sie können die Namen von Validierungsverantwortlichen per Drag-and-Drop zwischen den Phasen auf das Phasen-Diagramm ziehen. Verfügbare Stadien sind blau hervorgehoben.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Wiederholen Sie diesen Schritt für alle weiteren Schritte, die Sie der Vorlage hinzufügen möchten.

   Oben im Abschnitt **Workflow** wird ein Diagramm des automatisierten Workflows angezeigt, den Sie einrichten. Wenn Sie weitere Stadien hinzufügen, werden diese im Diagramm mit Zeilen angezeigt, die die Abhängigkeiten zwischen ihnen anzeigen. Sie können auf eine Phase im Diagramm klicken, um die Einstellungen für diese Phase anzuzeigen.

   Wenn Sie das Diagramm nicht sehen müssen, können Sie auf &quot;**&quot;**.

1. Wenn Sie **Benutzer im Abschnitt** Freigegeben für“ löschen möchten, klicken Sie auf die Schaltfläche Mehr ![](assets/more-icon.png) rechts und anschließend auf **Entfernen**.

## Erstellen von automatisierten Workflow-Vorlagengruppen {#create-automated-workflow-template-groups}

Als Workfront-Administrator können Sie alle automatisierten Workflow-Vorlagen im Konto Ihres Unternehmens anzeigen und verwalten. Es kann hilfreich sein, Vorlagen in Gruppen zu organisieren.

So erstellen Sie eine automatisierte Workflow-Vorlagengruppe:

{{step1-to-proofing}}

1. Klicken Sie **linken** auf „Workflows“.
1. Klicken Sie auf der **Workflow**-Registerkarte auf **Neu** > **Neue Vorlagengruppe**.
1. Geben Sie einen beschreibenden Namen für die neue Vorlagengruppe ein und drücken Sie dann die **Eingabetaste**.

Sie können die Vorlagen durch Ziehen und Ablegen zwischen Gruppen verschieben.

## Verwalten von automatisierten Workflow-Vorlagen

{{step1-to-proofing}}

1. Klicken Sie im linken Bedienfeld in Workfront Proof auf **Workflows**.
1. Führen Sie auf **angezeigten** „Workflows“ einen der folgenden Schritte aus:

   * Neue Vorlage hinzufügen
   * Hinzufügen einer neuen Vorlagengruppe
   * Eine oder mehrere Vorlagengruppen löschen
   * Zugriff auf Vorlagendetails
   * Ziehen einer Vorlage in eine andere Vorlagengruppe
