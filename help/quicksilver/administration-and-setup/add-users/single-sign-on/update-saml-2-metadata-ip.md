---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: SAML 2.0-Metadaten in Ihrem Identitätsanbieter aktualisieren
description: Sie können SAML 2.0-Metadaten in Ihrem Identitäts-Provider aktualisieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# SAML 2.0-Metadaten in Ihrem Identitäts-Provider aktualisieren

{{important-admin-console-onboard}}

In den folgenden Abschnitten wird beschrieben, wie Sie Ihre SAML 2.0-Metadaten (Security Assertion Markup Language) aktualisieren, wenn Sie Active Directory Federation Services (ADFS) als Identitätsanbieter verwenden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Verwenden Sie ADFS als Identitätsanbieter

Sie können Ihre ADFS-Metadaten vor oder nach der Aktualisierung des SAML 2.0-Zertifikats durch Adobe Workfront aktualisieren. Wenn Sie die ADFS-Metadaten aktualisieren möchten, bevor Workfront das SAML 2.0-Zertifikat aktualisiert, sind zusätzliche Schritte erforderlich.

* [ADFS-Metadaten aktualisieren](#update-your-adfs-metadata)
* [Aktualisieren Ihrer ADFS-Metadaten erzwingen](#force-your-adfs-metadata-to-update)

### ADFS-Metadaten aktualisieren {#update-your-adfs-metadata}

Um die automatische Aktualisierung Ihrer ADFS-Metadaten festzulegen, führen Sie die Schritte in diesem Abschnitt aus.

Standardmäßig ist ADFS so konfiguriert, dass es automatisch nach Aktualisierungen aller vertraulichen Trust-Metadaten der Parteien sucht. Der Standardwert ist jedoch nur alle 24 Stunden auf &quot;Abfrage&quot;. Sie können diesen Wert mit powershell-Befehlen ändern.

1. Melden Sie sich beim ADFS-Server an und öffnen Sie die ADFS Management Console.
1. Erweitern Sie im linken Bereich **ADFS 2.0,** und dann **Vertrauensbeziehungen**.

1. Klicken Sie auf den Ordner &quot;**Vertrauende GruppenTrusts**&quot;.
1. Wählen Sie die Vertrauenswürdigkeit des Vertrauenden aus, die Sie zuvor für die Verwendung mit Workfront konfiguriert haben, und klicken Sie dann im rechten Bereich auf **Von den Föderationsmetadaten aktualisieren**.
1. (Bedingt) Wenn diese Option abgeblendet ist (d. h. die Vertrauenswürdigkeit der vertrauenden Partei zuvor mithilfe einer Metadatendatei konfiguriert wurde), führen Sie Folgendes aus.

   1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Setup** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

   1. Klicken Sie auf **System** > **Single Sign On (SSO)**.

   1. Klicken Sie auf **Einstellungen bearbeiten.**
   1. Klicken Sie auf **Konfiguration bearbeiten** und wählen Sie dann **SAML 2.0** in der Dropdownliste **Typ** aus.

   1. Kopieren Sie die **Metadaten-URL**, die in etwa wie folgt aussehen sollte:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Klicken Sie auf dem ADFS-Server mit der rechten Maustaste auf die zuvor konfigurierte Vertrauenswürdigkeit der vertrauenswürdigen Partei und klicken Sie dann auf **Eigenschaften**.
   1. Klicken Sie auf die Registerkarte **Überwachung** und fügen Sie dann die URL, die Sie aus Workfront kopiert haben, in das Feld **Verknüpfungs-Metadaten-URL des Erstanbieters** ein.

   1. Aktivieren Sie die Optionen für **Verfolgen Sie die vertrauliche Partei** und **Aktualisieren Sie die vertrauliche Partei automatisch**.

   1. Klicken Sie auf **OK.**
   1. Wählen Sie die Vertrauenswürdigkeit des Vertrauenden aus, die Sie zuvor für die Verwendung mit Workfront konfiguriert haben, und klicken Sie dann im rechten Bereich auf **Von Föderationsmetadaten aktualisieren** .

1. Klicken Sie auf **OK** , um die Meldung zu einigen Inhalten in den Verknüpfungsmetadaten zu ignorieren, die von ADFS 2.0 nicht unterstützt werden.
1. Öffnen Sie **Windows Powershell-Module.**
1. Nachdem alle Module geladen wurden, führen Sie den folgenden Befehl in powershell aus:

   `Get-ADFSProperties`

1. Suchen Sie nach dem Wert neben **Überwachungsintervall**.

   Es wird eine Zahl sein, die die Anzahl der Minuten zwischen den Umfragen darstellt. Der Standardwert sollte 1440 (1440 Minuten = 24 Stunden) sein.

1. Legen Sie einen neuen Wert fest, indem Sie den folgenden Befehl in powershell ausführen:

   `Set-ADFSProperties -MonitoringInterval 1`

   Dadurch wird das Überwachungsintervall von alle 24 Stunden auf jede Minute geändert. Sie können den Wert &quot;1&quot;in einen anderen größeren Wert ändern, wenn Sie möchten, dass die Umfrage weniger häufig erfolgt.

1. Um sicherzustellen, dass dies ordnungsgemäß funktioniert, verwenden Sie den **Ereignis-Viewer**, um in den ADFS2.0-Protokollen nach den folgenden Informationen zu suchen:

   **Ereignis-ID 156 und 157**

### Aktualisieren Ihrer ADFS-Metadaten erzwingen {#force-your-adfs-metadata-to-update}

Um Ihre ADFS-Metadaten zu aktualisieren, führen Sie die Schritte im folgenden Abschnitt aus.

So erzwingen Sie den Austausch von Metadaten zwischen Workfront und Ihrem SAML 2.0-Provider bei Verwendung von Active Directory Federation Services (ADFS):

>[!NOTE]
>
>Einige dieser Änderungen müssen möglicherweise von Ihrer IT-Abteilung vorgenommen werden.

1. Melden Sie sich beim ADFS-Server an und öffnen Sie die **ADFS Management Console**.
1. Erweitern Sie im linken Bedienfeld **ADFS 2.0** und dann **Vertrauensbeziehungen**.

1. Klicken Sie auf den Ordner &quot;**Vertrauende GruppenTrusts**&quot;.
1. Wählen Sie die Vertrauenswürdigkeit des Vertrauenden aus, die Sie zuvor für die Verwendung mit Workfront konfiguriert haben, und klicken Sie dann im rechten Bereich auf **Von Födermetadaten aktualisieren** .

   Wenn diese Option abgeblendet ist und nicht ausgewählt werden kann, führen Sie Folgendes aus:

   (Die Option ist nur abgeblendet, wenn die Vertrauenswürdigkeit der vertrauenden Partei zuvor mithilfe einer Metadatendatei konfiguriert wurde.)

   1. Kopieren Sie in Workfront im Setup-Bereich die **Metadaten-URL** aus Ihrem Workfront Single Sign-On-Setup-Bildschirm.

      So greifen Sie auf die Informationen für die **Metadaten-URL** zu:

      1. Klicken Sie in der Symbolleiste für globale Navigation oben rechts in Adobe Workfront auf **Einrichten** .
      1. Klicken Sie auf > **System** > **Single Sign On (SSO)**.
      1. Klicken Sie auf **Einstellungen bearbeiten.**
      1. Klicken Sie auf **Konfiguration bearbeiten** und wählen Sie dann **SAML 2.0** in der Dropdownliste **Typ** aus.
      1. Kopieren Sie die **Metadaten-URL**, die in etwa wie folgt aussehen sollte:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. Klicken Sie auf dem ADFS-Server mit der rechten Maustaste auf die zuvor konfigurierte Vertrauenswürdigkeit der vertrauenswürdigen Partei und klicken Sie dann auf **Eigenschaften**.
   1. Klicken Sie auf die Registerkarte **Überwachung** und fügen Sie dann die URL, die Sie aus Workfront kopiert haben, in das Feld **Verknüpfungs-Metadaten-URL des Erstanbieters** ein.
   1. Aktivieren Sie die Optionen für **Verfolgen Sie die vertrauliche Partei** und **Aktualisieren Sie die vertrauliche Partei automatisch**.
   1. Klicken Sie auf **OK**.
   1. Wählen Sie die Vertrauenswürdigkeit des Vertrauenden aus, die Sie zuvor für die Verwendung mit Workfront konfiguriert haben, und klicken Sie dann im rechten Bereich auf **Von Föderationsmetadaten aktualisieren** .

1. Klicken Sie auf **OK** , um die Meldung zu einigen Inhalten in den Verknüpfungsmetadaten zu ignorieren, die von ADFS 2.0 nicht unterstützt werden.
1. Klicken Sie auf **Aktualisieren** , um die Aktualisierung der Verknüpfungsmetadaten abzuschließen.

Benutzer, die über den nativen Anmeldebildschirm mit Workfront-Anmeldedaten auf Workfront zugreifen dürfen (dies kann über die Profilseite der einzelnen Benutzer im Abschnitt **Zugriff** konfiguriert werden), können sich mit ihrem Workfront-Benutzernamen und Kennwort anmelden, indem sie zur folgenden URL navigieren: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Andere Identitätsanbieter verwenden

Bei Verwendung anderer Identitätsanbieter als ADFS (z. B. Ping, Okta oder Centrify) müssen Sie die Workfront-Metadaten erneut in Ihren Identitätsanbieter hochladen.

Weitere Informationen zum Abrufen einer neuen Workfront-Metadaten-URL finden Sie unter [Aktualisieren Ihrer ADFS-Metadaten](#update-your-adfs-metadata).

Weitere Informationen zur Verwendung von Active Directory Federation Services (ADFS) mit SAML 2.0 in Workfront finden Sie unter [Konfigurieren von Adobe Workfront mit SAML 2.0 mit ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
