---
product-area: projects
navigation-topic: create-projects
title: Erstellen eines Projekts, das mit Frame.io verbunden ist
description: Ein Projekt ist eine große Arbeitseinheit in Adobe Workfront. Sie können Projekte von Grund auf neu erstellen, eine Vorlage verwenden oder Probleme oder Aufgaben in Projekte konvertieren.
author: Courtney
feature: Work Management
hide: true
hidefromtoc: true
exl-id: 230d8e62-a3c9-4e38-9b26-5ba1c4f56391
source-git-commit: 321449202f629f75464870bea7fa3db8b4c0e0cb
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 1%

---

# Erstellen eines Projekts, das mit Frame.io verbunden ist

Durch die Integration von Workfront und Frame.io können Sie in Workfront Projekte erstellen, die in Frame.io gespiegelt werden. So erhalten Sie ein nahtloses Prüf- und Genehmigungs-Erlebnis.

Wenn ein Workfront-Projekt mit Frame.io verbunden ist, können Sie

* **Frame.io-Benutzer Aufgaben zuweisen**: Frame.io-aktivierte Benutzer werden per E-Mail benachrichtigt, wenn sie einer Workfront-Aufgabe zugewiesen werden. Dies signalisiert, dass noch Arbeit zu erledigen ist.
* **Projekt für Frame.io-Benutzer freigeben**: Wenn ein Projekt für Frame.io-fähige Benutzer freigegeben wird, haben diese sowohl in Workfront als auch in Frame.io Zugriff auf das Projekt.
* **Freigeben von Kreativmaterialien mit Frame.io**: Projektkoordinatoren können in Frame.io mithilfe eines unidirektionalen Synchronisierungsprojektordners Anweisungen und Materialien aus Workfront direkt an den Kreativbenutzer senden. [!BADGE Bald verfügbar]{type=Informative}
* **Verfolgen des Aufgabenfortschritts**: Kreative können fertige Assets senden und Aufgaben als abgeschlossen markieren - alles, ohne Frame.io verlassen zu müssen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

>[!IMPORTANT]
>
>Diese Funktion steht nur Organisationen zur Verfügung, die in das [!DNL Adobe Admin Console] integriert wurden.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Wenn Sie ein Projekt erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für das Projekt.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

* Richten Sie das standardmäßige Frame.io-Konto im Workfront-Setup-Bereich ein.
* Aktivieren von Frame.io-Benutzern im Workfront-Benutzerprofil



## Erstellen einer neuen Projektvorlage

Beim Erstellen einer neuen Vorlage können Sie die Informationen für alle Aufgaben und für Ihre zukünftigen Projekteinstellungen eingeben. Diese Informationen werden dann in alle Projekte übertragen, die Sie aus der Vorlage erstellen.

Projekte in Frame.io werden von Teams organisiert, die mit Workfront-Gruppen verbunden sind. Es wird empfohlen, zum Erstellen verbundener Projekte eine Projektvorlage zu verwenden, da Sie die Projektgruppe zuvor festlegen können.

Wenn Sie das Projekt von Grund auf neu erstellen, fügt Workfront automatisch die Standardprojektgruppe hinzu, und das Projekt „mirror.frame.io“ wird unter diesem Standardteam in Frame.io erstellt.

>[!NOTE]
>
>Beim Aktualisieren der Gruppe nach der Projekterstellung ändert sich das Frame.io-Team nicht.


### Erstellen Sie die Vorlage und geben Sie die Projektgruppe an

{{step1-to-templates}}

1. Klicken Sie auf **Neue Vorlage**.
1. Geben Sie einen Namen für Ihre Vorlage ein und drücken Sie dann **Eingabetaste** um den Namen zu speichern.
1. Klicken Sie im linken Bedienfeld auf **Vorlagendetails**.
1. Geben **im Abschnitt „Vorlagenzuordnung** eine Gruppe an. Wenn Sie keine Gruppe hinzufügen, wird die Standardprojektgruppe hinzugefügt und das Projekt in Frame.io unter dem entsprechenden Standardteam in Frame.io erstellt.

