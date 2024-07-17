---
product-area: projects
navigation-topic: create-projects
title: Erstellen Sie ein Projekt, das mit Frame.io verbunden ist
description: Ein Projekt ist eine große Arbeitseinheit in Adobe Workfront. Sie können Projekte von Grund auf neu erstellen, eine Vorlage verwenden oder Probleme oder Aufgaben in Projekte konvertieren.
author: Courtney
feature: Work Management
exl-id: 230d8e62-a3c9-4e38-9b26-5ba1c4f56391
source-git-commit: 0d737bc410f3db4eeff52fa8954acdb8a0eb1a6e
workflow-type: tm+mt
source-wordcount: '1158'
ht-degree: 1%

---

# Erstellen Sie ein Projekt, das mit Frame.io verbunden ist

Durch die Integration von Workfront und Frame.io können Sie in Workfront Projekte erstellen, die in Frame.io gespiegelt werden und eine nahtlose Überprüfung und Genehmigung ermöglichen.

Wenn ein Workfront-Projekt mit Frame.io verbunden ist, können Sie

* **Weisen Sie den Aufgaben Frame.io-Benutzer zu**: Benutzer, die für Frame.io aktiviert sind, werden per E-Mail benachrichtigt, wenn sie einer Workfront-Aufgabe zugewiesen werden. Dies zeigt an, dass die Arbeit abgeschlossen sein muss.
* **Freigeben des Projekts für Frame.io-Benutzer**: Wenn ein Projekt für Benutzer mit Frame.io freigegeben wird, haben diese sowohl in Workfront als auch in Frame.io Zugriff auf das Projekt.
* **Teilen Sie kreative Materialien mit Frame.io**: Projektkoordinatoren können Anweisungen und Materialien von Workfront direkt an den kreativen Benutzer in Frame.io senden, indem sie einen unidirektionalen Synchronisierungsprojektordner verwenden. [!BADGE In Kürze verfügbar]{type=Informative}
* **Fortschritt der Aufgabe verfolgen**: Kreative Benutzer können fertige Assets senden und Aufgaben als abgeschlossen markieren - alles ohne Frame.io zu verlassen.

## Zugriffsanforderungen

>[!IMPORTANT]
>
>Diese Funktion ist nur für Unternehmen verfügbar, die in den [!DNL Adobe Admin Console] integriert wurden.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Wenn Sie ein Projekt erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für das Projekt.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

* Einrichten des standardmäßigen Frame.io-Kontos im Workfront-Setup-Bereich
* Frame.io-Benutzer im Workfront-Benutzerprofil aktivieren

Weitere Informationen zu den oben genannten Voraussetzungen finden Sie unter [Konfigurieren der Integration [!DNL Workfront] und [!DNL Frame.io] Integration](/help/quicksilver/administration-and-setup/configure-integrations/configure-wf-and-frame.md).


## Neue Projektvorlage erstellen

Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann an jedes Projekt übertragen, das Sie aus der Vorlage erstellen.

Projekte in Frame.io werden von Teams organisiert, die mit Workfront-Gruppen verbunden sind. Es wird empfohlen, zur Erstellung von verbundenen Projekten eine Projektvorlage zu verwenden, da Sie die Projektgruppe zuvor festlegen können.

Wenn Sie sich dafür entscheiden, das Projekt von Grund auf neu zu erstellen, fügt Workfront automatisch die Standardprojektgruppe hinzu und das Spiegelframe.io-Projekt wird unter diesem Standardteam in Frame.io erstellt.

>[!NOTE]
>
>Das Aktualisieren der Gruppe nach der Projekterstellung ändert das Frame.io-Team nicht.


### Erstellen Sie die Vorlage und geben Sie die Projektgruppe an

{{step1-to-templates}}

1. Klicken Sie auf **Neue Vorlage**.
1. Geben Sie einen Namen für Ihre Vorlage ein und drücken Sie dann die **Eingabetaste** , um den Namen zu speichern.
1. Klicken Sie im linken Bereich auf **Vorlagendetails**.
1. Stellen Sie im Abschnitt **Vorlagenzuordnung** sicher, dass Sie eine Gruppe angeben. Wenn Sie keine Gruppe hinzufügen, wird die standardmäßige Projektgruppe hinzugefügt und das Projekt in Frame.io wird unter dem entsprechenden Standardteam in Frame.io erstellt.

