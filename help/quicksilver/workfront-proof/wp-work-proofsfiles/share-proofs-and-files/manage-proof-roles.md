---
product-previous: workfront-proof
product-area: documents
navigation-topic: share-proofs-and-files
title: Verwalten von Korrekturabzug-Rollen in [!DNL Workfront Proof]
description: Mit Korrekturabzug-Rollen können Sie Benutzern Berechtigungen erteilen, die durch das in ihrem Benutzerprofil konfigurierte Berechtigungsprofil eingeschränkt sind.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b371cc20-4226-49ce-96c6-9815b2e84713
source-git-commit: 6e24b9c717ecedd6efbdf62ec01e53ac98079cfe
workflow-type: tm+mt
source-wordcount: '1306'
ht-degree: 1%

---

# Verwalten von Korrekturabzugsrollen in [!DNL Workfront Proof]

<!-- Audited: 01/2024 -->

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Mit Korrekturabzug-Rollen können Sie Benutzern Berechtigungen erteilen, die durch das in ihrem Benutzerprofil konfigurierte Berechtigungsprofil eingeschränkt sind. (Weitere Informationen zu Berechtigungsprofilen finden Sie unter [Berechtigungsprofile für Korrekturabzüge in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).)

Korrekturabzug-Rollen unterscheiden sich von Account-Profilen. Ihr Kontoprofil bezieht sich auf die allgemeine Berechtigungsstufe, die Sie in Ihrem Konto haben, und wirkt sich auf die Rechte aus, die Sie an allen Korrekturabzügen in Ihrem Konto haben, auch wenn diese nicht explizit für Sie freigegeben wurden.