Fahren Sie mit dem nächsten Abschnitt fort.

![Vorlagengruppe](assets/template-group.png)

### Aufgaben hinzufügen und Frame.io-fähige Benutzer zuweisen

1. Klicken Sie im linken Bedienfeld auf **Vorlagenaufgaben**.
1. Klicken Sie **Vorlagenaufgaben hinzufügen**, um Ihrer Vorlage schnell Aufgaben hinzuzufügen. Sie können zusätzliche Einstellungen später konfigurieren.

   Oder

   Klicken Sie **Neue Vorlagenaufgabe**, um jeweils eine Aufgabe hinzuzufügen und zusätzliche Einstellungen zu konfigurieren.
   ![Aufgaben zur Vorlage hinzufügen](assets/add-tasks-to-template.png)
1. Aufgabennamen hinzufügen.
1. Weisen Sie im **Arbeitsaufträge** Benutzer oder Teams zu. Wenn Sie einen für Frame.io aktivierten Benutzer einzeln oder im Team zuweisen, erhält dieser Mitarbeiter Zugriff auf das Frame.io-Projekt und wird per E-Mail über die Aufgabe im Frame.io-Projekt informiert. Von dieser E-Mail aus können sie sich dem Frame.io-Projekt anschließen und mit der Arbeit beginnen.
1. Wiederholen Sie die Schritte 1 und 2 nach Bedarf.

Fahren Sie mit dem nächsten Abschnitt fort.

### Konfigurieren zusätzlicher Vorlagendetails

Workfront verfügt über leistungsstarke Projektmanagement-Funktionen. Es wird empfohlen, den [Projektvorlagen bearbeiten](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md) zu verwenden, um die folgenden Bereiche der Vorlage zu konfigurieren:

* Übersicht
* Finanzielle Details
* Benutzerdefinierte Formulare
* Projekteinstellungen
* Einstellungen für Aufgaben
* Problemeinstellungen
* Zugriff

### Erstellen eines Projekts aus der Vorlage

Nachdem Sie eine Vorlage erstellt haben, können Sie sie zum Erstellen von Projekten verwenden.

{{step1-to-projects}}

1. Klicken Sie auf **Neues Projekt aus Vorlage**.
1. Beginnen Sie mit der Eingabe des Namens der gewünschten Vorlage über das Suchfeld.
1. Wählen Sie den Vorlagennamen aus und klicken Sie dann auf **Vorlage verwenden**.
   ![Finden Sie Ihre Vorlage](assets/find-your-template.png)
1. Passen Sie alle Projekteinstellungen nach Bedarf an und klicken Sie dann auf **Projekt erstellen**.
1. Klicken Sie im linken Bedienfeld auf **Dokumente**.
1. Verwenden Sie den unidirektionalen Synchronisierungsordner, um Kreativmaterialien automatisch für Frame.io freizugeben. [!BADGE Bald verfügbar]{type=Informative}

   >[!NOTE]
   >
   >Diese Funktion befindet sich derzeit in der Entwicklung. Um Informationen für Benutzer in Frame.io freizugeben, laden Sie die Dateien in die Registerkarte Dokument hoch. Wenn der Status des Projekts auf Aktuell festgelegt ist, werden diese Dateien automatisch an Frame.io übertragen.

1. Ändern Sie in der Projekt-Kopfzeile das Projekt von **Planning** in **Current**.

