---
content-type: reference
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: Profile für Testberechtigungen im Workfront-Testversand
description: Als Workfront-Administrator oder Workfront Testversandadministrator können Sie einem Benutzer ein Profil für Testberechtigungen zuweisen, um die Testversandfunktionen anzugeben, die der Benutzer für alle Testsendungen im System verwenden kann. Informationen zum Konfigurieren des Profils eines Benutzers finden Sie unter Konfigurieren des Profils für Benutzerberechtigungen im Workfront-Testversand .
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 249aa332-c051-49ac-be85-264d8babfcad
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '1769'
ht-degree: 1%

---

# Profile für Testberechtigungen in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Als [!DNL Workfront] Administrator oder [!DNL Workfront Proof] Administrator können Sie einem Benutzer ein Profil für Testberechtigungen zuweisen, um die Testversandfunktionen anzugeben, die der Benutzer für alle Testsendungen im System nutzen kann. Informationen zum Konfigurieren des Profils für Testberechtigungen eines Benutzers finden Sie unter [Profil für Testberechtigungen eines Benutzers konfigurieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/config-user-pref-in-wp.md).

>[!NOTE]
>
>Sie können auch Folgendes tun:
>
>* Gewähren Sie Benutzern für einzelne Testsendungen spezifische Rollen. Weitere Informationen zu Testversandrollen finden Sie unter [Verwalten von Proof-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).
>* Erstellen Sie benutzerdefinierte Profile für Benutzer in Ihrer Organisation. Weitere Informationen finden Sie unter [Benutzerdefinierte Profile konfigurieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-custom-profiles.md).
>


In der folgenden Tabelle werden die für jedes Profil mit Testberechtigungen verfügbaren Berechtigungen angezeigt.

| **Eigene Elemente** |  |  |  |  | **Sonstige Benutzerelemente** |  |  | **Admin** | **Rechnungsstellung** |
|---|---|---|---|---|---|---|---|---|---|
|  | **Hinzufügen** | **Anzeigen** | **Bearbeiten** | **Löschen** | **Anzeigen** | **Bearbeiten** | **Löschen** | **Bearbeiten und Löschen** | **Bearbeiten** |
| Rechnungsadministrator | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |
| Admin | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |
| Supervisor | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |
| Manager | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) | ![](assets/cleaner2.png) |   |   |   |   |   |
| Beobachter |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |
| Besucher |   | ![](assets/cleaner2.png) |   |   |   |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

Beachten Sie Folgendes zu Rollen und Berechtigungen:

* Zugewiesene Profilberechtigungen beziehen sich nur auf die Benutzer und Elemente in Ihrem eigenen Konto. Die Ausnahme bilden Satellitenkonten, bei denen der Administrator und der Rechnungsadministrator für die Haupt-(Hub-)Konten auf die Kontoeinstellungen und die Abrechnung dieser Konten von der Hub-Kontoebene aus zugreifen und diese verwalten können.
* Rechnungsadministratoren und -administratoren können Benutzer löschen. Dies kann nur in den Kontoeinstellungen erfolgen.
* Wenn Billing-Administratoren und -Administratoren Testsendungen anzeigen, die anderen Benutzern in ihrem Konto gehören, sehen sie diese mit der Rolle eines Validierers an.
* Mit der Rolle &quot;Schreibgeschützt&quot;können Billing-Administratoren und -Administratoren auf Testsendungen in Ordnern zugreifen, die für sie freigegeben sind, oder in Ordnern, die von ihnen erstellt wurden.

In den folgenden Abschnitten werden die einzelnen Profile und die mit dem Profil verknüpften Berechtigungen in einem standardmäßigen [!DNL Workfront Proof] setup:

