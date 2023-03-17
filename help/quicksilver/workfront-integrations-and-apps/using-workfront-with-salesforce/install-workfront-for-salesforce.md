---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Installieren [!DNL Adobe Workfront] für [!DNL Salesforce]
description: So installieren Sie die App, bevor sie im [!DNL Salesforce] AppExchange, siehe Installieren [!DNL Workfront] für Salesforce , bevor es im AppExchange Marketplace verfügbar wird.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4fea9d8f-7729-4fee-86d3-1a986be29f74
source-git-commit: 254ffae14b21dbef19b8f6b66a1c11e348c85c85
workflow-type: tm+mt
source-wordcount: '878'
ht-degree: 1%

---

# Installieren [!DNL Adobe Workfront for Salesforce]

So installieren Sie die App, bevor sie im [!DNL Salesforce AppExchange], siehe [Installieren [!DNL Workfront for Salesforce] bevor sie im [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace).

Als [!DNL Salesforce] und [!DNL Adobe Workfront] Administrator, können Sie [!DNL Workfront for Salesforce] , um [!DNL Salesforce] Benutzer zum Senden [!DNL Workfront] -Anfragen und automatisch Projekte erstellen, ohne Salesforce verlassen zu müssen.

Für allgemeine Informationen zu den Erwartungen durch die Installation von [!DNL Workfront for Salesforce], siehe [[!DNL Adobe Workfront for Salesforce] Übersicht](../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce-overview.md).

* [Voraussetzungen für die Installation und Verwendung [!DNL Workfront for Salesforce]](#prerequisites-for-installing-and-using-workfront-for-salesforce-prerequisites-for-installing-and-using-workfront-for-salesforce)
* [Installieren [!DNL Workfront for Salesforce]](#install-adobe-workfront-for-salesforce)

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr>  </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen für die Installation und Verwendung [!DNL Workfront for Salesforce] {#prerequisites-for-installing-and-using-workfront-for-salesforce}

* Sie müssen über eine [!DNL Salesforce] -Instanz mit Zugriff auf ein Systemadministratorkonto, um die App zu installieren.
* Sie müssen über eine [!DNL Workfront] -Instanz mit Zugriff auf ein Systemadministratorkonto, um die Integration zu konfigurieren.
* [!UICONTROL Salesforce] -Benutzer müssen über eine [!DNL Workfront] , um

   * Erstellen [!DNL Workfront] Anforderungen von [!DNL Salesforce] oder
   * Ansicht [!DNL Workfront] Anfragen oder Projekte in Salesforce.

## Installieren [!DNL Workfrontfor Salesforce] {#installing-workfront-for-salesforce}

Sie müssen [!DNL Salesforce] und [!DNL Workfront] Systemadministrator zum Installieren und Konfigurieren [!DNL Workfront for Salesforce].

In den folgenden Unterabschnitten wird beschrieben, wie Sie die Installation [!DNL Workfront] für Ihre [!DNL Salesforce] Produktionsumgebung. Sie können dieselben Schritte zur Installation ausführen [!DNL Workfront] für Ihre [!DNL Salesforce] Sandbox-Umgebung.

* [Installieren [!DNL Workfront for Salesforce] bevor sie im [!DNL AppExchange] Marketplace](#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace-installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace)
* [Installieren [!DNL Workfront for Salesforce] im [!DNL Salesforce Classic] Framework](#installing-workfront-for-salesforce-in-the-salesforce-classic-framework)
* [Installieren [!DNL Workfront for Salesforce] im [!DNL Salesforce Lightning Experience] Framework](#installing-workfront-for-salesforce-in-the-salesforce-lightning-experience-framework)

### Installieren [!DNL Workfront for Salesforce] bevor sie im [!DNL AppExchange] Marketplace {#installing-workfront-for-salesforce-before-it-becomes-available-in-the-appexchange-marketplace}

[!DNL Workfront for Salesforce] wird im [!DNL Salesforce AppExchange] bald.

So installieren Sie die App, bevor sie verfügbar ist:

1. Navigieren Sie in Ihrer Produktionsumgebung zu

   `https://login.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002eRjb`

   Navigieren Sie in Ihrer Sandbox-Umgebung zu

   `https://test.salesforce.com/packaging/installPackage.apexp?p0=04t4K000002eRjb`

1. Überprüfen Sie die **[!UICONTROL Ja, Zugriff auf diese Drittanbieter-Websites gewähren]** ankreuzen.

   Ein Ladebildschirm wird angezeigt und die Installation kann einige Zeit in Anspruch nehmen.

1. Klicken **[!UICONTROL Fertig]** wenn die Installation abgeschlossen ist.

1. Navigieren Sie zu **[!UICONTROL Setup > Sicherheitskontrollen > Remote Site Settings]**.
1. (Bedingt) Wenn Sie Ihre [!DNL Workfront] Die in der **[!UICONTROL Alle Remote-Sites]** Liste, klicken Sie auf **[!UICONTROL Neue Remote-Site]**.

1. Geben Sie die **[!UICONTROL Remote Site Name]**.

   Beispiel, *[!DNL Workfront]*.

1. Geben Sie die **[!UICONTROL Remote Site URL]**.

   Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die [!DNL Workfront] Die App ist jetzt auf Ihrem [!DNL Salesforce] und **[!UICONTROL WorkfrontOpportunities]** und **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualkraft] In Ihrer Umgebung wurden Seiten erstellt.

   [!DNL Salesforce] -Benutzer können die App verwenden, sobald Sie die [!DNL Workfront] -Abschnitt [!UICONTROL Chancen] oder [!UICONTROL Konto] Seitenlayouts.\
   Informationen zum Konfigurieren des Workfront-Abschnitts für Benutzer finden Sie unter [Konfigurieren des Adobe Workfront-Abschnitts für Salesforce-Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installieren [!DNL Workfront] für [!DNL Salesforce] im [!DNL Salesforce Classic] Framework

1. Anmelden bei [!DNL Salesforce] als Systemadministrator.
1. Navigieren Sie zu **Einrichtung.**
1. Im **Build** Abschnitt, klicken Sie auf **AppExchange Marketplace**.

1. Im **AppExchange Apps durchsuchen** Feld, Typ **Workfront**.

1. Klicken Sie auf die App, sobald Sie sie gefunden haben, und klicken Sie dann auf **Jetzt downloaden**.
1. Klicken **[!UICONTROL Installation in Produktion]** , um [!DNL Workfront] App in Ihrer [!DNL Salesforce] Produktionsumgebung. (empfohlen)
1. Wählen Sie die **[!UICONTROL Ich habe die Nutzungsbedingungen gelesen und stimme ihnen zu.]** -Feld, nachdem Sie die Nutzungsbedingungen gelesen und akzeptiert haben.
1. Klicken **[!UICONTROL Bestätigen und installieren]**.
1. Auswählen **[!UICONTROL Für alle Benutzer installieren]** (empfohlen) und klicken Sie dann auf **[!UICONTROL Installieren]**.

1. (Bedingt) Wenn Sie gefragt werden, ob Sie den Zugriff eines Drittanbieters genehmigen möchten, müssen Sie **[!UICONTROL Ja, Zugriff auf diese Drittanbieter-Websites gewähren]** Klicken Sie auf **[!UICONTROL Weiter]**.

1. Klicken **[!UICONTROL Fertig]** wenn die Installation abgeschlossen ist.

   Die [!DNL Workfront] App ist unter aufgeführt **[!UICONTROL Installierte Pakete]**.


1. Navigieren Sie zu **[!UICONTROL Setup > Sicherheitskontrollen > Remote Site Settings]**.
1. (Bedingt) Wenn Sie Ihre [!DNL Workfront] Die in der **[!UICONTROL Alle Remote-Sites]** Liste, klicken Sie auf **[!UICONTROL Neue Remote-Site]**.\

1. Geben Sie die **[!UICONTROL Remote Site Name]**.\
   Beispiel, *[!DNL Workfront]*.

1. Geben Sie die **[!UICONTROL Remote Site URL]**.\
   Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.\
   Die [!DNL Workfront] Die App ist jetzt auf Ihrem [!DNL Salesforce] und **[!UICONTROL WorkfrontOpportunities]** und **[!UICONTROL WorkfrontAccounts]** [!UICONTROL Visualkraft] In Ihrer Umgebung wurden Seiten erstellt.\
   [!DNL Salesforce] -Benutzer können die App noch nicht verwenden, bis Sie die [!DNL Workfront] -Abschnitt [!UICONTROL Chancen] oder [!UICONTROL Konto] Seitenlayouts.\
   Informationen zum Konfigurieren der [!DNL Workfront] Abschnitt für Benutzer finden Sie unter [Konfigurieren Sie die [!DNL Adobe Workfront] Abschnitt für [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

### Installieren [!DNL Workfront for Salesforce] im [!DNL Salesforce Lightning Experience] Framework

1. Anmelden bei [!DNL Salesforce] als Systemadministrator.
1. Klicken Sie auf **[!UICONTROL Einrichtung] icon** Klicken Sie auf **[!UICONTROL Einrichtung]**.

1. Im **[!UICONTROL PLATTFORMWERKZEUGE]** Abschnitt erweitern **[!UICONTROL Apps].**

1. Klicken **[!DNL AppExchange Marketplace]**.
1. Im **[!UICONTROL Suche [!DNL AppExchange] Apps]** Feld, Typ **[!DNL Workfront]**.

1. Klicken Sie auf die App, sobald Sie sie gefunden haben, und klicken Sie dann auf **[!UICONTROL Jetzt downloaden]**.
1. Klicken **[!UICONTROL Anmeldebildschirm öffnen]**.\
   Sie müssen sich mit Ihrem [!DNL Workfront] Administratorkonto für [!DNL Salesforce].

1. Klicken **[!UICONTROL Zulassen]**.
1. Im **[!UICONTROL In dieser Organisation installieren]** Feld, klicken Sie auf **[!UICONTROL Installieren hier]** installieren [!DNL Workfront] in [!DNL Salesforce] Produktionsumgebung. (empfohlen)

1. Wählen Sie die **[!UICONTROL Ich habe die Nutzungsbedingungen gelesen und stimme ihnen zu.]** -Feld, nachdem Sie die Nutzungsbedingungen gelesen und akzeptiert haben.
1. Klicken **[!UICONTROL Bestätigen und installieren]**.
1. Auswählen **[!UICONTROL Für alle Benutzer installieren]** (empfohlen) und klicken Sie dann auf **[!UICONTROL Installieren]**.

1. (Bedingt) Wenn Sie gefragt werden, ob Sie den Zugriff eines Drittanbieters genehmigen möchten, müssen Sie **[!UICONTROL Ja, Zugriff auf diese Drittanbieter-Websites gewähren]** Klicken Sie auf **[!UICONTROL Weiter]**.

1. Klicken **[!UICONTROL Fertig]** wenn die Installation abgeschlossen ist.

   Die [!DNL Workfront] App ist unter aufgeführt **[!UICONTROL Installierte Pakete]**.

1. Navigieren Sie zu **[!UICONTROL Einrichtung].**
1. Im **[!UICONTROL EINSTELLUNGEN]** Abschnitt erweitern &#x200B;**[!UICONTROL Sicherheit].**

1. Klicken **[!UICONTROL Remote Site Settings]**.
1. (Bedingt) Wenn Sie Ihre [!DNL Workfront] Die in der **[!UICONTROL Alle Remote-Sites]** Liste, klicken Sie auf **[!UICONTROL Neue Remote-Site]**.

1. Geben Sie die **[!UICONTROL Remote Site Name]**.

   Beispiel, *[!DNL Workfront]*.

1. Geben Sie die **[!UICONTROL Remote Site URL]**.

   Beispiel: *yourDomain.my.workfront.com*.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Die [!DNL Workfront] Die App ist jetzt auf Ihrem [!DNL Salesforce] und die **[!DNL Workfront]** -Komponente wird nun zu Ihrer Umgebung hinzugefügt.

   [!UICONTROL Salesforce] -Benutzer können [!DNL Workfront] App nach dem Hinzufügen [!DNL Workfront] -Abschnitt [!UICONTROL Chancen] oder [!UICONTROL Konto] Seitenlayouts.\
   Informationen zum Konfigurieren der [!DNL Workfront] Abschnitt für Benutzer finden Sie unter [Konfigurieren Sie die [!DNL Adobe Workfront] Abschnitt für [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).
