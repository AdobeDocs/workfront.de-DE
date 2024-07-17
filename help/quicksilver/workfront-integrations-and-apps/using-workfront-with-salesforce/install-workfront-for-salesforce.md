---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installieren Sie [!DNL Adobe Workfront] für [!DNL Salesforce]
description: Um die App zu installieren, bevor sie in der AppExchange verfügbar wird, lesen Sie Installieren von [!DNL Workfront] für Salesforce , bevor sie im AppExchange Marketplace verfügbar wird. [!DNL Salesforce]
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: c0e7340e2bf650b6f9931ae12aee07c5f7d5292b
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---

# Installieren Sie [!DNL Adobe Workfront for Salesforce]

<!-- Audited: 1/2024 -->

>[!NOTE]
>
>Um die App zu installieren, bevor sie in [!DNL Salesforce AppExchange] verfügbar wird, lesen Sie den Abschnitt [Installieren [!DNL Workfront for Salesforce]  , bevor sie im  [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace) verfügbar wird.

Als [!DNL Salesforce] - und [!DNL Adobe Workfront] -Administrator können Sie [!DNL Workfront for Salesforce] installieren, damit Ihre [!DNL Salesforce] -Benutzer [!DNL Workfront] -Anforderungen senden und automatisch Projekte erstellen können, ohne Salesforce jemals verlassen zu müssen.

Ein allgemeines Verständnis darüber, was Sie durch die Installation von [!DNL Workfront for Salesforce] erwarten können, finden Sie unter [[!DNL Adobe Workfront for Salesforce] Übersicht](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Voraussetzungen für die Installation und Verwendung von [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installieren [!DNL Workfront for Salesforce]](#installing-workfrontfor-salesforce)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen für die Installation und Verwendung von [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Sie müssen über eine [!DNL Salesforce] -Instanz mit Zugriff auf ein Systemadministratorkonto verfügen, um die App installieren zu können.
* Sie müssen über eine [!DNL Workfront] -Instanz mit Zugriff auf ein Systemadministratorkonto verfügen, um die Integration konfigurieren zu können.
* Benutzer von [!UICONTROL Salesforce] müssen über ein [!DNL Workfront] -Konto verfügen, um Folgendes tun zu können:

   * [!DNL Workfront] Anforderungen von [!DNL Salesforce] erstellen
   * Anzeigen von [!DNL Workfront]-Anforderungen oder -Projekten in Salesforce

## Installieren von [!DNL Workfront for Salesforce] {#installing-workfront-for-salesforce}

Sie müssen ein [!DNL Salesforce] und ein [!DNL Workfront] Systemadministrator sein, um [!DNL Workfront for Salesforce] zu installieren und zu konfigurieren.

In den folgenden Unterabschnitten wird beschrieben, wie Sie [!DNL Workfront] für Ihre [!DNL Salesforce] -Produktionsumgebung installieren. Sie können dieselben Schritte ausführen, um [!DNL Workfront] für Ihre [!DNL Salesforce] Sandbox-Umgebung zu installieren.

* [Installieren von [!DNL Workfront for Salesforce] bevor es im  [!DNL AppExchange] Marketplace verfügbar wird](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installieren von [!DNL Workfront for Salesforce] im [!DNL Salesforce Classic] Framework](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installieren von [!DNL Workfront for Salesforce] im [!DNL Salesforce Lightning Experience] Framework](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installieren von [!DNL Workfront for Salesforce] , bevor es im [!DNL AppExchange] Marketplace verfügbar wird {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] wird bald in der [!DNL Salesforce AppExchange] verfügbar sein.

So installieren Sie die App, bevor sie verfügbar ist:

1. Navigieren Sie in Ihrer Produktionsumgebung zu

   [https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://login.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   Navigieren Sie in Ihrer Sandbox-Umgebung zu

   [https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk](https://test.salesforce.com/packaging/installPackage.apexp?p0=04tJ9000000HCqk)

   >[!NOTE]
   >
   >Sie müssen bei Salesforce angemeldet sein, um auf diese Seiten zugreifen zu können.

1. Aktivieren Sie die Option **[!UICONTROL Ja, gewähren Sie Zugriff auf diese Drittanbieter-Websites]**.

   Ein Ladebildschirm wird angezeigt. Die Installation kann einige Zeit in Anspruch nehmen.

1. Klicken Sie auf **[!UICONTROL Fertig]** , wenn die Installation abgeschlossen ist.

1. Navigieren Sie zu &quot;**[!UICONTROL Setup]**&quot;> &quot;**[!UICONTROL Sicherheit] Steuerelemente**&quot;> &quot;**[!UICONTROL Remote-Site-Einstellungen]**&quot;.
1. (Bedingt) Wählen Sie Workfront aus der Liste aus.

   Oder

   Wenn Ihre [!DNL Workfront]-URL nicht in der Liste **[!UICONTROL Alle Remote-Sites]** aufgeführt ist, klicken Sie auf **[!UICONTROL Neue Remote-Site]**.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie den **[!UICONTROL Remote Site Name]** an.

   Beispiel: *[!DNL Workfront]*.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie die **[!UICONTROL Remote Site URL]** an.

   Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die [!DNL Workfront] -App ist jetzt auf Ihrer [!DNL Salesforce] -Instanz installiert und die Seiten **[!UICONTROL WorkfrontOpportunities]** und **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] wurden in Ihrer Umgebung erstellt.

   [!DNL Salesforce] -Benutzer können die App verwenden, sobald Sie den Abschnitt [!DNL Workfront] zu ihren Seitenlayouts für [!UICONTROL Chancen] oder [!UICONTROL Konto] hinzugefügt haben.\
   Informationen zum Konfigurieren des Workfront-Abschnitts für Benutzer finden Sie unter [Konfigurieren des Adobe Workfront-Abschnitts für Salesforce-Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installieren von [!DNL Workfront] für [!DNL Salesforce] im [!DNL Salesforce Classic] Framework

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. Navigieren Sie zu **Setup.**
1. Klicken Sie im Abschnitt **Build** auf **AppExchange Marketplace**.

1. Geben Sie in das Feld **AppExchange-Apps durchsuchen** den Wert **Workfront** ein.

1. Klicken Sie auf die Workfront-App, sobald Sie sie gefunden haben, und klicken Sie dann auf **Jetzt abrufen**.
1. Klicken Sie auf **[!UICONTROL In Produktion installieren]** , um die [!DNL Workfront] -App in Ihrer [!DNL Salesforce] -Produktionsumgebung zu installieren. (empfohlen)
1. Nachdem Sie die Geschäftsbedingungen gelesen und akzeptiert haben, aktivieren Sie das Feld **[!UICONTROL Ich habe die Geschäftsbedingungen gelesen und stimme ihnen zu]**.
1. Klicken Sie auf **[!UICONTROL Bestätigen und installieren]**.
1. Wählen Sie **[!UICONTROL Für alle Benutzer installieren]** (empfohlen) und klicken Sie dann auf **[!UICONTROL Installieren]**.

1. (Bedingt) Wenn Sie gefragt werden, ob Sie den Zugriff eines Drittanbieters genehmigen möchten, müssen Sie &quot;**[!UICONTROL Ja&quot;auswählen, den Zugriff auf diese Drittanbieter-Websites gewähren]**&quot;und dann auf &quot;**[!UICONTROL Weiter]**&quot;klicken.

1. Klicken Sie auf **[!UICONTROL Fertig]** , wenn die Installation abgeschlossen ist.

   Die [!DNL Workfront]-App wird unter **[!UICONTROL Installierte Pakete]** aufgeführt.


1. Navigieren Sie zu **[!UICONTROL Einrichtung>Sicherheitssteuerung>Remote-Site-Einstellungen]**.
1. (Bedingt) Wenn Ihre [!DNL Workfront]-URL nicht in der Liste **[!UICONTROL Alle Remote-Sites]** aufgeführt ist, klicken Sie auf **[!UICONTROL Neue Remote-Site]**.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie den **[!UICONTROL Remote Site Name]** an.
Beispiel: *[!DNL Workfront]*.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie die **[!UICONTROL Remote Site URL]** an.
Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.\
   Die [!DNL Workfront] -App ist jetzt auf Ihrer [!DNL Salesforce] -Instanz installiert. Die Seiten **[!UICONTROL WorkfrontOpportunities]** und **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualforce] wurden in Ihrer Umgebung erstellt.\
   [!DNL Salesforce] -Benutzer können die App noch nicht verwenden, bis Sie den Abschnitt [!DNL Workfront] zu ihren Seitenlayouts für [!UICONTROL Chancen] oder [!UICONTROL Konto] hinzugefügt haben.\
   Informationen zum Konfigurieren des Abschnitts [!DNL Workfront] für Benutzer finden Sie unter Abschnitt [Konfigurieren des Abschnitts [!DNL Adobe Workfront] für  [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installieren von [!DNL Workfront for Salesforce] im [!DNL Salesforce Lightning Experience] Framework

1. Melden Sie sich bei [!DNL Salesforce] als Systemadministrator an.
1. Klicken Sie auf das Symbol **[!UICONTROL Einrichten]** und dann auf **[!UICONTROL Einrichtung]**.

1. Erweitern Sie im Abschnitt **[!UICONTROL PLATFORM TOOLS]** den Eintrag **[!UICONTROL Apps].**

1. Klicken Sie auf **[!DNL AppExchange Marketplace]**.
1. Geben Sie in das Feld **[!UICONTROL Suche [!DNL AppExchange] Apps]** den Wert **[!DNL Workfront]** ein.

1. Klicken Sie auf die Workfront-App, sobald Sie sie gefunden haben, und klicken Sie dann auf **Jetzt abrufen**.
1. Klicken Sie auf **[!UICONTROL Anmeldebildschirm öffnen]**.\
   Sie müssen sich mit Ihrem [!DNL Workfront] -Administratorkonto für [!DNL Salesforce] anmelden.

1. Klicken Sie auf **[!UICONTROL Allow]**.
1. Klicken Sie im Feld **[!UICONTROL In dieser Organisation installieren]** auf **[!UICONTROL Hier installieren]** , um [!DNL Workfront] in Ihrer [!DNL Salesforce] -Produktionsumgebung zu installieren. (empfohlen)

1. Nachdem Sie die Geschäftsbedingungen gelesen und akzeptiert haben, aktivieren Sie das Feld **[!UICONTROL Ich habe die Geschäftsbedingungen gelesen und stimme ihnen zu]**.
1. Klicken Sie auf **[!UICONTROL Bestätigen und installieren]**.
1. Wählen Sie **[!UICONTROL Für alle Benutzer installieren]** (empfohlen) und klicken Sie dann auf **[!UICONTROL Installieren]**.

1. (Bedingt) Wenn Sie gefragt werden, ob Sie den Zugriff eines Drittanbieters genehmigen möchten, müssen Sie &quot;**[!UICONTROL Ja&quot;auswählen, den Zugriff auf diese Drittanbieter-Websites gewähren]**&quot;und dann auf &quot;**[!UICONTROL Weiter]**&quot;klicken.

1. Klicken Sie auf **[!UICONTROL Fertig]** , wenn die Installation abgeschlossen ist.

   Die [!DNL Workfront]-App wird unter **[!UICONTROL Installierte Pakete]** aufgeführt.

1. Navigieren Sie zu **[!UICONTROL Setup].**
1. Erweitern Sie im Abschnitt **[!UICONTROL EINSTELLUNGEN]** den Eintrag **[!UICONTROL Sicherheit].**

1. Klicken Sie auf **[!UICONTROL Remote Site Settings]**.
1. (Bedingt) Wenn Ihre [!DNL Workfront]-URL nicht in der Liste **[!UICONTROL Alle Remote-Sites]** aufgeführt ist, klicken Sie auf **[!UICONTROL Neue Remote-Site]**.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie den **[!UICONTROL Remote Site Name]** an.
Beispiel: *[!DNL Workfront]*.

1. (Bedingt) Wenn Sie die Site hinzufügen, geben Sie die **[!UICONTROL Remote Site URL]** an.
Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die [!DNL Workfront] -App ist jetzt auf Ihrer [!DNL Salesforce] -Instanz installiert und die **[!DNL Workfront]** -Komponente wird jetzt Ihrer Umgebung hinzugefügt.

   Benutzer von [!UICONTROL Salesforce] können die [!DNL Workfront]-App verwenden, sobald Sie den Abschnitt [!DNL Workfront] zu ihren Seitenlayouts [!UICONTROL Opportunity] oder [!UICONTROL Account] hinzugefügt haben.\
   Informationen zum Konfigurieren des Abschnitts [!DNL Workfront] für Benutzer finden Sie unter Abschnitt [Konfigurieren des Abschnitts [!DNL Adobe Workfront] für  [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
