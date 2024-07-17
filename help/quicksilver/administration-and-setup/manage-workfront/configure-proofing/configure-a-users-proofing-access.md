---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Konfigurieren des Testversand-Zugriffs eines Benutzers
description: Als Adobe Workfront-Administrator oder Workfront Proof-Administrator können Sie den Zugriff eines Benutzers konfigurieren, um Testsendungen in Workfront und Workfront Proof zu erstellen und anzuzeigen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# Konfigurieren des Testversand-Zugriffs eines Benutzers

Als Adobe Workfront-Administrator oder Workfront Proof-Administrator können Sie den Zugriff eines Benutzers konfigurieren, um Testsendungen in Workfront und Workfront Proof zu erstellen und anzuzeigen.

Informationen zu den für grundlegende und integrierte Testsendungen verfügbaren Testversandfunktionen finden Sie unter [Zugriff auf die Testversandfunktion in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Workfront-Administrator oder Workfront Proof-Administrator sein. Weitere Informationen zu Workfront-Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Testversand für einen Benutzer aktivieren und deaktivieren (nur ältere Pläne) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Wenn Ihr Unternehmen als Workfront-Administrator einen bestehenden Select- oder Premium-Workfront-Plan verwendet, können Sie die Testversandfunktion für den Benutzer aktivieren und deaktivieren.

Wenn Sie den Testversand für einen Benutzer aktivieren, aktiviert Workfront die Option, dass die Testsendungen des Benutzers automatisch generiert werden.

Sie können einen Benutzer zwar als Testbenutzer aktivieren, müssen jedoch über Administratorberechtigungen verfügen, um direkt über das Workfront-Hauptmenü zur Workfront Proof-Benutzeroberfläche navigieren zu können. Informationen dazu, wie Sie diese Option für alle Testbenutzer in Ihrem Workfront-System aktivieren können, finden Sie unter [Konfigurieren des Workfront Proof-Zugriffs über das Workfront-Hauptmenü für alle Benutzer](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. Wählen Sie im **Hauptmenü** die Option **Benutzer** aus.

1. Wählen Sie einen Benutzer aus und klicken Sie dann auf das Symbol **Bearbeiten** .
1. Aktivieren oder deaktivieren Sie im Abschnitt **Zugriff** die Option **Benutzer kann Testsendungen generieren**.

## Profil für Testberechtigungen eines Benutzers konfigurieren

Das ausgewählte Berechtigungsprofil wird den Benutzern für jeden in Ihrer Organisation vorhandenen Testversand gewährt.

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Benutzer** ![](assets/users-icon-in-main-menu.png).![](assets/main-menu-icon.png)
1. Wählen Sie einen oder mehrere Benutzer aus und klicken Sie dann auf **Bearbeiten**.

1. Klicken Sie im Abschnitt **Zugriff** auf eine der folgenden Workfront Proof-Berechtigungsoptionen im Dropdown-Menü **Testversand-Berechtigungsprofil**:

   >[!NOTE]
   >
   >Wenn Sie einen alten Workfront-Plan verwenden, stellen Sie sicher, dass die Option **Benutzer kann Testsendungen generieren** aktiviert ist, wie oben im Abschnitt [Testversand für einen Benutzer aktivieren und deaktivieren (nur ältere Pläne)](#enable-and-disable-proofing-for-a-user-legacy-plans-only) beschrieben.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Benutzer können alle Testsendungen verwalten und anzeigen, die auf dem Konto Ihres Unternehmens erstellt wurden. Sie können auch Prüfer bearbeiten, die zu diesen Testsendungen hinzugefügt wurden. Benutzer mit diesem Berechtigungsprofil können keine Benutzer verwalten oder Workfront Proof-Einstellungen bearbeiten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Benutzer können Testsendungen verwalten und anzeigen, die in ihrem Unternehmen erstellt wurden oder sich im Besitz des Kontos befinden. Sie können Testsendungen anderer Benutzer nur anzeigen, wenn sie als Prüfer hinzugefügt wurden. Dies ist eine Standardeinstellung. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Benutzer erhalten in Workfront Proof Administratorberechtigungen und können Kontoeinstellungen bearbeiten. Benutzer können alle Testsendungen verwalten und anzeigen, die auf dem Konto Ihres Unternehmens erstellt wurden. Dazu gehören das Hinzufügen und Entfernen von Überprüfern, Testsendungen und Kommentaren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefiniert</strong> </td> 
      <td> <p>Nur verfügbar, wenn Sie ein benutzerdefiniertes Berechtigungsprofil in Workfront Proof konfiguriert haben.</p> <p><b>NOTE</b>:  <p>Stellen Sie sicher, dass das Berechtigungsprofil, das Sie hier gewähren, keinen höheren Zugriff bietet als die Zugriffsebene des Benutzers in Workfront (siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>). Wenn der Benutzer keinen höheren Zugriff erhält, kann er auf Testsendungen in Workfront Proof zugreifen, auf die er in Workfront nicht zugreifen kann.</p> <p>Dies ist besonders wichtig, wenn Sie allen Workfront-Benutzern den direkten Zugriff auf Workfront Proof über Workfront ermöglichen möchten, wie unter <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Zugriff auf Workfront Proof über Adobe Workfront</a> beschrieben.</p> <p>Standardmäßig haben nur Workfront-Administratoren über die globale Navigationsleiste von Workfront Zugriff auf einen direkten Link zur Workfront Proof-Site.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Das ausgewählte Berechtigungsprofil wird den Benutzern für jeden in Ihrer Organisation vorhandenen Testversand gewährt.

1. Klicken Sie auf **Änderungen speichern** , um die Aktualisierung der Benutzereinstellungen abzuschließen.

   >[!NOTE]
   >
   >Wenn Sie einen Benutzer in Workfront erstellen oder aktualisieren und die Workfront-E-Mail-Adresse des Benutzers mit der eines lizenzierten Workfront Proof-Benutzers übereinstimmt, aktiviert das System die Testprüfung für den Benutzer in Workfront. Weitere Informationen finden Sie unter [Benutzersynchronisierung zwischen Adobe Workfront und Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Überlegungen

Beachten Sie beim Festlegen von Berechtigungen die folgenden Informationen:

* Wenn Sie das Berechtigungsprofil eines Benutzers in ein Profil mit weniger Berechtigungen ändern, verliert der Benutzer möglicherweise die Sichtbarkeit zu vorhandenen Testsendungen in Workfront. Dies kann vorkommen, wenn ein Benutzer eine Aufgabe mit einem Benutzer in Workfront teilt, aber nicht den mit der Aufgabe verknüpften Testversand nutzt (siehe [Freigeben eines Testversands in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Freigeben eines Testversands in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Sie können Workfront Proof-Berechtigungen nur dann von Workfront aus festlegen, wenn Ihre Workfront-Umgebung in ein Workfront Proof Premium-Konto integriert ist. Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie die in diesem Abschnitt beschriebene Verwendung von Testsendungen nicht verwenden können.
* Mindestens ein Benutzer in Ihrer Workfront-Umgebung muss über Administratorberechtigungen für die Prüfung verfügen. Wenn Sie versuchen, die Administratorberechtigungen für den Testversand von allen Benutzern zu entfernen, wird eine Fehlermeldung angezeigt.
* Wenn Sie die Workfront-Zugriffsstufe eines Benutzers auf eine andere Ebene als &quot;Systemadministrator&quot;ändern, wird als Workfront Proof-Berechtigungsprofil des Benutzers standardmäßig &quot;Manager&quot;verwendet.

* Wenn Sie die Workfront-Zugriffsebene in &quot;Systemadministrator&quot;ändern, wird das Profil für die Berechtigung zum Testversand in &quot;Administrator&quot;geändert.

## Konfigurieren des Workfront Proof-Zugriffs über das Workfront-Hauptmenü für alle Benutzer {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Standardmäßig können nur Benutzer mit Administratorrechten innerhalb von Workfront wie in [Zugriff auf Workfront Proof über Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) beschrieben auf Workfront Proof zugreifen.

Sie können allen Benutzern im Workfront-Hauptmenü Zugriff auf die Workfront Proof-Schaltfläche gewähren, indem Sie den Workfront-Support kontaktieren und eine Anfrage senden.

>[!IMPORTANT]
>
> Wenn Sie allen Workfront-Benutzern direkten Zugriff über die Workfront Global Navigation Bar gewähren möchten, stellen Sie sicher, dass das Berechtigungsprofil für jeden Benutzer nicht mehr Zugriff bietet als die Zugriffsstufe des Benutzers in Workfront. Dadurch wird verhindert, dass Benutzer auf Testsendungen in Workfront Proof zugreifen, auf die sie in Workfront nicht zugreifen können. Weitere Informationen finden Sie unter [Aktivieren und Deaktivieren des Testversands für einen Benutzer (nur ältere Pläne)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Konfigurieren des Benutzerzugriffs auf den Desktop Proofing Viewer

Wenn Benutzer in Ihrem Unternehmen interaktive Inhalte lieber mit dem Desktop Proofing Viewer als mit dem Web Proofing Viewer überprüfen möchten, können Sie den Desktop Proofing Viewer so konfigurieren, dass er automatisch gestartet wird, wenn Benutzer interaktive Inhaltsanalysen öffnen. Weitere Informationen dazu, wie der Desktop Proofing Viewer und der Web Proofing Viewer unterscheiden, finden Sie unter [Grundlegendes zum Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) und [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer - Übersicht](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Klicken Sie in Workfront auf das Workfront Proof-Symbol in der Leiste &quot;Globale Navigation&quot;, um auf Workfront Proof zuzugreifen.

   ![](assets/proof-access-proofhq-350x39.png)

1. Klicken Sie oben rechts in Workfront Proof auf **Kontoeinstellungen** und dann auf die Registerkarte **Einstellungen**.

1. Klicken Sie unter &quot;**Proof Defaults**&quot;am Ende der Zeile &quot;**Desktop Proofing Viewer für interaktive Prüfung**&quot;auf &quot;**Einrichten**&quot;.

1. Ändern Sie die Einstellungen für den Desktop Proofing-Viewer, wie in [Desktop Proofing Viewer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) im Artikel [Konfigurieren der Testversandeinstellungen für Ihr Unternehmen](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) beschrieben.

1. Klicken Sie auf **Speichern**.

## Benutzerdefinierte Geräte für interaktive Testsendungen konfigurieren

Sie können Ihrem System beliebige benutzerdefinierte Geräte hinzufügen, sodass Benutzer interaktive Inhalte überprüfen und simulieren können, wie die Inhalte auf einem bestimmten Gerät angezeigt werden, wenn sie den Desktop Proofing Viewer verwenden. (Diese Funktion ist nicht im Web Proofing-Viewer verfügbar, in dem Benutzer interaktive Inhalte überprüfen können, sondern nur so, wie sie in verschiedenen Auflösungen und nicht auf verschiedenen Geräten angezeigt wird.)

Weitere Informationen finden Sie unter [Ändern der interaktiven Testversandauflösung im Testversand-Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Greifen Sie über Workfront auf die Workfront Proof-Benutzeroberfläche zu, wie unter [Zugriff auf Workfront Proof über Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) beschrieben.
1. Ändern Sie die Einstellungen für den Desktop Proofing-Viewer, wie in [Konfigurieren benutzerdefinierter Geräte für Testsendungen](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) im Artikel [Konfigurieren der Testversandeinstellungen für Ihr Unternehmen](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) beschrieben.
