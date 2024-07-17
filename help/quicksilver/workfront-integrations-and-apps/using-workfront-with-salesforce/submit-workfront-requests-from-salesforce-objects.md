---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Senden [!DNL Adobe Workfront] von Anforderungen von  [!DNL Salesforce] Objekten
description: Nach der Installation von [!DNL Adobe Workfront] für [!DNL Salesforce], you can submit [!DNL Workfront] Anforderungen von [!DNL Salesforce] Opportunities and Accounts. Diese Funktion ist sowohl in den klassischen als auch in den Blitzererlebnis-Frameworks verfügbar.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 1%

---

# Senden von [!DNL Adobe Workfront] -Anforderungen von [!DNL Salesforce] -Objekten

Nach der Installation von [!DNL Adobe Workfront for Salesforce] können Sie [!DNL Workfront] -Anfragen von [!DNL Salesforce] Opportunities and Accounts senden. Diese Funktion ist sowohl in den [!DNL Classic]- als auch in den [!DNL Lightning Experience]-Frameworks vorhanden.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel beschriebene Funktion verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plan*</p></td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] license*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Um eine [!DNL Workfront] -Anfrage von einer [!DNL Salesforce] -Gelegenheit oder einem Konto zu senden, stellen Sie sicher, dass Sie Folgendes in Ihrer Umgebung haben:

* Ihr [!DNL Workfront] -Administrator hat [!DNL Workfront for Salesforce] installiert.\
   Weitere Informationen zum Installieren von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md) .

* Ihr [!DNL Workfront] -Administrator hat den Abschnitt [!DNL Workfront] zu Ihren Seitenlayouts für [!UICONTROL Chancen] und [!UICONTROL Konto] hinzugefügt.\
   Weitere Informationen zum Hinzufügen des Abschnitts [!DNL Workfront] zu einem Seitenlayout finden Sie unter [Konfigurieren des Abschnitts [!DNL Adobe Workfront] für  [!DNL Salesforce] Benutzer](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Sie haben ein [!DNL Workfront] -Konto und können sich über den Abschnitt [!DNL Workfront] in Ihrer Opportunity oder Ihrem Konto bei ihm anmelden.\
   Nach der Anmeldung können Sie die Registerkarte [!UICONTROL Neue Anforderungen] sehen, auf der Sie mit der Eingabe von Anforderungen beginnen können.

## Senden von [!DNL Workfront] -Anforderungen von [!DNL Salesforce]

1. Gehen Sie zu einer Gelegenheit oder einem Konto in Salesforce.
1. Wechseln Sie zum Abschnitt &quot;[!DNL Workfront]&quot;.
1. Wählen Sie auf der Registerkarte **[!UICONTROL Neue Anforderungen]** im Dropdown-Menü **[!UICONTROL Anfragetyp auswählen]** einen Anfragetyp aus.

   Es werden dieselben Anforderungswarteschlangen angezeigt, auf die Sie Zugriff haben, um sie in Workfront anzuzeigen.

1. Füllen Sie zunächst die für Ihre Anfrage verfügbaren Felder aus.

   Die Übermittlung einer Anforderung von [!DNL Salesforce] entspricht der Übermittlung einer Anforderung in der [!DNL Workfront]-Webanwendung.

   >[!NOTE]
   >
   >Das Hochladen eines Dokuments mit dem Plug-in [!DNL Workfront] in [!DNL Salesforce] ist vorübergehend nicht verfügbar.

   Führen Sie weiterhin die unter [Erstellen und Senden [!DNL Adobe Workfront] von Anforderungen](../../manage-work/requests/create-requests/create-submit-requests.md) beschriebenen Schritte aus.

1. Klicken Sie auf **[!UICONTROL Senden]**.

## Anzeigen von [!DNL Workfront]-Anforderungen

1. Wechseln Sie in [!DNL Salesforce] zu einer Chance oder einem Konto.
1. Wechseln Sie zum Abschnitt &quot;**[!DNL Workfront]**&quot;.

   >[!NOTE]
   >
   >Je nachdem, wie Ihr [!DNL Workfront] -Administrator diesen Abschnitt konfiguriert hat, kann er einen anderen Namen haben.

1. Wählen Sie die Registerkarte **[!UICONTROL Gesendete Anforderungen]** aus.

   Sie können alle Anfragen anzeigen, die Sie oder andere über diese Gelegenheit oder dieses Konto gesendet haben. Anforderungen, die an diese Anforderungswarteschlange in der Webanwendung gesendet werden, werden nicht in dieser Liste in [!DNL Salesforce] angezeigt.

   >[!NOTE]
   >
   >Anforderungen, die in der Webanwendung an diese Anforderungswarteschlange gesendet werden, werden nicht in dieser Liste in Salesforce angezeigt.

   ![salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Sie können die folgenden Informationen zu den gesendeten Anfragen anzeigen:

   * Anforderungsname (in der Spalte [!UICONTROL Betreff] )
   * Referenznummer
   * Anfragetyp
   * Status
   * Gesendet am Datum
   * Angefordert nach Name
   * Zugeordneter Name\

     Wenn diese Informationen in [!DNL Workfront] aktualisiert werden, werden sie auch in dieser Liste aktualisiert.

1. (Optional) Klicken Sie auf den Namen der Anforderung, um sie in [!DNL Workfront] zu öffnen.

1. (Optional) Klicken Sie auf **[!UICONTROL Gehe zu[!DNL Salesforce]]** , um auf die Gelegenheit oder das Konto zuzugreifen, von der aus das Problem aus den folgenden Bereichen von Workfront stammt:

   * Im Abschnitt [!UICONTROL Details] des Problems
   * Wenn Sie das Problem in einer Liste auswählen, klicken Sie im Bedienfeld &quot;Zusammenfassung&quot;auf [!UICONTROL Zusammenfassung öffnen] ![](assets/summary-panel-icon.png) in der Symbolleiste der Liste.
   * In der Kopfzeile des Problems, wenn das Feld [!UICONTROL Integrationen] verfügbar ist. Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layout-Vorlage hinzufügen, um den Link Gehe zu Salesforce in der Kopfzeile des Problems anzuzeigen. Weitere Informationen finden Sie unter [Anpassen von Objektüberschriften mithilfe einer Layoutvorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >Der Link [!UICONTROL Gehe zu Salesforce] ist für alle [!DNL Workfront] Benutzer sichtbar, die das Problem anzeigen können. Sie müssen über ein [!DNL Salesforce] -Konto verfügen, um zur [!DNL Salesforce] Gelegenheit oder zum Konto wechseln zu können, bei der das Problem protokolliert wurde.
