---
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Erstellen und Verwalten von Vorlagen für automatisierte Workflows
description: Wenn als Adobe Workfront-Administrator der Inhaltsüberprüfungsprozess Ihres Unternehmens häufig wiederholt wird oder Inhalte häufig von denselben Personen geprüft werden, können Sie automatisierte Workflow-Vorlagen erstellen, die die validierungsverantwortlichen Benutzer mit von Ihnen festgelegten Testversandrollen und Benachrichtigungseinstellungen enthalten. Eine Automated Workflow-Vorlage kann einfach mit nur einem oder zwei Validierungsverantwortlichen oder komplex mit vielen Phasen und Abhängigkeiten sein.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: a9f182c0-11cb-4e94-be86-b19ba5102faa
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '2075'
ht-degree: 0%

---

# Erstellen und Verwalten von Vorlagen für automatisierte Workflows

<!-- Audited: 2/2024 -->

Wenn als Adobe Workfront-Administrator der Inhaltsüberprüfungsprozess Ihres Unternehmens häufig wiederholt wird oder Inhalte häufig von denselben Personen geprüft werden, können Sie automatisierte Workflow-Vorlagen erstellen, die die validierungsverantwortlichen Benutzer mit von Ihnen festgelegten Testversandrollen und Benachrichtigungseinstellungen enthalten. Eine Automated Workflow-Vorlage kann einfach mit nur einem oder zwei Validierungsverantwortlichen oder komplex mit vielen Phasen und Abhängigkeiten sein.

Automatisierte Workflow-Vorlagen erleichtern die Erstellung eines Testversands mit einem automatisierten Workflow. Wenn ein Benutzer einen Testversand erstellt, wählt er einfach die Vorlage aus, die er benötigt.

Sie können jederzeit problemlos jede Automated Workflow-Vorlage ändern, indem Sie Überprüfer und Phasen hinzufügen oder entfernen. Und Testversand-Ersteller, die die Vorlage verwenden, können Überprüfer für den Testversand hinzufügen oder entfernen.

Beachten Sie Folgendes, wenn Sie eine Vorlage für einen automatisierten Workflow verwenden:

1. Die Einstellungen einer Automated Workflow-Vorlage bestimmen, was Sie mit dem automatisierten Workflow für einen Testversand tun können. Wenn beispielsweise die Schaltfläche Phase hinzufügen in der Vorlage deaktiviert ist, ist sie nicht sichtbar, wenn Sie mit den Einstellungen für den automatisierten Workflow für den Testversand arbeiten.
1. Wenn eine Person in einer Vorlage für einen automatisierten Workflow zu einer Nutzung hinzugefügt, aber bereits als Validierer für den Testversand vorhanden ist, wird der Validierer durch Anwendung der Vorlage aus der Bühne entfernt. Wenn Sie keinen weiteren Validierer zur Bühne hinzufügen, werden Sie in einer Meldung aufgefordert, einen hinzuzufügen.
1. Ihre Fähigkeit, eine Vorlage für einen automatisierten Workflow zu ändern, hängt von den vom Workfront-Administrator konfigurierten Vorlageneinstellungen ab, wie in beschrieben. Wenn die Möglichkeit zur Änderung der Vorlage deaktiviert ist, kann sie nur vom Inhaber der Vorlage geändert werden.

