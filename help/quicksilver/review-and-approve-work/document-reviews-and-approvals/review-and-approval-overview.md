---
product-area: documents
navigation-topic: approvals
title: Überblick über Asset-Überprüfungen und -Genehmigungen
description: Erfahren Sie mehr über den formellen Prüfungs- und Genehmigungsprozess in Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: b0bd63012d86f38db238b555d21a1c51b0a8b165
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---


# Überblick über Asset-Überprüfungen und -Genehmigungen

Der neue Workflow zur Asset-Überprüfung und -Genehmigung basiert auf einer engen Integration zwischen Workfront und Frame.io. Diese Integration nutzt das Beste aus dem, was jedes Produkt zu bieten hat, und kombiniert es zu einem Erlebnis, das es allen an der Inhaltserstellung beteiligten Personen ermöglicht, in ihren bevorzugten Tools zu arbeiten, während sie gleichzeitig Zugriff auf Kommentare, Dateien und Statusaktualisierungen haben, die in Echtzeit auf beiden Systemen synchronisiert werden.

<!-- link to frame docs-->

## Beginn und Planung von Arbeiten in Workfront

Der Projektkoordinator beginnt in Workfront. Das Projekt wird erstellt, Aufgaben werden zugewiesen, Anweisungen werden gesendet.

Der Projektkoordinator erstellt ein WF-Projekt, verwendet den synchronisierten Projektordner, um Informationen und unterstützende Materialien an kreative Elemente innerhalb von Frame.io zu senden.

Validierungs-Workflow von Grund auf neu oder mithilfe von Vorlagen einrichten

Aufgaben zuweisen

Legt das Projekt auf Aktuell oder gleich zum Erstellen eines Frame-Projekts und Warnhinweiserstellung fest

### Standard-Frame.io-Konto konfigurieren

Workfront-Administratoren initiieren die Integration von Workfront und Frame.io, indem sie im Setup-Bereich von Workfront ein standardmäßiges Frame.io-Konto hinzufügen. Sobald ein standardmäßiges Frame.io-Konto eingerichtet ist, kann die Integration verbundene Projekte zwischen Workfront und Frame.io erstellen.

Weitere Informationen finden Sie unter [].


<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->


### Frame.io-Benutzer aktivieren

Workfront-Benutzer, die regelmäßig Frame.io verwenden, sollten als Frame.io-Benutzer markiert werden. Workfront-Administratoren können Frame.io-Benutzer im Workfront-Benutzerprofil bestimmen.

Wenn ein Benutzer in Workfront als Frame.io-Benutzer markiert und zu einem Projekt hinzugefügt wird:

* Sie werden als Mitwirkender in Frame.io hinzugefügt.
* Sie können Assets von Frame.io an Workfront zur formalen Überprüfung und Genehmigung senden

Weitere Informationen finden Sie unter [].

![](assets/Frame-enabled-user.png)

>[!TIP]
>
>Es wird empfohlen, Benutzern, die regelmäßig mit Kreativ-Tools arbeiten und Assets zur Überprüfung und Genehmigung hochladen, die Verwendung von Frame.io-Benutzern zu ermöglichen.

### Erstellen Sie ein Projekt, das mit Frame.io verbunden ist

Projektkoordinatoren können Workfront-Projekte erstellen, die mit Frame.io verbunden sind. Wenn Sie ein verbundenes Projekt erstellen, können Sie

* **Weisen Sie den Aufgaben Frame.io-Benutzer zu**: Benutzer, die für Frame.io aktiviert sind, werden per E-Mail benachrichtigt, wenn sie einer Aufgabe zugeordnet werden, die ihnen signalisiert, dass noch zu Ende gearbeitet werden muss.
* **Projekt für Frame.io-Benutzer freigeben**: Mit Frame.io freigegebene Projekte gewähren Benutzern Zugriff auf das Projekt innerhalb von Frame.io.
* **Geben Sie kreative Materialien mit Frame.io frei**: Sie können Anweisungen und Materialien von Workfront direkt an den kreativen Benutzer in Frame.io senden, indem Sie einen unidirektionalen Synchronisierungsprojektordner verwenden.
* **Fortschritt der Aufgabe verfolgen**: Kreative Benutzer können fertige Assets senden und Aufgaben als abgeschlossen markieren, ohne Frame.io zu verlassen.

