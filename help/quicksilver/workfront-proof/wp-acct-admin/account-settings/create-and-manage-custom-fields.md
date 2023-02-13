---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: account-settings-workfront-proof
title: Erstellen und verwalten Sie benutzerdefinierte Felder in [!DNL Workfront Proof]
description: A Select oder Premium [!DNL Workfront] Für die Verwendung dieser Funktion ist ein Plan erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter Workfront-Pläne .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 87c8aff7-b638-4d14-9c5a-7e316f1ec608
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '988'
ht-degree: 0%

---

# Erstellen und verwalten Sie benutzerdefinierte Felder in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

A Select oder Premium [!DNL Workfront] Für die Verwendung dieser Funktion ist ein Plan erforderlich. Weitere Informationen zu den verschiedenen verfügbaren Plänen finden Sie unter [Workfront-Pläne](https://www.workfront.com/plans).

Mit benutzerdefinierten Feldern können Sie zusätzliche Daten erfassen, wenn Sie einen neuen Testversand, einen neuen Benutzer oder einen neuen Gast erstellen.

Beispielsweise können Benutzer, die einen neuen Testversand erstellen, einen zusätzlichen Abschnitt einschließen, der es ihnen ermöglicht, eine Auftragsnummer, einen Abteilungscode oder eine Lieferantenreferenz zu erfassen.

>[!NOTE]
>
>* Wenn Sie diese Art von Informationen über benutzerdefinierte Felder auf der Seite Neuer Testversand erfassen, können Sie auch die Länge Ihres Testversands verkürzen, da diese Details nicht im Namen enthalten sein müssen. Weitere Informationen zur Seite Neuer Testversand finden Sie unter &quot;Erstellen von Testsendungen in [!DNL Workfront Proof].&quot;
>
>Sobald ein benutzerdefiniertes Feld für einen Testversand, einen Benutzer oder eine Kontaktperson verwendet wurde, können Sie es nicht mehr löschen oder den Feldtyp bearbeiten. Sie können sie jedoch verbergen (über die [!UICONTROL Benutzerdefinierte Feldeinstellungen] -Seite), damit sie nicht für neue Elemente verwendet wird.
>
>Wenn Sie einen benutzerdefinierten Feldabschnitt ausblenden, werden auch alle Felder im Abschnitt ausgeblendet, selbst wenn die einzelnen Felder als sichtbar festgelegt sind.

In diesem Artikel wird beschrieben, wie Sie Folgendes tun:

## Benutzerdefinierte Felder erstellen

Zunächst müssen Sie den Abschnitt Benutzerdefiniertes Feld einrichten, dem Sie benutzerdefinierte Felder hinzufügen.

1. Klicken **[!UICONTROL Einstellungen]** >**[!UICONTROL Kontoeinstellungen]**, und öffnen Sie dann die **[!UICONTROL Benutzerdefinierte Felder]** Registerkarte.

1. Klicken **[!UICONTROL Abschnitt für benutzerdefinierte Felder hinzufügen]** im entsprechenden Modul (Testversand, Benutzer oder Kontakte).
1. Geben Sie einen **Name** Klicken Sie für den Abschnitt mit benutzerdefinierten Feldern auf **[!UICONTROL Speichern]**.

   Jetzt können Sie benutzerdefinierte Felder im Abschnitt einrichten:

1. Klicken Sie auf **[!UICONTROL Benutzerdefinierte Feldeinstellungen]** Registerkarte, um die Seite zu aktualisieren.
1. Klicken Sie auf den Namen Ihres neuen benutzerdefinierten Felds, um den **[!UICONTROL Benutzerdefiniertes Feld] Abschnitt** Seite für den neuen Abschnitt.
1. Klicken Sie auf **[!UICONTROL Neues benutzerdefiniertes Feld]** in der Nähe der oberen rechten Ecke.
1. Im **[!UICONTROL Neues benutzerdefiniertes Feld]** Seite, die angezeigt wird, geben Sie die Details für das benutzerdefinierte Feld an:

   | **Obligatorisch** | Workfront erfordert, dass Benutzer das Feld ausfüllen. |
   |---|---|
   | **Durchsuchbar** | Ermöglicht Benutzern das Suchen nach Elementen durch Suchen nach den benutzerdefinierten Felddaten. |
   | **Ausgeblendet** | Blendet das benutzerdefinierte Feld im [!UICONTROL Neuer Testversand], neuer Gast und [!UICONTROL Neuer Benutzer] pages |

   {style=&quot;table-layout:auto&quot;}

1. Klicken Sie auf **[!UICONTROL Speichern]**.
1. Im **Benutzerdefiniertes Feld** angezeigt wird, klicken Sie auf die **[!UICONTROL Benutzerdefinierte Feldeinstellungen]** Registerkarte, um die Seite zu aktualisieren.

1. Nehmen Sie weitere Änderungen an den Einstellungen für das Feld vor:

   * Blenden Sie den Abschnitt für das benutzerdefinierte Feld ein oder aus, indem Sie auf die Schaltfläche **[!UICONTROL Mehr]** (drei Punkte) rechts neben dem Namen des benutzerdefinierten Felderabschnitts und klicken Sie dann auf **[!UICONTROL Abschnitt ausblenden]** oder **[!UICONTROL Bereich einblenden]**.

   * Durch Auswahl der Schaltfläche **[!UICONTROL Mehr]** (drei Punkte) rechts neben dem Namen des benutzerdefinierten Felderabschnitts und klicken Sie dann auf **[!UICONTROL Benutzerdefiniertes Feld ausblenden]** oder **[!UICONTROL Benutzerdefiniertes Feld einblenden]**.

   * Ändern Sie die Reihenfolge der Felder mithilfe der Pfeile nach oben/unten, die rechts neben ihrem Namen angezeigt werden (wenn Sie mehrere Felder in einem Abschnitt hinzugefügt haben).

1. Öffnen Sie die **[!UICONTROL Sichtbarkeitsregeln]** Registerkarte.\
   Mit Sichtbarkeitsregeln können Sie festlegen, welche zusätzlichen Felder angezeigt werden, je nach Abschluss des ersten benutzerdefinierten Felds. Wenn das abhängige Feld beispielsweise A und das Kontrollfeld X ist, ist Feld A nur sichtbar, wenn Feld X ausgefüllt ist.

   Sie können Werte mithilfe von Kontrollwerten bestimmen, welche Werte im Kontrollfeld angezeigt werden, was bei Auswahl dazu führt, dass das abhängige Feld sichtbar wird. Angenommen, das abhängige Feld ist A und das Kontrollfeld X, und die Kontrollwerte in X sind nur Optionen 1 und 2. Das bedeutet, dass Feld A nur sichtbar ist, wenn Feld X Option 1 oder 2 ausgewählt ist. Wenn also Feld X Optionen 3 oder 4 ausgewählt sind, wird Feld A nicht angezeigt. Öffnen Sie die **[!UICONTROL Sichtbarkeitsregeln]** Registerkarte.

   So fügen Sie eine Sichtbarkeitsregel hinzu:

   1. Klicken **[!UICONTROL Neue Sichtbarkeitsregel]** für das Modul, dem Sie die Regel hinzufügen möchten.
   1. Wählen Sie die gewünschten Einstellungen für die Regel aus und klicken Sie auf **[!UICONTROL Speichern]**.

1. Öffnen Sie die **[!UICONTROL Abhängigkeitsregeln]** Registerkarte.

   Mit Abhängigkeitsregeln können Sie die im abhängigen Feld verfügbaren Optionen bestimmen, wenn bestimmte Optionen im Kontrollfeld ausgewählt sind. Wenn das abhängige Feld beispielsweise &quot;B&quot;und das Kontrollfeld &quot;Y&quot;lautet, können Sie es wie folgt einrichten:

   Wenn Option 1 in Feld Y ausgewählt ist, werden nur die Optionen 1 und 2 in Feld B angezeigt.

   Wenn Option 2 in Feld Y ausgewählt ist, werden nur die Optionen 3 und 4 in Feld B angezeigt.

   So fügen Sie eine Abhängigkeitsregel hinzu:

   1. Klicken **[!UICONTROL Neue Abhängigkeitsregel]** für das Modul, das Sie der Regel hinzufügen möchten.
   1. Wählen Sie die Einstellungen für die Abhängigkeit aus und klicken Sie auf **[!UICONTROL Speichern]**.

## Benutzerdefinierte Felder verwalten

Sie können die Details Ihres Bereichs Benutzerdefiniertes Feld oder einzelne benutzerdefinierte Felder anzeigen und bearbeiten.

1. Klicken **[!UICONTROL Einstellungen]** >**[!UICONTROL Kontoeinstellungen]**, und öffnen Sie dann die **[!UICONTROL Benutzerdefinierte Felder]** Registerkarte.

1. Klicken Sie auf den Namen des benutzerdefinierten Feldabschnitts oder des einzelnen benutzerdefinierten Felds.
1. (Bedingt) Wenn Sie einen benutzerdefinierten Feldabschnitt verwalten, nehmen Sie eine der folgenden Änderungen in der **[!UICONTROL Benutzerdefinierter Feldabschnitt]** Seite:

   * Bearbeiten Sie den Namen des Abschnitts.
   * Verschieben Sie es in ein anderes Modul.
   * Bereich ausblenden/einblenden.

1. (Bedingt) Wenn Sie ein benutzerdefiniertes Feld verwalten, nehmen Sie eine der folgenden Änderungen an der **[!UICONTROL Benutzerdefiniertes Feld]** Seite:

   * Verschieben Sie das Feld in einen anderen Abschnitt.
   * Bearbeiten Sie den Namen des Felds.
   * Hilfetext für die Eingabe (neben dem Feldabschnitt wird ein Fragezeichen-Symbol angezeigt und der Text wird angezeigt, wenn der Mauszeiger darüber bewegt wird).
   * Aktivieren/deaktivieren Sie die **[!UICONTROL Obligatorisch]** auf das Feld gesetzt.
   * Aktivieren/deaktivieren Sie die **[!UICONTROL Durchsuchbar]** auf das Feld gesetzt.
   * Das Feld ein-/ausblenden.
   * Bearbeiten Sie den Feldtyp.
   * Legen Sie einen Standardwert für das Feld fest/bearbeiten Sie ihn.
   * Einrichten von Sichtbarkeits- und Abhängigkeitsregeln (wie oben in den Schritten 11 und 12 beschrieben).