Fahren Sie mit dem nächsten Abschnitt fort.

![](assets/template-group.png)

### Aufgaben hinzufügen und Benutzer zuweisen, für die Frame.io aktiviert ist

1. Klicken Sie im linken Bereich auf **Vorlagenaufgaben**.
1. Klicken Sie auf **Hinzufügen von Vorlagenaufgaben starten** , um Ihrer Vorlage schnell Aufgaben hinzuzufügen. Sie können später weitere Einstellungen konfigurieren.

   Oder

   Klicken Sie auf **Neue Vorlagenaufgabe** , um jeweils eine Aufgabe hinzuzufügen und zusätzliche Einstellungen zu konfigurieren.
   ![](assets/add-tasks-to-template.png)
1. Fügen Sie einen Aufgabennamen hinzu.
1. Weisen Sie im Bereich **Zuweisungen** Benutzer oder Teams zu. Wenn Sie einen Frame.io-fähigen Benutzer entweder einzeln oder in einem Team zuweisen, erhalten diese Mitarbeiter Zugriff auf das Frame.io-Projekt und werden per E-Mail über die Aufgabe im Frame.io-Projekt benachrichtigt. Von dieser E-Mail aus können sie dem Projekt Frame.io beitreten und mit der Arbeit beginnen.
1. Wiederholen Sie die Schritte 1 und 2 nach Bedarf.

Fahren Sie mit dem nächsten Abschnitt fort.

### Zusätzliche Vorlagendetails konfigurieren

Workfront verfügt über robuste Projektverwaltungsfunktionen. Es wird empfohlen, den Artikel [Projektvorlagen bearbeiten](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) zu verwenden, um die folgenden Bereiche der Vorlage zu konfigurieren:

* Übersicht
* Finanzielle Details
* Benutzerdefinierte Formulare
* Projekteinstellungen
* Aufgabeneinstellungen
* Problemeinstellungen
* Zugriff

### Erstellen eines Projekts aus einer Vorlage

Nachdem Sie eine Vorlage erstellt haben, können Sie sie zum Erstellen von Projekten verwenden.

{{step1-to-projects}}

1. Klicken Sie auf **Neues Projekt aus Vorlage**.
1. Geben Sie über das Suchfeld den Namen der gewünschten Vorlage ein.
1. Wählen Sie den Vorlagennamen aus und klicken Sie auf **Vorlage verwenden**.
   ![](assets/find-your-template.png)
1. Passen Sie die gewünschten Projekteinstellungen an und klicken Sie dann auf **Projekt erstellen**.
1. Klicken Sie im linken Bereich auf **Dokumente**.
1. Verwenden Sie den unidirektionalen Synchronisierungsordner, um kreative Materialien automatisch für Frame.io freizugeben. [!BADGE In Kürze verfügbar]{type=Informative}

   >[!NOTE]
   >
   >Diese Funktion wird derzeit entwickelt. Um Informationen für Benutzer in Frame.io freizugeben, laden Sie die Dateien auf die Registerkarte &quot;Dokument&quot;hoch. Wenn der Status des Projekts auf Aktuell festgelegt ist, werden diese Dateien automatisch an Frame.io gesendet.

1. Ändern Sie in der Projektheader das Projekt von **Planung** in **Aktuell**.

Nachdem das Projekt erstellt wurde und Kreative abgeschlossene Assets hochladen, können Sie dem Asset in Workfront einen Arbeitsablauf für Überprüfung und Genehmigung zuweisen. Weitere Informationen finden Sie unter [Erstellen einer Dokumentüberprüfungs- oder Genehmigungsanforderung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) <!-- name may need to change -->.

## Neues Projekt von Grund auf neu erstellen

Sie können bei Bedarf ein neues Projekt von Grund auf neu erstellen.

