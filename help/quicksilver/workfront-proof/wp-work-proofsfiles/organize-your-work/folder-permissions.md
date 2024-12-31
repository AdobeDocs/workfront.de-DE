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
source-wordcount: '557'
ht-degree: 15%

---

# Grundlegendes zu Ordnerberechtigungen in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf Funktionen im eigenständigen [!DNL Workfront Proof]. Informationen zu Proofing in [!DNL Adobe Workfront] finden Sie unter [Proofing](../../../review-and-approve-work/proofing/proofing.md).

Wenn eine Person berechtigt ist, ein Element in einem Ordner anzuzeigen, kann sie auch den Ordner selbst sehen. Sie können jedoch nur die Elemente im Ordner sehen, die explizit für sie freigegeben wurden.

## Öffentliche Ordner

Wenn ein Ordner öffentlich ist, können Benutzer im -Konto (mit Ausnahme von Beobachtern und Light-Benutzern) den Ordnernamen in der linken Seitenleiste sehen.

Ihr Berechtigungsprofil wirkt sich auch auf die Rechte aus, die Sie an öffentlichen Ordnern haben:

| **Profil/Aktion** | **Alle Elemente im Ordner anzeigen** | **Siehe explizit für sie freigegebene Elemente** | **Elemente hinzufügen** | **Elemente löschen** | **Hinzufügen von Unterordnern** | **Löschen von Unterordnern** | **Ordnerdetails bearbeiten** |
|---|---|---|---|---|---|---|---|
| **Ersteller** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Abrechnungs-Administrator** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Administrator** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Verantwortlicher** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Manager** | Nein | Ja | Ja | Nein | Ja | Nein | Ja |
| **Beobachter** | Nein | Ja | Nein | Nein | Nein | Nein | Nein |

{style="table-layout:auto"}

Wenn der öffentliche Ordner einem Manager gehört, kann dieser den Stammordner und alle Unterordner löschen.

Weitere Informationen finden Sie unter [Profile für Korrekturabzugsberechtigungen in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Private Ordner

Wenn ein Ordner privat ist, können andere Benutzer im selben Konto den Namen des Ordners in der linken Seitenleiste nur sehen, wenn der Ordner oder die Elemente im Ordner explizit für sie freigegeben wurden oder sie das Profil eines Supervisors, Administrators oder Abrechnungsadministrators haben:

| **Profil/Aktion** | **Alle Elemente im Ordner anzeigen** | **Siehe explizit für sie freigegebene Elemente** | **Elemente hinzufügen** | **Elemente löschen** | **Hinzufügen von Unterordnern** | **Löschen von Unterordnern** | **Ordnerdetails bearbeiten** |
|---|---|---|---|---|---|---|---|
| **Ersteller** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Abrechnungs-Administrator** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Administrator** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Verantwortlicher** | Ja | Ja | Ja | Ja | Ja | Ja | Ja |
| **Manager** | Nein | Ja | Nein | Nein | Nein | Nein | Nein |
| **Beobachter** | Nein | Ja | Nein | Nein | Nein | Nein | Nein |

{style="table-layout:auto"}

Wenn Sie beispielsweise möchten, dass Ihr Projekt-Manager und seine Teams nur bestimmte Ordner sehen, kann der Projekt-Manager einen privaten Ordner einrichten und diesen dann für bestimmte Benutzer freigeben.

Bei der Freigabe eines privaten Ordners können Sie festlegen, ob Manager Ordnerelemente erstellen, bearbeiten und löschen können sollen.

Sie können dies für jede Person einzeln auf der Seite Neuer Ordner festlegen und im Abschnitt [!UICONTROL Freigegeben für] der Seite Ordnerdetails ändern. Weitere Informationen finden Sie unter [Erstellen von Ordnern in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) und [Verwalten von Ordnern und deren Inhalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Wenn ein privater Ordner für einen - oder -Beobachter freigegeben ist, hat er Lesezugriff auf alle Elemente im Ordner. Weitere Informationen finden Sie unter [Korrekturabzugsberechtigungsprofile in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) und [Ordner freigeben in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Wenn ein übergeordneter Ordner privat ist, sind alle Unterordner ebenfalls privat. Sie können keinen öffentlichen Unterordner unter einem privaten übergeordneten Ordner haben. Sie können jedoch einen privaten Unterordner unter einem öffentlichen übergeordneten Ordner haben.
>* Der Ersteller und Besitzer des Ordners hat immer Zugriff darauf und kann nicht entfernt werden.
>* Nur der Ersteller und Besitzer des privaten Ordners kann den Ordner löschen.

