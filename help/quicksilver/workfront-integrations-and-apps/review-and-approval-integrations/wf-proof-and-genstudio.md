---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Erste Schritte mit der Integration von GenStudio for Performance Marketing und Workfront Proof
description: Erste Schritte mit der Integration von GenStudio for Performance Marketing und Workfront Proof
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
TQID: https://experienceleague.adobe.com/1UOceajaDUpiW1jweaaQQ0hXMFIkhKf1sb229irQRZg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 588
ht-degree: 6%

---

# Erste Schritte mit der Integration von GenStudio for Performance Marketing und Workfront Proof

Durch die Integration zwischen GenStudio for Performance Marketing und Workfront Proof können Sie

* Verwenden von Workfront-Korrekturabzugsvorlagen zum Definieren von Prüfungs- und Genehmigungs-Workflows

* Überprüfen und Genehmigen von GenStudio for Performance Marketing-Entwurfsinhalten im Workfront Proofing Viewer

* Anzeigen von Überprüfungsentscheidungen in GenStudio for Performance Marketing zur endgültigen Genehmigung und Veröffentlichung

Weitere Informationen zur Überprüfung und Genehmigung in GenStudio for Performance Marketing finden Sie unter [Integration von Workfront Proof mit GenStudio for Performance Marketing](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/approve/proof-integration).


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> 
   <p>Beliebig</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Standard </p> 
   <p>Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zusätzliche Produkte</td> 
   <td> 
   <p> Sie müssen über GenStudio for Performance Marketing verfügen und dem Produkt müssen Sie als Benutzer in der Admin Console hinzugefügt werden. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Integrationsanforderungen

* Workfront und GenStudio for Performance Marketing müssen in derselben Identity Management System (IMS)-Organisation bereitgestellt werden.

* Benutzende können nur zu einer Workfront-Instanz innerhalb der IMS-Organisation gehören.

* Die Integration muss im Bereich &quot;Workfront-Setup“ aktiviert werden.


## Integration in Workfront aktivieren

Sie müssen Systemadministrator sein, um diese Integration zu aktivieren.

1. Klicken Sie oben links auf **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) und dann auf **[!UICONTROL Setup]** ![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Klicken Sie im linken Bedienfeld auf **Überprüfen und** > **Adobe GenStudio**.
1. Aktivieren **Korrekturabzugsgenehmigungen verwenden**.
   ![Aktivieren des Proofings für die GenStudio-Einstellung](assets/enable-proofing-gs.png)

## Verwenden von Workfront-Korrekturabzugsvorlagen zur Definition von Genehmigungs-Workflows

Wenn der Prozess der Inhaltsüberprüfung in Ihrem Unternehmen häufig wiederholt wird oder von denselben Personen geprüft wird, können Sie Korrekturabzugsvorlagen verwenden, um Prüfungs- und Genehmigungs-Workflows zu automatisieren.

### Erstellen einer Testversandvorlage in Workfront

Sie können einfache, einstufige Vorlagen für nur einen oder zwei Prüfer erstellen oder automatisierte, mehrstufige Vorlagen für komplexe Prüfungen mit vielen Phasen und Abhängigkeiten erstellen.

Weitere Informationen zum Erstellen automatisierter Workflows und Vorlagen in Workfront finden Sie unter

* [Überblick über den automatisierten Workflow](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [Erstellen und Verwalten von automatisierten Workflow-Vorlagen](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

### Auswählen oder Ändern der Vorlage in GenStudio for Performance Marketing

Wenn ein(e) Benutzende(r) eine Überprüfung in GenStudio for Performance Marketing startet, wählt er/sie einfach die gewünschte Vorlage aus. Benutzer können jederzeit problemlos jede Korrekturabzugs-Workflow-Vorlage ändern und Prüfer und Phasen hinzufügen oder entfernen.

Weitere Informationen finden Sie unter [Überprüfung und Genehmigung &#x200B;](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/approve/request-review).

## Überprüfen und Genehmigen von GenStudio for Performance Marketing-Entwurfsinhalten im Workfront Proofing Viewer

Entwurfsinhalte können direkt in GenStudio for Performance Marketing im Workfront Proofing Viewer überprüft und genehmigt werden.

Mit dem Proofing Viewer können Sie

* Kommentare hinterlassen
* Markup-Entwurf, um anzuzeigen, was geändert werden muss
* Entscheidung treffen

Weitere Informationen finden Sie unter [Inhalt überprüfen und bearbeiten](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/approve/review-and-edit).


>[!IMPORTANT]
>
>Benutzer müssen den [Überprüfen interaktiver Inhalte mit dem Adobe Workfront-Überprüfungs-Tool“ installieren](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-proof-in-web-viewer-extension.md) bevor sie Entwürfe in GenStudio for Performance Marketing überprüfen können.


## Anzeigen von Überprüfungsentscheidungen in GenStudio for Performance Marketing zur endgültigen Genehmigung und Veröffentlichung

Sobald das Asset den Prüfungs- und Genehmigungsprozess durchlaufen hat, können Sie die Überprüfungsentscheidung anzeigen und den Inhalt direkt in GenStudio for Performance Marketing veröffentlichen.

Weitere Informationen finden Sie unter [Genehmigte Inhalte veröffentlichen](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/approve/publish-content).