Weitere Informationen finden Sie unter [].

<!--Preassign approval templates to asks coming in the future-->


## Inhaltserstellung und -zusammenarbeit in Frame.io

Kreative können in ihren Tools ihrer Wahl bleiben und die Freiheit haben, Peer Reviews innerhalb von Frame.io zu erstellen, zu iterieren und durchzuführen.

Wenn einem integrierten Projekt ein kreatives Element hinzugefügt wird, können sie alle folgenden Aufgaben ausführen, ohne Frame.io zu verlassen:

* Zugriffsanweisungen des Projektkoordinators
* Durchführung informeller Peer Reviews
* Senden fertiger Assets an Workfront zur formalen Überprüfung und Genehmigung
* Status einer Aufgabe ändern oder sie als abgeschlossen kennzeichnen
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->


## Überprüfen und Genehmigen von Assets in Workfront

Sobald ein Kreativelement ein fertiges Asset von Frame.io an Workfront sendet, kann der Projektkoordinator den formalen Überprüfungs- und Genehmigungsprozess in Workfront starten. Alle Prüfungs- und Validierungsaktivitäten werden in Workfront aufgezeichnet.

Alle in Frame.io abgegebenen Kommentare werden auch auf der Registerkarte Updates in Workfront angezeigt. In Workfront vorgenommene Antworten werden in Frame.io nicht wiedergegeben.

Kommentare, die nur als Team gekennzeichnet sind, werden nicht auf der Registerkarte Workfront-Updates angezeigt.

### Initiierung formeller Prüfungen und Genehmigungen

Sie können einmalige Überprüfungen und Genehmigungen erstellen oder wiederverwendbare Genehmigungsvorlagen im Bereich Einrichtung der Arbeitsfläche erstellen:

Sie haben die Möglichkeit, Überprüfer, Genehmiger oder eine Mischung aus beiden zuzuweisen:

* **Überprüfer** kann Assets kommentieren und markieren. Nach Abschluss können sie ihre Überprüfung als abgeschlossen markieren. <!--example of when to add reviewers-->
* **Genehmiger** Können Assets kommentieren, markieren und eine Entscheidung treffen, um den Genehmigungsprozess voranzutreiben.

Validierungsverantwortliche und Validierungsverantwortliche können zu Vorlagen für die einmalige Verwendung oder Genehmigung hinzugefügt werden:

<!--can also assign teams and set deadline-->

* **Einzelanwendungsgenehmigungen**: Festlegen der Genehmigungsfristen

* **Validierungsvorlagen**
Im Workfront-Setup-Bereich können Benutzer mit einer Standardlizenz wiederverwendbare Genehmigungsvorlagen erstellen. In einer Vorlage können Benutzer einen Zeitraum angeben und Überprüfer und Genehmiger hinzufügen. <!--do we want to mention any upcoming plans here? -->

  Nachdem eine Vorlage erstellt wurde, kann sie auf Assets angewendet werden, die von Frame.io gesendet werden, um den formalen Review- und Genehmigungsprozess in Workfront zu starten.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

### Validierungs- und Validierungsbenachrichtigungen

Kombinieren Sie mit anderen Abschnitten?

Startseite Erwartung meiner Validierungs-Widget E-Mail - Deadline-E-Mails 72, 24 und am Termin.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Assets überprüfen und genehmigen

Mit Frame.io verbundene Asset-Stakeholder können im Frame-Viewer mit Kommentaren, die mit dem Update-Stream &quot;Workfront&quot;synchronisiert werden, Entscheidungen überprüfen und genehmigen, usw.

<!-- include screenshot from frame.io-->

Externe WF-Benutzer werden aufgefordert, eine Anmeldung für Frame zu erstellen

Wenn das Asset nicht mit einem Frame verbunden ist, kann es Miniaturansichten in WF anzeigen und den Kommentar-Stream verwenden. Überprüfungs- und Validierungsentscheidungen können getroffen werden.

### Metriken für Überprüfung und Genehmigung verfolgen

Widget im Bericht zur Genehmigungsgeschwindigkeit für die Startseite

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


* Laden Sie ein Asset aus Workfront hoch und senden Sie es an Frame zur Überprüfung und Genehmigung - In Kürze verfügbar?

## Beispiel für einen Workflow zur Asset-Genehmigung einer Kampagne

intro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
