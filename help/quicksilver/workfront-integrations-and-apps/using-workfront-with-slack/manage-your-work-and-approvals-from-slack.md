---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Arbeiten und Genehmigungen von Slack verwalten
description: Sie können direkt von Slack aus auf Ihre Startseiten-Arbeitsliste zugreifen, Aufgaben und Probleme überprüfen und der Arbeit an diesen zustimmen und Genehmigungen überprüfen oder Entscheidungen treffen.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 802a2f16-d827-455e-9e49-f58f4c5fc482
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 1%

---

# Verwalten Sie Ihre Arbeit und Genehmigungen von [!DNL Slack]

Nach der Installation von [!DNL Adobe Workfront for Slack] haben Sie folgende Möglichkeiten:

* Zugreifen auf Listen Ihrer [!UICONTROL Startseite]-Elemente aus [!DNL Slack]
* Aufgaben und Probleme von [!DNL Slack] überprüfen und akzeptieren
* Genehmigungen von [!DNL Slack] überprüfen und Entscheidungen treffen

Weitere Informationen zum Konfigurieren von [!DNL Workfront] mit [!DNL Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] Plan</a>*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Bevor Sie Ihre Arbeit und Genehmigungen von [!DNL Slack] aus verwalten können, müssen Sie

* Konfigurieren von [!DNL Workfront for Slack]\
  Anweisungen zum Konfigurieren von [!DNL Workfront for Slack] finden Sie unter [Konfigurieren [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## Verwalten von Arbeit aus [!DNL Slack]

1. Melden Sie sich bei Ihrer [!DNL Slack]-Instanz an und melden Sie sich von [!DNL Slack] aus bei [!DNL Workfront] an.\
   Weitere Informationen zum Anmelden bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt „Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal den folgenden Befehl in das Feld Nachricht ein:

   `/workfront home`

   >[!NOTE]
   >
   >* Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Die Schaltflächen, über die Sie auf Listen Ihrer Aufgaben, Probleme und Genehmigungen zugreifen können, werden angezeigt. Durch Klicken auf eine der Schaltflächen werden die ersten 20 Elemente jeder Liste in [!DNL Slack] angezeigt.

1. (Optional) Klicken Sie auf **[!UICONTROL Aufgaben]**, um alle Ihre Aufgaben anzuzeigen.

   Weitere Informationen zum Verwalten von Aufgaben in [!DNL Slack] finden Sie unter [Verwalten Ihrer Aufgaben aus [!DNL Slack]](#manage-your-tasks-from-slack-manage-your-tasks-from-slack).

1. (Optional) Klicken Sie auf **[!UICONTROL Probleme]**, um alle Ihre Probleme anzuzeigen.

   Weitere Informationen zum Verwalten von Problemen in [!DNL Slack] finden Sie unter [Verwalten Ihrer Probleme von [!DNL Slack]](#manage-your-issues-from-slack-manage-your-issues-from-slack).

1. (Optional) Klicken Sie auf **[!UICONTROL Genehmigungen]**, um alle Genehmigungen anzuzeigen, die auf Ihre Entscheidung warten.\
   Weitere Informationen zum Verwalten Ihrer Genehmigungen in [!DNL Slack] finden Sie unter [Verwalten Ihrer Genehmigungen von [!DNL Slack]](#manage-your-approvals-from-slack-manage-your-approvals-from-slack).

## Verwalten von Aufgaben über [!DNL Slack] {#manage-your-tasks-from-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack]-Instanz an und melden Sie sich von [!DNL Slack] aus bei [!DNL Workfront] an.\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt „Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal einen der folgenden Befehle in das Feld Nachricht ein:

   `/workfront home` und klicken Sie dann auf **[!UICONTROL Aufgaben]**

   Oder

   `/workfront tasks`

   >[!NOTE]
   >
   >* Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Die ersten 20 Aufgaben in Ihrer Liste werden angezeigt.

1. Klicken Sie auf **[!UICONTROL +`<remaining number>` weitere]**, um zusätzliche Aufgaben anzuzeigen.
1. Sie sollten die folgenden Informationen zu Ihren Arbeitselementen überprüfen:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Projektname]** oder **[!DNL Parent Object Name]**

   * **[!DNL Planned Completion Date]** des Arbeitselements.
   * **[!DNL Assigned By Name]**: Dies ist der Name des Benutzers, der Ihnen die Aufgabe zugewiesen hat.
   * **[!UICONTROL Status]**

1. (Optional) Klicken Sie auf den Namen eines Elements, um es in Workfront in einer separaten Browser-Registerkarte zu öffnen.
1. (Optional) Wählen Sie **[!UICONTROL Feld &quot;]**&quot; einen neuen Status aus.
1. (Optional) Klicken Sie auf **[!UICONTROL Zeit erfassen]** und wählen Sie dann einen **[!UICONTROL Stundentyp]** und einen Stundenbetrag aus, um die Zeit für das Element zu erfassen.

   >[!NOTE]
   >
   >* Sie können Stunden nur in Schritten von einer ganzen oder halben Stunde, bis zu 12 Stunden und 30 Minuten protokollieren.
   >* Die Stunden, die Sie protokollieren, haben das Eingabedatum „Heute“. Sie können die Zeit für ein vergangenes oder künftiges Datum nicht von [!DNL Slack] protokollieren.

   Sie erhalten eine Bestätigung, dass die Zeit protokolliert wurde.

1. (Optional) Klicken Sie auf **[!UICONTROL Bearbeiten]**, um die Bearbeitung einer Aufgabe anzunehmen. Die [!UICONTROL Bearbeiten“-] verschwindet.

## Verwalten von Problemen über [!DNL Slack] {#manage-your-issues-from-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack]-Instanz an und melden Sie sich von [!DNL Slack] aus bei [!DNL Workfront] an.\
   Weitere Informationen zur Anmeldung bei [!DNL Workfront] von [!DNL Slack] finden Sie unter [Anmelden bei [!DNL Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md#logging-in-to-workfront) section in [Access [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal einen der folgenden Befehle in das Feld Nachricht ein:

   `/workfront home` und klicken Sie dann auf **[!UICONTROL Probleme]**

   Oder

   `/workfront issues`

   >[!NOTE]
   >
   >* Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Die ersten 20 Probleme in Ihrer Liste werden angezeigt.

1. Klicken Sie auf **[!UICONTROL + `<number>` weitere]**, um weitere Elemente anzuzeigen.
1. Sie sollten die folgenden Informationen zu Ihren Arbeitselementen überprüfen:

   * **[!UICONTROL Name]**
   * **[!UICONTROL Projekt]** Name oder Name des übergeordneten Objekts
   * **[!UICONTROL Fällig am]** Datum: Dies ist das geplante Abschlussdatum des Arbeitselements.
   * **[!DNL Requested by]**: Dies ist der Primäre Kontakt (bei Problemen) oder der Benutzer, der den Arbeitsauftrag erteilt hat (bei Aufgaben).

1. (Optional) Klicken Sie auf den Namen des Problems, um es in Workfront in einer separaten Browser-Registerkarte zu öffnen.
1. (Optional) Klicken Sie auf **[!DNL Work on it]** , um mit Problemen zu arbeiten, die Sie noch nicht akzeptiert haben.

   Die [!UICONTROL Bearbeiten“-] verschwindet.

## Verwalten Sie Ihre Genehmigungen von [!DNL Slack] {#manage-your-approvals-from-slack}

1. Melden Sie sich bei Ihrer [!DNL Slack]-Instanz an und melden Sie sich von [!DNL Slack] aus bei [!DNL Workfront] an.\
   Weitere Informationen zum Anmelden bei [!DNL Workfront] von [!DNL Slack] finden Sie im Abschnitt „Anmelden bei [!DNL Workfront] von [!DNL Slack]&quot; in [Zugriff [!DNL Adobe Workfront] von [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. Geben Sie in einem beliebigen Kanal einen der folgenden Befehle in das Feld Nachricht ein:

   `/workfront home` und klicken Sie dann auf **[!UICONTROL Genehmigungen]**

   Oder

   `/workfront approvals`

   >[!NOTE]
   >
   >* Bei Befehlen wird zwischen Groß- und Kleinschreibung unterschieden.
   >* Sie können Ihren Befehl mit `/wf` anstelle von `/workfront` starten.

   Die ersten 20 Elemente Ihrer **[!UICONTROL Genehmigungen]**-Liste werden angezeigt. Es werden auch zusätzliche Informationen zu den Elementen angezeigt, z. B. der Name des Benutzers, der sie angefordert hat, oder der Name des Projekts, zu dem das Element gehört.

1. Klicken Sie auf **[!UICONTROL + `<number>` weitere]**, um weitere Elemente anzuzeigen.

1. Erwägen Sie, Genehmigungen für die folgenden Objekte zu verwalten:

   * **Projekte**

     Klicken Sie **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]**, um die Statusänderung eines Projekts zu akzeptieren oder abzulehnen.

   * **Aufgaben**

     Klicken Sie **[!UICONTROL Genehmigen]** oder **[!UICONTROL Ablehnen]**, um die Statusänderung einer Aufgabe zu akzeptieren oder abzulehnen.

   * **Probleme**

     Klicken Sie **[!UICONTROL Genehmigen]** oder **[!DNL Reject]**, um die Statusänderung eines Problems zu akzeptieren oder abzulehnen.

   * **Dokumente**

     Klicken Sie auf **[!UICONTROL Genehmigen]**, um ein Dokument zu genehmigen, **[!UICONTROL Ablehnen]**, um es abzulehnen, oder **[!UICONTROL Änderungen]**, um anzugeben, dass Sie es genehmigen, für das Dokument jedoch zusätzliche Änderungen erforderlich sind.\
     (Optional) Bewegen Sie den Mauszeiger über die Miniaturansicht des Dokuments, um auf die Lupe zu klicken und eine Vorschau des Dokuments anzuzeigen.

   * **Korrekturabzüge**&#x200B; Klicken Sie auf den Namen des Korrekturabzugs, um ihn in einer separaten Registerkarte in [!DNL Workfront] zu öffnen und die Genehmigung zu verwalten.
   * **Zugriffsanfragen**

     Klicken Sie auf **[!UICONTROL Zugriff gewähren]**, um dem angeforderten Objekt erweiterte Berechtigungen zu gewähren, oder **[!UICONTROL Ignorieren]**, um die Anfrage für weiteren Zugriff zu ignorieren.

1. (Optional) Klicken Sie auf den Namen des Objekts, das zur Genehmigung eingereicht wurde, um es in [!DNL Workfront] in einer neuen Browser-Registerkarte zu öffnen.
