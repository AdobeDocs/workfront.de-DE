---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Verschieben von Benutzern zwischen Konten mithilfe von [!DNL Workfront Proof]
description: Wenn Sie [!DNL Workfront Proof] und wenn ein oder mehrere Satellitenkonten mit Ihrem Hauptkonto verbunden sind, können Sie die Benutzer zwischen diesen Konten verschieben.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 0%

---

# Verschieben von Benutzern zwischen Konten mithilfe von [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie [!DNL Workfront] Testversand-Administrator und Sie haben ein oder mehrere Satellitenkonten mit Ihrem Hauptkonto verbunden, können Sie die Benutzer zwischen all diesen Konten verschieben.

## Wechsel zwischen Connected Accounts

1. Klicken **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]**.

1. Öffnen Sie die **[!UICONTROL Benutzer]** Registerkarte.
1. Klicken Sie auf **[!UICONTROL Benutzer verschieben]** Symbol (1). ![Move_user2.png](assets/move-user2-350x95.png)

1. Bestätigen Sie im sich öffnenden Feld Benutzer verschieben den Benutzer, den Sie verschieben möchten (1).
1. Wählen Sie in der Liste der verbundenen Konten ein Zielkonto aus (2).
1. Weisen Sie die Profilberechtigung (3) zu, die dieser Benutzer für das neue Konto haben sollte.
1. Wählen Sie einen Benutzer (4) aus, der Eigentümer der nicht verschobenen Elemente sein soll.
Dazu gehören die Elemente, die Sie im alten Konto belassen möchten, und die Elemente, die nicht verschoben werden können (siehe [Elemente, die nicht verschoben werden können](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) unten).

1. Aktivieren Sie die Kontrollkästchen, wenn Sie die Testsendungen (5) und Dateien (6) zusammen mit dem Benutzer verschieben möchten.
1. Erstellen Sie einen Namen für den Ordner (7), in dem alle verschobenen Elemente im neuen Konto abgelegt werden.
1. Klicken **[!UICONTROL Benutzer verschieben]** (8), um den Prozess zu starten.
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

Wenn Sie den Benutzer ohne Testsendungen und Dateien verschieben, wird diese Aktion sofort durchgeführt. Wenn Sie den Benutzer zusammen mit seinen Testsendungen und Dateien verschieben, wird das Profil des Benutzers sofort neu zugewiesen. Die Testsendungen und Dateien werden jedoch allmählich im Zielkonto angezeigt, da für diesen Vorgang Zeit zum Übertragen der Daten benötigt wird.

Je nach der Anzahl der Dateien und Testsendungen kann das Verschieben von Dateien etwas von einigen Minuten bis zu einigen Stunden dauern.

>[!NOTE]
>
>Wenn Sie vermuten, dass der Prozess länger dauert als erwartet oder die verschobenen Testsendungen und/oder Dateien nicht auf dem neuen Konto erscheinen, wenden Sie sich bitte an unser Support-Team.

## Elemente, die nicht verschoben werden können

### Ordner, die vom Benutzer &quot;Verschieben&quot;erstellt oder gehört wurden

Aufgrund der verschiedenen Berechtigungen, die auf Ordner und deren Inhalt angewendet werden (z. B. sie können für andere Benutzer und Konten freigegeben werden), können wir keine Ordnerstrukturen für den Benutzer verschieben.

Wenn ein Ordner dem verschobenen Benutzer gehört, wird das Eigentum an den ausgewählten Benutzer (4) im Popup &quot;Benutzer verschieben&quot;übertragen.

>[!NOTE]
>
>Wenn ein Ordner vom verschobenen Benutzer erstellt wurde, bleibt er dessen Ersteller - nur das Eigentum wird übertragen. Der Ordner bleibt für den verschobenen Benutzer in der Seitenleiste seines neuen Kontos sichtbar. Der verschobene Benutzer hat weiterhin &quot;schreibgeschützt&quot;Zugriff auf die Elemente, die in diesen Ordnern platziert werden.

Wenn Sie nicht möchten, dass der verschobene Benutzer diese Berechtigungen behält oder der verschobene Benutzer seine alten Ordner nicht im alten&amp;-Konto sehen möchte, besteht die Lösung hier darin, die Ordner wie folgt zu löschen:

1. Erstellen Sie einen neuen Ordner für das alte Konto.
1. Verschieben Sie alle Elemente aus den Ordnern des verschobenen Benutzers in den neu erstellten Ordner.
1. Löschen Sie alle vom verschobenen Benutzer verbleibenden Ordner.

### Versionssätze mit verschiedenen Eigentümern

Wenn ein Testversand einige Versionen enthält und jeder von ihnen einem anderen Benutzer gehört, werden die Versionen des verschobenen Benutzers nicht verschoben. Das Eigentum an diesen Versionen wird gemäß Ihrer Wahl (4) im Feld Benutzer verschieben auf einen anderen Benutzer übertragen. (Weitere Informationen finden Sie unter .)

>[!NOTE]
>
>Ein verschobener Benutzer muss Inhaber aller Testversandversionen im Satz sein, damit der Testversand weitergeführt werden kann.

### Gruppen

Gruppen müssen vom verschobenen Benutzer in seinem neuen Konto neu erstellt werden. Weitere Informationen finden Sie unter [Erstellen von Testversandgruppen mit [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### Benutzerdefinierte Ansichten

Persönliche benutzerdefinierte Ansichten müssen vom verschobenen Benutzer in seinem neuen Konto neu erstellt werden. Weitere Informationen finden Sie unter [Benutzerdefinierte Ansichten erstellen und verwalten in [!DNL Workfront Proof] Testversand](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Benutzerdefinierte Felder

Benutzerdefinierte Felder können nicht verschoben werden und Daten aus benutzerdefinierten Feldern gehen verloren. Generieren Sie daher vor dem Verschieben Berichte zu den erforderlichen Elementen.

### Automatisierte Workflow-Vorlagen

Automatisierte Workflow-Vorlagen müssen für das neue Konto neu erstellt werden, die Phasen werden jedoch bei den verschobenen Testsendungen beibehalten, die mit den Vorlagen erstellt wurden.

### Aktionen zu Kommentaren

Die Maßnahmen zu Kommentaren werden zwar weiterhin bei den Testsendungen durchgeführt, sie können jedoch nicht mehr danach gefiltert werden. Eine Lösung bestünde darin, übereinstimmende Aktionen für das neue Konto zu erstellen und die Kommentare bei Bedarf erneut mit den neuen Aktionen zu kennzeichnen.
