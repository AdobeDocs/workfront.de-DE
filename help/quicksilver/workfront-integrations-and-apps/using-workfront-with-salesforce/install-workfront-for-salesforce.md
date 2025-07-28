---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installieren [!DNL Adobe Workfront] für [!DNL Salesforce]
description: Informationen zum Installieren der App, bevor sie in der  [!DNL Salesforce] AppExchange verfügbar wird, finden Sie unter " [!DNL Workfront]  für Salesforce", bevor sie im AppExchange Marketplace verfügbar wird.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1092'
ht-degree: 1%

---

# Installieren von [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses wird die Integration von Workfront mit Salesforce nach dem 28. **2026 nicht mehr**.
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Salesforce zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Salesforce finden Sie unter [Salesforce-Module](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Als [!DNL Salesforce]- und [!DNL Adobe Workfront] können Sie [!DNL Workfront for Salesforce] installieren, damit Ihre [!DNL Salesforce]-Benutzer [!DNL Workfront]-Anfragen senden und Projekte automatisch erstellen können, ohne Salesforce verlassen zu müssen.

Allgemeine Informationen dazu, was Sie bei der Installation von [!DNL Workfront for Salesforce] erwarten können, finden Sie unter [[!DNL Adobe Workfront for Salesforce] Übersicht](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Voraussetzungen für die Installation und Verwendung [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Wird installiert [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Funktionen nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen für die Installation und Verwendung von [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Sie müssen über eine [!DNL Salesforce]-Instanz mit Zugriff auf ein Systemadministratorkonto verfügen, um die App zu installieren.
* Sie müssen über eine [!DNL Workfront] mit Zugriff auf ein Systemadministratorkonto verfügen, um die Integration konfigurieren zu können.
* [!UICONTROL Salesforce]-Benutzer müssen über ein [!DNL Workfront] verfügen, damit sie:

   * Erstellen von [!DNL Workfront] Anfragen aus [!DNL Salesforce]
   * Anzeigen von [!DNL Workfront] oder Projekten in Salesforce

## Installieren von [!DNL Workfront for Salesforce]  {#installing-workfront-for-salesforce}

Sie müssen [!DNL Salesforce] und [!DNL Workfront] sein, um [!DNL Workfront for Salesforce] installieren und konfigurieren zu können.

In den folgenden Unterabschnitten wird beschrieben, wie Sie [!DNL Workfront] für Ihre [!DNL Salesforce] Produktionsumgebung installieren. Sie können die gleichen Schritte ausführen, um [!DNL Workfront] für Ihre [!DNL Salesforce] Sandbox-Umgebung zu installieren.

* [Installation  [!DNL Workfront for Salesforce] , bevor es im  [!DNL AppExchange]  verfügbar wird](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installieren  [!DNL Workfront for Salesforce]  Framework [!DNL Salesforce Classic] ](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installieren  [!DNL Workfront for Salesforce]  Framework [!DNL Salesforce Lightning Experience] ](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installieren von [!DNL Workfront for Salesforce], bevor es im [!DNL AppExchange] Marketplace verfügbar wird {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] wird in Kürze in der [!DNL Salesforce AppExchange] verfügbar sein.

So installieren Sie die App, bevor sie verfügbar ist:

1. Wechseln Sie in Ihrer Produktionsumgebung zu .

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   Navigieren Sie in Ihrer Sandbox-Umgebung zu .

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >Sie müssen bei Salesforce angemeldet sein, um auf diese Seiten zugreifen zu können.

1. Aktivieren Sie **[!UICONTROL Kontrollkästchen „Ja, Zugriff auf diese Websites von Drittanbietern gewähren]**.

   Ein Ladebildschirm wird angezeigt. Die Installation kann einige Zeit in Anspruch nehmen.

1. Klicken Sie **[!UICONTROL Abschluss]** Installation auf „Fertig“.

1. Navigieren Sie zu **[!UICONTROL Setup]** > **[!UICONTROL Sicherheit] Controls** > **[!UICONTROL Remote-Site-Einstellungen]**.
1. (Bedingt) Wählen Sie Workfront in der Liste aus.

   Oder

   Wenn Ihre [!DNL Workfront]-URL nicht in der Liste &quot;**[!UICONTROL Remotestandorte“ aufgeführt]**, klicken Sie auf **[!UICONTROL Neue Remotesite]**.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie den **[!UICONTROL Remote-Site-Namen]** an.

   Beispiel: *[!DNL Workfront]*.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie die **[!UICONTROL Remote-Site-URL]** an.

   Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die [!DNL Workfront] App ist jetzt auf Ihrer [!DNL Salesforce]-Instanz installiert und die **[!UICONTROL WorkfrontOpportunities]** und **[!UICONTROL WorkfrontAccounts]** [!UICONTROL VisualForce] Seiten wurden in Ihrer Umgebung erstellt.

   [!DNL Salesforce] Benutzer können die App verwenden, sobald Sie den [!DNL Workfront] Abschnitt zu ihren [!UICONTROL Opportunity]- oder [!UICONTROL Account]-Layouts hinzugefügt haben.\
   Informationen zum Konfigurieren des Workfront-Bereichs für Benutzerinnen und Benutzer finden Sie unter [Konfigurieren des Adobe Workfront-Bereichs für Salesforce-Benutzerinnen und -Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installieren von [!DNL Workfront] für [!DNL Salesforce] im [!DNL Salesforce Classic] Framework

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. Navigieren Sie zu **Setup.**
1. Klicken **im Abschnitt** auf **AppExchange Marketplace**.

1. Geben Sie in das Feld **AppExchange-Apps suchen** **Workfront ein**.

1. Klicken Sie auf die Workfront-App, wenn Sie sie gefunden haben, und klicken **auf „Jetzt abrufen**.
1. Klicken Sie **[!UICONTROL In Produktion installieren]**, um die [!DNL Workfront] App in Ihrer [!DNL Salesforce] Produktionsumgebung zu installieren. (empfohlen)
1. Nachdem Sie die Nutzungsbedingungen gelesen und akzeptiert haben, aktivieren Sie das Feld **[!UICONTROL Ich habe die Nutzungsbedingungen gelesen und stimme ihnen zu]**.
1. Klicken Sie **[!UICONTROL Bestätigen und installieren]**.
1. Wählen Sie **[!UICONTROL Für alle Benutzer installieren]** (empfohlen) aus und klicken Sie dann auf **[!UICONTROL Installieren]**.

1. (Bedingt) Wenn Sie gefragt werden, ob Sie den Zugriff eines Drittanbieters genehmigen möchten, müssen Sie **[!UICONTROL Ja, Zugriff auf diese Websites von Drittanbietern gewähren]** auswählen und dann auf **[!UICONTROL Weiter]** klicken.

1. Klicken Sie **[!UICONTROL Abschluss]** Installation auf „Fertig“.

   Die [!DNL Workfront] App wird unter &quot;**[!UICONTROL Pakete“]**.


1. Navigieren Sie **[!UICONTROL Setup > Sicherheitskontrollen > Einstellungen für Remote-Standort]**.
1. (Bedingt) Wenn Ihre [!DNL Workfront]-URL nicht in der Liste &quot;**[!UICONTROL Remote-Standorte“ aufgeführt]**, klicken Sie auf **[!UICONTROL Neue Remote-Standort]**.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie den **[!UICONTROL Remote-Site-Namen]** an.
Beispiel: *[!DNL Workfront]*.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie die **[!UICONTROL Remote-Site-URL]** an.
Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.\
   Die [!DNL Workfront]-App ist jetzt auf Ihrer [!DNL Salesforce]-Instanz installiert. Die **[!UICONTROL WorkfrontOpportunities]** und **[!UICONTROL WorkfrontAccounts]** [!UICONTROL VisualForce] Seiten wurden in Ihrer Umgebung erstellt.\
   [!DNL Salesforce] Benutzer können die App erst verwenden, wenn Sie den [!DNL Workfront] Abschnitt zu ihren [!UICONTROL Opportunity]- oder [!UICONTROL Account]-Layouts hinzugefügt haben.\
   Informationen zum Konfigurieren des [!DNL Workfront] für Benutzer finden Sie unter [Konfigurieren des  [!DNL Adobe Workfront]  für  [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installieren von [!DNL Workfront for Salesforce] im [!DNL Salesforce Lightning Experience] Framework

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. Klicken Sie auf **[!UICONTROL Setup]-Symbol** und dann auf **[!UICONTROL Setup]**.

1. Erweitern Sie im **[!UICONTROL PLATFORM TOOLS]** den Eintrag **[!UICONTROL Apps].**

1. Klicken Sie auf **[!DNL AppExchange Marketplace]**.
1. Geben Sie in das **[!UICONTROL Suche [!DNL AppExchange] Apps]**-Feld **[!DNL Workfront]** ein.

1. Klicken Sie auf die Workfront-App, wenn Sie sie gefunden haben, und klicken **auf „Jetzt abrufen**.
1. Klicken Sie **[!UICONTROL Anmeldebildschirm öffnen]**.\
   Sie müssen sich zum [!DNL Workfront] mit Ihrem [!DNL Salesforce] Administratorkonto anmelden.

1. Klicken Sie **[!UICONTROL Zulassen]**.
1. Klicken Sie im Feld **[!UICONTROL In dieser Organisation installieren]** auf **[!UICONTROL Hier]**, um [!DNL Workfront] in Ihrer [!DNL Salesforce] Produktionsumgebung zu installieren. (empfohlen)

1. Nachdem Sie die Nutzungsbedingungen gelesen und akzeptiert haben, aktivieren Sie das Feld **[!UICONTROL Ich habe die Nutzungsbedingungen gelesen und stimme ihnen zu]**.
1. Klicken Sie **[!UICONTROL Bestätigen und installieren]**.
1. Wählen Sie **[!UICONTROL Für alle Benutzer installieren]** (empfohlen) aus und klicken Sie dann auf **[!UICONTROL Installieren]**.

1. (Bedingt) Wenn Sie gefragt werden, ob Sie den Zugriff eines Drittanbieters genehmigen möchten, müssen Sie **[!UICONTROL Ja, Zugriff auf diese Websites von Drittanbietern gewähren]** auswählen und dann auf **[!UICONTROL Weiter]** klicken.

1. Klicken Sie **[!UICONTROL Abschluss]** Installation auf „Fertig“.

   Die [!DNL Workfront] App wird unter &quot;**[!UICONTROL Pakete“]**.

1. Navigieren Sie zu **[!UICONTROL Setup].**
1. Erweitern Sie **[!UICONTROL Abschnitt]** EINSTELLUNGEN“ **[!UICONTROL Sicherheit].**

1. Klicken Sie auf **[!UICONTROL Einstellungen für Remote-Standort]**.
1. (Bedingt) Wenn Ihre [!DNL Workfront]-URL nicht in der Liste &quot;**[!UICONTROL Remote-Standorte“ aufgeführt]**, klicken Sie auf **[!UICONTROL Neue Remote-Standort]**.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie den **[!UICONTROL Remote-Site-Namen]** an.
Beispiel: *[!DNL Workfront]*.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie die **[!UICONTROL Remote-Site-URL]** an.
Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die [!DNL Workfront]-App ist jetzt auf Ihrer [!DNL Salesforce]-Instanz installiert, und die **[!DNL Workfront]**-Komponente wird jetzt zu Ihrer Umgebung hinzugefügt.

   [!UICONTROL Salesforce]-Benutzer können die [!DNL Workfront]-App verwenden, sobald Sie den [!DNL Workfront] Abschnitt zu ihren Seiten[!UICONTROL Layouts „Opportunity] oder [!UICONTROL Account] hinzugefügt haben.\
   Informationen zum Konfigurieren des [!DNL Workfront] für Benutzer finden Sie unter [Konfigurieren des  [!DNL Adobe Workfront]  für  [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

## Konfigurieren von Berechtigungen für die Integration von Workfront mit Salesforce

### Berechtigungen für `workfront_business`

1. Navigieren Sie zu **Setup** > **Sicherheit** > **Vertrauenswürdige URLs**.
1. Wählen Sie `workfront_business` aus der Liste aus.
1. Klicken Sie **Bearbeiten**.
1. Überprüfen Sie unter CSP-Anweisungen die folgenden Optionen:

   * connect-src (Skripte)
   * font-src (Schriftarten)
   * frame-src (iframe-Inhalt)
   * img-src (Bilder)
   * media-src (Audio und Video)
   * style-src (stylesheets)

1. Klicken Sie auf **Speichern**.


### Berechtigungen für workfront_session

1. Navigieren Sie zu **Setup** > **Sicherheit** > **Vertrauenswürdige URLs**.
1. Wählen Sie `workfront_session` aus der Liste aus.
1. Klicken Sie **Bearbeiten**.
1. Überprüfen Sie unter CSP-Anweisungen die folgenden Optionen:

   * connect-src (Skripte)
   * font-src (Schriftarten)
   * frame-src (iframe-Inhalt)
   * img-src (Bilder)
   * media-src (Audio und Video)
   * style-src (stylesheets)

1. Klicken Sie auf **Speichern**.

