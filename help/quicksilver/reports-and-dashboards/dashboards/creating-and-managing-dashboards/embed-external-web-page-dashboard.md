---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Einbetten einer externen Webseite in ein Dashboard
description: Sie können eine externe Webseite in ein Dashboard einbetten, um Zugriff auf zugehörige Informationen von anderen Systemen in Adobe Workfront oder anderen Workfront-Seiten zu ermöglichen.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Einbetten einer externen Webseite in ein Dashboard

Sie können eine externe Webseite in ein Dashboard einbetten, um Zugriff auf zugehörige Informationen von anderen Systemen in Adobe Workfront oder anderen Workfront-Seiten zu ermöglichen.

Wenn Ihr Unternehmen beispielsweise über ein webbasiertes Dokument-Repository, ein Wiki oder ein anderes Content Management-System verfügt, das Projektinformationen enthält, auf die regelmäßig über eine URL zugegriffen wird, können Sie diese Informationen in Workfront anzeigen, indem Sie eine externe Seite in einem Dashboard erstellen.

>[!IMPORTANT]
>
>Aus Sicherheitsgründen ist es auf einigen Websites nicht möglich, Webseiten als iframe einzubetten. Wenn die Webseite, die Sie in ein Dashboard einbetten möchten, dies nicht zulässt, wird die Seite nicht im Dashboard angezeigt. Sie können jedoch weiterhin auf die externe Seite zugreifen, indem Sie auf den Namen des Dashboards klicken.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Wenden Sie sich an Ihren Webadministrator, um die Einbettung für eine Website zu ermöglichen, deren Inhaber Sie sind. **X-Frame-Options** -Einstellung. Weitere Informationen finden Sie unter [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für das Dashboard verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen ein Dashboard erstellen, bevor Sie eine externe Seite darin einbetten können.

Informationen zum Erstellen von Dashboards finden Sie unter [Dashboard erstellen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Externe Seite in ein Dashboard einbetten

>[!IMPORTANT]
>
>Sie können eine externe Seite aus einem Dashboard entfernen, wenn sie nicht mehr benötigt wird. Eine externe Seite kann jedoch nicht gelöscht werden, nachdem sie in Workfront erstellt wurde. Sie können eine externe Seite nur mithilfe der API löschen. Weitere Informationen finden Sie unter [Externe Seite aus einem Dashboard entfernen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).

1. Suchen Sie die URL der Seite, die in Workfront angezeigt werden soll, und kopieren Sie die URL in die Adressleiste.

   >[!NOTE]
   >
   >Wenn Sie URLs für Workfront-Objekte freigeben, denken Sie daran, dass einige URLs im Laufe der Zeit ablaufen. Beispielsweise laufen Dokument-URLs nach dem Öffnen ab. Dies wird als Sicherheitsmaßnahme konfiguriert und sie werden standardmäßig als nicht statische URLs betrachtet und sollten nicht freigegeben werden.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png)Klicken Sie auf **Dashboards**.

1. Um ein vorhandenes Dashboard zu bearbeiten, wählen Sie das Dashboard aus, in das Sie die Website-Seite einbetten möchten, und klicken Sie dann auf **Dashboard-Aktionen** und wählen Sie **Bearbeiten** aus dem Menü.\
   Oder\
   Um ein neues Dashboard zu erstellen, klicken Sie auf **Neues Dashboard**.\
   Weitere Informationen zum Erstellen eines Dashboards finden Sie unter [Dashboard erstellen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Klicken **Externe Seite hinzufügen**.

   ![](assets/qs-add-external-page-350x239.png)

1. Geben Sie eine **Name** für die externe Seite.
1. Geben Sie eine **Beschreibung**.
1. Fügen Sie die zuvor kopierte URL in die **URL** -Feld.\
   Sie können die folgenden URL-Typen angeben:

   * Eine (verschlüsselte) HTTPS-URL zu einer Webseite.\
      Nur HTTPS-Seiten (verschlüsselt) werden mit der URL geladen.\
      ![](assets/add-external-page-dialog-qs-350x247.png)

   * Eine Vorlagen-URL, die Sitzungsinformationen für eine bestimmte Website enthält.\
      Beispiel: *https://localhost/?session={!$$SESSION}*
Sie müssen bei der angegebenen Website angemeldet sein, um die externe Seite anzuzeigen.\
      Informationen zum Abrufen einer SessionID von Workfront finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md).\
      Ihr Workfront-Administrator kann Ihre Systemvoreinstellungen so konfigurieren, dass die Verwendung von Sitzungsinformationen auf Ihren externen Seiten aus Sicherheitsgründen nicht zulässig ist. In diesem Fall wird die externe Seite nicht im Dashboard geladen.\
      Weitere Informationen zu den Systemsicherheitseinstellungen finden Sie unter [Systemsicherheitsvoreinstellungen konfigurieren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
      ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

1. Klicken Sie auf **Speichern**.\
   Die Seite wird automatisch zum Dashboard hinzugefügt. Wenn zukünftige Dashboards erstellt werden, kann die externe Seite hinzugefügt werden. Die externe Seite wird unter den verfügbaren Berichten aufgeführt.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Alina: *** This is linked to: Creating Dashboards, and Editing Dashboards.)
   </MadCap:conditionalText>
   -->

## Externe Seite in einem Dashboard aktualisieren

So aktualisieren Sie die Informationen für eine in einem Dashboard verwendete externe Seite:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png)Klicken Sie auf **Dashboards**.
1. Wählen Sie das Dashboard aus, das Sie aktualisieren möchten, und klicken Sie auf **Bearbeiten** ![](assets/edit-icon.png).

   ![Wählen Sie das Symbol Bearbeiten aus.](assets/nwe-editdashboard2021-350x188.png)

1. Suchen Sie rechts im Bildschirm die zu aktualisierende externe Seite und klicken Sie auf die Schaltfläche **Bearbeiten** Symbol.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. Im **Externe Seite bearbeiten** Dialogfeld, aktualisieren Sie die zu ändernden Felder und klicken Sie auf **Speichern**.
1. (Optional) Klicken Sie auf die **Löschen** icon ![](assets/delete.png) , um die externe Seite aus dem Dashboard zu entfernen. Weitere Informationen finden Sie unter [Externe Seite aus einem Dashboard entfernen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Klicken Sie unten links auf **Speichern und schließen**.

## Anzeigen externer Seiten in einem Bericht

Sie können alle externen Seiten in Workfront in einem Bericht &quot;Externe Seite&quot;anzeigen.

1. Navigieren Sie zu **Hauptmenü** icon ![](assets/main-menu-icon.png) > **Berichte**.
1. Klicken **Neuer Bericht** > Auswählen **Externe Seite**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Optional) Aktualisieren Sie die Registerkarten Ansicht, Filter oder Gruppierungen des Berichts.

   Weitere Informationen finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klicken **Speichern+Schließen**.

   Sie können den Namen und die URL, die mit den externen Seiten in Ihrem System verknüpft sind, im neuen Bericht anzeigen.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
