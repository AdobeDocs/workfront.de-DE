---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Verwalten von Proof-Rollen in  [!DNL Workfront Proof]
description: Mithilfe von Proof-Rollen können Sie Benutzern Berechtigungen erteilen, die durch das in ihrem Benutzerprofil konfigurierte Berechtigungsprofil eingeschränkt sind.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 0%

---

# Verwalten von Proof-Rollen in [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Mithilfe von Proof-Rollen können Sie Benutzern Berechtigungen erteilen, die durch das in ihrem Benutzerprofil konfigurierte Berechtigungsprofil eingeschränkt sind. (Weitere Informationen zu Berechtigungsprofilen finden Sie unter [Profile für Testberechtigungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Die Rollen für Testsendungen unterscheiden sich von den Kontoprofilen. Ihr Kontoprofil bezieht sich auf die allgemeine Berechtigungsstufe Ihres Kontos und wirkt sich auf die Rechte aus, die Sie für alle Testsendungen in Ihrem Konto haben, selbst wenn diese nicht explizit für Sie freigegeben wurden.

Weitere Informationen finden Sie unter [Profile für Testberechtigungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Über Proof Roles

Die folgenden Rollen für den Testversand werden Benutzern zum Zeitpunkt der Einladung zur Überprüfung des Testversands für einen individuellen Testversand zugewiesen:

* [Schreibgeschützt](#read-only)
* [Prüfende Person](#reviewer)
* [Genehmigende Person](#approver)
* [Prüfer und genehmigende Person](#reviewer-approver)
* [Verfassende Person](#author)
* [Moderierende Person](#moderator)

Die Rolle &quot;Testversand&quot;definiert, welche Aktionen ein Validierer in Bezug auf diesen spezifischen Testversand ausführen kann.

Wenn Sie beispielsweise Überprüfer sind, werden Sie aufgefordert, den Testversand durch Hinzufügen von Markierungen und Kommentaren zu überprüfen. Wenn Sie Reviewer und Genehmiger sind, werden Sie aufgefordert, den Testversand zu überprüfen und auch eine Entscheidung über ihn zu treffen.

Bestimmte Testversand-Rollen verleihen einem Validierer Bearbeitungsrechte für den Testversand (auch wenn sein Profil dies nicht tut) und ermöglichen ihm die Verwendung einiger zusätzlicher Funktionen wie das Hinzufügen von Aktionen zu Kommentaren, das Erstellen neuer Versionen und das Hinzufügen weiterer Validierer zum Testversand.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Verwenden von Aktionen für Testversand-Kommentare](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Freigeben eines Testversands in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Schreibgeschützt

{#read-only}

![cleaner.png](assets/cleaner.png) Kann einen Beweis anzeigen

![no.png](assets/no.png) Markups können nicht hinzugefügt werden

![no.png](assets/no.png) Kommentare können nicht hinzugefügt werden

![no.png](assets/no.png) Entscheidung kann nicht getroffen werden

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht gelöscht werden

![no.png](assets/no.png) Hat keine Bearbeitungsrechte für den Testversand

>[!NOTE]
>
>Wenn ein Ordner für einen Benutzer von [!DNL Workfront Proof] freigegeben wird, erhält er automatisch Schreibschutzrechte für alle vorhandenen und anschließend hinzugefügten Elemente im Ordner.

Weitere Informationen finden Sie unter [Ordner in  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md) freigeben.

### Prüfende Person {#reviewer}

![cleaner.png](assets/cleaner.png) Kann einen Beweis anzeigen

![cleaner.png](assets/cleaner.png) Kann Markups hinzufügen

![cleaner.png](assets/cleaner.png) Kann Kommentare hinzufügen

![[!DNL cleaner].png](assets/cleaner.png) Kann eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind

![no.png](assets/no.png) Entscheidung kann nicht getroffen werden

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet oder gelöscht werden

![no.png](assets/no.png) Hat keine Bearbeitungsrechte für den Testversand

### Genehmigende Person {#approver}

![cleaner.png](assets/cleaner.png) Kann einen Beweis anzeigen

![cleaner.png](assets/cleaner.png) Kann eine Entscheidung treffen

![no.png](assets/no.png) Markups können nicht hinzugefügt werden

![no.png](assets/no.png) Kommentare können nicht hinzugefügt werden

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet oder gelöscht werden

![no.png](assets/no.png) Hat keine Bearbeitungsrechte für den Testversand

### Prüfer und genehmigende Person {#reviewer-approver}

![cleaner.png](assets/cleaner.png) Kann einen Beweis anzeigen

![cleaner.png](assets/cleaner.png) Kann Markups hinzufügen

![cleaner.png](assets/cleaner.png) Kann Kommentare hinzufügen

![[!DNL cleaner].png](assets/cleaner.png) Kann eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind

![cleaner.png](assets/cleaner.png) Kann eine Entscheidung treffen

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet oder gelöscht werden

![no.png](assets/no.png) Hat keine Bearbeitungsrechte für den Testversand

### Verfassende Person {#author}

![cleaner.png](assets/cleaner.png) Kann Markups hinzufügen

![cleaner.png](assets/cleaner.png) Kann Kommentare hinzufügen

![[!DNL cleaner].png](assets/cleaner.png) Kann eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind

![cleaner.png](assets/cleaner.png) Kann eine Entscheidung treffen

![cleaner.png](assets/cleaner.png) Kann neue Versionen senden

![cleaner.png](assets/cleaner.png) Kann eine Kopie des Testversands erstellen

![cleaner.png](assets/cleaner.png) Kann den Testversand für andere Personen freigeben

![cleaner.png](assets/cleaner.png) Kann Aktionen auf Kommentare anwenden

![cleaner.png](assets/cleaner.png) Kann Kommentare auflösen

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet oder gelöscht werden

>[!NOTE]
>
>Diese Rolle kann nur Benutzern von [!DNL Workfront Proof] zugewiesen werden.

### Moderierende Person {#moderator}

![cleaner.png](assets/cleaner.png) Kann Markups hinzufügen

![cleaner.png](assets/cleaner.png) Kann Kommentare hinzufügen

![[!DNL cleaner].png](assets/cleaner.png) Kann eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind

![cleaner.png](assets/cleaner.png) Kann eine Entscheidung treffen

![cleaner.png](assets/cleaner.png) Kann neue Versionen senden

![cleaner.png](assets/cleaner.png) Kann neue Überprüfer hinzufügen

![cleaner.png](assets/cleaner.png) Kann Aktionen auf Kommentare anwenden

![cleaner.png](assets/cleaner.png) Kann Kommentare auflösen

![cleaner.png](assets/cleaner.png) Kann Kommentare und Antworten auf den Testversand löschen (von sich selbst oder anderen erstellt)

* Durch Löschen des ersten Kommentars in einem Kommentar-Thread wird der gesamte Thread gelöscht
* Durch Löschen von Antworten im Kommentar-Thread wird diese Antwort nur gelöscht

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet werden

Diese Funktion ermöglicht es der Person, die Testversandkommentare zu verwalten und zu moderieren, sodass sie nur relevante Kommentare zum Testversand speichern und nicht relevante Kommentare entfernen kann.

>[!NOTE]
>
>Diese Rolle kann nur Benutzern von [!DNL Workfront Proof] zugewiesen werden.

## Zuweisen von Testrollen

Sie können Testversandrollen beim Erstellen neuer Testsendungen, beim Erstellen neuer Versionen vorhandener Testsendungen oder bei vorhandenen Testsendungen zuweisen.

### Neue Testsendungen {#new-proofs}

Während der Erstellung des Testversands (1) können den Validierern auf der Seite [!UICONTROL Neuer Testversand] Testversandrollen zugewiesen werden.

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Neue Versionen {#new-versions}

Bei der Erstellung einer neuen Version eines Testversands werden die validierungsverantwortlichen Benutzer der vorherigen Version automatisch angezeigt (mit der Rolle der vorherigen Version).

Sie können die Testversandrollen bearbeiten, die bei der Erstellung der neuen Version (1) auf die Validierungsverantwortlichen angewendet werden.

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Vorhandene Testsendungen {#existing-proofs}

Wenn Sie die Rolle einer Person in einem vorhandenen Testversand ändern möchten, können Sie dies auf der Seite [!UICONTROL Testversand-Details] tun, indem Sie ihre Rolle im Workflow-Abschnitt (1) inline bearbeiten.

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## Rollen im Proof-Viewer überprüfen

Sie können die Rolle eines Validierers direkt im Proof Viewer (1) überprüfen und bei Bedarf bearbeiten (2).

![Proof_roles_-_Proof_Viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Standardmäßige Proof-Rollen

Sie können Ihre standardmäßige Testversand-Rolle auf der Seite [!DNL Proofing Defaults] in Ihren persönlichen Einstellungen festlegen. Das bedeutet, dass beim Hinzufügen zu einem Testversand Ihre standardmäßige Testversand-Rolle automatisch ausgefüllt wird. Bitte beachten Sie, dass diese Rolle auf Testversandebene von einem Benutzer mit Bearbeitungsrechten für einen Testversand geändert werden kann.

>[!NOTE]
>
>Nur Benutzer mit Administrator- oder Rechnungsadministrator-Profilen können die Standardeinstellungen für die Prüfung für andere Benutzer in ihrem Konto ändern.

Weitere Informationen finden Sie unter [Persönliche Einstellungen in  [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Ersteller und Inhaber

Ersteller und Inhaber verfügen über vollständige Bearbeitungsrechte für den Testversand.

### Ersteller {#creators}

Der Ersteller des Testversands ist die Person, die den Testversand in der ersten Instanz hochlädt. Der Testversand-Ersteller wird automatisch in der Personenliste für den Testversand angezeigt (in seiner Standardrolle).

Auf der Seite [!UICONTROL Neuer Testversand] können Sie dem Ersteller des Testversands (außer seiner Standardrolle) eine andere Rolle zuweisen.

Der Testversand-Ersteller kann nicht geändert oder aus einem Testversand entfernt werden.

### Inhaber {#owners}

Standardmäßig ist der Ersteller auch Eigentümer des Testversands. Der Ersteller kann jedoch bei der anfänglichen Erstellung des Testversands (auf der Seite [!UICONTROL Neuer Testversand] ) eine andere Person zum Testversand-Inhaber machen.

So ändern Sie den Inhaber auf der Seite Neuer Testversand :

1. Klicken Sie auf den Link zum Ändern neben dem Namen des Erstellers.
1. Wählen Sie den neuen Inhaber aus dem Dropdown-Menü aus. Absatz 2

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

Nach der Erstellung des Testversands ist es weiterhin möglich, den Besitzer zu wechseln. Jeder, der über Bearbeitungsrechte für den Testversand verfügt, kann über die Seite [!UICONTROL Testversand-Details] den Testversand-Besitz in einen anderen Benutzer ändern (siehe unten).

Die Möglichkeit, den Inhaber eines Testversands zu ändern, ist insbesondere aus Sicht der Workflow-Verwaltung nützlich. Dadurch kann die für das Projekt verantwortliche Person das Eigentum an Testsendungen übernehmen und ihnen Bearbeitungsrechte für die Testsendungen und die Möglichkeit geben, sie in der Ansicht [!UICONTROL Meine Testsendungen] anzuzeigen.

So ändern Sie den Inhaber des Testversands über die Seite [!UICONTROL Testversand-Details] :

* Klicken Sie auf das Menü Aktionen neben dem Namen der Person, die Sie zum Inhaber machen möchten.
* Wählen Sie [!UICONTROL **Inhaber machen**] aus dem Dropdownmenü aus.
* Alternativ können Sie auf das Feld [!UICONTROL **Inhaber**] neben dem Testversand-Bild klicken und den neuen Inhaber aus der Dropdown-Liste auswählen.

Danach wird neben dem Namen der Person das Wort &quot;Inhaber&quot;angezeigt.

>[!NOTE]
>
>Nur ein Benutzer desselben Kontos oder eines Partnerkontos kann zum Besitzer eines Testversands gemacht werden. Ein Benutzer in einem Partnerkonto kann nur dann zum Eigentümer eines Testversands gemacht werden, wenn:
>
>* Zwischen den Konten besteht eine bestehende Partnerbeziehung. Weitere Informationen finden Sie unter [Partnerkonten in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* Auf der Seite [!UICONTROL Neuer Testversand] gibt es keine benutzerdefinierten Felder.
>* Der Testversand wurde keinem Ordner zugewiesen.
>* Auf den Testversand wurden keine Tags angewendet.

Informationen zum temporären Delegieren des Testversandeigentums innerhalb von [!DNL Workfront Proof] finden Sie unter [Ausweisen von temporären Testversand-Inhabern in  [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
