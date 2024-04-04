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
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 7e970f4f707937a62f68c191a7cbd5dfa26e471c
workflow-type: tm+mt
source-wordcount: '909'
ht-degree: 0%

---

# Überblick über Asset-Überprüfungen und -Genehmigungen

Der neue Workflow zur Asset-Überprüfung und -Genehmigung basiert auf einer engen Integration zwischen Workfront und Frame.io. Diese Integration nutzt das Beste aus dem, was jedes Produkt zu bieten hat, und kombiniert es zu einem Erlebnis, das es allen an der Inhaltserstellung beteiligten Personen ermöglicht, in ihren bevorzugten Tools zu arbeiten, während sie gleichzeitig Zugriff auf Kommentare, Dateien und Statusaktualisierungen haben, die in Echtzeit auf beiden Systemen synchronisiert werden.

Weitere Informationen zu Frame.io finden Sie unter [Erste Schritte mit Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Beginn und Planung von Arbeiten in Workfront

Der Workfront-Administrator aktiviert die Integration zwischen Workfront und Frame.io, indem er das standardmäßige Frame.io-Konto im Setup-Bereich konfiguriert und dann Frame.io-Benutzer in Workfront benennt. Dadurch kann der Koordinator die Arbeit mithilfe von Workfront-Projekten planen und initiieren sowie eine formelle Überprüfung und Genehmigung vornehmen.

### Standard-Frame.io-Konto konfigurieren

Workfront-Administratoren initiieren die Integration von Workfront und Frame.io, indem sie im Setup-Bereich von Workfront ein standardmäßiges Frame.io-Konto hinzufügen. Sobald ein standardmäßiges Frame.io-Konto eingerichtet ist, erstellt die Integration verbundene Projekte zwischen Workfront und Frame.io.

Weitere Informationen finden Sie unter [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Frame.io-Benutzer aktivieren

Workfront-Benutzer, die regelmäßig Frame.io verwenden, sollten als Frame.io-Benutzer markiert werden. Workfront-Administratoren können Frame.io-Benutzer im Workfront-Benutzerprofil bestimmen.

Wenn ein Benutzer in Workfront als Frame.io-Benutzer markiert und zu einem Projekt hinzugefügt wird,

* Sie werden als Mitwirkender in Frame.io hinzugefügt.
* Sie können Assets von Frame.io an Workfront zur formalen Überprüfung und Genehmigung senden

>[!TIP]
>
>Es wird empfohlen, Benutzern, die regelmäßig mit Kreativ-Tools arbeiten und Assets zur Überprüfung und Genehmigung hochladen, die Verwendung von Frame.io-Benutzern zu ermöglichen.


Weitere Informationen finden Sie unter [].

![](assets/Frame-enabled-user.png)


### Erstellen Sie ein Projekt, das mit Frame.io verbunden ist

Sobald das standardmäßige Frame.io-Konto hinzugefügt und Frame.io-Benutzer bestimmt wurden, können Projektkoordinatoren Workfront-Projekte erstellen, die mit Frame.io verbunden sind. Wenn Sie ein verbundenes Projekt erstellen, können Sie

* **Weisen Sie den Aufgaben Frame.io-Benutzer zu**: Benutzer, die für Frame.io aktiviert sind, werden per E-Mail benachrichtigt, wenn sie einer Aufgabe zugewiesen werden. Dies signalisiert, dass die Arbeit abgeschlossen ist.
* **Projekt für Frame.io-Benutzer freigeben**: Mit Frame.io freigegebene Projekte gewähren Benutzern Zugriff auf das Projekt in Frame.io.
* **Geben Sie kreative Materialien mit Frame.io frei**: Sie können Anweisungen und Materialien von Workfront direkt an den kreativen Benutzer in Frame.io senden, indem Sie einen unidirektionalen Synchronisierungsprojektordner verwenden.
* **Fortschritt der Aufgabe verfolgen**: Kreative Benutzer können fertige Assets senden und Aufgaben als abgeschlossen markieren, ohne Frame.io zu verlassen.

Weitere Informationen finden Sie unter [].

<!--Preassign approval templates to tasks coming in the future-->


## Inhaltserstellung und -zusammenarbeit in Frame.io

Kreative können in ihren Tools ihrer Wahl bleiben und können in Frame.io Peer Reviews erstellen, durchlaufen und durchführen.

Wenn einem verbundenen Projekt ein kreatives Element hinzugefügt wird, können sie Folgendes tun, ohne Frame.io zu verlassen:

* Zugriffsanweisungen des Projektkoordinators
* Durchführung informeller Peer Reviews
* Senden fertiger Assets an Workfront zur formalen Überprüfung und Genehmigung
* Status einer Aufgabe ändern oder sie als abgeschlossen kennzeichnen
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Weitere Informationen zum Überprüfen von Assets in Frame.io finden Sie unter

## Überprüfen und Genehmigen von Assets

Sobald ein Kreativelement ein fertiges Asset von Frame.io an Workfront sendet, kann der Projektkoordinator den formalen Review- und Genehmigungsprozess in Workfront starten.

Nachdem die Genehmigung erstellt wurde, gehen Benutzer zurück zu Frame.io, um das Asset zu kommentieren und zu markieren. Sie können auch eine Genehmigungsentscheidung im Frame.io-Viewer treffen.

### Einleitung förmlicher Prüfungen und Genehmigungen in Workfront

Projektkoordinatoren können im Einrichtungsbereich von Workfront einmalige Prüfungs- und Validierungsvorlagen oder wiederverwendbare Genehmigungsvorlagen erstellen. Alle in Frame.io durchgeführten Review- und Genehmigungsaktivitäten werden ebenfalls in Workfront aufgezeichnet.

Projektkoordinatoren haben die Möglichkeit, Prüfer, Genehmiger oder eine Mischung aus beiden zuzuweisen:

* **Überprüfer** kann Assets kommentieren und markieren. Nach Abschluss können sie ihre Überprüfung als abgeschlossen markieren. <!--example of when to add reviewers-->
* **Genehmiger** kann Markup-Assets kommentieren. Sie müssen eine Entscheidung treffen, um den Genehmigungsprozess voranzubringen.



Alle in Frame.io abgegebenen Kommentare werden auf der Registerkarte &quot;Updates&quot;in Workfront angezeigt. In Workfront vorgenommene Antworten werden nicht in Frame.io angezeigt.

Kommentare, die nur als Team gekennzeichnet sind, werden nicht auf der Registerkarte Workfront-Updates angezeigt.

Validierungsverantwortliche und Validierungsverantwortliche können zu Vorlagen für die einmalige Verwendung oder Genehmigung hinzugefügt werden:

<!--can also assign teams and set deadline-->

* **Einzelanwendungsgenehmigungen**: Festlegen der Genehmigungsfristen

* **Validierungsvorlagen**
Im Workfront-Setup-Bereich können Benutzer mit einer Standardlizenz wiederverwendbare Genehmigungsvorlagen erstellen. In einer Vorlage können Benutzer einen Zeitraum festlegen und Überprüfer und Genehmiger hinzufügen. <!--do we want to mention any upcoming plans here? -->

  Nachdem eine Vorlage erstellt wurde, kann sie auf Assets angewendet werden, die von Frame.io gesendet werden, um den formalen Review- und Genehmigungsprozess in Workfront zu starten.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Laden Sie ein Asset aus Workfront hoch und senden Sie es an Frame zur Überprüfung und Genehmigung - In Kürze verfügbar?

### Genehmigen von Assets in Frame.io

Mit Frame.io verbundene Asset-Stakeholder können im Frame.io-Viewer mit Kommentaren, die mit dem Workfront-Aktualisierungsstream synchronisiert werden, Entscheidungen usw. überprüfen und genehmigen.

<!-- include screenshot from frame.io-->

Wenn Sie ausschließlich in Frame arbeiten, können Sie per E-Mail über eine Anfrage benachrichtigt werden.

Wenn Sie ausschließlich in Workfront arbeiten, können Sie das Genehmigungs-Widget zu Hause verwenden.

Sie können von jeder Arbeit aus auf den Viewer Frame.io zugreifen

**Genehmigen von Assets aus Frame.io**
wie sie benachrichtigt werden

eine Entscheidung treffen - genehmigen, mit Änderungen genehmigen, arbeiten müssen

**Genehmigen von Assets aus Workfront**
wie sie benachrichtigt werden

Startseite auf mein Genehmigungs-Widget warten

E-Mail - Deadline-E-Mails 72, 24 und On-Deadline.

Externe WF-Benutzer werden aufgefordert, eine Anmeldung für Frame zu erstellen

Wenn das Asset nicht mit einem Frame verbunden ist, kann es Miniaturansichten in WF anzeigen und den Kommentar-Stream verwenden. Überprüfungs- und Genehmigungsentscheidungen können getroffen werden.

<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Metriken für Überprüfung und Genehmigung verfolgen

Widgets im Bericht zur Genehmigungsgeschwindigkeit von Homepages ?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Beispiel für einen Workflow zur Asset-Genehmigung einer Kampagne

intro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
