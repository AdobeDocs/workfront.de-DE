---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Grundlegendes zu Ordnerberechtigungen in [!DNL Workfront Proof]
description: Wenn eine Person berechtigt ist, ein Element in einem Ordner anzuzeigen, kann sie auch den Ordner selbst sehen. Sie können jedoch nur die Elemente im Ordner sehen, die explizit für sie freigegeben wurden.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 17%

---

# Grundlegendes zu Ordnerberechtigungen in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen in [!DNL Adobe Workfront], siehe [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn eine Person berechtigt ist, ein Element in einem Ordner anzuzeigen, kann sie auch den Ordner selbst sehen. Sie können jedoch nur die Elemente im Ordner sehen, die explizit für sie freigegeben wurden.

## Öffentliche Ordner

Wenn ein Ordner öffentlich ist, können Benutzer im Konto (außer Beobachter und leichte Benutzer) den Ordnernamen in der linken Seitenleiste sehen.

Ihr Berechtigungsprofil wirkt sich auch auf die Rechte aus, die Sie über öffentliche Ordner haben:

| **Profil/Aktion** | **Alle Elemente im Ordner anzeigen** | **Elemente anzeigen, die explizit für sie freigegeben wurden** | **Elemente hinzufügen** | **Elemente löschen** | **Unterordner hinzufügen** | **Löschen von Unterordnern** | **Ordnerdetails bearbeiten** |
|---|---|---|---|---|---|---|---|
| **Ersteller** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Rechnungsadministrator** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Administrator** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Supervisor** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Manager** | Nein | Ja | Ja | Nein | Ja | Nein | Ja |
| **Beobachter** | Nein | Ja | Nein | Nein | Nein | Nein | Nein |

{style=&quot;table-layout:auto&quot;}

Wenn der öffentliche Ordner Eigentum eines Managers ist, kann er den Stammordner und alle Unterordner löschen.

Weitere Informationen finden Sie unter [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Private Ordner

Wenn ein Ordner privat ist, können andere Benutzer desselben Kontos den Namen des Ordners nicht in der linken Seitenleiste sehen, es sei denn, die Ordner oder Elemente im Ordner wurden explizit für sie freigegeben oder sie haben das Profil &quot;Supervisor&quot;, &quot;Administrator&quot;oder &quot;Rechnungsadministrator&quot;:

| **Profil/Aktion** | **Alle Elemente im Ordner anzeigen** | **Elemente anzeigen, die explizit für sie freigegeben wurden** | **Elemente hinzufügen** | **Elemente löschen** | **Unterordner hinzufügen** | **Löschen von Unterordnern** | **Ordnerdetails bearbeiten** |
|---|---|---|---|---|---|---|---|
| **Ersteller** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Rechnungsadministrator** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Administrator** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Supervisor** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Manager** | Nein | Ja | Nein | Nein | Nein | Nein | Nein |
| **Beobachter** | Nein | Ja | Nein | Nein | Nein | Nein | Nein |

{style=&quot;table-layout:auto&quot;}

Wenn beispielsweise Ihr Projektmanager und seine Teams nur bestimmte Ordner sehen sollen, kann der Projektmanager einen privaten Ordner einrichten und diesen dann für bestimmte Benutzer freigeben.

Beim Freigeben eines privaten Ordners können Sie entscheiden, ob Manager Ordnerelemente erstellen, bearbeiten und löschen können sollen.

Sie können dies für jede Person einzeln auf der Seite &quot;Neuer Ordner&quot;festlegen und sie im [!UICONTROL Freigegeben für] auf der Seite Ordnerdetails. Weitere Informationen finden Sie unter [Erstellen von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) und [Verwalten Sie Ordner und deren Inhalte in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Wenn ein privater Ordner für einen - oder -Beobachter freigegeben ist, hat er schreibgeschützten Zugriff auf alle Elemente im Ordner. Weitere Informationen finden Sie unter [Profile für Testberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) und [Ordner freigeben in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Wenn ein übergeordneter Ordner privat ist, sind alle Unterordner ebenfalls privat. Sie können keinen öffentlichen Unterordner unter einem privaten übergeordneten Ordner haben. Sie können jedoch einen privaten Unterordner unter einem öffentlichen übergeordneten Ordner haben.
>* Der Ersteller und Eigentümer des Ordners hat immer Zugriff darauf und kann nicht entfernt werden.
>* Nur der Ersteller und Eigentümer des privaten Ordners kann den Ordner löschen.