>[!IMPORTANT]
>
>* Projekte in Frame.io werden von Teams organisiert, die mit Workfront-Gruppen verbunden sind. Es wird empfohlen, zur Erstellung von verbundenen Projekten eine Projektvorlage zu verwenden, da Sie die Projektgruppe zuvor festlegen können.
>
>
>* Wenn Sie sich dafür entscheiden, das Projekt von Grund auf neu zu erstellen, fügt Workfront automatisch die Standardprojektgruppe hinzu und das Spiegelframe.io-Projekt wird unter diesem Standardteam in Frame.io erstellt.
>
>Das Aktualisieren der Gruppe nach der Projekterstellung ändert das Frame.io-Team nicht.

### Projekt erstellen

{{step1-to-projects}}

1. Klicken Sie auf **Neues Projekt**.
1. Geben Sie einen Namen für Ihr Projekt ein und drücken Sie dann **Enter** , um den Namen zu speichern.

Fahren Sie mit dem nächsten Abschnitt fort.

### Aufgaben hinzufügen und Benutzer zuweisen, für die Frame.io aktiviert ist

1. Klicken Sie im linken Bereich auf **Aufgaben**.
1. Klicken Sie auf **Starten des Hinzufügens von Aufgaben** , um Ihrem Projekt schnell Aufgaben hinzuzufügen. Sie können später weitere Einstellungen konfigurieren.

   Oder

   Klicken Sie auf **Neue Aufgabe** , um jeweils eine Aufgabe hinzuzufügen und zusätzliche Einstellungen zu konfigurieren.
   ![](assets/add-project-tasks.png)
1. Fügen Sie einen Aufgabennamen hinzu.
1. Weisen Sie im Bereich **Zuweisungen** Benutzer oder Teams zu. Wenn Sie einen Frame.io-fähigen Benutzer entweder einzeln oder in einem Team zuweisen, erhalten diese Mitarbeiter Zugriff auf das Frame.io-Projekt und werden per E-Mail über die Aufgabe im Frame.io-Projekt benachrichtigt. Von dieser E-Mail aus können sie dem Projekt Frame.io beitreten und mit der Arbeit beginnen.
1. Wiederholen Sie die Schritte 1 und 2 nach Bedarf.

Fahren Sie mit dem nächsten Abschnitt fort.

### Hochladen von kreativen Materialien

1. Klicken Sie im linken Bereich auf **Dokumente**.
1. Verwenden Sie den unidirektionalen Synchronisierungsordner, um kreative Materialien automatisch für Frame.io freizugeben. [!BADGE In Kürze verfügbar]{type=Informative}

   >[!NOTE]
   >
   >Diese Funktion wird derzeit entwickelt. Um Informationen für Benutzer in Frame.io freizugeben, laden Sie die Dateien auf die Registerkarte &quot;Dokument&quot;hoch. Wenn der Status des Projekts auf &quot;Aktuell&quot;festgelegt ist, werden diese Dateien automatisch an Frame.io gesendet

Fahren Sie mit dem nächsten Abschnitt fort.

### Konfigurieren zusätzlicher Projektdetails

Workfront verfügt über robuste Projektverwaltungsfunktionen. Es wird empfohlen, den Artikel [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) zu verwenden, um die folgenden Bereiche des Projekts zu konfigurieren:

* Übersicht
* Finanzielle Details
* Benutzerdefinierte Formulare
* Projekteinstellungen
* Aufgabeneinstellungen
* Problemeinstellungen
* Zugriff

### Festlegen des Projekts auf aktuell

1. Ändern Sie in der Projektheader das Projekt von Planung in Aktuell .
Nachdem das Projekt erstellt wurde und Kreative abgeschlossene Assets hochladen, können Sie dem Asset in Workfront einen Arbeitsablauf für Überprüfung und Genehmigung zuweisen.

Nachdem das Projekt erstellt wurde und Kreative abgeschlossene Assets hochladen, können Sie dem Asset in Workfront einen Arbeitsablauf für Überprüfung und Genehmigung zuweisen.

Weitere Informationen finden Sie unter [Erstellen einer Dokumentüberprüfungs- oder Genehmigungsanforderung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) <!-- name may need to change -->.
