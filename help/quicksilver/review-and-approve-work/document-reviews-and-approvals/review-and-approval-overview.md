---
product-area: documents
navigation-topic: approvals
title: Asset-Überprüfung und -Genehmigung - Übersicht
description: Erfahren Sie mehr über den formalen Überprüfungs- und Genehmigungsprozess in Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 959bd3cab0de8b76c94fad1be5b6b2b8b7ae904b
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# Asset-Überprüfung und -Genehmigung - Übersicht

Der neue Workflow für die Überprüfung und Genehmigung von Assets basiert auf einer engen Integration zwischen Workfront und Frame.io. Bei dieser Integration wird das Beste aus dem genommen, was jedes Produkt zu bieten hat, und kombiniert dies zu einem Erlebnis, das es allen an der Inhaltserstellung beteiligten Personen ermöglicht, in ihren bevorzugten Tools zu arbeiten und gleichzeitig in Echtzeit Zugriff auf Kommentare, Dateien und Statusaktualisierungen auf beiden Systemen zu haben.

Weitere Informationen zu Frame.io finden Sie unter [Erste Schritte mit Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Arbeitsaufnahme und -planung in Workfront

Der Workfront-Administrator ermöglicht die Integration zwischen Workfront und Frame.io, indem er das standardmäßige Frame.io-Konto im Bereich „Setup“ konfiguriert und dann in Workfront Frame.io-Benutzer angibt. Auf diese Weise kann der Koordinator seine Arbeit mithilfe von Workfront-Projekten und formellen Prüfungs- und Genehmigungs-Workflows planen und starten.

### Konfigurieren eines standardmäßigen Frame.io-Kontos

Workfront-Administratoren initiieren die Integration von Workfront und Frame.io, indem sie im Bereich „Setup“ von Workfront ein standardmäßiges Frame.io-Konto hinzufügen. Nachdem ein standardmäßiges Frame.io-Konto eingerichtet wurde, wird für alle in Workfront erstellten Projekte ein Spiegelprojekt in Frame.io erstellt.

Weitere Informationen finden Sie unter [].

<!-- in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Frame.io-Benutzer aktivieren

Workfront-Benutzer, die regelmäßig Frame.io verwenden, sollten als Frame.io-Benutzer gekennzeichnet werden. Workfront-Administratoren können im Workfront-Benutzerprofil Frame.io-Benutzer festlegen.

Wenn ein(e) Benutzende(r) in Workfront als Frame.io-Benutzende(r) markiert und zu einem Projekt hinzugefügt wird,

* Sie werden als Collaborator in Frame.io hinzugefügt
* Sie können Assets von Frame.io zur formellen Überprüfung und Genehmigung an Workfront senden
* Sie können Informationen im unidirektionalen Synchronisierungsordner von Workfront aus anzeigen

>[!TIP]
>
>Es wird empfohlen, Benutzer, die regelmäßig mit Kreativ-Tools arbeiten, zu aktivieren und Assets zur Überprüfung und Genehmigung als Frame.io-Benutzer hochzuladen.

Weitere Informationen finden Sie unter [].

![](assets/Frame-enabled-user.png)


### Erstellen eines mit Frame.io verbundenen Projekts

Sobald das standardmäßige Frame.io-Konto hinzugefügt und Frame.io-Benutzer zugewiesen wurden, können Projektkoordinatoren mit Frame.io verbundene Workfront-Projekte erstellen. Wenn Sie ein verbundenes Projekt erstellen, können Sie

* **Zuweisen von Frame.io-Benutzern zu Aufgaben**: Frame.io-fähige Benutzer werden per E-Mail benachrichtigt, wenn sie einer Aufgabe zugewiesen werden. Dies signalisiert, dass noch viel Arbeit zu erledigen ist.
* **Freigeben des Projekts für Frame.io-Benutzer**: Projekte, für die Frame.io aktiviert ist, gewähren Benutzern Zugriff auf das Projekt in Frame.io.
* **Teilen von kreativen Materialien mit Frame.io**: Sie können in Frame.io mithilfe eines unidirektionalen Synchronisierungsprojektordners Anweisungen und Material aus Workfront direkt an den Kreativprofi senden.
* **Verfolgen des Aufgabenfortschritts**: Kreative können fertige Assets senden und Aufgaben als abgeschlossen markieren, ohne Frame.io verlassen zu müssen.

Weitere Informationen finden Sie unter [].

<!--Preassign approval templates to tasks coming in the future-->


## Inhaltserstellung und Zusammenarbeit in Frame.io

Kreative können in ihren Tools der Wahl bleiben und die Freiheit haben, Peer Reviews in Frame.io zu erstellen, zu iterieren und durchzuführen.

Wenn ein Kreativprofi einem verbundenen Projekt hinzugefügt wird, kann er Folgendes tun, ohne Frame.io verlassen zu müssen:

* Zugreifen auf Anweisungen des Projektkoordinators
* Durchführung informeller Peer Reviews
* Senden fertiger Assets zur formellen Überprüfung und Genehmigung an Workfront
* Status einer Aufgabe ändern oder als abgeschlossen markieren
<!-- * Notification of decision
* Upload new versions of connected assets marked as needs more work < will automatically connect>-->

Weitere Informationen zum Überprüfen von Assets in Frame.io finden Sie unter

## Überprüfen und Genehmigen von Assets

Sobald ein Kreativprofi ein fertiges Asset von Frame.io an Workfront sendet, kann der Projektkoordinator den formalen Prüfungs- und Genehmigungsprozess in Workfront einleiten.

Nachdem die Genehmigung erstellt wurde, gehen Benutzer zurück zu Frame.io, um das Asset zu kommentieren und zu markieren. Sie können auch eine Genehmigungsentscheidung im Frame.io-Viewer treffen.

### Starten von formellen Überprüfungen und Genehmigungen in Workfront

Projektkoordinatoren können im Bereich „Setup“ von Workfront einmalige Prüfungs- und Validierungsvorlagen oder wiederverwendbare Validierungsvorlagen erstellen. Alle in Frame.io durchgeführten Prüf- und Genehmigungsaktivitäten werden ebenfalls in Workfront aufgezeichnet.

#### Validierungsverantwortliche und genehmigende Personen hinzufügen

Projektkoordinatoren haben die Möglichkeit, Prüfer, genehmigende Personen oder eine Mischung aus beidem zuzuweisen:

* **Reviewer** können Assets kommentieren und markieren. Nach Abschluss können sie ihre Überprüfung als abgeschlossen markieren. <!--example of when to add reviewers-->
* **Genehmigende Personen** können Assets kommentieren und markieren. Sie müssen eine Entscheidung treffen, um den Genehmigungsprozess voranzubringen.


#### Erstellen eines Prüfungs- und Validierungs-Workflows

Reviewer und genehmigende Personen können einem einmaligen Genehmigungs-Workflow oder einer Genehmigungsvorlage hinzugefügt werden:

<!--can also assign teams and set deadline-->
E-Mail - Fristablauf E-Mails 72, 24 und am Fristablauf.

* **Einmalige Genehmigungen**: Festlegen von Validierungsfristen

* **Validierungsvorlagen**
Im Bereich &quot;Workfront Setup“ können Benutzende mit einer Standardlizenz wiederverwendbare Genehmigungsvorlagen erstellen. Innerhalb einer Vorlage können Benutzer einen Zeitrahmen angeben und Validierungsverantwortliche und Genehmigende hinzufügen. <!--do we want to mention any upcoming plans here? -->

  Nachdem eine Vorlage erstellt wurde, kann sie auf Assets angewendet werden, die von Frame.io gesendet werden, um den formalen Prüfungs- und Genehmigungsprozess in Workfront zu starten.
  ![](assets/assign-template.png)

<!-- can set timreframe which calculates deadline once approval is started. >

    For more information, see [Create and manage Approval Templates](/)<!--don't forget link-->

* Asset aus Workfront hochladen und zur Überprüfung und Genehmigung an Frame senden - in Kürze verfügbar?

### Genehmigen von Assets in Frame.io

Stakeholder können verbundene Assets mit dem Frame.io-Viewer überprüfen und genehmigen.

#### Zugriff auf den Frame.io-Viewer

Benutzende können auf folgende Weise auf den Frame.io-Viewer zugreifen:

* Das Widget „Warten auf meine Genehmigung“ im neuen Bereich &quot;Workfront Home“
* Workfront-E-Mail-Benachrichtigungen.

Externe Workfront-Benutzer werden aufgefordert, eine Frame.io-Anmeldung zu erstellen, um Assets zu überprüfen und zu genehmigen.

#### Kommentieren und Markieren von Assets

Alle im Frame.io-Viewer abgegebenen Kommentare werden auch auf der Registerkarte Workfront-Update aufgezeichnet. In Workfront durchgeführte Antworten werden nicht in Frame.io angezeigt. Kommentare, die als Nur Team markiert sind, werden nicht auf der Registerkarte Workfront-Updates angezeigt.

#### Entscheidung treffen

Genehmigende Personen müssen eine der folgenden Entscheidungen treffen:

* Genehmigen: Dies
* Mit Änderungen genehmigt
* Muss bearbeitet werden

Reviewer können ihre Reviews innerhalb der Frame.io-Viewer als abgeschlossen markieren.

<!-- include screenshot from frame.io-->



<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->


### Nachverfolgen von Prüfungs- und Genehmigungsmetriken

Widgets im Geschwindigkeitsbericht für die Startseiten-Genehmigung ?

<!--
### Published approved assets to Adobe Experience Manager Assets

Use the native integration to send approved assets to AEM.
-->


## Beispiel für einen Workflow zur Validierung von Kampagnen-Assets

Intro para?

![](assets/example-workflow.png) <!-- probbly need a different version of this but add something similar rather than typing all out?-->
