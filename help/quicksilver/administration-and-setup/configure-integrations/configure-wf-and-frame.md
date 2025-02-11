---
title: 'Konfigurieren der Integration  [!DNL Workfront] und [!DNL Frame.io] '
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: Als  [!DNL Adobe Workfront]  können Sie  [!DNL Workfront]  mit integrieren  [!DNL Frame.io]  Ihrer Organisation eine nahtlose Möglichkeit bieten, Assets zu überprüfen und zu genehmigen.
author: Courtney
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
hide: true
hidefromtoc: true
exl-id: 7d909976-d3ff-4e60-9158-c3bffe498e6e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Konfigurieren der Integration von [!DNL Workfront] und [!DNL Frame.io]

Der Workfront-Administrator ermöglicht die Integration zwischen Workfront und Frame.io, indem er das standardmäßige Frame.io-Konto im Bereich „Setup“ konfiguriert und dann in Workfront Frame.io-Benutzer bestimmt. Auf diese Weise kann der Projektkoordinator mithilfe von Workfront-Projekten und Prüfungs- und Genehmigungs-Workflows Arbeiten planen und initiieren.


## Zugriffsanforderungen

>[!IMPORTANT]
>
>Diese Funktion steht nur Organisationen zur Verfügung, die in das [!DNL Adobe Admin Console] integriert wurden.

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table>
  <tr>
   <td>[!DNL Adobe Workfront] Plan</td>
   <td>Beliebig</td>
  </tr>
  <tr>
   <td>[!DNL Adobe Workfront] Lizenzen
   </td>
   <td><p>Aktuell: [!UICONTROL Plan]</p>
   <p>Neu: [!UICONTROL Standard]</p></td>
  </tr>
  <tr>
   <td>Konfigurationen der Zugriffsebene
   </td>
   <td>Sie müssen [!DNL Workfront] sein.
   </td>
  </tr>

</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren eines [!DNL Frame.io] Standardkontos [!BADGE in Kürze verfügbar]{type=Informative}

Nachdem ein standardmäßiges [!DNL Frame.io] eingerichtet wurde, wird für alle in [!DNL Workfront] erstellten Projekte ein Spiegelprojekt in Frame.io erstellt.

>[!IMPORTANT]
>
>Diese Funktion wird in Kürze verfügbar sein. Im Moment werden Frame.io-Konten manuell vom Workfront-Team hinzugefügt. Wenden Sie sich an Ihren Adobe-Kundenbetreuer.

## Konfigurieren eines einzelnen Frame.io-Kontos mit einer Workfront-Gruppe

Sie können eine einzelne Workfront-Gruppe mit einem einzelnen Frame.io-Konto verbinden, das sich vom Standardkonto unterscheidet.

So konfigurieren Sie ein einzelnes Frame.io-Konto mit einer Workfront-Gruppe:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen**.
1. Wählen Sie eine vorhandene Gruppe aus oder klicken Sie auf **Gruppe erstellen**.
1. Klicken Sie im linken Bedienfeld auf **Mit Frame.io verbinden**.
1. Geben Sie das API-Entwickler-Token ein.
1. Klicken Sie **Verbindung starten**.
1. (Bedingt) Wenn Sie Administrator von mehr als einem Frame.io-Konto sind, wählen Sie das Konto aus, das Sie verwenden möchten.

## Frame.io-Benutzer aktivieren

Workfront-Benutzer, die regelmäßig Frame.io verwenden, sollten als Frame.io-Benutzer gekennzeichnet werden. Workfront-Administratoren können im Workfront-Benutzerprofil Frame.io-Benutzer festlegen.

>[!TIP]
>
>Es wird empfohlen, Benutzer, die regelmäßig mit Kreativ-Tools arbeiten und Assets zur Überprüfung und Genehmigung hochladen, als Frame.io-Benutzer zu aktivieren.

Wenn ein(e) Benutzende(r) in Workfront als Frame.io-Benutzende(r) gekennzeichnet und einem Projekt hinzugefügt wird:

* Sie werden als Collaborator in Frame.io hinzugefügt. <!--do we need to be more explicit about a frame license being provisioned for them?-->
* Sie können Assets von Frame.io zur formellen Überprüfung und Genehmigung an Workfront senden.
* Sie können Informationen im unidirektionalen Synchronisierungsordner von Workfront anzeigen. [!BADGE Bald verfügbar]{type=Informative}

So aktivieren Sie Frame.io-Benutzer:

{{step-1-to-users}}

1. Wählen Sie einen oder mehrere Benutzer aus und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).
1. Aktivieren Sie im Abschnitt Zugriff das Kontrollkästchen Zu Projekten in Frame.io hinzufügen und wählen Sie **Dropdown-Menü**Ja“ aus.
   ![Zum Frame-Projekt hinzufügen](assets/add-to-frame-project.png)

   >[!NOTE]
   >
   >Wenn dieses Kontrollkästchen deaktiviert ist, behält der Benutzer den Zugriff auf frühere Zuweisungen bei und wird zu Frame.io-Projekten hinzugefügt, die in Zukunft durchgeführt werden.<!-- If the user is deactivated, they lose all access to previous assignments and are removed from the Frame.io account.-->
