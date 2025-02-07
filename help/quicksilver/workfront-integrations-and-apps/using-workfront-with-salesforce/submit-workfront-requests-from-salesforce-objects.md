---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Submit [!DNL Adobe Workfront] requests from [!DNL Salesforce] objects
description: Nach der Installation [!DNL Adobe Workfront] für [!DNL Salesforce], you can submit [!DNL Workfront] Anfragen von [!DNL Salesforce] Opportunities und Konten. Diese Funktion ist sowohl im Classic- als auch im Lightning Experience-Framework verfügbar.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 1%

---

# Senden von [!DNL Adobe Workfront]-Anfragen von [!DNL Salesforce]

Nach der Installation von [!DNL Adobe Workfront for Salesforce] können Sie [!DNL Workfront] Anfragen von [!DNL Salesforce] Opportunities und Konten senden. Diese Funktion ist sowohl im [!DNL Classic]- als auch im [!DNL Lightning Experience]-Framework verfügbar.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die in diesem Artikel beschriebenen Funktionen nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] Plan*</p></td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] Lizenz*</p></td> 
   <td> <p>[!UICONTROL-Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Um eine [!DNL Workfront]-Anfrage von einer [!DNL Salesforce] Opportunity oder einem Konto zu senden, stellen Sie sicher, dass Sie Folgendes in Ihrer Umgebung haben:

* Ihr [!DNL Workfront] hat [!DNL Workfront for Salesforce] installiert.\
   Weitere Informationen zum Installieren von [!DNL Workfront for Salesforce] finden Sie unter [Installieren [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Ihr [!DNL Workfront] hat den Abschnitt [!DNL Workfront] zu Ihren Seitenlayouts [!UICONTROL Opportunity] und [!UICONTROL Konto] hinzugefügt.\
   Weitere Informationen zum Hinzufügen des Abschnitts &quot;[!DNL Workfront]&quot; zu einem Seitenlayout finden Sie unter [Konfigurieren  [!DNL Adobe Workfront]  Abschnitts für  [!DNL Salesforce] -](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Sie haben ein [!DNL Workfront] Konto und können sich über den [!DNL Workfront] Abschnitt in Ihrem Opportunity- oder Konto anmelden.\
   Nach der Anmeldung sehen Sie die Registerkarte [!UICONTROL Neue Anfragen] auf der Sie Anfragen eingeben können.

## [!DNL Workfront] Anfragen von [!DNL Salesforce] senden

1. Wechseln Sie zu einer Opportunity oder einem Konto in Salesforce.
1. Navigieren Sie zum Abschnitt [!DNL Workfront] .
1. Wählen **[!UICONTROL auf der Registerkarte]** Neue Anfragen **[!UICONTROL im Dropdown-Menü Anfragetyp auswählen]** einen Anfragetyp aus.

   Es werden dieselben Anforderungswarteschlangen angezeigt, auf die Sie in Workfront Zugriff haben.

1. Füllen Sie die verfügbaren Felder für Ihre Anfrage aus.

   Das Senden einer Anfrage über [!DNL Salesforce] entspricht dem Senden einer Anfrage in der [!DNL Workfront] Web-Anwendung.

   >[!NOTE]
   >
   >Das Hochladen eines Dokuments mit dem [!DNL Workfront]-Plug-in in [!DNL Salesforce] ist vorübergehend nicht verfügbar.

   Fahren Sie mit den unter &quot;[ und Senden [!DNL Adobe Workfront] Anfragen“ beschriebenen ](../../manage-work/requests/create-requests/create-submit-requests.md) fort.

1. Klicken Sie **[!UICONTROL Senden]**.

## [!DNL Workfront] anzeigen

1. Zu einer Opportunity oder einem Konto in [!DNL Salesforce] gehen.
1. Navigieren Sie zum Abschnitt **[!DNL Workfront]** .

   >[!NOTE]
   >
   >Je nachdem, wie Ihr [!DNL Workfront] diesen Abschnitt konfiguriert hat, kann er einen anderen Namen haben.

1. Wählen Sie die **[!UICONTROL Gesendete Anfragen]** aus.

   Sie können alle Anfragen, die Sie oder andere von dieser Opportunity oder diesem Konto gesendet haben, auf dieser Registerkarte anzeigen. Anfragen, die an diese Anfrage-Warteschlange in der Web-Anwendung gesendet wurden, werden in dieser Liste nicht in [!DNL Salesforce] angezeigt.

   >[!NOTE]
   >
   >Anfragen, die an diese Anforderungswarteschlange in der Web-Anwendung gesendet werden, werden in dieser Liste in Salesforce nicht angezeigt.

   ![Salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Sie können die folgenden Informationen zu den gesendeten Anfragen anzeigen:

   * Name der Anfrage (in der Spalte [!UICONTROL Betreff])
   * Referenznummer
   * Anfragetyp
   * Status
   * Gesendet am
   * Angefordert von Name
   * Name zugewiesen\

     Wenn diese Informationen in [!DNL Workfront] aktualisiert werden, werden sie auch in dieser Liste aktualisiert.

1. (Optional) Klicken Sie auf den Namen der Anfrage, um sie in [!DNL Workfront] zu öffnen.

1. (Optional) Klicken Sie auf **[!UICONTROL Wechseln zu[!DNL Salesforce]]**, um auf die Opportunity oder das Konto zuzugreifen, bei dem das Problem aus den folgenden Bereichen von Workfront stammt:

   * Im [!UICONTROL Details] des Problems
   * Wenn Sie das Problem in einer Liste im Bedienfeld Zusammenfassung auswählen, nachdem Sie in der Symbolleiste der Liste auf [!UICONTROL Zusammenfassung öffnen] ![Symbol ](assets/summary-panel-icon.png)Zusammenfassungsbereich“ geklickt haben.
   * In der Problem-Kopfzeile, wenn das Feld [!UICONTROL Integrationen] verfügbar ist. Ihr System- oder Gruppenadministrator muss das Feld [!UICONTROL Integrationen] zu Ihrer Layoutvorlage hinzufügen, um den Link Wechseln zu Salesforce in der Anfragekopfzeile anzuzeigen. Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >Der [!UICONTROL Wechseln zu Salesforce]-Link ist für alle [!DNL Workfront] Benutzer sichtbar, die das Problem anzeigen können. Sie müssen über ein [!DNL Salesforce]-Konto verfügen, um zu dem Opportunity-Konto oder [!DNL Salesforce]-Konto gehen zu können, in dem das Problem protokolliert wurde.
