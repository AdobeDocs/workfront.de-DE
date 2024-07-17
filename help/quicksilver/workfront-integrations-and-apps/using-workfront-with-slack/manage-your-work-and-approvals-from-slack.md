---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Verwalten Sie Ihre Arbeit und Ihre Validierungen über Slack
description: Sie können direkt über Slack auf Ihre Hausarbeitsliste zugreifen, Aufgaben und Probleme überprüfen und damit einverstanden sein und Entscheidungen über Genehmigungen treffen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 1%

---

# Verwalten Sie Ihre Arbeit und Ihre Genehmigungen über [!DNL Slack]

Nachdem Sie [!DNL Adobe Workfront for Slack] installiert haben, können Sie Folgendes tun:

* Auf Listen Ihrer [!UICONTROL Home]-Elemente von [!DNL Slack] zugreifen
* Überprüfen und akzeptieren Sie die Arbeit an Aufgaben und Problemen von [!DNL Slack]
* Überprüfen und treffen Sie Entscheidungen über Genehmigungen von [!DNL Slack]

Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit [!DNL Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie Ihre Arbeit und Genehmigungen mit [!DNL Slack] verwalten können, müssen Sie

* Konfigurieren von [!DNL Workfront for Slack]\
  Anweisungen zum Konfigurieren von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Verwalten Ihrer Arbeit über [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz an und melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an.\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt &quot;Anmeldung bei [!DNL Workfront] von [!DNL Slack]&quot;unter [Zugriff [!DNL Adobe Workfront]  von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus den folgenden Befehl in das Meldungsfeld ein:

   `/workfront home`

   >[!NOTE]
   >
   >* Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Die Schaltflächen, über die Sie auf Listen Ihrer Aufgaben, Probleme und Genehmigungen zugreifen können, werden angezeigt. Wenn Sie auf eine der Schaltflächen klicken, werden die ersten 20 Elemente jeder Liste in [!DNL Slack] angezeigt.

1. (Optional) Klicken Sie auf **[!UICONTROL Aufgaben]** , um alle Ihre Aufgaben anzuzeigen.

   Weitere Informationen zum Verwalten von Aufgaben in [!DNL Slack] finden Sie unter [Verwalten Ihrer Aufgaben von  [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Optional) Klicken Sie auf **[!UICONTROL Probleme]** , um alle Ihre Probleme anzuzeigen.

   Weitere Informationen zum Verwalten von Problemen in [!DNL Slack] finden Sie unter [Verwalten Ihrer Probleme über  [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Optional) Klicken Sie auf **[!UICONTROL Genehmigungen]** , um alle Genehmigungen anzuzeigen, die auf Ihre Entscheidung warten.\
   Weitere Informationen zur Verwaltung Ihrer Genehmigungen in [!DNL Slack] finden Sie unter [Verwalten Ihrer Genehmigungen von  [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Verwalten Ihrer Aufgaben über [!DNL Slack] {#manage-your-tasks-from-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz an und melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an.\
   Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt &quot;Anmeldung bei [!DNL Workfront] von [!DNL Slack]&quot;unter [Zugriff [!DNL Adobe Workfront] von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus einen der folgenden Befehle in das Meldungsfeld ein:

   `/workfront home` und klicken Sie dann auf **[!UICONTROL Aufgaben]**

   Oder

   `/workfront tasks`

   >[!NOTE]
   >
   >* Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Die ersten 20 Aufgaben Ihrer Liste werden angezeigt.

1. Klicken Sie auf **[!UICONTROL +`<remaining number>` more]** , um weitere Aufgaben anzuzeigen.
1. Überprüfen Sie die folgenden Informationen zu Ihren Arbeitselementen:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Projektname]** oder **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** des Arbeitselements.
   * **[!DNL Assigned By Name]**: Dies ist der Name des Benutzers, der Ihnen die Aufgabe zugewiesen hat.
   * **[!UICONTROL Status]**

1. (Optional) Klicken Sie auf den Namen eines Elements, um es in Workfront auf einer separaten Browser-Registerkarte zu öffnen.
1. (Optional) Wählen Sie im Feld **[!UICONTROL Status]** einen neuen Status aus.
1. (Optional) Klicken Sie auf **[!UICONTROL Protokollzeit]** und wählen Sie dann einen **[!UICONTROL Stunden-Typ]** und einen Stundenwert für die Protokollzeit des Elements aus.

   >[!NOTE]
   >
   >* Sie können Stunden nur in Schritten von einer vollen oder halben Stunde, bis zu 12 Stunden und 30 Minuten protokollieren.
   >* Die Stunden, die Sie protokollieren, haben ein Eintragsdatum von heute. Sie können die Zeit nicht für ein vergangenes oder künftiges Datum von [!DNL Slack] protokollieren.

   Sie erhalten eine Bestätigung, dass die Zeit protokolliert wurde.

1. (Optional) Klicken Sie auf **[!UICONTROL Bearbeiten]** , um die Bearbeitung einer Aufgabe zu akzeptieren. Die Schaltfläche [!UICONTROL Bearbeiten] wird ausgeblendet.

## Probleme in [!DNL Slack] verwalten {#manage-your-issues-from-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz an und melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an.\
   Weitere Informationen zum Anmelden bei [!DNL Workfront] von [!DNL Slack] finden Sie unter [Anmelden bei  [!DNL Workfront] von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus einen der folgenden Befehle in das Meldungsfeld ein:

   `/workfront home` und klicken Sie dann auf **[!UICONTROL Probleme]**

   Oder

   `/workfront issues`

   >[!NOTE]
   >
   >* Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Die ersten 20 Probleme in Ihrer Liste werden angezeigt.

1. Klicken Sie auf **[!UICONTROL + verbleibende `<number>` Mehr]** , um weitere Elemente anzuzeigen.
1. Überprüfen Sie die folgenden Informationen zu Ihren Arbeitselementen:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Projekt]** Name oder übergeordneter Objektname
   * **[!UICONTROL Fälligkeitsdatum am]** Datum: Dies ist das geplante Abschlussdatum des Arbeitselements.
   * **[!DNL Requested by]** Name: Dies ist der Primäre Kontakt (für Probleme) oder der Benutzer, der die Zuweisung vorgenommen hat (für Aufgaben).

1. (Optional) Klicken Sie auf den Namen des Problems, um es in Workfront in einer separaten Browser-Registerkarte zu öffnen.
1. (Optional) Klicken Sie auf **[!DNL Work on it]** , um mit der Arbeit an Problemen zu beginnen, die Sie noch nicht akzeptiert haben.

   Die Schaltfläche [!UICONTROL Bearbeiten] wird ausgeblendet.

## Verwalten von Genehmigungen über [!DNL Slack] {#manage-your-approvals-from-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack] -Instanz an und melden Sie sich von [!DNL Slack] bei [!DNL Workfront] an.\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt &quot;Anmeldung bei [!DNL Workfront] von [!DNL Slack]&quot;unter [Zugriff [!DNL Adobe Workfront]  von  [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie von jedem Kanal aus einen der folgenden Befehle in das Meldungsfeld ein:

   `/workfront home` und klicken Sie dann auf **[!UICONTROL Genehmigungen]**

   Oder

   `/workfront approvals`

   >[!NOTE]
   >
   >* Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Die ersten 20 Elemente in Ihrer Liste **[!UICONTROL Genehmigungen]** werden angezeigt. Zusätzliche Informationen zu den Elementen werden ebenfalls angezeigt, z. B. der Name des Benutzers, der sie angefordert hat, oder der Name des Projekts, zu dem das Element gehört.

1. Klicken Sie auf **[!UICONTROL + verbleibende `<number>` Mehr]** , um weitere Elemente anzuzeigen.

1. Sie sollten Genehmigungen für die folgenden Objekte verwalten:

   * **Projekte**

     Klicken Sie auf **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]** , um die Statusänderung eines Projekts zu akzeptieren oder abzulehnen.

   * **Aufgaben**

     Klicken Sie auf **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]** , um die Statusänderung einer Aufgabe zu akzeptieren oder abzulehnen.

   * **Probleme**

     Klicken Sie auf **[!UICONTROL Genehmigen]** oder **[!DNL Reject]** , um die Statusänderung eines Problems zu akzeptieren oder abzulehnen.

   * **Dokumente**

     Klicken Sie auf &quot;**[!UICONTROL Genehmigen]**&quot;, um ein Dokument zu genehmigen, &quot;**[!UICONTROL Ablehnen]**&quot;, um es abzulehnen,&quot;oder &quot;**[!UICONTROL Änderungen]**&quot;, um anzugeben, dass Sie es genehmigen, das Dokument jedoch zusätzliche Änderungen erfordert.\
     (Optional) Bewegen Sie den Mauszeiger über die Dokumentminiatur, um auf das Lupensymbol zu klicken und eine Vorschau des Dokuments anzuzeigen.

   * **Testsendungen** &#x200B; Klicken Sie auf den Testversand-Namen, um ihn in [!DNL Workfront] auf einer separaten Registerkarte zu öffnen und die Genehmigung zu verwalten.
   * **Zugriffsanforderungen**

     Klicken Sie auf **[!UICONTROL Zugriff gewähren]** , um dem angeforderten Objekt erweiterte Berechtigungen zu gewähren, oder auf **[!UICONTROL Ignorieren]** , um die Anfrage für weiteren Zugriff zu ignorieren.

1. (Optional) Klicken Sie auf den Namen des zur Genehmigung gesendeten Objekts, um es in [!DNL Workfront] in einer neuen Registerkarte des Browsers zu öffnen.
