---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: SAML 2.0-Metadaten in Ihrem Identitätsanbieter aktualisieren
description: Sie können SAML 2.0-Metadaten in Ihrem Identitätsanbieter aktualisieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# SAML 2.0-Metadaten in Ihrem Identitätsanbieter aktualisieren

{{important-admin-console-onboard}}

In den folgenden Abschnitten wird beschrieben, wie Sie Ihre SAML 2.0-Metadaten (Security Assertion Markup Language) aktualisieren, wenn Sie Active Directory Federation Services (ADFS) als Identitätsanbieter verwenden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Verwenden von ADFS als Identitätsanbieter

Sie können Ihre ADFS-Metadaten vor oder nach dem Aktualisieren des SAML 2.0-Zertifikats durch Adobe Workfront aktualisieren. Wenn Sie die ADFS-Metadaten aktualisieren möchten, bevor Workfront das SAML 2.0-Zertifikat aktualisiert, sind zusätzliche Schritte erforderlich.

* [Aktualisieren der ADFS-Metadaten](#update-your-adfs-metadata)
* [Aktualisierung der ADFS-Metadaten erzwingen](#force-your-adfs-metadata-to-update)

### Aktualisieren von ADFS-Metadaten {#update-your-adfs-metadata}

Um Ihre ADFS-Metadaten so einzurichten, dass sie automatisch aktualisiert werden, führen Sie die Schritte in diesem Abschnitt aus.

Standardmäßig ist ADFS so konfiguriert, dass automatisch nach Aktualisierungen aller Vertrauensmetadaten der vertrauenden Seite gesucht wird. Die Standardeinstellung ist jedoch so festgelegt, dass nur alle 24 Stunden eine Abfrage durchgeführt wird. Sie können diesen Wert mit PowerShell-Befehlen ändern.

1. Melden Sie sich beim ADFS-Server an und öffnen Sie die ADFS-Verwaltungskonsole.
1. Erweitern Sie im linken Bedienfeld **ADFS 2.0** erweitern Sie dann **Vertrauensstellungen.**

1. Klicken Sie auf **Ordner Vertrauenswürdige** .
1. Wählen Sie die Vertrauensstellung der vertrauenden Seite aus, die Sie zuvor für die Verwendung mit Workfront konfiguriert haben, und klicken Sie dann im rechten Bedienfeld auf **Aus Verbundmetadaten aktualisieren**.
1. (Bedingt) Wenn diese Option abgeblendet ist (was bedeutet, dass die Vertrauensstellung der vertrauenden Seite zuvor mithilfe einer Metadatendatei konfiguriert wurde), führen Sie die folgenden Schritte aus.

   1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) oben rechts in Adobe Workfront und dann auf **Setup** ![](assets/gear-icon-settings.png).

   1. Klicken Sie **System** > **Single Sign On (SSO)**.

   1. Klicken Sie **Einstellungen bearbeiten.**
   1. Klicken Sie **Konfiguration bearbeiten** und wählen Sie dann **SAML 2.0** in der **Typ** Dropdown-Liste aus.

   1. Kopieren Sie **Metadaten-URL**, die etwa wie folgt aussehen sollte:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Klicken Sie auf dem ADFS-Server mit der rechten Maustaste auf die Vertrauensstellung der vertrauenden Seite, die Sie zuvor konfiguriert haben, und klicken Sie dann auf **Eigenschaften.**
   1. Klicken Sie auf **Monitoring** und fügen Sie dann die URL, die Sie aus Workfront kopiert haben, in das Feld **Verbundmetadaten-URL des** ein.

   1. Markieren Sie die Optionen **vertrauende Seite überwachen** und **vertrauende Seite automatisch aktualisieren**.

   1. Klicken Sie auf **OK.**
   1. Wählen Sie die Vertrauensstellung der vertrauenden Seite aus, die Sie zuvor für die Verwendung mit Workfront konfiguriert haben, und klicken Sie dann im rechten Bedienfeld auf **Aus Verbundmetadaten aktualisieren.**

1. Klicken Sie **OK**, um die Meldung zu ignorieren, dass einige Inhalte in den Verbundmetadaten von ADFS 2.0 nicht unterstützt werden.
1. Öffnen Sie **Windows PowerShell-Module.**
1. Nachdem alle Module geladen wurden, führen Sie den folgenden Befehl in PowerShell aus:

   `Get-ADFSProperties`

1. Suchen Sie nach dem Wert neben **Überwachungsintervall.**

   Diese Zahl steht für die Anzahl der Minuten zwischen den Abfragen. Der Standardwert sollte 1440 sein (1440 Minuten = 24 Stunden).

1. Legen Sie einen neuen Wert fest, indem Sie den folgenden Befehl in PowerShell ausführen:

   `Set-ADFSProperties -MonitoringInterval 1`

   Dadurch wird das Überwachungsintervall von alle 24 Stunden auf jede Minute geändert. Sie können den Wert 1 in einen anderen größeren Wert ändern, wenn Sie möchten, dass er seltener abgefragt wird.

1. Um sicherzustellen, dass dies ordnungsgemäß funktioniert, verwenden Sie die **Ereignisanzeige**, um in den ADFS2.0-Protokollen nach den folgenden Informationen zu suchen:

   **Ereignis-ID 156 und 157**

### Aktualisierung der ADFS-Metadaten erzwingen {#force-your-adfs-metadata-to-update}

Um Ihre ADFS-Metadaten zu aktualisieren, führen Sie die Schritte im folgenden Abschnitt aus.

So erzwingen Sie den Austausch von Metadaten zwischen Workfront und Ihrem SAML 2.0-Provider bei Verwendung von Active Directory Federation Services (ADFS):

>[!NOTE]
>
>Einige dieser Änderungen müssen möglicherweise von Ihrer IT-Abteilung vorgenommen werden.

1. Melden Sie sich beim ADFS-Server an und öffnen Sie die **ADFS-Verwaltungskonsole**.
1. Erweitern Sie im linken Bedienfeld **ADFS 2.0** und dann **Vertrauensstellungen**.

1. Klicken Sie auf **Ordner Vertrauenswürdige** .
1. Wählen Sie die Vertrauensstellung der vertrauenden Seite aus, die Sie zuvor für die Verwendung mit Workfront konfiguriert haben, und klicken Sie dann im rechten Bedienfeld auf **Aus Verbundmetadaten aktualisieren**.

   Wenn diese Option abgeblendet ist und nicht ausgewählt werden kann, führen Sie Folgendes aus:

   (Die Option ist nur abgeblendet, wenn die Vertrauensstellung der vertrauenden Seite zuvor mithilfe einer Metadatendatei konfiguriert wurde.)

   1. Kopieren Sie in Workfront im Bereich Setup die **Metadaten-URL** aus Ihrem Workfront-Setup für einmaliges Anmelden .

      So greifen Sie auf die Informationen für die **Metadaten-URL** zu:

      1. Klicken **oben rechts** Adobe Workfront in der Symbolleiste für globale Navigation auf „Setup“.
      1. Klicken Sie auf **System** > **Single Sign On (SSO)**.
      1. Klicken Sie **Einstellungen bearbeiten.**
      1. Klicken Sie **Konfiguration bearbeiten** und wählen Sie dann **SAML 2.0** in der **Typ** Dropdown-Liste aus.
      1. Kopieren Sie **Metadaten-URL**, die etwa wie folgt aussehen sollte:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Klicken Sie auf dem ADFS-Server mit der rechten Maustaste auf die Vertrauensstellung der vertrauenden Seite, die Sie zuvor konfiguriert haben, und klicken Sie dann auf **Eigenschaften.**
   1. Klicken Sie auf **Monitoring** und fügen Sie dann die URL, die Sie aus Workfront kopiert haben, in das Feld **Verbundmetadaten-URL des** ein.
   1. Markieren Sie die Optionen **vertrauende Seite überwachen** und **vertrauende Seite automatisch aktualisieren**.
   1. Klicken Sie **OK**.
   1. Wählen Sie die Vertrauensstellung der vertrauenden Seite aus, die Sie zuvor für die Verwendung mit Workfront konfiguriert haben, und klicken Sie dann im rechten Bedienfeld auf **Aus Verbundmetadaten aktualisieren.**

1. Klicken Sie **OK**, um die Meldung zu ignorieren, dass einige Inhalte in den Verbundmetadaten von ADFS 2.0 nicht unterstützt werden.
1. Klicken Sie auf **Aktualisieren**, um die Aktualisierung Ihrer Verbundmetadaten abzuschließen.

Benutzende, die über den nativen Anmeldebildschirm mit Workfront-Anmeldeinformationen auf Workfront zugreifen dürfen (dies kann auf der Profilseite jedes Benutzenden im Abschnitt **Zugriff** konfiguriert werden), können sich mit ihrem Workfront-Benutzernamen und -Kennwort anmelden, indem sie zur folgenden URL navigieren: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Verwenden anderer Identitätsanbieter

Wenn Sie andere Identitätsanbieter als ADFS verwenden (z. B. Ping, Okta oder Centrify), müssen Sie die Workfront-Metadaten erneut in Ihren Identitätsanbieter hochladen.

Weitere Informationen zum Abrufen einer neuen Workfront-Metadaten-URL finden Sie unter [Aktualisieren Ihrer ADFS-Metadaten](#update-your-adfs-metadata).

Weitere Informationen zur Verwendung von Active Directory Federation Services (ADFS) mit SAML 2.0 in Workfront finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0 mithilfe von ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
