---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Konfigurieren von Genehmigungsentscheidungen in  [!DNL Workfront Proof]
description: Sie können Optionen für Genehmigungsentscheidungen für alle Testsendungen konfigurieren, die von [!DNL Workfront Proof] Benutzern in Ihrer Organisation erstellt wurden.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 9e1c2a4e-0641-4334-8ff9-dbb203ccbc82
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 0%

---

# Entscheidungsoptionen für Genehmigungen in [!DNL Workfront Proof] konfigurieren

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront Proof] -Administrator, der einen Premium- oder Auswahlplan verwendet, können Sie die Optionen für Genehmigungsentscheidungen auf folgende Weise für alle von [!DNL Workfront Proof] -Benutzern in Ihrer Organisation erstellten Testsendungen konfigurieren:

* Ändern des Namens der Entscheidung
* Ändern der Reihenfolge der Entscheidungen, die im Testversand-Viewer angezeigt werden
* Entscheiden, welche Entscheidungen angezeigt werden sollen

In diesem Artikel wird Folgendes erläutert:

## Konfigurieren von Entscheidungseinstellungen

1. Klicken Sie auf **[!UICONTROL Kontoeinstellungen]**.
1. Öffnen Sie die Registerkarte **[!UICONTROL Entscheidungen]** .
1. Nehmen Sie eine der folgenden Änderungen vor:

   * Um eine Entscheidung auszublenden, klicken Sie auf **[!UICONTROL Ausblenden]** rechts neben der Entscheidung, die Sie nicht benötigen.
   * Um eine Entscheidung umzubenennen, klicken Sie auf den Namen der Entscheidung, bearbeiten Sie sie und klicken Sie dann außerhalb des Felds auf (oder drücken Sie die Eingabetaste). [!DNL Workfront Proof] aktualisiert den Namen der Entscheidung für alle vorhandenen Testsendungen in Ihrem System.

     >[!IMPORTANT]
     >
     >Behalten Sie die Logik für eine Entscheidung bei, wenn Sie sie umbenennen. Beispielsweise könnte die Standardentscheidung &quot;Abgelehnt&quot;in &quot;Neue Version erforderlich&quot;geändert werden, sollte jedoch nicht in &quot;An Drucker senden&quot;geändert werden.

     Wenn Sie zur Standardeinstellung [!DNL Workfront Proof] zurückkehren möchten, können Sie auf Standardentscheidungen wiederherstellen klicken.

>[!NOTE]
>
>* Die den Entscheidungen zugrunde liegende Logik wird verwendet, um den Gesamtstatus eines Testversand-Workflows zu berechnen, wenn mehrere Entscheidungen verschiedener Ebenen vorliegen.
>* Die Entscheidungen &quot;Genehmigt&quot;und &quot;Mit Änderungen genehmigt&quot;werden in einem automatischen Workflow in der nächsten Phase Trigger.
>* Wenn Sie eine Entscheidung umbenennen und die Logik überprüfen möchten, können Sie im linken Navigationsbereich auf **[!UICONTROL Aktivität]** klicken und Ihr Aktivitätsprotokoll überprüfen, in dem die ursprünglichen Entscheidungen in Klammern angezeigt werden.
>
>  ![2016-12-20_1921.png](assets/2016-12-20-1921-350x132.png)>

## Erstellen von Entscheidungsgründen

Entscheidungsgründe sind eine gute Möglichkeit, zusätzliche Entscheidungsinformationen über einen Beweis zu erfassen.

1. Klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]**.

1. Öffnen Sie die Registerkarte **[!UICONTROL Entscheidungen]** .
Standardmäßig stehen allen Entscheidungsträgern für Ihre Testsendungen die entsprechenden Gründe zur Verfügung. Sie können dies jedoch auf Primäre Entscheidungsträger beschränken.
Je nach Ihren Anforderungen können Sie die Auswahl mehrerer Gründe zulassen oder aus einer Auswahlliste wählen. Sie können die Gründe auch als zwingend angeben, d. h. die Prüfer müssen einen Grund auswählen, bevor sie ihre Entscheidung auf einem Testversand speichern können.
   ![Gründe_setup.png](assets/reasons-setup-350x121.png)

1. Klicken Sie im Abschnitt **[!UICONTROL Gründe]** auf **[!UICONTROL Neuer Grund]**.
   ![new_reason.png](assets/new-reason-350x135.png)

1. Geben Sie in das Feld unter **[!UICONTROL Grund]** einen Titel für den Abschnitt &quot;Gründe&quot;ein.
1. Wenn Sie ein Textfeld einschließen möchten, wählen Sie **[!UICONTROL Textfeld einschließen]**.
1. Klicken Sie auf **[!UICONTROL Speichern]**.
   ![reasons_setup_2.png](assets/reasons-setup-2-350x146.png)
Der wichtigste Schritt besteht darin, die Entscheidungen auszuwählen, für die die Gründe angezeigt werden sollen. Wenn Sie dies vergessen, werden die Gründe nicht auf Ihren Testsendungen angezeigt.

1. Markieren Sie die Kästchen in der Spalte **[!UICONTROL Anzeigegründe]** in der Entscheidungsliste oben auf der Seite. Sie können aus Ihren Gründen eine oder mehrere Entscheidungen auswählen.
   ![reasons_-_decision_selection.png](assets/reasons---decision-selection-350x150.png)

## Post-Entscheidungsnachricht erstellen

Sie können eine Nachricht zur Beitragsentscheidung erstellen, die angezeigt wird, nachdem ein Prüfer seine Entscheidung über den Testversand gespeichert hat.

1. Klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]**.

1. Öffnen Sie die Registerkarte **[!UICONTROL Entscheidungen]** .
1. Klicken Sie im Abschnitt **[!UICONTROL Post-Entscheidungsmeldung]** am Ende der Zeile **[!UICONTROL Meldung]** auf **[!UICONTROL Bearbeiten]** .
Sie können auch entscheiden, ob die Nachricht allen Entscheidungsträgern angezeigt werden soll oder ob Sie sie auf den Primären Entscheidungsträger beschränken möchten.
   ![post_decision_message_set_up.png](assets/post-decision-message-set-up-350x125.png)

1. Geben Sie in der Spalte **[!UICONTROL Nachricht anzeigen]** die Entscheidungen an, auf denen diese Nachricht angezeigt werden soll.
Wenn Sie nicht mindestens eine Entscheidung auswählen, wird die Nachricht nicht in Ihren Testsendungen angezeigt. Aktivieren Sie mindestens ein Kontrollkästchen in dieser Spalte.
   ![post_decision_message_set_up_2.png](assets/post-decision-message-set-up-2-350x151.png)
