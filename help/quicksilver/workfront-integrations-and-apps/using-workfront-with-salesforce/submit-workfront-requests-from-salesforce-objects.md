---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Einsenden [!DNL Adobe Workfront] Anforderungen von [!DNL Salesforce] Objekte
description: Nach der Installation [!DNL Adobe Workfront] für [!DNL Salesforce], you can submit [!DNL Workfront] Anforderungen von [!DNL Salesforce] Möglichkeiten und Konten. Diese Funktion ist sowohl in den klassischen als auch in den Blitzererlebnis-Frameworks verfügbar.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# Einsenden [!DNL Adobe Workfront] Anforderungen von [!DNL Salesforce] Objekte

Nach der Installation [!DNL Adobe Workfront for Salesforce], können Sie [!DNL Workfront] Anforderungen von [!DNL Salesforce] Möglichkeiten und Konten. Diese Funktion ist in beiden [!DNL Classic] und [!DNL Lightning Experience] Frameworks.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] Plan*</p></td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] license*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

So senden Sie eine [!DNL Workfront] Anfrage von [!DNL Salesforce] Chancen oder Konto stellen sicher, dass Sie Folgendes in Ihrer Umgebung haben:

* Ihre [!DNL Workfront] Der Administrator hat [!DNL Workfront for Salesforce].\
   Weitere Informationen zur Installation [!DNL Workfront for Salesforce], siehe [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Ihre [!DNL Workfront] -Administrator hat [!DNL Workfront] zu Ihrer [!UICONTROL Chancen] und [!UICONTROL Konto] Seitenlayouts.\
   Weitere Informationen zum Hinzufügen des [!DNL Workfront] Abschnitt zu einem Seitenlayout hinzufügen, siehe [Konfigurieren Sie die [!DNL Adobe Workfront] Abschnitt für [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Sie haben eine [!DNL Workfront] und Sie können sich über das [!DNL Workfront] in Ihrer Opportunity oder Ihrem Konto.\
   Nach der Anmeldung können Sie die [!UICONTROL Neue Anforderungen] Registerkarte, auf der Sie mit der Eingabe von Anforderungen beginnen können.

## Einsenden [!DNL Workfront] Anforderungen von [!DNL Salesforce]

1. Gehen Sie zu einer Gelegenheit oder einem Konto in Salesforce.
1. Navigieren Sie zu [!DNL Workfront] Abschnitt.
1. Im **[!UICONTROL Neue Anforderungen]** wählen Sie einen Anfragetyp im **[!UICONTROL Anfragetyp auswählen]** Dropdown-Menü.

   Es werden dieselben Anforderungswarteschlangen angezeigt, auf die Sie Zugriff haben, um sie in Workfront anzuzeigen.

1. Füllen Sie zunächst die für Ihre Anfrage verfügbaren Felder aus.

   Senden einer Anfrage von [!DNL Salesforce] entspricht dem Senden einer Anforderung im [!DNL Workfront] Webanwendung.

   >[!NOTE]
   >
   >Hochladen eines Dokuments mit dem [!DNL Workfront] Plugin [!DNL Salesforce] ist vorübergehend nicht verfügbar.

   Befolgen Sie weiterhin die Schritte unter [Erstellen und Senden [!DNL Adobe Workfront] requests](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Klicken **[!UICONTROL Einsenden]**.

## Ansicht [!DNL Workfront] requests

1. Gehen Sie zu einer Gelegenheit oder einem Konto in [!DNL Salesforce].
1. Navigieren Sie zu **[!DNL Workfront]** Abschnitt.

   >[!NOTE]
   >
   >Je nachdem, wie Ihre [!DNL Workfront] Administrator diesen Abschnitt konfiguriert haben, kann es einen anderen Namen haben.

1. Wählen Sie die **[!UICONTROL Gesendete Anfragen]** Registerkarte.

   Auf dieser Registerkarte können Sie alle Anfragen anzeigen, die Sie oder andere über diese Gelegenheit oder dieses Konto gesendet haben. Anforderungen, die an diese Anforderungswarteschlange in der Webanwendung gesendet werden, werden nicht in dieser Liste in [!DNL Salesforce].

   >[!NOTE]
   >
   >Anforderungen, die in der Webanwendung an diese Anforderungswarteschlange gesendet werden, werden nicht in dieser Liste in Salesforce angezeigt.

   ![salesforce_sent_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Sie können die folgenden Informationen zu den gesendeten Anfragen anzeigen:

   * Anforderungsname (in der [!UICONTROL Betreff] column)
   * Referenznummer
   * Anfragetyp
   * Status
   * Gesendet am Datum
   * Angefordert nach Name
   * Zugeordneter Name\

      Wenn diese Informationen aktualisiert werden in [!DNL Workfront], wird sie auch in dieser Liste aktualisiert.

1. (Optional) Klicken Sie auf den Namen der Anforderung, um sie in [!DNL Workfront].

1. (Optional) Klicken Sie auf **[!UICONTROL Navigieren Sie zu[!DNL Salesforce]]** , um auf die Möglichkeit oder das Konto zuzugreifen, bei der das Problem aus den folgenden Bereichen von Workfront stammt:

   * Im [!UICONTROL Details] Abschnitt des Problems
   * Wenn Sie das Problem in einer Liste auswählen, klicken Sie im Bereich &quot;Zusammenfassung&quot;auf [!UICONTROL Zusammenfassung öffnen] ![](assets/summary-panel-icon.png) in der Symbolleiste der Liste.
   * Wenn in der Kopfzeile des Problems die Variable [!UICONTROL Integrationen] -Feld verfügbar ist. Ihr System- oder Gruppenadministrator muss [!UICONTROL Integrationen] in Ihre Layout-Vorlage ein, um den Link Gehe zu Salesforce in der Problemüberschrift anzuzeigen. Weitere Informationen finden Sie unter [Objektüberschriften mithilfe einer Layoutvorlage anpassen](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >Die [!UICONTROL Gehe zu Salesforce] Link für alle sichtbar [!DNL Workfront] Benutzer, die das Problem anzeigen können. Sie müssen über eine [!DNL Salesforce] -Konto, um zur [!DNL Salesforce] Gelegenheit oder Konto, bei dem das Problem protokolliert wurde.
