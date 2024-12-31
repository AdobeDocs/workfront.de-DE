---
product-previous: workfront-proof
product-area: documents;system-administration;user-management
navigation-topic: users-workfront-proof
title: Benutzer zwischen Konten verschieben mit [!DNL Workfront Proof]
description: Wenn Sie Administrator  [!DNL Workfront Proof]  und mindestens ein Satellitenkonto mit Ihrem Hauptkonto verbunden ist, können Sie die Benutzer zwischen all diesen Konten verschieben.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: a7cf8086-8291-4a27-abd1-afd8217f1fcc
source-git-commit: 1a85f2a214036b62d13cb01f0b7a77392648a5fd
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Benutzer mithilfe von [!DNL Workfront Proof] zwischen Konten verschieben

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie Administrator eines [!DNL Workfront]-Korrekturabzugs sind und mit Ihrem Hauptkonto ein oder mehrere Satellitenkonten verbunden sind, können Sie die Benutzer zwischen all diesen Konten verschieben.

## Benutzer werden zwischen verbundenen Konten verschoben

1. Klicken Sie **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]**.

1. Öffnen Sie die Registerkarte **[!UICONTROL Benutzer]**.
1. Klicken Sie auf **[!UICONTROL Symbol „Benutzer]**&quot; (1). ![Move_user2.png](assets/move-user2-350x95.png)

1. Bestätigen Sie im angezeigten Feld Benutzer verschieben den Benutzer, den Sie verschieben möchten (1).
1. Wählen Sie ein Zielkonto aus der Liste Verbundene Konten (2).
1. Weisen Sie die Profilberechtigung (3) zu, die dieser Benutzer für das neue Konto haben soll.
1. Wählen Sie einen Benutzer (4) aus, der für die Elemente, die nicht verschoben werden sollen, verantwortlich sein soll.
Dazu gehören die Elemente, die Sie im alten Konto belassen möchten, und die Elemente, die nicht verschoben werden können (siehe [Elemente, die nicht verschoben werden können](https://support.workfront.com/knowledge/articles/115004087708/en-us?brand_id=662728&amp;return_to=%2Fhc%2Fen-us%2Farticles%2F115004087708#Items-that-can&#39;t-be-moved) unten).

1. Aktivieren Sie die Kontrollkästchen, wenn Sie die Korrekturabzüge (5) und Dateien (6) zusammen mit dem/der Benutzenden verschieben möchten.
1. Erstellen Sie einen Namen für den Ordner (7), in dem alle verschobenen Elemente in dem neuen Konto abgelegt werden.
1. Klicken Sie **[!UICONTROL Benutzer verschieben]** (8), um den Vorgang zu starten.
   ![Moving_users_pop-up.png](assets/moving-users-pop-up-350x380.png)

Wenn Sie den/die Benutzende(n) ohne seine/ihre Korrekturabzüge und Dateien verschieben möchten, wird diese Aktion sofort ausgeführt. Wenn Sie den Benutzer zusammen mit seinen Korrekturabzügen und Dateien verschieben, wird das Benutzerprofil sofort neu zugewiesen, aber die Korrekturabzüge und Dateien werden nach und nach im Zielkonto angezeigt, da dieser Vorgang Zeit zur Übertragung der Daten erfordert.

Je nach Anzahl der Dateien und Korrekturabzüge kann das Verschieben von Prozessen einige Minuten bis zu ein paar Stunden dauern.

>[!NOTE]
>
>Wenn Sie vermuten, dass der Vorgang länger als erwartet dauert oder die verschobenen Korrekturabzüge und/oder Dateien nicht im neuen Konto angezeigt werden, wenden Sie sich bitte an unser Support-Team.

## Elemente, die nicht verschoben werden können

### Ordner, die vom verschobenen Benutzer erstellt wurden oder ihm gehören

Aufgrund der Art verschiedener Berechtigungen, die auf Ordner und deren Inhalte angewendet werden (z. B. können diese mit anderen Benutzern und Konten geteilt werden), können wir keine Ordnerstrukturen mit dem Benutzer verschieben.

Wenn ein Ordner dem verschobenen Benutzer gehört, wird die Eigentümerschaft an den ausgewählten Benutzer (4) im Pop-up „Benutzer verschieben“ übertragen.

>[!NOTE]
>
>Wenn ein Ordner vom verschobenen Benutzer erstellt wurde, bleibt er dessen Ersteller - nur das Eigentum wird übertragen. Der Ordner bleibt für verschobene Benutzende in der Seitenleiste ihres neuen Kontos sichtbar. Der verschobene Benutzer hat weiterhin schreibgeschützten Zugriff auf die Elemente, die in diesen Ordnern platziert sind.

Wenn Sie nicht möchten, dass der verschobene Benutzer diese Berechtigungen behält, oder der verschobene Benutzer seine alten Ordner im alten Konto und nicht sehen möchte, besteht die Lösung hier darin, die Ordner wie folgt zu löschen:

1. Erstellen Sie einen neuen Ordner mit dem alten Konto.
1. Verschieben Sie alle Elemente aus den Ordnern der verschobenen Person in den neu erstellten Ordner.
1. Löschen Sie alle Ordner, die von dem verschobenen Benutzer übrig geblieben sind.

### Sets von Versionen mit verschiedenen Inhabern

Wenn ein Korrekturabzug einige Versionen hat und jede Version einem anderen Benutzer gehört, werden die Versionen, die dem verschobenen Benutzer gehören, nicht mitverschoben. Das Eigentum an diesen Versionen wird gemäß Ihrer Wahl (4) im Feld Benutzer verschieben auf einen anderen Benutzer übertragen. (Weitere Informationen finden Sie unter .)

>[!NOTE]
>
>Ein verschobener Benutzer muss Eigentümer aller Korrekturabzugsversionen im Satz sein, damit der Korrekturabzug verschoben werden kann.

### Gruppen

Gruppen müssen vom verschobenen Benutzer in seinem neuen Konto neu erstellt werden. Weitere Informationen finden Sie unter [Erstellen von Proofing-Gruppen mit [!DNL Workfront Proof]](../../../workfront-proof/wp-mnguserscontacts/groups/create-proofing-groups.md).

### Benutzerdefinierte Ansichten

Persönliche benutzerdefinierte Ansichten müssen vom verschobenen Benutzer in seinem neuen Konto neu erstellt werden. Weitere Informationen finden Sie unter [Erstellen und Verwalten von benutzerdefinierten Ansichten in [!DNL Workfront Proof] Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

### Benutzerdefinierte Felder

Benutzerdefinierte Felder können nicht verschoben werden und Daten aus benutzerdefinierten Feldern gehen verloren. Stellen Sie daher sicher, dass Sie vor dem Verschieben Berichte zu den erforderlichen Elementen erstellen.

### Automatisierte Workflow-Vorlagen

Automatisierte Workflow-Vorlagen müssen im neuen Konto neu erstellt werden, aber die Stadien bleiben bei den verschobenen Korrekturabzügen erhalten, die mit den Vorlagen erstellt wurden.

### Aktionen bei Kommentaren

Aktionen zu Kommentaren bleiben auf den Korrekturabzügen, aber es ist nicht mehr möglich, nach ihnen zu filtern. Die Lösung bestünde darin, übereinstimmende Aktionen für das neue Konto zu erstellen und die Kommentare bei Bedarf mit den neuen Aktionen umzukennzeichnen.