Informationen zu automatisierten Workflows finden Sie unter [Übersicht über den automatisierten Workflow](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Neu: Beliebig</p><p>Aktuell: Pro oder höher</p><p>Veraltet: Premium oder Select</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Neu: Standard</p><p>Aktuell: Arbeit oder Plan</p> <p>Veraltet: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>In Ihrem Profil für Testberechtigungen muss "Administrator"ausgewählt sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Automated Workflow-Vorlage

{{step1-to-proofing}}

1. Klicks **Workflows** im linken Bereich.
1. Im **Workflow** Registerkarte, klicken **Neu** > **Neue Vorlage**.

1. Im **Details** Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vorlagenname</td> 
      <td>(Erforderlich) Geben Sie einen Namen für Ihre Vorlage ein. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorlageninhaber</td> 
      <td>Sie können den Workfront-Administrator oder Workfront Proof-Administrator auswählen, der die Vorlage verwaltet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorlagengruppe</td> 
      <td> <p> Wenn die automatisierten Workflows Ihres Unternehmens in Gruppen unterteilt sind, können Sie den Namen der Gruppe auswählen. Siehe <a href="#create-automated-workflow-template-groups" class="MCXref xref">Erstellen von Vorlagengruppen für automatisierte Workflows</a> später in diesem Artikel für weitere Informationen.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Zeitzonen-Vorlage </td> 
      <td> <p>Die standardmäßige Zeitzone für die Vorlage ist diejenige, in der Sie arbeiten. Wenn die Zeitzone der Testversand-Ersteller und -validierer, die die Vorlage verwenden werden, unterschiedlich ist, können Sie sie hier ändern, um sicherzustellen, dass die Bereitstellungsfristen für diese Benutzer zum richtigen Zeitpunkt festgelegt werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zulassen</td> 
      <td> <p>Sie können die Staging-Aktivitäten auswählen, die der Person, die Testsendungen erstellt, mit der Vorlage zur Verfügung stehen sollen.</p> 
      <p><b>WARNUNG</b>: Wenn Sie die Optionen Phase hinzufügen und Personen zu Bühnen hinzufügen nicht auswählen, können weder der Vorlageninhaber noch der Besitzer eines Testversands, der diese Vorlage verwendet, eine Bühne hinzufügen oder den Testversand freigeben. 
      </p>
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Im **Phasen** konfigurieren Sie die einzelnen Phasen der Vorlage &quot;Automatisierter Workflow&quot;.

   Sie können mehrere Bühnen hinzufügen und zwischen ihnen erstellen.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td> <p>Der Staging-Name wird im Diagramm Automatisierter Workflow oben im Abschnitt Workflow , auf der Seite Testversanddetails und in den an die Validierer gesendeten E-Mail-Benachrichtigungen angezeigt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Phase aktivieren</td> 
      <td> <p>Geben Sie an, ob die Bühne automatisch oder manuell aktiviert wird. Im ersten Schritt können Sie <strong>Erstellen eines Testversands</strong>, <strong>An einem bestimmten Datum und zu einer bestimmten Uhrzeit</strong>oder <strong>Manuell</strong>.</p> <p>Die anderen Optionen werden verfügbar, wenn Sie eine zweite Phase hinzufügen, da Sie eine übergeordnete Phase auswählen müssen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Errechneter Termin</td> 
      <td> <p>Geben Sie an, wie der Termin berechnet werden soll:</p> 
       <ul> 
        <li> <p><strong>Erstellung von Testsendungen</strong>: In der Dropdownliste unter <strong>Termin (+ Geschäftstage)</strong>wählen Sie die Anzahl der Geschäftstage aus, die Sie dem Erstellungsdatum des Testversands hinzufügen möchten, um automatisch einen Termin für den Testversand festzulegen.</p> </li> 
        <li><strong>Wenn die Phase beginnt</strong>: In der Dropdownliste unter <strong>Termin (+ Geschäftstage)</strong>wählen Sie die Anzahl der Geschäftstage aus, die Sie dem Aktivierungsdatum der Bühne hinzufügen möchten, um automatisch einen Termin für den Testversand festzulegen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bühne sperren</td> 
      <td>Geben Sie an, ob die Bühne für Kommentare gesperrt werden soll. Die Optionen bestehen darin, eine Phase manuell oder automatisch zu sperren, entweder wenn die nächste Phase beginnt oder wenn alle Entscheidungen auf der übergeordneten Phase getroffen werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Primärer Entscheidungsträger</td> 
      <td> <p>Die verfügbaren Entscheidungsträger werden erst in der Liste angezeigt, nachdem Sie die Prüfer zur Bühne hinzugefügt haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nur eine Entscheidung erforderlich</td> 
      <td>Der Überprüfungsprozess für die Phase wird abgeschlossen, sobald einer der Entscheidungsträger seine Entscheidung vorlegt. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurieren der Testversandeinstellungen in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Private Bühne</td> 
      <td>Blendet Kommentare und Entscheidungen von für Personen aus, die nicht zur Bühne hinzugefügt werden oder keine Workfront-Administratoren sind. Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Übersicht über den automatisierten Workflow</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Löschen dieser Phase nicht zulassen</td> 
      <td> <p>Macht die Bühne obligatorisch.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Wenn die Testsendungen, die diese Vorlage verwenden, immer an dieselben Personen in der Bühne gesendet werden, fügen Sie sie hier hinzu, damit Benutzer sie nicht jedes Mal hinzufügen müssen, wenn sie einen Testversand erstellen.

   Wählen Sie die **Rolle** für die Testsendungen, die diese Vorlage verwenden, und die **E-Mail-Warnungen** Sie möchten, dass der Benutzer beim Arbeiten an Testsendungen, die diese Vorlage verwenden, erhält.

   Informationen zu den Rollen bei einem Testversand finden Sie unter [Konfigurieren von standardmäßigen Testrollen](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md). Informationen zu Testversand-E-Mail-Warnungen finden Sie im Abschnitt [Konfigurieren der Standardwerte für den Testversand eines Benutzers](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur) im Artikel  [E-Mail-Benachrichtigungseinstellungen in Workfront Proof konfigurieren](../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Jeder Benutzer kann nur einer Phase hinzugefügt werden. Sie können so viele Benutzer hinzufügen, wie Sie für eine Bühne benötigen.

   >[!TIP]
   >
   >Sie können Überprüfernamen per Drag-and-Drop zwischen Phasen in das Bühnen-Diagramm ziehen. Die verfügbaren Bühnen sind blau hervorgehoben.

1. Wiederholen Sie die beiden vorherigen Schritte für alle anderen Schritte, die Sie zur Vorlage hinzufügen möchten.

   Oben im **Workflow** angezeigt, können Sie ein Diagramm des von Ihnen eingerichteten automatisierten Workflows sehen. Während Sie weitere Bühnen hinzufügen, werden diese im Diagramm mit Linien angezeigt, die die Abhängigkeiten zwischen ihnen zeigen. Sie können auf eine Bühne im Diagramm klicken, um die Einstellungen für diese Bühne anzuzeigen.

   Wenn Sie das Diagramm nicht sehen müssen, können Sie auf **Diagramm ausblenden**.

1. Im **Vorlage freigeben für** auf eine Option klicken (sofern die Vorlage noch nicht für die gesamte Organisation freigegeben wurde), um anzugeben, wer sie verwenden kann.

   Standardmäßig werden neue Automated Workflow-Vorlagen für alle Mitarbeiter in Ihrem Unternehmen freigegeben.

1. Klicken Sie auf **Erstellen**.

## Ändern einer Automated Workflow-Vorlage

Als Workfront Proof-Administrator können Sie eine Vorlage für den automatisierten Workflow ändern. Ihre Änderungen werden automatisch gespeichert, wenn Sie sie vornehmen.

{{step1-to-proofing}}

1. Klicks **Workflows** im linken Bereich.
1. Im **Workflow-Vorlagen** angezeigt wird, klicken Sie auf die Vorlage, die Sie ändern möchten.
1. Im **Details** Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Vorlagenname</td> 
      <td>(Erforderlich) Geben Sie einen Namen für Ihre Vorlage ein. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorlageninhaber</td> 
      <td>Sie können den Workfront-Administrator oder Workfront Proof-Administrator auswählen, der die Vorlage verwaltet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vorlagengruppe</td> 
      <td> <p> Wenn die automatisierten Workflows Ihres Unternehmens in Gruppen unterteilt sind, können Sie den Namen der Gruppe auswählen. Siehe <a href="#create-automated-workflow-template-groups" class="MCXref xref">Erstellen von Vorlagengruppen für automatisierte Workflows</a> später in diesem Artikel für weitere Informationen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeitzonen-Vorlage </td> 
      <td> <p>Die standardmäßige Zeitzone für die Vorlage ist diejenige, in der Sie arbeiten. Wenn die Zeitzone der Testversand-Ersteller und -validierer, die die Vorlage verwenden werden, unterschiedlich ist, können Sie sie hier ändern, um sicherzustellen, dass die Bereitstellungsfristen für diese Benutzer zum richtigen Zeitpunkt festgelegt werden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zulassen</td> 
      <td> <p>Wählen Sie die Staging-Aktivitäten aus, die Benutzern, die mithilfe der Vorlage Testsendungen erstellen, zur Verfügung stehen sollen. </p> <p><b>WARNUNG</b>: Wenn Sie die Optionen Phase hinzufügen und Personen zu Bühnen hinzufügen nicht auswählen, können weder der Vorlageninhaber noch der Besitzer eines Testversands, der diese Vorlage verwendet, eine Bühne hinzufügen oder den Testversand freigeben.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Im **Workflow** ändern Sie den Namen einer Phase und erweitern Sie die Einstellungen ![](assets/arrow-button.png) um erforderliche Änderungen vorzunehmen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Errechneter Termin</td> 
      <td> <p>Geben Sie an, wie der Termin berechnet werden soll:</p> 
       <ul> 
        <li> <p><strong>Aus der Erstellung des Testversands berechnete Frist</strong>: Im <strong>Festlegen des Staging-Termins</strong> in der Dropdown-Liste die Anzahl der Geschäftstage auswählen, die Sie zum Erstellungsdatum des Testversands hinzufügen möchten, um automatisch einen Termin für den Testversand festzulegen.</p> </li> 
        <li><strong>Von der Staging-Aktivierung berechnete Frist</strong>: Im <strong>Festlegen des Staging-Termins</strong> in der Dropdown-Liste die Anzahl der Geschäftstage auswählen, die Sie zum Aktivierungsdatum der Bühne hinzufügen möchten, um automatisch einen Termin für den Testversand festzulegen.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Phase aktivieren</td> 
      <td> <p>Geben Sie an, ob die Bühne automatisch oder manuell aktiviert wird. Im ersten Schritt können Sie <strong>Erstellen eines Testversands</strong>, <strong>An einem bestimmten Datum und zu einer bestimmten Uhrzeit</strong>oder <strong>Manuell</strong>.</p> <p>Die anderen Optionen werden verfügbar, wenn Sie eine zweite Phase hinzufügen, da Sie eine übergeordnete Phase auswählen müssen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bühne sperren</td> 
      <td>Geben Sie an, ob die Bühne für Kommentare gesperrt werden soll. Die Optionen bestehen darin, eine Phase manuell oder automatisch zu sperren, entweder wenn die nächste Phase beginnt oder wenn alle Entscheidungen auf der übergeordneten Phase getroffen werden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidung</td> 
      <td>Beendet die Phase, wenn ein Entscheidungsträger seine Entscheidung zum ersten Mal vorlegt. Weitere Informationen finden Sie unter <a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Konfigurieren der Testversandeinstellungen in Workfront Proof</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datenschutz</td> 
      <td>Blendet Kommentare und Entscheidungen von an Personen aus, die nicht zur Bühne hinzugefügt werden oder die keine Supervisoren und höher im Konto sind. Weitere Informationen finden Sie unter <a href="../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md" class="MCXref xref">Übersicht über den automatisierten Workflow</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Staging-Löschen</td> 
      <td>Macht die Bühne obligatorisch.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mehr <img src="assets/more-icon.png"></td> 
      <td>Fügen Sie Überprüfer zur Bühne hinzu oder löschen Sie die Bühne.<p>Wenn jeder Ihrer Testsendungen an dieselben Personen in einer bestimmten Phase gesendet wird, können Sie hier seinen Namen angeben, damit Sie ihn nicht jedes Mal hinzufügen müssen, wenn Sie einen Testversand erstellen. Geben Sie den Namen eines Benutzers ein, den Sie der Bühne hinzufügen möchten, und fügen Sie dann dessen <strong>Rolle</strong> auf den Nachweis und <strong>E-Mail-Warnungen</strong> -Einstellungen, die Sie für den Benutzer wünschen. Informationen zu Testing-Rollen finden Sie unter <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md" class="MCXref xref">Konfigurieren von standardmäßigen Testrollen</a>. Informationen zu Testversand-E-Mail-Warnungen finden Sie im Abschnitt <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md#configur" class="MCXref xref">Konfigurieren der Standardwerte für den Testversand eines Benutzers</a> im Artikel <a href="../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md" class="MCXref xref">E-Mail-Benachrichtigungseinstellungen in Workfront Proof konfigurieren</a>.</p><p>Sie können so viele Benutzer hinzufügen, wie Sie möchten</p><p>Tipp: Sie können Überprüfernamen per Drag-and-Drop zwischen Bühnen in das Bühnen-Diagramm ziehen. Die verfügbaren Bühnen sind blau hervorgehoben.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Wiederholen Sie den Schritt für alle anderen Phasen, die Sie der Vorlage hinzufügen möchten.

   Oben im **Workflow** angezeigt, können Sie ein Diagramm des von Ihnen eingerichteten automatisierten Workflows sehen. Während Sie weitere Bühnen hinzufügen, werden diese im Diagramm mit Linien angezeigt, die die Abhängigkeiten zwischen ihnen zeigen. Sie können auf eine Bühne im Diagramm klicken, um die Einstellungen für diese Bühne anzuzeigen.

   Wenn Sie das Diagramm nicht sehen müssen, können Sie auf **Diagramm ausblenden**.

1. Im **Freigegeben für** zum Löschen eines Benutzers auf Mehr klicken ![](assets/more-icon.png) Schaltfläche rechts und klicken Sie dann auf **Entfernen**.

## Erstellen von Vorlagengruppen für automatisierte Workflows {#create-automated-workflow-template-groups}

Als Workfront-Administrator können Sie alle Automated Workflow-Vorlagen im Konto Ihres Unternehmens anzeigen und verwalten. Es kann hilfreich sein, Vorlagen in Gruppen zu organisieren.

So erstellen Sie eine Vorlagengruppe für einen automatisierten Workflow:

{{step1-to-proofing}}

1. Klicks **Workflows** im linken Bereich.
1. Im **Workflow** Registerkarte, klicken **Neu** > **Neue Vorlagengruppe**.
1. Geben Sie einen beschreibenden Namen für die neue Vorlagengruppe ein und drücken Sie dann die Eingabetaste **Eingabe**.

Sie können die Vorlagen durch Ziehen und Ablegen zwischen Gruppen verschieben.

## Verwalten von Vorlagen für automatisierte Workflows

{{step1-to-proofing}}

1. Klicken Sie im linken Bereich in Workfront Proof auf **Workflows**.
1. Im **Workflows** -Seite angezeigt wird, führen Sie einen der folgenden Schritte aus:

   * Neue Vorlage hinzufügen
   * Neue Vorlagengruppe hinzufügen
   * Eine oder mehrere Vorlagengruppen löschen
   * Zugriff auf die Details einer Vorlage
   * Ziehen Sie eine Vorlage in eine andere Vorlagengruppe