Weitere Informationen finden Sie unter [Profile für Korrekturabzugsberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Über Korrekturabzug-Rollen

Die folgenden Korrekturabzug-Rollen werden Benutzenden für einen einzelnen Korrekturabzug gewährt, wenn der/die Benutzende zur Überprüfung des Korrekturabzugs eingeladen wird:

* [Schreibgeschützt](#read-only)
* [Prüfende Person](#reviewer)
* [Genehmigende Person](#approver)
* [Prüfer und genehmigende Person](#reviewer-approver)
* [Verfassende Person](#author)
* [Moderierende Person](#moderator)

Die Rolle des Korrekturabzugs definiert, welche Aktionen ein Prüfer in Bezug auf diesen spezifischen Korrekturabzug durchführen kann.

Wenn Sie z. B. ein Reviewer sind, werden Sie aufgefordert, den Korrekturabzug zu überprüfen, indem Sie Markierungen und Kommentare hinzufügen. Wenn Sie ein Prüfer und eine genehmigende Person sind, werden Sie aufgefordert, den Korrekturabzug zu überprüfen und auch eine Entscheidung darüber zu treffen.

Bestimmte Korrekturabzug-Rollen verleihen einem Prüfer Bearbeitungsrechte für den Korrekturabzug (auch wenn sein Kontoprofil dies nicht tut) und ermöglichen es ihm, einige zusätzliche Funktionen zu verwenden, z. B. das Hinzufügen von Aktionen zu Kommentaren, das Erstellen neuer Versionen und das Hinzufügen weiterer Prüfer zum Korrekturabzug.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Aktionen für Korrekturabzugskommentare verwenden](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md)
* [Freigeben eines Korrekturabzugs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md)

### Schreibgeschützt

{#read-only}

![cleaner.png](assets/cleaner.png) Kann einen Korrekturabzug anzeigen

![no.png](assets/no.png) Es können keine Markierungen hinzugefügt werden

![no.png](assets/no.png) Kommentare können nicht hinzugefügt werden

![no.png](assets/no.png) Es kann keine Entscheidung getroffen werden

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht gelöscht werden

![no.png](assets/no.png) Verfügt nicht über Bearbeitungsrechte für den Korrekturabzug

>[!NOTE]
>
>Wenn ein Ordner für einen Benutzer von [!DNL Workfront Proof] freigegeben wird, erhält er automatisch Leseberechtigungen für alle vorhandenen und nachfolgend hinzugefügten Elemente im Ordner.

Weitere Informationen finden Sie unter [Freigeben von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

### Prüfende Person {#reviewer}

![cleaner.png](assets/cleaner.png) Kann einen Korrekturabzug anzeigen

![cleaner.png](assets/cleaner.png) Kann Markierungen hinzufügen

![cleaner.png](assets/cleaner.png) Kommentare hinzufügen

![[!DNL cleaner].png](assets/cleaner.png) Kann eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind

![no.png](assets/no.png) Es kann keine Entscheidung getroffen werden

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet oder gelöscht werden

![no.png](assets/no.png) Verfügt nicht über Bearbeitungsrechte für den Korrekturabzug

### Genehmigende Person {#approver}

![cleaner.png](assets/cleaner.png) Kann einen Korrekturabzug anzeigen

![cleaner.png](assets/cleaner.png) Kann eine Entscheidung treffen

![no.png](assets/no.png) Es können keine Markierungen hinzugefügt werden

![no.png](assets/no.png) Kommentare können nicht hinzugefügt werden

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet oder gelöscht werden

![no.png](assets/no.png) Verfügt nicht über Bearbeitungsrechte für den Korrekturabzug

### Prüfer und genehmigende Person {#reviewer-approver}

![cleaner.png](assets/cleaner.png) Kann einen Korrekturabzug anzeigen

![cleaner.png](assets/cleaner.png) Kann Markierungen hinzufügen

![cleaner.png](assets/cleaner.png) Kommentare hinzufügen

![[!DNL cleaner].png](assets/cleaner.png) Kann eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind

![cleaner.png](assets/cleaner.png) Kann eine Entscheidung treffen

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet oder gelöscht werden

![no.png](assets/no.png) Verfügt nicht über Bearbeitungsrechte für den Korrekturabzug

### Verfassende Person {#author}

![cleaner.png](assets/cleaner.png) Kann Markierungen hinzufügen

![cleaner.png](assets/cleaner.png) Kommentare hinzufügen

![[!DNL cleaner].png](assets/cleaner.png) Kann eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind

![cleaner.png](assets/cleaner.png) Kann eine Entscheidung treffen

![cleaner.png](assets/cleaner.png) Kann neue Versionen senden

![cleaner.png](assets/cleaner.png) Kann eine Kopie des Korrekturabzugs erstellen

![cleaner.png](assets/cleaner.png) Kann den Korrekturabzug für andere Personen freigeben

![cleaner.png](assets/cleaner.png) Kann Aktionen auf Kommentare anwenden

![cleaner.png](assets/cleaner.png) Kann Kommentare auflösen

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet oder gelöscht werden

>[!NOTE]
>
>Diese Rolle kann nur Benutzenden von [!DNL Workfront Proof] zugewiesen werden.

### Moderierende Person {#moderator}

![cleaner.png](assets/cleaner.png) Kann Markierungen hinzufügen

![cleaner.png](assets/cleaner.png) Kommentare hinzufügen

![[!DNL cleaner].png](assets/cleaner.png) Kann eigene Kommentare bearbeiten, wenn keine Antworten vorhanden sind

![cleaner.png](assets/cleaner.png) Kann eine Entscheidung treffen

![cleaner.png](assets/cleaner.png) Kann neue Versionen senden

![cleaner.png](assets/cleaner.png) Kann neue Reviewer hinzufügen

![cleaner.png](assets/cleaner.png) Kann Aktionen auf Kommentare anwenden

![cleaner.png](assets/cleaner.png) Kann Kommentare auflösen

![cleaner.png](assets/cleaner.png) Kann Kommentare und Antworten auf den Korrekturabzug löschen (von sich selbst oder anderen)

* Wenn Sie den ersten Kommentar in einem Kommentar-Thread löschen, wird der gesamte Thread gelöscht
* Durch das Löschen von Antworten im Kommentar-Thread wird nur diese Antwort gelöscht

![no.png](assets/no.png) Kommentare anderer Benutzer können nicht bearbeitet werden

In dieser Rolle kann die Person die Korrekturabzugskommentare verwalten und moderieren, sodass sie nur relevante Kommentare zum Korrekturabzug beibehalten und nicht relevante Kommentare entfernen kann.

>[!NOTE]
>
>Diese Rolle kann nur Benutzenden von [!DNL Workfront Proof] zugewiesen werden.

## Zuweisen von Korrekturabzug-Rollen

Sie können Korrekturabzug-Rollen zuweisen, wenn Sie neue Korrekturabzüge erstellen, neue Versionen vorhandener Korrekturabzüge erstellen oder vorhandene Korrekturabzüge bearbeiten.

### Neue Korrekturabzüge {#new-proofs}

Korrekturabzug-Rollen können Prüfern auf der Seite &quot;[!UICONTROL  Korrekturabzug] während des Erstellungsprozesses des Korrekturabzugs zugewiesen werden (1).

![Proof_roles_-_New_Proof_page.png](assets/proof-roles---new-proof-page-350x184.png)

### Neue Versionen {#new-versions}

Beim Erstellen einer neuen Version eines Korrekturabzugs werden die Reviewer aus der vorherigen Version automatisch angezeigt (mit derselben Rolle wie die vorherige Version).

Sie können die Rollen des Korrekturabzugs bearbeiten, die bei der Erstellung der neuen Version auf die Prüfer angewendet werden (1).

![Proof_roles_-_New_Version_page.png](assets/proof-roles---new-version-page-350x164.png)

### Vorhandene Korrekturabzüge {#existing-proofs}

Wenn Sie die Rolle einer Person bei einem vorhandenen Korrekturabzug ändern möchten, können Sie dies auf der Seite [!UICONTROL Korrekturabzugsdetails] tun, indem Sie ihre Rolle im Workflow-Abschnitt (1) inline bearbeiten.

![Proof_Roles_-_Proof_Details_page_2.png](assets/proof-roles---proof-details-page-2-350x131.png)

## Überprüfen von Rollen in der Korrekturabzugsansicht

Sie können die Rolle eines Prüfers direkt in der Korrekturabzugsansicht (1) überprüfen und bei Bedarf bearbeiten (2).

![Proof_roles_-_proof_viewer.png](assets/proof-roles---proof-viewer-350x300.png)

## Standard-Korrekturabzug-Rollen

Sie können die Standardrolle für den Korrekturabzug auf der Seite [!DNL Proofing Defaults] in Ihren persönlichen Einstellungen festlegen. Das bedeutet, dass beim Hinzufügen zu einem Korrekturabzug Ihre standardmäßige Korrekturabzugsrolle automatisch ausgefüllt wird. Beachten Sie, dass diese Rolle auf der Korrekturabzugsebene von einem Benutzer mit Bearbeitungsrechten für einen Korrekturabzug geändert werden kann.

>[!NOTE]
>
>Nur Benutzer mit Administrator- oder Billing-Administratorprofilen können die Proofing-Standardeinstellungen für andere Benutzer in ihrem Konto ändern.

Weitere Informationen finden Sie unter &quot;[ Einstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/personal-settings.md).

## Ersteller und Inhaber

Ersteller und Besitzer haben vollständige Bearbeitungsrechte für den Korrekturabzug.

### Ersteller {#creators}

Der Korrekturabzug-Ersteller ist die Person, die den Korrekturabzug in der ersten Instanz hochlädt. Der Ersteller des Korrekturabzugs wird automatisch in der Liste der Personen für den Korrekturabzug angezeigt (in seiner Standardrolle).

Auf der Seite [!UICONTROL Neuer Korrekturabzug] können Sie dem Ersteller des Korrekturabzugs eine andere Korrekturabzugsrolle zuweisen (außer seiner Standardrolle).

Die Erstellerin bzw. der Ersteller des Korrekturabzugs kann nicht geändert oder aus einem Korrekturabzug entfernt werden.

### Inhaber {#owners}

Standardmäßig ist der Ersteller auch der Inhaber des Korrekturabzugs. Der Ersteller kann jedoch eine andere Person zum Besitzer des Korrekturabzugs machen, wenn er den Korrekturabzug anfänglich erstellt (auf der Seite &quot;[!UICONTROL  Korrekturabzug]).

So ändern Sie den Inhaber auf der Seite Neuer Korrekturabzug :

1. Klicken Sie auf den Link Ändern neben dem Namen des Erstellers.
1. Wählen Sie den neuen Inhaber aus dem Dropdown-Menü aus. 2)

![Proof_roles_-_new_proof_page_change_owner_2.png](assets/proof-roles---new-proof-page-change-owner-2-350x185.png)

Sobald der Korrekturabzug erstellt wurde, kann der Besitzer noch geändert werden. Jeder Benutzer mit Bearbeitungsrechten für den Korrekturabzug kann über die Seite „Korrekturabzugsdetails“ ([!UICONTROL  unten) die Eigentümerschaft ] Korrekturabzugs an einen anderen Benutzer ändern.

Die Möglichkeit, den/die Verantwortliche(n) für einen Korrekturabzug zu ändern, ist aus Sicht der Workflow-Verwaltung besonders nützlich. Dadurch kann die für das Projekt verantwortliche Person die Verantwortung für den Testversand übernehmen, indem ihr Bearbeitungsrechte für die Testsendungen erteilt werden und sie in der Ansicht &quot;[!UICONTROL  Testsendungen“ ] kann.

So ändern Sie den/die Verantwortliche für den Korrekturabzug über die Seite [!UICONTROL Details des Korrekturabzugs]:

* Klicken Sie auf das Menü Aktionen neben dem Namen der Person, die Sie zum Besitzer machen möchten.
* Wählen [!UICONTROL **aus dem Dropdown**] Menü „Besitzer erstellen“ aus.
* Alternativ können Sie in das Feld [!UICONTROL **Verantwortlicher**] neben dem Bild des Korrekturabzugs klicken und den neuen Verantwortlichen aus der angezeigten Dropdown-Liste auswählen.

Sobald dies geschehen ist, wird das Wort „Besitzer“ neben dem Namen dieser Person angezeigt.

>[!NOTE]
>
>Nur ein Benutzer aus demselben Konto oder einem Partnerkonto kann zum Besitzer eines Korrekturabzugs gemacht werden. Ein Benutzer in einem Partnerkonto kann nur dann zum Besitzer eines Korrekturabzugs gemacht werden, wenn:
>
>* Es wurde eine bestehende Partnerbeziehung zwischen den Konten eingerichtet. Weitere Informationen finden Sie unter [Partnerkonten in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/partner-accounts/partner-accounts.md).
>* Es gibt keine benutzerdefinierten Felder auf der Seite [!UICONTROL Neuer Korrekturabzug].
>* Der Korrekturabzug wurde keinem Ordner zugewiesen.
>* Es wurden keine Tags auf den Korrekturabzug angewendet.

Informationen zum vorübergehenden Delegieren der Eigentümerschaft an Korrekturabzügen in [!DNL Workfront Proof] finden Sie unter [Bestimmen von Eigentümern temporärer Korrekturabzüge in [!DNL Workfront Proof]](../../../workfront-proof/wp-getstarted/personal-settings/designate-temp-proof-owners.md).