* [Rechnungsadministrator](#billing-administrator)
* [Administrator](#administrator)
* [Supervisor](#supervisor)
* [Manager](#manager)
* [Beobachter](#observer)
* [Besucher](#visitor)
* [Gastgeber](#guest)

## Rechnungsadministrator {#billing-administrator}

Rechnungsadministratoren haben Zugriff auf [Kontoeinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md) and [The [!DNL Workfront Proof] Rechnungsseite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md)und über die folgenden Berechtigungen verfügen:

![](assets/cleaner2.png)Kann Testsendungen generieren, Dateien hochladen und Ordner erstellen. Weitere Informationen finden Sie unter [Testsendungen generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Hochladen von Dateien und Webinhalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)und [Erstellen von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kann eigene Testsendungen und von ihnen erstellte Dateien anzeigen, bearbeiten und löschen.

![](assets/cleaner2.png)Kann von allen Benutzern in der Organisation erstellte Testsendungen und Dateien anzeigen, bearbeiten und löschen.

![](assets/cleaner2.png)Kann die öffentlichen Ordner anderer Benutzer löschen. Weitere Informationen finden Sie unter [Verwalten von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Hat Bearbeitungsrechte für alle im Konto erstellten Testsendungen.

![](assets/cleaner2.png)Kann als Inhaber der Dropzone festgelegt werden. Weitere Informationen finden Sie unter [Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kann auf die Rechnungsseite zugreifen und die Rechnungsdetails bearbeiten. Weitere Informationen finden Sie unter [Die [!DNL Workfront Proof] Rechnungsseite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

![](assets/cleaner2.png)Kann auf die Seite Kontoeinstellungen zugreifen und die Kontodetails bearbeiten. Weitere Informationen finden Sie unter [Kontoeinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Kann den Müll leeren. Weitere Informationen finden Sie unter [Wiederherstellen und Löschen des Papierkorbs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Kann Benutzer hinzufügen, bearbeiten und löschen.

![](assets/cleaner2.png)Kann Gruppen erstellen und neue Kontakte hinzufügen.

![](assets/cleaner2.png)Kann Kontakte löschen.

![](assets/cleaner2.png)Kann Testsendungen bearbeiten, wenn keine Antworten darauf vorhanden sind.

![](assets/no2.png)Testversandantworten können nicht bearbeitet werden.

![](assets/no2.png)Die privaten Ordner anderer Benutzer können nicht gelöscht werden. Weitere Informationen finden Sie unter [Verwalten von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

Informationen zu Kontoeinstellungen finden Sie unter [Kontoeinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

Informationen zur Rechnungsstellung finden Sie unter [Die [!DNL Workfront Proof] Rechnungsseite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Administrator {#administrator}

Administratoren haben Zugriff auf [Kontoeinstellungen](https://support.workfront.com/hc/en-us/sections/115000912147-Account-Settings)und über die folgenden Berechtigungen verfügen:

![](assets/cleaner2.png)Kann Testsendungen erstellen, Dateien hochladen und Ordner erstellen. Weitere Informationen finden Sie unter [Testsendungen generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Hochladen von Dateien und Webinhalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)und [Erstellen von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Können von ihnen erstellte Testsendungen und Dateien anzeigen, bearbeiten und löschen.

![](assets/cleaner2.png)Kann von allen Benutzern in der Organisation erstellte Testsendungen und Dateien anzeigen, bearbeiten und löschen.

![](assets/cleaner2.png)Kann die öffentlichen Ordner anderer Benutzer löschen. Weitere Informationen finden Sie unter [Verwalten von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Hat Bearbeitungsrechte für alle im Konto erstellten Testsendungen.

![](assets/cleaner2.png)Kann als Inhaber der Dropzone festgelegt werden. Weitere Informationen finden Sie unter [Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kann auf die Seite Kontoeinstellungen zugreifen und die Kontodetails bearbeiten. Weitere Informationen finden Sie unter [Kontoeinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/cleaner2.png)Kann den Müll leeren. Weitere Informationen finden Sie unter [Wiederherstellen und Löschen des Papierkorbs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/cleaner2.png)Kann Benutzer hinzufügen, bearbeiten und löschen.

![](assets/cleaner2.png)Kann Gruppen erstellen und neue Kontakte hinzufügen.

![](assets/cleaner2.png)Kann Kontakte löschen.

![](assets/cleaner2.png)Kann Testsendungen bearbeiten, wenn keine Antworten darauf vorhanden sind.

![](assets/no2.png)Testversandantworten können nicht bearbeitet werden.

![](assets/no2.png)Die privaten Ordner anderer Benutzer können nicht gelöscht werden. Weitere Informationen finden Sie unter [Verwalten von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Zugriff auf die Seite &quot;Rechnungsstellung&quot;oder Bearbeitung der Rechnungsdetails nicht möglich. Weitere Informationen finden Sie unter [Die [!DNL Workfront Proof] Rechnungsseite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md).

### Supervisor {#supervisor}

Supervisoren haben die folgenden Berechtigungen:

![](assets/cleaner2.png)Kann Testsendungen erstellen, Dateien hochladen und Ordner erstellen. Weitere Informationen finden Sie unter [Testsendungen generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Hochladen von Dateien und Webinhalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)und [Erstellen von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kann eigene Testsendungen und von ihnen erstellte Dateien anzeigen, bearbeiten und löschen.

![](assets/cleaner2.png)Kann von allen Benutzern in der Organisation erstellte Testsendungen und Dateien anzeigen, bearbeiten und löschen.

![](assets/cleaner2.png)Kann die öffentlichen Ordner anderer Benutzer löschen. Weitere Informationen finden Sie unter [Verwalten von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/cleaner2.png)Hat Bearbeitungsrechte für alle im Konto erstellten Testsendungen.

![](assets/cleaner2.png)Kann als Inhaber der Dropzone festgelegt werden. Weitere Informationen finden Sie unter [Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/cleaner2.png)Kann Gruppen erstellen und neue Kontakte hinzufügen.

![](assets/cleaner2.png)Kann Kontakte löschen.

![](assets/cleaner2.png)Kann Testsendungen bearbeiten, wenn keine Antworten darauf vorhanden sind.

![](assets/no2.png)Testversandantworten können nicht bearbeitet werden.

![](assets/no2.png)Die privaten Ordner anderer Benutzer können nicht gelöscht werden. Weitere Informationen finden Sie unter [Ordner in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/folders.md).

![](assets/no2.png)Zugriff auf die Seite &quot;Rechnungsstellung&quot;oder die Kontoeinstellungen nicht möglich. Weitere Informationen finden Sie unter [Die [!DNL Workfront Proof] Rechnungsseite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) und [Kontoeinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Benutzer können nicht hinzugefügt, bearbeitet oder gelöscht werden.

![](assets/no2.png)Der Müll kann nicht geleert werden. Weitere Informationen finden Sie unter [Wiederherstellen und Löschen des Papierkorbs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

### Manager {#manager}

Manager haben die folgenden Berechtigungen:

![](assets/cleaner2.png)Kann Testsendungen erstellen, Dateien hochladen und Ordner erstellen. Weitere Informationen finden Sie unter [Testsendungen generieren in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md), [Hochladen von Dateien und Webinhalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md)und [Erstellen von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md).

![](assets/cleaner2.png)Kann eigene Testsendungen und Dateien, die sie erstellen oder besitzen, anzeigen, bearbeiten und löschen.

![](assets/cleaner2.png)Können Testsendungen anderer Benutzer anzeigen, überprüfen und genehmigen, die explizit für sie freigegeben wurden (schreibgeschützte Berechtigungen für alle in einem freigegebenen Ordner). Weitere Informationen finden Sie unter [Verwalten von Proof-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kann Gruppen erstellen und einen neuen Kontakt hinzufügen.

![](assets/no2.png)Testsendungen und Dateien, die von anderen Benutzern in der Organisation erstellt wurden, können nicht angezeigt, bearbeitet oder gelöscht werden.

![](assets/no2.png)Testsendungen oder Antworten können nicht bearbeitet werden.

![](assets/no2.png)Die privaten Ordner anderer Benutzer können nicht gelöscht werden. Weitere Informationen finden Sie unter [Verwalten von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Öffentliche Ordner anderer Benutzer können nicht gelöscht werden. Weitere Informationen finden Sie unter [Verwalten von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Zugriff auf die Seite &quot;Rechnungsstellung&quot;oder die Kontoeinstellungen nicht möglich. Weitere Informationen finden Sie unter [Die [!DNL Workfront Proof] Rechnungsseite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) und [Kontoeinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Kann nicht als Eigentümer der Dropzone festgelegt werden. Weitere Informationen finden Sie unter [Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Der Müll kann nicht geleert werden. Weitere Informationen finden Sie unter [Wiederherstellen und Löschen des Papierkorbs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Benutzer können nicht hinzugefügt, bearbeitet oder gelöscht werden.

![](assets/no2.png)Kontakte können nicht gelöscht werden.

### Beobachter {#observer}

Beobachter haben die folgenden Berechtigungen:

![](assets/cleaner2.png)Kann Testsendungen anderer Benutzer anzeigen, überprüfen und genehmigen, die explizit für sie freigegeben wurden (schreibgeschützte Berechtigungen für alle in einem freigegebenen Ordner). Weitere Informationen finden Sie unter [Verwalten von Proof-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kann Dateien anzeigen, die explizit für sie freigegeben sind.

![](assets/cleaner2.png) Kann Kontakte und Gruppen anzeigen

![](assets/no2.png)Es können keine Testsendungen erstellt, Dateien hochgeladen und Ordner erstellt werden. Weitere Informationen finden Sie unter [Hochladen von Dateien und Webinhalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Testsendungen und Dateien, die von anderen Benutzern in der Organisation erstellt wurden, können nicht angezeigt, bearbeitet oder gelöscht werden.

![](assets/no2.png)Testsendungen oder Antworten können nicht bearbeitet werden.

![](assets/no2.png)Es können keine in der Organisation erstellten Elemente gelöscht werden.

![](assets/no2.png)Zugriff auf die Seite &quot;Rechnungsstellung&quot;oder die Kontoeinstellungen nicht möglich. Weitere Informationen finden Sie unter [Die [!DNL Workfront Proof] Rechnungsseite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) und [Kontoeinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Kann nicht als Eigentümer der Dropzone festgelegt werden. Weitere Informationen finden Sie unter [Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Der Müll kann nicht geleert werden. Weitere Informationen finden Sie unter [Wiederherstellen und Löschen des Papierkorbs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Benutzer können nicht hinzugefügt, bearbeitet oder gelöscht werden.

![](assets/no2.png)Es können keine Gruppen erstellt oder neue Kontakte hinzugefügt werden.

![](assets/no2.png)Kontakte können nicht gelöscht werden.

>[!NOTE]
>
>Die für Beobachter verfügbaren Menüs und Funktionen sind begrenzt.
>
>* Beobachter sehen weder das Menü Kopfzeile noch das grüne Menü Neu im Dashboard
>* Beobachter sehen die folgenden Links nicht in ihren Einstellungen: Kontoeinstellungen, Rechnungsstellung
>


### Besucher {#visitor}

Besucher haben die folgenden Berechtigungen:

![](assets/cleaner2.png)Können Testsendungen anderer Benutzer anzeigen, überprüfen und genehmigen, die explizit für sie freigegeben wurden (schreibgeschützte Berechtigungen für alle in einem freigegebenen Ordner). Weitere Informationen finden Sie unter [Verwalten von Proof-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

![](assets/cleaner2.png)Kann Dateien anzeigen, die explizit für sie freigegeben sind.

![](assets/no2.png) Kontakte und Gruppen können nicht angezeigt werden

![](assets/no2.png)Es können keine Testsendungen erstellt, Dateien hochgeladen und Ordner erstellt werden. Weitere Informationen finden Sie unter [Hochladen von Dateien und Webinhalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

![](assets/no2.png)Testsendungen und Dateien, die von anderen Benutzern in der Organisation erstellt wurden, können nicht angezeigt, bearbeitet oder gelöscht werden.

![](assets/no2.png)Testsendungen oder Antworten können nicht bearbeitet werden.

![](assets/no2.png)Es können keine in der Organisation erstellten Elemente gelöscht werden.

![](assets/no2.png)Zugriff auf die Seite &quot;Rechnungsstellung&quot;oder die Kontoeinstellungen nicht möglich. Weitere Informationen finden Sie unter [Die [!DNL Workfront Proof] Rechnungsseite](../../../workfront-proof/wp-billingsettings/manage-your-billing/wp-billing-page.md) und [Kontoeinstellungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/account-settings.md).

![](assets/no2.png)Kann nicht als Eigentümer der Dropzone festgelegt werden. Weitere Informationen finden Sie unter [Konfigurieren Sie die Dropzone in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/configure-dropzone-in-wp.md).

![](assets/no2.png)Der Müll kann nicht geleert werden. Weitere Informationen finden Sie unter [Wiederherstellen und Löschen des Papierkorbs in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/restore-and-empty-trash.md).

![](assets/no2.png)Benutzer können nicht hinzugefügt, bearbeitet oder gelöscht werden.

![](assets/no2.png)Es können keine Gruppen erstellt oder neue Kontakte hinzugefügt werden.

![](assets/no2.png)Kontakte können nicht gelöscht werden.

>[!NOTE]
>
>Die für Besucher verfügbaren Menüs und Funktionen sind begrenzt.
>
>* Besucher sehen weder das Menü &quot;Kopfzeile&quot;noch das grüne Menü &quot;Neu&quot;im Dashboard
>* Besucher sehen die folgenden Links nicht in ihren Einstellungen: Kontoeinstellungen, Rechnungsstellung
>


### Gastgeber {#guest}

Das Gastprofil wird verwendet, um Prüfern, die kein eigenes Workfront-Testkonto haben, Zugriff auf Testsendungen zu gewähren. Sie können auf Testsendungen zugreifen, die ihnen direkt über ihre persönlichen E-Mail-Benachrichtigungen zugestellt werden.

![](assets/cleaner2.png)Können explizit für sie freigegebene Testsendungen anzeigen, überprüfen und genehmigen.

![](assets/cleaner2.png)Kann Dateien anzeigen, die explizit für sie freigegeben sind.

![](assets/no2.png)Zugriff auf das Dashboard ist nicht möglich.

![](assets/no2.png)Ordner können nicht für sie freigegeben werden. Weitere Informationen finden Sie unter [Verwalten von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders.md).

![](assets/no2.png)Kann nicht als Autoren oder Moderatoren zu den Testsendungen hinzugefügt werden. Weitere Informationen finden Sie unter [Verwalten von Proof-Rollen in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

>[!NOTE]
>
>Die Gäste sind keine Workfront-Testbenutzer, sodass sie nicht alle Testsendungen sehen können, die für sie in ihrem eigenen Dashboard freigegeben wurden.

## Profil für Testberechtigungen eines Benutzers bearbeiten

Administratoren und Rechnungsadministratoren können die Berechtigungsprofile aller Benutzer im Konto bearbeiten.

1. Führen Sie einen der folgenden Schritte aus, um den zu bearbeitenden Benutzer zu finden:

   * Navigieren Sie zu **[!UICONTROL Kontoeinstellungen]** und klicken Sie dann auf **[!UICONTROL Benutzer]** Registerkarte.

   * Navigieren Sie zu **[!UICONTROL Kontakte]** Seite.

1. Klicken Sie auf den Namen des Benutzers, dessen Berechtigungen Sie bearbeiten möchten. ![](assets/screenshot-2018-03-30-14-16-05a-350x69.png)

1. Klicken Sie auf **[!UICONTROL Berechtigungsprofil]** aus und wählen Sie ein neues Berechtigungsprofil aus. :

   ![Screenshot_2018-03-30_14-18-03.png](assets/screenshot-2018-03-30-14-18-03a.png)

   Berechtigungsprofile sind Administrator, Supervisor, Manager und Beobachter.

1. Klicken Sie auf eine beliebige Stelle außerhalb des Menüs, um zu speichern.

>[!NOTE]
>
>Administratoren können das Profil &quot;Rechnungsadministrator&quot;nicht zuweisen. Eine Liste der Profiländerungen finden Sie in den folgenden Protokollen:
>
>* Die Protokolle der Kontoaktivitäten
>* Das Profilprotokoll des Benutzers (nur für diesen Benutzer zugänglich)
>


Weitere Informationen zu Aktivitätsprotokollen finden Sie unter [Grundlagen zum [!DNL Workfront Proof] Aktivitäts-Audit-Protokoll](../../../workfront-proof/wp-work-proofsfiles/basic-features/activity-audit-trail.md).
