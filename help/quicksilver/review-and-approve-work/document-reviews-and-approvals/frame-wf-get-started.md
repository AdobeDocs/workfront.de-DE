---
product-area: documents
navigation-topic: approvals
title: Erste Schritte mit der Asset-Überprüfung und -Genehmigung mit Frame.io
description: Erfahren Sie mehr über den formalen Überprüfungs- und Genehmigungsprozess in mit Workfront und Frame.io.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 68b91aad-af76-473f-861d-da846fdfb84c
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Erste Schritte mit der Asset-Überprüfung und -Genehmigung mit Frame.io

Der neue Workflow für die Überprüfung und Genehmigung von Assets basiert auf einer engen Integration zwischen Workfront und Frame.io. Diese Integration nutzt die besten Funktionen, die jedes Produkt zu bieten hat, und kombiniert sie zu einem Erlebnis, das es allen an der Inhaltserstellung Beteiligten ermöglicht, in ihren Tools ihrer Wahl zu arbeiten und gleichzeitig Zugriff auf Kommentare, Dateien und Statusaktualisierungen zu haben - alles in Echtzeit auf beiden Systemen synchronisiert.

Weitere Informationen zu Frame.io finden Sie unter [Erste Schritte mit Frame.io](https://support.frame.io/en/collections/49298-getting-started).

## Arbeitsaufnahme und -planung in Workfront

Der Workfront-Administrator ermöglicht die Integration zwischen Workfront und Frame.io, indem er das standardmäßige Frame.io-Konto im Bereich „Setup“ konfiguriert und dann in Workfront Frame.io-Benutzer bestimmt. Auf diese Weise kann der Koordinator die Arbeit mithilfe von Workfront-Projekten und formalen Prüfungs- und Genehmigungs-Workflows planen und initiieren.

### Konfigurieren des Standard-Frame.io-Kontos [!BADGE in Kürze verfügbar]{type=Informative}

Workfront-Administratoren initiieren die Integration von Workfront und Frame.io, indem sie im Bereich „Setup“ von Workfront ein standardmäßiges Frame.io-Konto hinzufügen. Sobald das standardmäßige Frame.io-Konto eingerichtet ist, wird für alle in Workfront erstellten Projekte ein Spiegelprojekt in Frame.io erstellt.

>[!IMPORTANT]
>
>Diese Funktion wird in Kürze verfügbar sein. Im Moment werden Frame.io-Konten manuell vom Workfront-Team hinzugefügt. Wenden Sie sich an Ihren Adobe-Kundenbetreuer, um Hilfe zu erhalten.

<!--For more information, see [Configure the [!DNL Workfront] and [!DNL Frame.io] integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

 in procedure article we need to cover how groups work with projects and how the frame account is associated with a group. And that accounts other than the default can be added on a 1:1 basis using the dev token. -->

### Frame.io-Benutzer aktivieren Jetzt verfügbar

Workfront-Benutzer, die regelmäßig Frame.io verwenden, sollten als Frame.io-Benutzer gekennzeichnet werden. Workfront-Administratoren können im Workfront-Benutzerprofil Frame.io-Benutzer festlegen.

>[!TIP]
>
>Es wird empfohlen, Benutzer, die regelmäßig mit Kreativ-Tools arbeiten und Assets zur Überprüfung und Genehmigung hochladen, als Frame.io-Benutzer zu aktivieren.

Wenn ein(e) Benutzende(r) in Workfront als Frame.io-Benutzende(r) gekennzeichnet und einem Projekt hinzugefügt wird:

* Sie werden als Collaborator in Frame.io hinzugefügt.
* Sie können Assets von Frame.io zur formellen Überprüfung und Genehmigung an Workfront senden.
* Sie können Informationen im unidirektionalen Synchronisierungsordner von Workfront anzeigen. [!BADGE Bald verfügbar]{type=Informative}

Weitere Informationen finden Sie unter [Konfigurieren der  [!DNL Workfront] - [!DNL Frame.io] -Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).

![Frame-fähiger Benutzer](assets/Frame-enabled-user.png)


### Erstellen eines Projekts, das mit Frame.io verbunden ist

Sobald das standardmäßige Frame.io-Konto hinzugefügt und Frame.io-Benutzer zugewiesen wurden, können Projektkoordinatoren mit Frame.io verbundene Workfront-Projekte erstellen. Wenn Sie ein verbundenes Projekt erstellen, können Sie

* **Frame.io-Benutzer Aufgaben zuweisen**: Frame.io-aktivierte Benutzer werden per E-Mail benachrichtigt, wenn sie einer Workfront-Aufgabe zugewiesen werden. Dies signalisiert, dass noch Arbeit zu erledigen ist.
* **Projekt für Frame.io-Benutzer freigeben**: Wenn ein Projekt für Frame.io-fähige Benutzer freigegeben wird, haben diese sowohl in Workfront als auch in Frame.io Zugriff auf das Projekt.
* **Freigeben von Kreativmaterialien mit Frame.io**: Projektkoordinatoren können in Frame.io mithilfe eines unidirektionalen Synchronisierungsprojektordners Anweisungen und Materialien aus Workfront direkt an den Kreativbenutzer senden. [!BADGE Bald verfügbar]{type=Informative}
* **Verfolgen des Aufgabenfortschritts**: Kreative können fertige Assets senden und Aufgaben als abgeschlossen markieren - alles, ohne Frame.io verlassen zu müssen.

Weitere Informationen finden Sie unter [Erstellen eines Projekts, das mit Frame.io verbunden ](/help/quicksilver/manage-work/projects/create-projects/create-frame-connected-project.md).


## Inhaltserstellung und Zusammenarbeit in Frame.io

Kreative können in ihren Tools der Wahl bleiben und die Freiheit haben, Peer Reviews in Frame.io zu erstellen, zu iterieren und durchzuführen.

Wenn ein Kreativprofi einem verbundenen Projekt hinzugefügt wird, kann er in Frame.io Folgendes tun:

<!--* Access instructions from the project coordinator -->
* Durchführen informeller Peer Reviews
* Senden fertiger Assets an Workfront zur formellen Überprüfung und Genehmigung
* Status einer Aufgabe ändern oder als abgeschlossen markieren
* Neue Versionen hochladen und dann erneut zur Genehmigung <!--do they have to send to frame.io again?-->

Weitere Informationen zu Frame.io finden Sie unter [Ich wurde eingeladen, an einem Projekt mitzuarbeiten](https://support.frame.io/en/articles/11125-i-ve-been-invited-to-collaborate-on-a-project).

## Überprüfen und Genehmigen von Assets

Sobald ein Kreativprofi ein fertiges Asset von Frame.io an Workfront sendet, kann der Projektkoordinator den formalen Prüfungs- und Genehmigungsprozess in Workfront einleiten.

Nachdem der Genehmigungs-Workflow erstellt wurde, gehen Prüfer und genehmigende Personen zurück zu Frame.io, um Kommentare hinzuzufügen und das Asset zu markieren. Sie können die Genehmigungsentscheidung auch im Frame.io-Viewer treffen.

### Starten von formellen Überprüfungen und Genehmigungen in Workfront

Projektkoordinatoren können einmalige Prüfungs- und Genehmigungsvorlagen oder wiederverwendbare Genehmigungsvorlagen erstellen. Alle Prüf- und Genehmigungsaktivitäten in Frame.io werden auch in Workfront aufgezeichnet.

Projektkoordinatoren haben die Möglichkeit, Prüfer, genehmigende Personen oder eine Mischung aus beidem zuzuweisen:

* **Reviewer** können Kommentare hinzufügen und Assets markieren. Nach Abschluss können sie ihre Überprüfung als abgeschlossen markieren. Das Markieren der Überprüfung als abgeschlossen ist nicht erforderlich, damit das Asset im Genehmigungsprozess fortfahren kann.
* **Genehmigende Personen** können Kommentare hinzufügen und Assets markieren. Sie müssen eine Entscheidung treffen, um den Genehmigungsprozess voranzubringen.


#### Erstellen eines Prüfungs- und Genehmigungs-Workflows

Reviewer und genehmigende Personen können einem Genehmigungs-Workflow für den einmaligen Gebrauch oder einer wiederverwendbaren Genehmigungsvorlage hinzugefügt werden:

* **Einmalgenehmigungen**: In dem Projekt oder der Aufgabe, in dem bzw. der sich das Asset befindet, kann der Projektkoordinator Validierungsverantwortliche und genehmigende Personen zuweisen und eine Abschlussfrist festlegen. Validierungsverantwortliche und genehmigende Personen werden 72 und 24 Stunden vor Fristablauf sowie innerhalb der Frist selbst per E-Mail erinnert.

  Weitere Informationen finden Sie unter * [Erstellen einer Überprüfungs- oder Genehmigungsanfrage für ein Frame.io-Asset](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-request-for-frame-asset.md).

* **Validierungsvorlagen**: Im Bereich &quot;Workfront-Setup“ können Projektkoordinatoren wiederverwendbare Validierungsvorlagen erstellen. Innerhalb einer Vorlage können Benutzer Validierungsverantwortliche und genehmigende Personen hinzufügen und einen Fertigstellungszeitraum festlegen. Wenn die Validierungsvorlage auf ein Asset angewendet wird, wird die Frist aus dem angegebenen Zeitrahmen berechnet.

  Nachdem eine Vorlage erstellt wurde, kann sie auf Assets angewendet werden, die von Frame.io gesendet werden, um den formellen Prüfungs- und Genehmigungsprozess in Workfront zu starten.

  Weitere Informationen finden Sie unter [Erstellen einer Validierungsvorlage](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)


![Vorlage zuweisen](assets/assign-template.png)


#### Zugriff auf den Frame.io-Viewer

Benutzer können auf folgende Weise auf den Viewer Frame.io zugreifen:

* Workfront-E-Mail-Benachrichtigungen
* Das Widget „Meine Genehmigung“ im neuen Workfront-Startbereich
  ![Warten auf meine Genehmigung](assets/awaiting-my-approval.png)

>[!NOTE]
>
>Externe Workfront-Benutzer werden per E-Mail benachrichtigt und aufgefordert, eine Frame.io-Anmeldung zu erstellen, um Assets zu überprüfen und zu genehmigen.

#### Hinzufügen von Kommentaren und Markieren von Assets

Alle im Frame.io-Viewer abgegebenen Kommentare werden auch auf der Registerkarte Workfront-Aktualisierungen aufgezeichnet. In Workfront erstellte Antworten werden nicht in Frame.io angezeigt. Wenn Kommentare im Viewer Frame.io als „Nur Team“ gekennzeichnet sind, werden sie nicht auf der Registerkarte Workfront-Aktualisierungen angezeigt.

#### Entscheidung treffen

Sobald alle Prüfungsaktivitäten abgeschlossen sind, müssen genehmigende Personen eine der folgenden Entscheidungen treffen:

* **Genehmigen**: Das Asset benötigt keine Änderungen und ist einsatzbereit.
* **Mit Änderungen genehmigen**: Das Asset muss geändert werden und ist nach der Vornahme einsatzbereit. Eine zusätzliche Genehmigung ist nicht erforderlich.
* **Muss bearbeitet**: Das Asset muss geändert werden und ist nicht einsatzbereit. Sobald die angegebenen Änderungen vorgenommen wurden, muss das Asset als neue Version hochgeladen werden und eine weitere Genehmigungsrunde durchlaufen. <!--is the same approval workflow automatically applied? Does the coordinator have to do anything to get the approval going? -->

Reviewer können ihre Überprüfung im Viewer Frame.io als abgeschlossen markieren. Dies ist jedoch nicht erforderlich, damit das Asset im Genehmigungsprozess fortgesetzt werden kann.

Weitere Informationen zu Entscheidungen in Workfront finden Sie unter [Übersicht über den ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

![Frame-Viewer und Entscheidung](assets/frame-viewer-and-decision.png)


<!-- upload assets directly to workfront to be reviewed in Frame.io/ Will have to send manually at first

Reviewer/approver needs to go through email to get to frame vier
-->

### Nachverfolgen von Prüfungs- und Genehmigungsmetriken

Projektkoordinatoren können den Fortschritt bei allen während des Fluges erteilten Genehmigungen im Bereich &quot;Workfront-Startseite“ mit dem folgenden Widget überwachen:

* **Alle Genehmigungen**: Zeigt zwei Diagramme mit Informationen über die durchschnittliche Genehmigungsdauer und -entscheidungen sowie Listenansichten mit ausstehenden und überfälligen Genehmigungen an.
  ![Alle Genehmigungen](assets/all-approvals.png)