Nachdem das Projekt erstellt und Kreative fertige Assets hochgeladen haben, können Sie dem Asset in Workfront einen Prüfungs- und Genehmigungs-Workflow zuweisen. Weitere Informationen finden Sie unter [Erstellen einer Dokumentüberprüfungs- oder Genehmigungsanfrage](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->

## Neues Projekt von Grund auf neu erstellen

Sie können bei Bedarf ein neues Projekt von Grund auf neu erstellen.

>[!IMPORTANT]
>
>* Projekte in Frame.io werden von Teams organisiert, die mit Workfront-Gruppen verbunden sind. Es wird empfohlen, zum Erstellen verbundener Projekte eine Projektvorlage zu verwenden, da Sie die Projektgruppe zuvor festlegen können.
>
>
>* Wenn Sie das Projekt von Grund auf neu erstellen, fügt Workfront automatisch die Standardprojektgruppe hinzu, und das Projekt „mirror.frame.io“ wird unter diesem Standardteam in Frame.io erstellt.
>
>Beim Aktualisieren der Gruppe nach der Projekterstellung ändert sich das Frame.io-Team nicht.

### Erstellen des Projekts

{{step1-to-projects}}

1. Klicken Sie auf **Neues Projekt**.
1. Geben Sie einen Namen für Ihr Projekt ein und drücken Sie dann **Eingabetaste**, um den Namen zu speichern.

Fahren Sie mit dem nächsten Abschnitt fort.

### Aufgaben hinzufügen und Frame.io-fähige Benutzer zuweisen

1. Klicken Sie im linken Bedienfeld auf **Aufgaben**.
1. Klicken Sie auf **Aufgaben hinzufügen**, um Ihrem Projekt schnell Aufgaben hinzuzufügen. Sie können zusätzliche Einstellungen später konfigurieren.

   Oder

   Klicken Sie **Neue Aufgabe**, um jeweils eine Aufgabe hinzuzufügen und zusätzliche Einstellungen zu konfigurieren.
   ![Neue Aufgabe](assets/add-project-tasks.png)
1. Aufgabennamen hinzufügen.
1. Weisen Sie im **Arbeitsaufträge** Benutzer oder Teams zu. Wenn Sie einen für Frame.io aktivierten Benutzer einzeln oder im Team zuweisen, erhält dieser Mitarbeiter Zugriff auf das Frame.io-Projekt und wird per E-Mail über die Aufgabe im Frame.io-Projekt informiert. Von dieser E-Mail aus können sie sich dem Frame.io-Projekt anschließen und mit der Arbeit beginnen.
1. Wiederholen Sie die Schritte 1 und 2 nach Bedarf.

Fahren Sie mit dem nächsten Abschnitt fort.

### Hochladen von Kreativmaterial

1. Klicken Sie im linken Bedienfeld auf **Dokumente**.
1. Verwenden Sie den unidirektionalen Synchronisierungsordner, um Kreativmaterialien automatisch für Frame.io freizugeben. [!BADGE Bald verfügbar]{type=Informative}

   >[!NOTE]
   >
   >Diese Funktion befindet sich derzeit in der Entwicklung. Um Informationen für Benutzer in Frame.io freizugeben, laden Sie die Dateien in die Registerkarte Dokument hoch. Wenn der Status des Projekts auf Aktuell festgelegt ist, werden diese Dateien automatisch an Frame.io übertragen

Fahren Sie mit dem nächsten Abschnitt fort.

### Konfigurieren zusätzlicher Projektdetails

Workfront verfügt über leistungsstarke Projektmanagement-Funktionen. Es wird empfohlen, den Artikel [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md) zu verwenden, um die folgenden Bereiche des Projekts zu konfigurieren:

* Übersicht
* Finanzielle Details
* Benutzerdefinierte Formulare
* Projekteinstellungen
* Einstellungen für Aufgaben
* Problemeinstellungen
* Zugriff

### Projekt auf „aktuell“ festlegen

1. Ändern Sie in der Projekt-Kopfzeile das Projekt von Planung in Aktuell.
Nachdem das Projekt erstellt und Kreative fertige Assets hochgeladen haben, können Sie dem Asset in Workfront einen Prüfungs- und Genehmigungs-Workflow zuweisen.

Nachdem das Projekt erstellt und Kreative fertige Assets hochgeladen haben, können Sie dem Asset in Workfront einen Prüfungs- und Genehmigungs-Workflow zuweisen.

Weitere Informationen finden Sie unter [Erstellen einer Dokumentüberprüfungs- oder Genehmigungsanfrage](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md). <!-- name may need to change -->
