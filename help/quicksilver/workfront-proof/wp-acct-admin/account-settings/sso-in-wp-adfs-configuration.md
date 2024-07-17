---
product-previous: workfront-proof
product-area: documents;system-administration;user-
navigation-topic: account-settings-workfront-proof
title: 'Single Sign-On in [!DNL Workfront Proof]: AD FS-Konfiguration'
description: Wenn Sie Administrator auf Ihrem AD-Server sind, können Sie AD FS installieren und konfigurieren.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 670422e9-5db8-4f06-baf8-1f9ce83873fe
source-git-commit: a6cd3fe793c197308105da27369191d84cb59377
workflow-type: tm+mt
source-wordcount: '928'
ht-degree: 0%

---

# Single Sign-On in [!DNL Workfront Proof]: AD FS-Konfiguration

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Wenn Sie Administrator auf Ihrem AD-Server sind, können Sie AD FS installieren und konfigurieren.

## Installieren und Konfigurieren von AD FS

1. Laden Sie [AD FS 2.0](http://www.microsoft.com/en-us/download/details.aspx?id=10909) auf Ihren Computer herunter.
1. Öffnen Sie die heruntergeladene Datei &quot;AdfsSetup.exe&quot;, um den Installationsassistenten für ADFS (Active Directory Federation Services) zu starten.
1. Wählen Sie im Bildschirm &quot;Serverrolle&quot;eine der Optionen aus (Sie benötigen mindestens einen Föderierungsserver).
1. Wenn Sie IIS auf Ihrem AD-Server nicht für das Internet verfügbar machen möchten (Ports 80 und 443 für HTTP und HTTPS), können Sie zunächst einen Föderations-Server hinter der Firewall einrichten und dann einen zweiten Föderations-Server-Proxy erstellen, der Anfragen über die Firewall an den Föderationsserver weiterleitet.
1. Nachdem Sie die Einrichtung von AD FS abgeschlossen haben, wählen Sie **[!UICONTROL Starten Sie das Management-Snap-In für AD FS 2.0]** und klicken Sie dann auf **[!UICONTROL Beenden]**. Sobald dies abgeschlossen ist, sollte das Verwaltungsfenster für AD FS 2.0 sofort geöffnet werden. Ist dies nicht der Fall, können Sie ihn über &quot;**[!UICONTROL Start]**&quot;> &quot;**[!UICONTROL Verwaltung&quot;]** &quot;> &quot;**[!UICONTROL Verwaltung von AD FS 2.0&quot;]** öffnen. Dies ist die wichtigste AD FS-Kontrollanwendung.

1. Beginnen Sie mit der Auswahl des Assistenten für die Konfiguration des Verbandsservers AD FS 2.0.
Dadurch können Sie AD FS konfigurieren und über IIS und AD mit dem Internet verbinden.
1. Wenn Sie einen neuen AD FS-Server konfigurieren, wählen Sie **[!UICONTROL Create a new Federation Service]**.
1. Wählen Sie **[!UICONTROL eigenständigen Verknüpfungsserver]** (zu Test- und Auswertungszwecken).

1. Klicken Sie für hohe Verfügbarkeit und Lastenausgleich auf Neue Farm des Verbands-Servers .
1. Geben Sie den Namen Ihres Föderierungsdiensts an.
Standardmäßig ruft der Konfigurationsassistent das an die Standard-Website in IIS gebundene SSL-Zertifikat ab und verwendet den dort angegebenen Betreffnamen. Wenn Sie ein Platzhalterzertifikat verwenden, müssen Sie den Namen des Föderationsdiensts eingeben.
Wenn in IIS kein SSL-Zertifikat konfiguriert ist, sucht der Konfigurationsassistent im Zertifikatspeicher des lokalen Computers nach gültigen Zertifikaten. Diese werden in der Dropdown-Liste SSL-Zertifikat angezeigt. Wenn keine Zertifikate gefunden wurden, können Sie den Server Certificate Generator in IIS verwenden, um eines zu erstellen.

1. Fahren Sie mit der Konfiguration fort und klicken Sie nach Abschluss auf **[!UICONTROL Schließen]** .

## Konfigurieren von [!DNL Workfront Proof] Single Sign-On

Wenn Sie ein [!DNL Workfront Proof] -Administrator sind, können Sie Single Sign-On auf der Seite [!DNL Workfront Proof] konfigurieren. Weitere Informationen finden Sie unter [Single Sign-On in [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/single-sign-on-overview.md).

1. Klicken Sie auf **[!UICONTROL Einstellungen]** > **[!UICONTROL Kontoeinstellungen]** und öffnen Sie dann die Registerkarte **[!UICONTROL Single Sign-on]** .

1. Fügen Sie im Feld **SSO-URL** Ihre Entitäts-ID ein.
Im Folgenden finden Sie ein Beispiel für eine Entitäts-ID:
http://*&lt;adfs.your-company.com>*/adfs/services/trust
Ihre Entitäts-ID finden Sie in Ihrer XML-Datei &quot;Federation Metadata&quot;.
   ![ProofHQ_configuration_02.png](assets/proofhq-configuration-02-350x80.png)

1. Federation-Metadaten finden Sie im Ordner AD FS 2.0-Snap-In > Dienst > Endpunkte . Suchen Sie im Abschnitt Metadaten den mit dem Metadatentyp &quot;Federation&quot;. Fügen Sie diesen Endpunkt in Ihren Browser ein, um Metadaten anzuzeigen. Sie können auch direkt zu diesem Link gehen: https://*&lt;adfs.your-company.com>*/FederationMetadata/2007-06/FederationMetadata.xml , nachdem Sie die Datei {adfs.your-company.com} durch Ihre eigenen Details ersetzt haben.
1. Fügen Sie in das Feld **[!UICONTROL Anmelde-URL]** Ihre SSO-Anmeldung ein.
1. Im Folgenden finden Sie ein Beispiel für eine SSO-Anmeldung:
1. http://*&lt;adfs.your-company.com>*/adfs/ls.
1. Dieser Link befindet sich in der XML-Datei &quot;Federation Metadata&quot;.
   ![ProofHQ_configuration_03.png](assets/proofhq-configuration-03-350x90.png)

1. Geben Sie in das Feld **[!UICONTROL URL abmelden]** den Link ein und speichern Sie ihn.
Im Folgenden finden Sie ein Beispiel für eine Abmelde-URL:
https://*&lt;adfs.your-company.com>*/adfs/ls/?wa=wsignout1.0

   1. Wechseln Sie zu Ihrem AD FS Manager > Vertrauensbeziehungen > Vertrauenswürdige GruppenTrusts - Eigenschaften von ProofHQ.
   1. Klicken Sie unter den Endpunkten auf [!UICONTROL Hinzufügen und geben Sie den Eintrag] mit den folgenden Details ein:

      * Endpunkttyp = SAML-Abmeldung
      * Bindung = POST
      * URL = https://*&lt;adfs.your-company.com*>/adfs/ls/?wa=wsignout1.0
      * Dieser Schritt kann nach der Konfiguration des Vertrauenswürdigkeit der Partei (siehe unten) in Ihrem AD FS abgeschlossen werden.
   1. Geben Sie in das Feld **[!UICONTROL Certificate fingerprint]** die Daten aus Ihrem Zertifikat ein.
   1. Navigieren Sie zu Ihrem ADFS 2.0-Snap-In zu Dienst > Zertifikate > Token-Signatur.
   1. Klicken Sie mit der rechten Maustaste auf diesen Eintrag, um das Zertifikat anzuzeigen.
   1. Kopieren Sie auf der Registerkarte [!UICONTROL Zertifikatdetails] den Thumbprint und fügen Sie ihn in die Konfigurationsregisterkarte **[!UICONTROL Workfront Proof Single Sign-On]** ein.

   1. Die Fingerabdruckzeichen können durch Doppelpunkte oder Leerzeichen getrennt werden. Es wird jedoch empfohlen, sie zu entfernen. Wenn Sie Probleme mit Ihrer Single-Sign-On-Konfiguration haben, wenden Sie sich an den Support.


## Hinzufügen eines Vertrauenspartenvertrauens

Sobald die Konfiguration abgeschlossen ist, müssen Sie in Ihrem AD FS im Abschnitt &quot;Vertrauende Partei - Trusts&quot;arbeiten.

1. Navigieren Sie zum Ordner **[!UICONTROL Vertrauensbeziehungen]** > **[!UICONTROL Vertrauenswürdige Parteivertrauer]** und klicken Sie dann auf **[!UICONTROL Vertrauenswürdigen Parteivertrauens hinzufügen]** , um den Konfigurationsassistenten zu starten.

1. Wählen Sie Ihre Datenquelle aus.
Alle Metadaten für Ihr [!DNL ProofHQ] -Konto befinden sich unter einem Link wie diesem:
https://`<yoursubdomain*>`.proofhq.com/saml/module.php/saml/sp/metadata.php/phq
Dadurch wird der Großteil des Vertrauens der vertrauenden Partei konfiguriert.

   >[!NOTE]
   >
   >* Wenn Sie Probleme bei der Herstellung der Verbindung über die URL haben, speichern Sie die Metadaten als Datei und wählen Sie den Import von Daten aus einer Datei aus.
   >* Wenn Sie eine vollständige benutzerdefinierte Domäne (z. B. www.your-proofing.com) für Ihr [!DNL ProofHQ]-Konto konfiguriert haben, ersetzen Sie den gesamten &quot;{yoursubdomain}.proofhq.com&quot;-Teil durch Ihre eigene Domäne, um Ihren &quot;[!DNL ProofHQ]&quot;-Metadaten-Link zu erstellen.


## Konfigurieren von Anforderungsregeln

Sobald die Konfiguration des Vertrauens der vertraulichen Partei abgeschlossen ist, können Sie die Schadensregeln konfigurieren, um die Einrichtung abzuschließen. Sie konfigurieren zwei Schadensregeln für ProofHQ: E-Mail und Name ID.

1. Öffnen Sie das Dialogfeld **[!UICONTROL Anforderungsregeln bearbeiten]** .
1. Gehen Sie zu **[!UICONTROL ProofHQ Relying Party Trust]** und klicken Sie dann auf **[!UICONTROL Edit Claim Rules]** (1).\
   Das Popup-Fenster sollte automatisch geöffnet werden, wenn Sie diese Option am Ende der Vertrauenskonfiguration ausgewählt haben.

1. Klicken Sie auf **[!UICONTROL Regel hinzufügen]** (2) , um das Fenster zur Schadenskonfiguration zu öffnen.

   * E-Mail (Senden von LDAP-Attributen als Schadensregelvorlage)
   * NameID (Regelvorlage für eingehende Anforderung transformieren)
