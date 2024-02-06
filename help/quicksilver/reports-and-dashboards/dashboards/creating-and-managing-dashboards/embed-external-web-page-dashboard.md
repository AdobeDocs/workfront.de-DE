---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Einbetten einer externen Webseite in ein Dashboard
description: Sie können eine externe Webseite in ein Dashboard einbetten, um Zugriff auf zugehörige Informationen von anderen Systemen in Adobe Workfront oder anderen Workfront-Seiten zu ermöglichen.
author: Nolan
feature: Reports and Dashboards
exl-id: 04b623b5-38b0-4c32-b54e-204f1d422e45
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 0%

---

# Einbetten einer externen Webseite in ein Dashboard

<!--Audited: 01/2024-->

Sie können eine externe Webseite in ein Dashboard einbetten, um Zugriff auf zugehörige Informationen aus anderen Systemen oder aus Adobe Workfront zu ermöglichen.

Wenn Ihr Unternehmen beispielsweise über ein webbasiertes Dokument-Repository, ein Wiki oder ein anderes Content Management-System verfügt, das Projektinformationen enthält, auf die regelmäßig über eine URL zugegriffen wird, können Sie diese Informationen in Workfront anzeigen, indem Sie eine externe Seite in einem Dashboard erstellen.

>[!IMPORTANT]
>
>* Aus Sicherheitsgründen ist es auf einigen Websites nicht möglich, Webseiten als iframe einzubetten. Wenn die Webseite, die Sie in ein Dashboard einbetten möchten, dies nicht zulässt, wird die Seite nicht im Dashboard angezeigt. Sie können jedoch weiterhin auf die externe Seite zugreifen, indem Sie auf den Namen des Dashboards klicken.\
>![](assets/qs-empty-external-page-report-350x165.png)\
>Wenden Sie sich an Ihren Webadministrator, um die Einbettung für eine Website zu ermöglichen, deren Inhaber Sie sind. **X-Frame-Options** -Einstellung. Weitere Informationen finden Sie unter [X-Frame-Options](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/X-Frame-Options).
>
>
>* Dashboard-Seiten werden nicht mehr als eingebettete externe Seiten in Dashboards unterstützt. Vorhandene Dashboards werden zwar nicht automatisch geändert, um diese externen Seiten zu entfernen, doch können Änderungen an einem Dashboard, das einen solchen Verweis enthält, erst gespeichert werden, wenn der Verweis entfernt oder geändert wurde.
> Insbesondere werden die folgenden Workfront.com Subdomains nicht mehr unterstützt:
>
>     * /dashboards &#x200B;
>     * /dashboard/:ID-&#x200B;
>     * /portfolio/:ID/content-dashboard__:dashboardID &#x200B;
>     * /program/:ID/content-dashboard__:dashboardID &#x200B;
>     * /project/:ID/content-dashboard__:dashboardID &#x200B;
>     * /task/:ID/content-dashboard__:dashboardID &#x200B;
>     * /template/:ID/content-dashboard__:dashboardID &#x200B;
>     * /templatetask/:ID/content-dashboard__:dashboardID &#x200B;
>     * /resourceManagement/:ID/
>     * content-dashboard__:dashboardID &#x200B;
>     * /team/:ID/content-dashboard__:dashboardID &#x200B;
>     * /iteration/:ID/content-dashboard__:dashboardID &#x200B;
>     * /requests/:ID/content-dashboard__:dashboardID &#x200B;
>     * /group/:ID/content-dashboard__:dashboardID &#x200B;
>     * /billingrecord/:ID/content-dashboard__:dashboardID
>
>Alternativ können Sie auch einen Listenbericht in Ihr Dashboard einfügen, wie hier beschrieben: [Einen Bericht zu einem Dashboard hinzufügen](/help/quicksilver/reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md)

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Abo</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Aktuell: Plan </p>
   Oder
   <p>Neu: Standard </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

{{step1-to-dashboards}}

