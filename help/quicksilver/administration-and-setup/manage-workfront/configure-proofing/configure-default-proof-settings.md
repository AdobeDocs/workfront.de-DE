---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Konfigurieren der standardmäßigen Testversandeinstellungen
description: Mit diesen Einstellungen können Sie Standardwerte festlegen, die für alle neuen Testsendungen gelten, die von Ihren Benutzern erstellt wurden. Die meisten dieser Einstellungen können jedoch beim Erstellen eines Testversands überschrieben werden.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 7%

---

# Konfigurieren der standardmäßigen Testversandeinstellungen

Mit diesen Einstellungen können Sie Standardwerte festlegen, die für alle neuen Testsendungen gelten, die von Ihren Benutzern erstellt wurden. Die meisten dieser Einstellungen können jedoch beim Erstellen eines Testversands überschrieben werden.

## Neue Standardeinstellungen für den Testversand konfigurieren

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup**.![](assets/main-menu-icon.png)
1. Klicken Sie im linken Bereich auf **Testsendungen** > **Testversandeinstellungen**.
1. Konfigurieren Sie im Abschnitt **Neue Testversand-Standardwerte** die folgenden Einstellungen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Empfängerinnen und Empfänger</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anmeldung erforderlich</td> 
      <td> <p>Überprüfer müssen sich mit ihrer E-Mail-Adresse und ihrem Passwort anmelden, bevor sie in Ihrem Unternehmenskonto erstellte Testsendungen anzeigen können. Wenn diese Option aktiviert ist, können Benutzer den Testversand nicht für Gastreviewer freigeben.</p> <p><b>WICHTIG</b>: Wenn diese Option aktiviert ist, ist die Anmeldung für alle neu erstellten Testsendungen erforderlich.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kopieren des Inhabers aus dem Original-Korrekturabzug für neue Versionen</td> 
      <td> <p>Der Eigentümer der ersten Version eines Testversands ist auch Eigentümer aller aufeinander folgenden Versionen des Testversands, unabhängig davon, wer diese Versionen erstellt. Diese Einstellung ist standardmäßig aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzern die Möglichkeit geben, ihre Kommentare zu Korrekturabzügen zu löschen</td> 
      <td>Benutzer können ihre eigenen Kommentare löschen. Diese Einstellung ist standardmäßig aktiviert.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entscheidungen müssen elektronisch signiert werden </td> 
      <td> <p>Entscheidungsträger werden aufgefordert, ihre Workfront-Anmeldedaten einzugeben, wenn sie eine Entscheidung über einen Testversand treffen.</p> <p><b>WICHTIG</b>: Wenn diese Option aktiviert ist, können Benutzer den Testversand nicht für Gastreviewer freigeben, die keine Anmeldeinformationen haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Frist</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardgültigkeit festlegen</td> 
      <td> <p>Das System wendet diese Frist auf alle neuen Testsendungen in Ihrem Konto an, die keinen automatisierten Workflow haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benachrichtigung der Empfänger vor Gefährdung des Testversands</td> 
      <td>Die Empfänger werden per E-Mail benachrichtigt, bevor der Testversand in Abhängigkeit von der oben genannten Frist als gefährdet gilt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>E-Mail-Benachrichtigungen</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Empfänger benachrichtigen, wenn sie zu einem Korrekturabzug hinzugefügt werden</td> 
      <td>Empfänger werden per E-Mail benachrichtigt, wenn sie einem Testversand hinzugefügt werden.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern**.

## Konfigurieren von Testentscheidungen

Benutzer können Testversandentscheidungen verwenden, um den Status des Testversands nach Überprüfung anzugeben.

>[!NOTE]
>
>Die Logik hinter den Testversandentscheidungen wird verwendet, um den Gesamtstatus eines Testversand-Workflows zu berechnen, wenn mehrere Entscheidungen verschiedener Ebenen vorliegen. Die Entscheidungen &quot;Genehmigt&quot; und &quot;Mit Änderungen validiert&quot; werden im nächsten Schritt in einem automatischen Workflow Trigger.

So konfigurieren Sie Testversandentscheidungen:

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup**.![](assets/main-menu-icon.png)
1. Klicken Sie im linken Bereich auf **Testsendungen** > **Testversandeinstellungen**.
1. Im Abschnitt **Entscheidungen** können Sie

   1. **Benennen Sie die Entscheidung um**: Klicken Sie auf den Text im Entscheidungsfeld und beginnen Sie mit der Eingabe der neuen Entscheidungsbeschriftung.

      >[!TIP]
      >
      >Behalten Sie die Logik für eine Entscheidung bei, wenn Sie sie umbenennen. Beispielsweise kann die Standardentscheidung Abgelehnt in *Neue Version erforderlich* geändert werden, sie sollte jedoch nicht in *An Drucker senden* geändert werden.

      ![](assets/rename-decision-350x109.png)

   1. **Die Entscheidungsreihenfolge neu anordnen**: Ziehen Sie die Entscheidungsfelder in die Reihenfolge, in der sie im Testversand-Viewer angezeigt werden sollen.

      ![](assets/move-decision-350x110.png)

   1. **Entscheidung ausblenden**: Bewegen Sie den Mauszeiger über das Entscheidungsfeld und klicken Sie auf das Symbol Ausblenden in der oberen rechten Ecke.

      ![](assets/hide-decision-350x109.png)

1. (Optional) Um zu den Workfront-Standardeinstellungen zurückzukehren, klicken Sie auf **Standardangaben wiederherstellen**.
1. Klicken Sie auf **Speichern**.
