---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Konfigurieren des Proofing-Zugriffs von Benutzern
description: Als Adobe Workfront- oder Workfront Proof-Administrator können Sie den Zugriff eines Benutzers konfigurieren, um in Workfront und Workfront Proof Testsendungen zu erstellen und anzuzeigen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '1242'
ht-degree: 0%

---

# Konfigurieren des Proofing-Zugriffs von Benutzern

Als Adobe Workfront- oder Workfront Proof-Administrator können Sie den Zugriff eines Benutzers konfigurieren, um in Workfront und Workfront Proof Testsendungen zu erstellen und anzuzeigen.

Informationen zu den für grundlegendes und integriertes Proofing verfügbaren Proofing-Funktionen finden Sie [Zugriff auf die Proofing-Funktionen in Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Sie müssen ein Workfront- oder Workfront Proof-Administrator sein. Informationen zu Workfront-Administratoren finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Aktivieren und Deaktivieren des Proofings für einen Benutzer (nur für veraltete Pläne) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Wenn Ihr Unternehmen einen älteren Select- oder Premium-Workfront-Plan verwendet, können Sie als Workfront-Administrator die Proofing-Funktion für den Benutzer aktivieren und deaktivieren.

Wenn Sie das Proofing für einen Benutzer aktivieren, aktiviert Workfront die Option zum automatischen Generieren der Korrekturabzüge durch den Benutzer.

Sie können einen Benutzer zwar als Proofing-Benutzer aktivieren, er muss jedoch über Administratorberechtigungen verfügen, um direkt über das Workfront-Hauptmenü zur Workfront Proof-Benutzeroberfläche zu navigieren. Informationen dazu, wie Sie diese Option für alle Proofing-Benutzer in Ihrem Workfront-System aktivieren können, finden Sie [Konfigurieren des Workfront Proof-Zugriffs über das Workfront-Hauptmenü für alle Benutzer](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. Wählen Sie im **Hauptmenü** die Option **Benutzer** aus.

1. Wählen Sie einen Benutzer aus und klicken Sie dann auf das Symbol **Bearbeiten**.
1. Wählen Sie im Abschnitt **Zugriff** die Option (Benutzer kann **Korrekturabzüge generieren** aus oder heben Sie die Auswahl auf.

## Konfigurieren des Berechtigungsprofils für Korrekturabzüge von Benutzenden

Das ausgewählte Berechtigungsprofil wird den Benutzern für jeden Korrekturabzug gewährt, der in Ihrer Organisation vorhanden ist.

{{step-1-to-users}}

1. Wählen Sie einen oder mehrere Benutzer aus und klicken Sie dann auf **Bearbeiten**.

1. Klicken Sie **Abschnitt** auf eine der folgenden Workfront Proof-Berechtigungsoptionen im Dropdown **Menü Testversandberechtigungsprofil**:

   >[!NOTE]
   >
   >Wenn Sie einen alten Workfront-Plan verwenden, stellen Sie sicher, dass die Option **Benutzer kann Korrekturabzüge generieren** aktiviert ist, wie oben im Abschnitt [Aktivieren und Deaktivieren des Korrekturabzugs für einen Benutzer (nur für alte Pläne)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Verantwortlicher</strong> </td> 
      <td>Benutzer können alle im Konto Ihrer Organisation erstellten Korrekturabzüge verwalten und anzeigen. Sie können auch Prüfer bearbeiten, die zu diesen Korrekturabzügen hinzugefügt wurden. Benutzende mit diesem Berechtigungsprofil können keine Benutzenden verwalten oder Workfront Proof-Einstellungen bearbeiten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Manager</strong> </td> 
      <td> <p> Benutzer können Korrekturabzüge verwalten und anzeigen, die im Konto Ihres Unternehmens erstellt wurden oder sich in dessen Besitz befinden. Sie können die Korrekturabzüge anderer Benutzer nur anzeigen, wenn sie als Prüferin bzw. Prüfer hinzugefügt werden. Dies ist eine Standardeinstellung. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrator</strong> </td> 
      <td> Benutzende erhalten in Workfront Proof Administratorberechtigungen und können Kontoeinstellungen bearbeiten. Benutzer können alle im Konto Ihrer Organisation erstellten Korrekturabzüge verwalten und anzeigen. Dazu gehört das Hinzufügen und Entfernen von Reviewern, Testsendungen und Kommentaren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefiniert</strong> </td> 
      <td> <p>Nur verfügbar, wenn Sie ein benutzerdefiniertes Berechtigungsprofil in Workfront Proof konfiguriert haben.</p> <p><b>HINWEIS</b>:  <p>Stellen Sie sicher, dass das hier gewährte Berechtigungsprofil keinen höheren Zugriff bietet als die Zugriffsebenen-Einstellung des Benutzers in Workfront (siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>). Wenn es einen höheren Zugriff bietet, kann der/die Benutzende in Workfront Proof auf Korrekturabzüge zugreifen, auf die er/sie nicht in Workfront zugreifen kann.</p> <p>Dies ist besonders wichtig, wenn Sie planen, allen Workfront-Benutzenden den direkten Zugriff auf Workfront Proof über Workfront zu ermöglichen, wie unter <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Zugriff auf Workfront Proof über Adobe Workfront</a> beschrieben.</p> <p>Standardmäßig haben nur Workfront-Administratoren Zugriff auf einen direkten Link zur Workfront Proof-Site über die globale Navigationsleiste von Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Das ausgewählte Berechtigungsprofil wird den Benutzern für jeden Korrekturabzug gewährt, der in Ihrer Organisation vorhanden ist.

1. Klicken Sie **Änderungen speichern**, um die Aktualisierung der Benutzereinstellungen abzuschließen.

   >[!NOTE]
   >
   >Wenn Sie einen Benutzer in Workfront erstellen oder aktualisieren und die Workfront-E-Mail-Adresse des Benutzers mit der eines lizenzierten Workfront Proof-Benutzers übereinstimmt, aktiviert das System das Proofing für den Benutzer in Workfront. Weitere Informationen finden Sie unter [Benutzersynchronisierung zwischen Adobe Workfront und Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Aspekte

Beachten Sie beim Festlegen von Berechtigungen die folgenden Informationen:

* Wenn Sie das Berechtigungsprofil eines/r Benutzenden in ein Profil mit weniger Berechtigungen ändern, kann es sein, dass der/die Benutzende die Sichtbarkeit vorhandener Korrekturabzüge in Workfront verliert. Dies kann vorkommen, wenn eine Person eine Aufgabe für eine Benutzerin oder einen Benutzer in Workfront freigibt, den an die Aufgabe angehängten Korrekturabzug jedoch nicht freigibt (siehe [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Freigeben eines Korrekturabzugs in Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Sie können Workfront Proof-Berechtigungen nur dann von Workfront aus festlegen, wenn Ihre Workfront-Umgebung mit einem Workfront Proof Premium-Konto integriert ist. Wenn Sie Proofing nicht wie in diesem Abschnitt erläutert verwenden können, wenden Sie sich an Ihren Workfront-Administrator.
* Mindestens ein Benutzer in Ihrer Workfront-Umgebung muss über Administratorberechtigungen für das Proofing verfügen. Eine Fehlermeldung wird angezeigt, wenn Sie versuchen, allen Benutzern die Administratorberechtigungen für das Proofing zu entfernen.
* Wenn Sie die Workfront-Zugriffsebene einer Benutzerin oder eines Benutzers in eine andere Ebene als „Systemadministrator“ ändern, wird für das Workfront Proof-Berechtigungsprofil der Benutzerin oder des Benutzers standardmäßig „Manager“ festgelegt.

* Wenn Sie die Workfront-Zugriffsebene in „Systemadministrator“ ändern, ändert sich das Profil für Korrekturabzugsberechtigungen in „Administrator“.

## Konfigurieren des Workfront Proof-Zugriffs für alle Benutzer über das Workfront-Hauptmenü {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Standardmäßig können nur Benutzende mit Administratorrechten in Workfront wie unter (Zugriff auf Workfront Proof [ Adobe Workfront) beschrieben auf Workfront Proof ](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Sie können allen Benutzenden Zugriff auf die Schaltfläche Workfront Proof im Hauptmenü von Workfront gewähren, indem Sie sich an den Workfront-Support wenden und eine Anfrage senden.

>[!IMPORTANT]
>
> Wenn Sie allen Workfront-Benutzenden erlauben möchten, direkt über die globale Navigationsleiste von Workfront auf Workfront Proof zuzugreifen, stellen Sie sicher, dass das Berechtigungsprofil der einzelnen Benutzenden nicht mehr Zugriff bietet als die Zugriffsebene der Benutzenden in Workfront. Dadurch wird verhindert, dass Benutzende in Workfront Proof auf Korrekturabzüge zugreifen, auf die sie nicht in Workfront zugreifen können. Weitere Informationen finden Sie unter [Aktivieren und Deaktivieren des Proofings für einen Benutzer (nur für ältere Pläne)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Konfigurieren des Benutzerzugriffs auf den Desktop Proofing Viewer

Wenn Benutzende in Ihrer Organisation lieber den Desktop Proofing Viewer anstelle des Web Proofing Viewers zur Überprüfung interaktiver Inhalte verwenden möchten, können Sie den Desktop Proofing Viewer so konfigurieren, dass er automatisch gestartet wird, wenn Benutzende interaktive Korrekturabzüge für Inhalte öffnen. Weitere Informationen dazu, wie sich der Desktop Proofing Viewer vom Web Proofing Viewer unterscheidet, finden Sie unter [Grundlegendes zum Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) und [Unterschiede zwischen dem Web Proofing Viewer und dem Desktop Proofing Viewer](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. Klicken Sie in Workfront in der globalen Navigationsleiste auf das Workfront Proof-Symbol, um auf Workfront Proof zuzugreifen.

   ![Korrekturabzug-Symbol](assets/proof-access-proofhq-350x39.png)

1. Klicken **oben rechts** Workfront Proof auf „Kontoeinstellungen“ und dann auf die Registerkarte **Einstellungen**.

1. Klicken **unter** Testversand-Standardeinstellungen“ am Ende der Zeile **Desktop Proofing Viewer für interaktives**&quot; auf **Setup**.

1. Ändern Sie die Einstellungen für die Desktop-Proofing-Viewer, wie [Desktop-Proofing](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer)Viewer) im Artikel [Konfigurieren der Korrekturabzugseinstellungen für Ihr Unternehmen](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) beschrieben.

1. Klicken Sie auf **Speichern**.

## Konfigurieren von benutzerdefinierten Geräten für interaktive Korrekturabzüge

Sie können Ihrem System beliebige benutzerdefinierte Geräte hinzufügen, damit Benutzer interaktive Inhalte überprüfen und simulieren können, wie die Inhalte auf einem bestimmten Gerät angezeigt werden, wenn sie den Desktop Proofing Viewer verwenden. (Diese Funktion ist im Web Proofing Viewer nicht verfügbar, in dem Benutzende interaktive Inhalte überprüfen können, sondern nur so, wie sie in verschiedenen Auflösungen und nicht auf verschiedenen Geräten angezeigt werden.)

Weitere Informationen finden Sie unter [Ändern der interaktiven Korrekturabzugsauflösung im Proofing Viewer](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Greifen Sie über Workfront auf die Workfront Proof-Benutzeroberfläche zu, wie in [Zugriff auf Workfront Proof über Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) beschrieben.
1. Ändern Sie die Einstellungen der Desktop-Korrekturabzugsanzeige, wie unter [Konfigurieren benutzerdefinierter Geräte für Korrekturabzüge](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) im Artikel [Konfigurieren der Korrekturabzugseinstellungen für Ihre Organisation](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md) beschrieben.