1. Um ein vorhandenes Dashboard zu bearbeiten, wählen Sie das Dashboard aus, in das Sie die Website-Seite einbetten möchten, und klicken Sie dann auf **Dashboard-Aktionen** Klicken Sie auf **Bearbeiten**
Oder\
   Um ein neues Dashboard zu erstellen, klicken Sie auf **Neues Dashboard**.\
   Weitere Informationen zum Erstellen eines Dashboards finden Sie unter [Dashboard erstellen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

1. Klicks **Externe Seite hinzufügen** unter **Layout auswählen/Berichte hinzufügen/Kalender hinzufügen** Bereich.

   ![](assets/qs-add-external-page-350x239.png)

   Die **Externe Seite hinzufügen** angezeigt.

1. Geben Sie die folgenden Informationen zur externen Seite an:

   * **Name**: Benennen Sie das Dashboard.
   * **Beschreibung**: Fügen Sie weitere Informationen zum Dashboard hinzu, um die darin enthaltenen Informationen zu identifizieren. Die Beschreibung wird nach dem Speichern im Dashboard für alle Benutzer angezeigt, die Zugriff auf sie haben.
   * **URL**: Fügen Sie die zuvor kopierte URL in dieses Feld ein.

     Sie können die folgenden URL-Typen angeben:

      * Eine (verschlüsselte) HTTPS-URL zu einer Webseite.\
        Nur HTTPS-Seiten (verschlüsselt) werden mit der URL geladen.\
        ![](assets/add-external-page-dialog-qs-350x247.png)

      * Eine Vorlagen-URL mit Sitzungsinformationen für eine bestimmte Website.\
        Beispiel: *https://localhost/?session={!$$SESSION}*
Sie müssen bei der angegebenen Website angemeldet sein, um die externe Seite anzuzeigen.\
        Informationen zum Abrufen einer SessionID von Workfront finden Sie unter [API-Grundlagen](../../../wf-api/general/api-basics.md).\
        Ihr Workfront-Administrator kann Ihre Systemvoreinstellungen so konfigurieren, dass die Verwendung von Sitzungsinformationen auf Ihren externen Seiten aus Sicherheitsgründen nicht zulässig ist. In diesem Fall wird die externe Seite nicht im Dashboard geladen.\
        Weitere Informationen zu den Systemsicherheitseinstellungen finden Sie unter [Systemsicherheitsvoreinstellungen konfigurieren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).\
        ![external_page_with_session_id_example.png](assets/external-page-with-session-id-example-350x134.png)

     >[!WARNING]
     >
     >Die Verwendung der SessionID ist unsicher und wird nicht empfohlen.
     >

   * **Höhe**: Geben Sie eine Zahl größer 0 ein, um den Platz zu definieren, den die externe Seite im Dashboard belegt. Die Standardhöhe ist 500.

1. Klicken Sie auf **Speichern**.

   Die Seite wird automatisch zum Dashboard hinzugefügt.

   Wenn Sie zusätzliche Dashboards erstellen, können Sie diese externe Seite suchen und sie zu anderen Dashboards hinzufügen. Bei der Erstellung oder Bearbeitung eines Dashboards finden Sie alle vorhandenen externen Seiten in der Liste Verfügbare Berichte und Kalender .

   <!--
    *** This is linked to: Creating Dashboards, and Editing Dashboards.
   -->

## Externe Seite in einem Dashboard aktualisieren

So aktualisieren Sie die Informationen für eine in einem Dashboard verwendete externe Seite:

{{step1-to-dashboards}}

1. Klicken Sie auf den Namen des Dashboards, das Sie aktualisieren möchten, um es zu öffnen, und klicken Sie auf **Dashboard-Aktionen**, dann **Bearbeiten**.

   Die **Dashboard-Details** wird geöffnet.

1. Im **Layout auswählen/Berichte hinzufügen/Kalender hinzufügen** der **Dashboard-Details** , suchen Sie die externe Seite, die Sie aktualisieren möchten, bewegen Sie den Mauszeiger darüber und klicken Sie auf **Bearbeiten** Symbol.\
   ![](assets/nwe-inline-edit-external-page-350x226.png)

1. Im **Externe Seite bearbeiten** , aktualisieren Sie die Felder, die Sie ändern möchten, und klicken Sie auf **Speichern**.
1. (Optional) Klicken Sie auf die **Löschen** icon ![](assets/delete.png) , um die externe Seite aus dem Dashboard zu entfernen. Weitere Informationen finden Sie unter [Externe Seite aus einem Dashboard entfernen](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/remove-external-page-from-dashboard.md).
1. Klicken Sie auf **Speichern + schließen**.

## Anzeigen externer Seiten in einem Bericht

Sie können alle externen Seiten in Workfront in einem Bericht &quot;Externe Seite&quot;anzeigen.

{{step1-to-reports}}

1. Klicks **Neuer Bericht** > Auswählen **Externe Seite**.

   ![](assets/external-page-new-report-in-dropdown-nwe.png)

1. (Optional) Aktualisieren Sie die Registerkarten Ansicht, Filter oder Gruppierungen des Berichts.

   Weitere Informationen finden Sie unter [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Klicks **Speichern+Schließen**.

   Sie können den Namen und die URL, die mit den externen Seiten in Ihrem System verknüpft sind, im neuen Bericht anzeigen.

   ![](assets/external-page-report-name-url-columns-nwe-350x213.png)
