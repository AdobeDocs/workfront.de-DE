---
filename: gitlab-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: GitLab-Module
description: Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.
author: Becky
feature: Workfront Fusion
exl-id: bf6c1d82-7926-4bf9-8424-e658650ee6b1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '4070'
ht-degree: 0%

---


# [!UICONTROL GitLab] -Module

Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!UICONTROL GitLab] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

>[!NOTE]
>
>Dieser Artikel erwartet einige Kenntnisse der API-Dokumentation und der Funktionen von [!DNL GitLab] im Allgemeinen.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL GitLab] mit [!DNL Workfront Fusion] verbinden {#connect-gitlab-to-workfront-fusion}

1. Klicken Sie in einem beliebigen [!DNL Workfront Fusion] [!DNL Gitlab] -Modul neben dem Verbindungsfeld auf **[!UICONTROL Hinzufügen]** .
1. Konfigurieren Sie die folgenden Felder:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Verbindungsname]</td> 
      <td> <p>Geben Sie einen Namen für die Verbindung ein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL GitLab] URL]</td> 
      <td>Geben Sie die URL Ihrer [!DNL GitLab] -Instanz ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Zugriffstoken]</td> 
      <td><p>Geben Sie Ihren [!UICONTROL Private Token] oder [!UICONTROL Personal Access Token] ein.</p><p>Informationen zum Suchen oder Erstellen eines persönlichen Zugriffstokens in [!DNL GitLab] finden Sie unter "Erstellen eines persönlichen Zugriffstokens"in <a href="https://docs.gitlab.com/ee/user/profile/personal_access_tokens.html">Persönliche Zugriffstoken</a> in der Dokumentation zu [!DNL GitLab].</p></td> 
     </tr> 
    </tbody> 
   </table>


1. Klicken Sie auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf **[!UICONTROL Autorisieren]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL GitLab] Module und ihre Felder

Wenn Sie [!DNL GitLab] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL GitLab] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Trigger

+++**[!UICONTROL Build-Status überwachen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn sich der Status eines Builds ändert.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das vom Webhook auf Build-Statusänderungen überwacht werden soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Commit/MR/issue/Snippet-Kommentare ansehen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn ein Kommentar zu einem Commit, einer Zusammenführungsanfrage, einem Problem oder einem Codeausschnitt erstellt wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das der Webhook auf Kommentare überwachen soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Überwachen von Commits (pushes)]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn ein Commit in ein Repository gesendet wird. Dieses Modul startet kein Szenario, wenn ein Tag gepusht wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das der Webhook auf Commits überwachen soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Behobener Problemkommentar anzeigen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn zu einem Problem ein Kommentar abgegeben wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das der Webhook auf Problemkommentare überwachen soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Überwachungsprobleme]**

Dieses [!UICONTROL Instant Trigger]-Modul startet ein Szenario, wenn ein Problem erstellt wird oder ein vorhandenes Problem aktualisiert, geschlossen oder erneut geöffnet wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das der Webhook auf Probleme überwachen soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Zusammenführungsanfragen überwachen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn eines der folgenden Ereignisse eintritt:

* Eine neue Zusammenführungsanforderung wird erstellt
* Eine vorhandene Zusammenführungsanfrage wird aktualisiert, zusammengeführt oder geschlossen
* Im Quellzweig wird ein Commit hinzugefügt


<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das vom Webhook auf Zusammenführungsanfragen überwacht werden soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Kommentare zu Zusammenführungsanfragen ansehen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn ein Kommentar für eine Zusammenführungsanforderung erstellt wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das der Webhook auf Zusammenführungsanfragekommentare überwachen soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Pipeline-Status überwachen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn sich der Status einer Pipeline ändert.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das vom Webhook auf Pipeline-Statusänderungen überwacht werden soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Projekte ansehen]**

Dieses Modul für geplante Trigger startet ein Szenario, wenn ein neues Projekt hinzugefügt wird, dem der authentifizierte Benutzer angehört.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL GitLab]-Kontos mit [!DNL Workfront] Fusion finden Sie in diesem Artikel unter <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL GitLab] mit [!DNL Workfront] Fusion</a> .</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max Ergebnisse</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios überwachen soll.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Repository-Verzweigungen beobachten]**

Dieses geplante Trigger-Modul startet ein Szenario, wenn einem Repository eine neue Verzweigung hinzugefügt wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL GitLab]-Kontos mit [!DNL Workfront] Fusion finden Sie in diesem Artikel unter <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL GitLab] mit [!DNL Workfront] Fusion</a> .</td> 
   </tr> 
   <tr> 
   <td role="rowheader">Max Ergebnisse</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios überwachen soll.</p> </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Repository-Tags überwachen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn ein Tag in einem Repository erstellt oder gelöscht wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das vom Webhook auf Tags überwacht werden soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Snippet-Kommentare ansehen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn ein neuer Kommentar zu einem Snippet erstellt wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das der Webhook auf Kommentare überwachen soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL TODOS ansehen]**

Dieses geplante Trigger-Modul startet ein Szenario, wenn ein neues Tool hinzugefügt wird. Wenn kein Filter angewendet wird, wird der Trigger ausgeführt, wenn ein neues ausstehendes Tool hinzugefügt wird.

Informationen zu Feldern finden Sie unter [Abrufen einer Liste von zu dos](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Wiki-Seite ansehen]**

Dieses Instant Trigger-Modul startet ein Szenario, wenn eine Wiki-Seite erstellt oder bearbeitet wird.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td><p>Wählen Sie den Webhook aus, den Sie für diesen Trigger verwenden möchten, oder fügen Sie einen neuen Webhook hinzu. </p><p>Um einen neuen Webhook hinzuzufügen, <ol><li>Klicken Sie neben dem Feld [!UICONTROL Webhook] auf <b>[!UICONTROL Hinzufügen]</b>.</li><li>Geben Sie Folgendes ein: <ul><li>Ein Name für den Webhook</li><li>Die Verbindung, die Sie für diesen Webhook verwenden möchten</li><li>Das Projekt, das der Webhook auf Wiki-Seiten überwachen soll</li></ul></li><li>Klicken Sie auf <b>[!UICONTROL Save]</b> , um den Webhook zu speichern und zum Modul zurückzukehren. </td> 
   </tr> 
   </tbody> 
</table>

+++

### Aktionen

+++**[!UICONTROL Anfrage zum Zusammenführen akzeptieren]**

Dieses Aktionsmodul führt gesendete Änderungen mit der angegebenen Zusammenführungsanforderung zusammen.

Informationen zu Feldern finden Sie unter [Anfrage zum Zusammenführen akzeptieren](https://docs.gitlab.com/ee/api/merge_requests.html#accept-mr) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Abbrechen eines Builds]**

Dieses Aktionsmodul bricht einen einzelnen Build eines Projekts ab.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL GitLab]-Kontos mit [!DNL Workfront] Fusion finden Sie in diesem Artikel unter <a href="#connect-gitlab-to-workfront-fusion-connect-gitlab-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL GitLab] mit [!DNL Workfront] Fusion</a> .</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID]</td> 
   <td> <p>Wählen Sie das Projekt aus oder ordnen Sie es zu, das den Build enthält, den Sie abbrechen möchten.</p> </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Build-ID]</td> 
   <td>Wählen Sie den Build aus oder ordnen Sie ihn zu, den Sie abbrechen möchten.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Commit Commit Message]</td> 
   <td> Geben Sie eine Commit-Meldung für die Zusammenführung ein oder ordnen Sie sie zu.
    </td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Sollte Quellverzweigung entfernen]</td> 
   <td>Wählen Sie aus, ob die Quellverzweigung nach Abschluss der Zusammenführung entfernt werden soll.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Zusammenführen bei erfolgreichem Build]</td> 
   <td>Wählen Sie aus, ob die Zusammenführungsanfrage zusammengeführt werden soll, sobald der Build abgeschlossen ist.</td> 
   </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL SHA]</td> 
   <td>Falls vorhanden, muss diese SHA mit der HEAD der Quellverzweigung übereinstimmen. Wenn sie nicht übereinstimmt, schlägt die Zusammenführung fehl.</td> 
   </tr> 
   </tbody> 
</table>

+++

+++**[!UICONTROL Abbrechen der Builds einer Pipeline]**

Dieses Aktionsmodul bricht die Builds für eine einzelne Pipeline ab.

Informationen zu Feldern finden Sie unter [Abbrechen von Vorgängen einer Pipeline](https://docs.gitlab.com/ee/api/pipelines.html#cancel-a-pipelines-jobs) in der [!DNL GitLab] -Dokumentation.

+++

+++**[!UICONTROL Zusammenführung abbrechen, wenn die Pipeline erfolgreich ist]**

Wenn eine Zusammenführungsanfrage so eingestellt ist, dass sie beim Erfolg einer Pipeline zusammengeführt wird, bricht dieses Aktionsmodul diese Aktion ab.

Informationen zu Feldern finden Sie unter [Zusammenführung abbrechen, wenn die Pipeline erfolgreich ist](https://docs.gitlab.com/ee/api/merge_requests.html) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Vererben wählt einen Commit]**

Diese Aktionsmodul-Kirsche wählt eine Bindung zu einem bestimmten Zweig aus.

Informationen zu Feldern finden Sie unter [Auswahl eines Commit](https://docs.gitlab.com/ee/api/commits.html#cherry-pick-a-commit) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erstellen einer neuen Bezeichnung]**

Dieses Aktionsmodul erstellt eine neue Bezeichnung für das angegebene Repository.

Informationen zu Feldern finden Sie unter [Erstellen einer neuen Beschriftung](https://docs.gitlab.com/ee/api/labels.html#create-a-new-label) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erstellen einer neuen Pipeline]**

Dieses Aktionsmodul erstellt eine neue Pipeline für das jeweilige Projekt.

Informationen zu Feldern finden Sie unter [Erstellen einer neuen Pipeline](https://docs.gitlab.com/ee/api/pipelines.html#create-a-new-pipeline) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erstellen einer neuen Version]**

Dieses Aktionsmodul fügt dem vorhandenen Git-Tag Versionshinweise hinzu.

Informationen zu Feldern finden Sie unter [Release erstellen](https://docs.gitlab.com/ee/api/releases/#create-a-release) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Erstellen eines neuen Tags]**

Dieses Aktionsmodul erstellt ein neues Tag im Repository, das auf die bereitgestellte Referenz verweist.

Informationen zu Feldern finden Sie unter [Neues Tag erstellen](https://docs.gitlab.com/ee/api/tags.html#create-a-new-tag) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Erstellen eines TODO]**

Dieses Aktionsmodul erstellt ein Tool für den aktuellen Benutzer zum ausgewählten Problem. Der aktuelle Benutzer ist der Benutzer, der durch die Anmeldeinformationen der für dieses Modul verwendeten Verbindung identifiziert wird.

Informationen zu Feldern finden Sie unter [Erstellen eines Aufgabenbereichs](https://docs.gitlab.com/ee/api/issues.html#create-a-todo) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erstellen eines TODO für eine Zusammenführungsanforderung]**

Dieses Aktionsmodul erstellt für den aktuellen Benutzer ein todo für die ausgewählte Zusammenführungsanforderung. Der aktuelle Benutzer ist der Benutzer, der durch die Anmeldeinformationen der für dieses Modul verwendeten Verbindung identifiziert wird.

Informationen zu Feldern finden Sie unter [Erstellen eines Aufgabenbereichs](https://docs.gitlab.com/ee/api/merge_requests.html#create-a-todo) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erstellen einer Zusammenführungsanforderung]**

Dieses Aktionsmodul erstellt eine neue Zusammenführungsanforderung für ein Projekt.

Informationen zu Feldern finden Sie unter [Zusammenführungsanfrage erstellen](https://docs.gitlab.com/ee/api/merge_requests.html#create-mr) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Neue Datei im Repository erstellen]**

Dieses Aktionsmodul erstellt eine neue Datei im ausgewählten Repository.

Informationen zu Feldern finden Sie unter [Neue Datei im Repository erstellen](https://docs.gitlab.com/ee/api/repository_files.html#create-new-file-in-repository) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erstellen Sie eine neue Problembeschreibung]**

Dieses Aktionsmodul erstellt einen Problemhinweis für ein einzelnes Projektproblem.

Informationen zu Feldern finden Sie unter [Neues Problem erstellen](https://docs.gitlab.com/ee/api/notes.html#create-new-issue-note) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erstellen Sie eine neue Notiz für die Zusammenführungsanforderung]**

Dieses Aktionsmodul erstellt eine Notiz für eine einzelne Zusammenführungsanforderung.

Weitere Informationen zu Feldern finden Sie unter [Neue Notiz für Zusammenführungsanfragen erstellen](https://docs.gitlab.com/ee/api/notes.html#create-new-merge-request-note) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erstellen eines neuen Meilensteins]**

Dieses Aktionsmodul erstellt einen neuen Meilenstein für ein Projekt.

Informationen zu Feldern finden Sie unter [Neuen Meilenstein erstellen](https://docs.gitlab.com/ee/api/milestones.html#create-new-milestone) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Neue Codefragment-Notiz erstellen]**

Dieses Aktionsmodul erstellt eine neue Notiz für ein einzelnes Snippet. Snippet-Hinweise sind Kommentare, die Benutzer in einem Snippet posten können.

Weitere Informationen zu Feldern finden Sie unter [Neues Snippet-Hinweis erstellen](https://docs.gitlab.com/ee/api/notes.html#create-new-snippet-note) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Repository-Verzweigung erstellen]**

Dieses Aktionsmodul erstellt eine einzelne Repository-Verzweigung.

Informationen zu Feldern finden Sie unter [Repository-Verzweigung erstellen](https://docs.gitlab.com/ee/api/branches.html#create-repository-branch) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Build-Variable erstellen]**

Dieses Aktionsmodul erstellt eine neue Build-Variable.

Informationen zu Feldern finden Sie unter [Variable erstellen](https://docs.gitlab.com/ee/api/project_level_variables.html#create-variable) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Löschen einer Zusammenführungsanforderung]**

Dieses Aktionsmodul ist nur für Administratoren und Projekteigentümer geeignet. Löscht die fragliche Zusammenführungsanforderung

Informationen zu Feldern finden Sie unter [Eine Zusammenführungsanforderung löschen](https://docs.gitlab.com/ee/api/merge_requests.html#delete-a-merge-request) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Vorhandene Datei im Repository löschen]**

Dieses Aktionsmodul löscht eine vorhandene Datei aus dem Repository.

Informationen zu Feldern finden Sie unter [Vorhandene Datei im Repository löschen](https://docs.gitlab.com/ee/api/repository_files.html#delete-existing-file-in-repository) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Repository-Verzweigung löschen]**

Dieses Aktionsmodul löscht eine Verzweigung aus dem Repository.

Informationen zu Feldern finden Sie unter [Repository-Verzweigung löschen](https://docs.gitlab.com/ee/api/branches.html#delete-repository-branch) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Problem bearbeiten]**

Dieses Aktionsmodul aktualisiert ein vorhandenes Projektproblem. Dieser Aufruf wird auch verwendet, um ein Problem als geschlossen zu kennzeichnen.

Informationen zu Feldern finden Sie unter [Problem bearbeiten](https://docs.gitlab.com/ee/api/issues.html#edit-issue) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Meilenstein bearbeiten]**
Dieses Aktionsmodul aktualisiert einen vorhandenen Projekt-Meilenstein.

Informationen zu Feldern finden Sie unter [Meilenstein bearbeiten](https://docs.gitlab.com/ee/api/milestones.html#edit-milestone) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Löschen eines Builds]**

Dieses Aktionsmodul löscht einen Build eines Projekts (entfernt Auftragsartefakte und Auftragsprotokolle).

Informationen zu Feldern finden Sie unter [Auftrag löschen](https://docs.gitlab.com/ee/api/jobs.html#erase-a-job) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Liste der Aufgaben abrufen]**

Dieses Suchmodul ruft eine Liste von zu erledigenden Elementen ab.

Informationen zu Feldern finden Sie unter [Abrufen einer Liste von zu dos](https://docs.gitlab.com/ee/api/todos.html#get-a-list-of-todos) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Einen einzelnen Build abrufen]**

Dieses Aktionsmodul ruft einen einzelnen Auftrag eines Projekts ab.

Informationen zu Feldern finden Sie unter [Einen einzelnen Auftrag abrufen](https://docs.gitlab.com/ee/api/jobs.html#get-a-single-job) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Abrufen eines einzelnen Repository-Tags]**

Dieses Aktionsmodul ruft ein bestimmtes Repository-Tag ab, das durch seinen Namen bestimmt wird.

Informationen zu Feldern finden Sie unter [Abrufen eines einzelnen Repository-Tags](https://docs.gitlab.com/ee/api/tags.html#get-a-single-repository-tag) in der [!DNL GitLab] -Dokumentation.

+++

+++**[!UICONTROL Bestimmte Bereitstellung abrufen]**

Dieses Aktionsmodul ruft eine bestimmte Bereitstellung ab.

Informationen zu Feldern finden Sie unter [Bestimmte Bereitstellung abrufen](https://docs.gitlab.com/ee/api/deployments.html#get-a-specific-deployment) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Abrufen aller Probleme, die einem einzigen Meilenstein zugewiesen sind]**

Dieses Suchmodul ruft alle Probleme ab, die einem einzelnen Projekt-Meilenstein zugewiesen sind.

Informationen zu Feldern finden Sie unter [Alle Probleme einem einzigen Meilenstein zuweisen](https://docs.gitlab.com/ee/api/milestones.html#get-all-issues-assigned-to-a-single-milestone) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Datei aus Repository abrufen]**

Dieses Aktionsmodul ruft Informationen zu einer Datei im Repository ab, z. B. Name, Größe oder Inhalt.

Informationen zu Feldern finden Sie unter [Datei aus Repository abrufen](https://docs.gitlab.com/ee/api/repository_files.html#get-file-from-repository) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Projektbenutzer abrufen]**

Dieses Suchmodul ruft die Benutzer des Projekts ab.

Informationen zu Feldern finden Sie unter [Projektbenutzer abrufen](https://docs.gitlab.com/ee/api/projects.html#get-project-users) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Abrufen eines einzelnen Problems]**

Dieses Aktionsmodul ruft Problemdetails ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Informationen zum Erstellen einer neuen Verbindung finden Sie unter <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] to Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt]</td> 
   <td> <p>Wählen Sie das Projekt aus, das das Problem enthält, zu dem Sie Details abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Problem-ID]</td> 
   <td> <p>Geben Sie den Namen des Problems ein oder ordnen Sie ihn zu, zu dem Sie Details abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Einzelne Problembeschreibung abrufen]**

Dieses Aktionsmodul ruft eine einzelne Notiz für ein bestimmtes Projektproblem ab.

Informationen zu Feldern finden Sie unter [Einzelne Problembeschreibung abrufen](https://docs.gitlab.com/ee/api/notes.html#get-single-issue-note) in der [!DNL GitLab] -Dokumentation.

+++

+++**[!UICONTROL Einzelne Zusammenführungsanforderung abrufen]**

Dieses Aktionsmodul ruft Informationen zu einer einzelnen Zusammenführungsanfrage ab.

Weitere Informationen zu Feldern finden Sie unter [Einzelne Zusammenführungsanforderung abrufen](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr) in der [!DNL GitLab] -Dokumentation.

+++

+++**[!UICONTROL Einzelne Änderungen an Zusammenführungsanfragen abrufen]**

Dieses Suchmodul ruft Informationen über die Zusammenführungsanforderung ab, einschließlich der zugehörigen Dateien und Änderungen.

Informationen zu Feldern finden Sie unter [Abrufen von Änderungen an einzelnen Zusammenführungsanfragen](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-changes) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Abrufen einzelner Zusammenführungsanforderungszusagen]**

Dieses Aktionsmodul ruft eine Liste von Zusammenführungsanforderungscommits ab.

Weitere Informationen zu Feldern finden Sie unter [Get single merge request commits](https://docs.gitlab.com/ee/api/merge_requests.html#get-single-mr-commits) in der [!DNL GitLab] -Dokumentation.

+++

+++**[!UICONTROL Hinweis für eine einzelne Zusammenführungsanforderung abrufen]**

Dieses Aktionsmodul gibt eine einzelne Notiz für eine bestimmte Zusammenführungsanforderung zurück.

Informationen zu Feldern finden Sie unter [Hinweis zur einzelnen Zusammenführungsanfrage abrufen](https://docs.gitlab.com/ee/api/notes.html#get-single-merge-request-note) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Einen Milestone abrufen]**

Dieses Aktionsmodul ruft Meilensteindetails ab.

Informationen zu Feldern finden Sie unter [Einzelne Meilensteine abrufen](https://docs.gitlab.com/ee/api/milestones.html#get-single-milestone) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Einzelnes Projekt abrufen]**

Dieses Aktionsmodul ruft Projektdetails ab.

Informationen zu Feldern finden Sie unter [Einzelnes Projekt abrufen](https://docs.gitlab.com/ee/api/projects.html#get-single-project) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Abrufen einer einzelnen Repository-Verzweigung]**

Dieses Aktionsmodul ruft Details zu Repository-Verzweigungen ab.

Informationen zu Feldern finden Sie unter [Abrufen einer einzelnen Repository-Verzweigung](https://docs.gitlab.com/ee/api/branches.html#get-single-repository-branch) in der [!DNL GitLab] -Dokumentation.

+++

+++**[!UICONTROL Codeausschnitt-Notiz abrufen]**

Dieses Modul ruft eine einzelne Notiz für ein bestimmtes Snippet ab.

Informationen zu Feldern finden Sie unter [Einen einzelnen Codeausschnitt-Hinweis abrufen](https://docs.gitlab.com/ee/api/notes.html#get-single-snippet-note) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Abrufen der Kommentare zu einem Commit]**

Dieses Suchmodul ruft Kommentare zu einem Commit in einem Projekt ab.

Informationen zu Feldern finden Sie unter [Abrufen der Kommentare zu einem Commit](https://docs.gitlab.com/ee/api/commits.html#get-the-comments-of-a-commit) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Abrufen des Vergleichs eines Commit]**

Dieses Aktionsmodul erhält den Vergleich eines Commit in einem Projekt.

Informationen zu Feldern finden Sie unter [Abrufen des Vergleichs eines Commit](https://docs.gitlab.com/ee/api/commits.html#get-the-diff-of-a-commit) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Artefakte beibehalten]**

Verhindert, dass Artefakte gelöscht werden, wenn der Ablauf festgelegt ist.

Informationen zu Feldern finden Sie unter [Artefakte beibehalten](https://docs.gitlab.com/ee/api/job_artifacts.html#keep-artifacts) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Alle Notizen zur Zusammenführungsanforderung auflisten]**

Dieses Suchmodul ruft eine Liste aller Hinweise für eine einzelne Zusammenführungsanforderung ab.

Informationen zu Feldern finden Sie unter [Auflisten aller Notizen von Zusammenführungsanfragen](https://docs.gitlab.com/ee/api/notes.html#list-all-merge-request-notes) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Alle Codefragmentnotizen auflisten]**

Dieses Modul erhält eine Liste aller Hinweise für ein einzelnes Snippet. Snippet-Hinweise sind Kommentare, die Benutzer in einem Snippet posten können.

Informationen zu Feldern finden Sie unter [?](https://docs.gitlab.com/ee/api/notes.html#list-all-snippet-notes) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Auflisten von Commit-Builds]**

Dieses Suchmodul gibt eine Liste von Builds für einen bestimmten Commit in einem Projekt zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Informationen zum Erstellen einer neuen Verbindung finden Sie unter <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] to Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID]</td> 
   <td> <p>Wählen Sie das Projekt aus, das den Commit enthält, für den Sie Builds auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Umfang]</td> 
   <td> Um die Suche auf einen bestimmten Status zu beschränken, wählen Sie den Status aus. Wenn Sie dieses Feld leer lassen, werden alle Builds des Commit zurückgegeben.  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Listenprobleme]**

Dieses Suchmodul gibt alle Probleme anhand der angegebenen Filtereinstellungen zurück.

Informationen zu Feldern finden Sie unter [Listenprobleme](https://docs.gitlab.com/ee/api/issues.html#list-issues) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Auflisten von Problemen, die beim Zusammenführen geschlossen werden]**

Dieses Suchmodul ruft alle Probleme ab, die durch Zusammenführen der bereitgestellten Zusammenführungsanfrage geschlossen werden würden.

Informationen zu Feldern finden Sie unter [Listen-Probleme, die beim Zusammenführen geschlossen werden](https://docs.gitlab.com/ee/api/merge_requests.html#list-issues-that-will-close-on-merge) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Listenbeschriftungen]**

Dieses Suchmodul ruft alle Bezeichnungen im Projekt ab.

Informationen zu Feldern finden Sie unter [Listen-Beschriftungen](https://docs.gitlab.com/ee/api/labels.html#list-labels) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Auflisten von Zusammenführungsanforderungen]**

Dieses Suchmodul ruft alle Zusammenführungsanfragen anhand der Filtereinstellungen ab.

Informationen zu Feldern finden Sie unter [Listen-Zusammenführungsanfragen](https://docs.gitlab.com/ee/api/merge_requests.html#list-merge-requests) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Eigene Projekte auflisten]**

Dieses Suchmodul ruft Projekte ab, bei denen der authentifizierte Benutzer als Eigentümer festgelegt ist.

Informationen zu Feldern finden Sie unter [Auflisten von Benutzerprojekten](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Auflisten von Projekt-Builds]**

Dieses Suchmodul ruft eine Liste von Builds in einem Projekt ab.

Informationen zu Feldern finden Sie unter [Auflisten von Projektaufträgen](https://docs.gitlab.com/ee/api/jobs.html#list-project-jobs) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Auflisten von Projektbereitstellungen]**

Dieses Suchmodul ruft eine Liste von Bereitstellungen in einem Projekt ab.

Informationen zu Feldern finden Sie unter [Auflisten von Projektbereitstellungen](https://docs.gitlab.com/ee/api/deployments.html#list-project-deployments) in der Dokumentation [!DNL GitLab] .

+++

+++**[!UICONTROL Auflisten von Projektproblemen]**

Dieses Suchmodul ruft eine Liste aller Hinweise zu einem einzelnen Problem ab.

Informationen zu Feldern finden Sie unter [Hinweise zu Projektproblemen auflisten](https://docs.gitlab.com/ee/api/notes.html#list-project-issue-notes) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Projektprobleme auflisten]**

Dieses Suchmodul gibt alle Probleme in einem angegebenen Projekt zurück.

Informationen zu Feldern finden Sie unter [Auflisten von Projektproblemen](https://docs.gitlab.com/ee/api/issues.html#list-project-issues) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Projekt-Meilensteine auflisten]**

Dieses Suchmodul ruft alle Meilensteine im Projekt ab.

Informationen zu Feldern finden Sie unter [Auflisten von Projekt-Meilensteinen](https://docs.gitlab.com/ee/api/milestones.html#list-project-milestones) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Projekt-Pipelines auflisten]**

Dieses Suchmodul ruft alle Pipelines für das Projekt ab.

Informationen zu Feldern finden Sie unter [Auflisten von Projekt-Pipelines](https://docs.gitlab.com/ee/api/pipelines.html#list-project-pipelines) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Projekt-Repository-Tags auflisten]**

Dieses Suchmodul ruft eine Liste von Repository-Tags aus einem Projekt ab, sortiert nach Namen in umgekehrter alphabetischer Reihenfolge.

Informationen zu Feldern finden Sie unter [Auflisten von Projekt-Repository-Tags](https://docs.gitlab.com/ee/api/tags.html#list-project-repository-tags) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Projektvariablen auflisten]**

Dieses Suchmodul ruft eine Liste der Variablen eines Projekts ab.

Informationen zu Feldern finden Sie unter [Auflisten von Projektvariablen](https://docs.gitlab.com/ee/api/project_level_variables.html#list-project-variables) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Auflisten von Projekten]**

Dieses Suchmodul ruft alle Projekte ab, denen der authentifizierte Benutzer angehört.

Informationen zu Feldern finden Sie unter [Alle Projekte auflisten](https://docs.gitlab.com/ee/api/projects.html#list-all-projects) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Repository-Verzweigungen auflisten]**

Dieses Modul sucht nach Repository-Verzweigungen anhand des Suchbegriffs.

Informationen zu Feldern finden Sie unter [Auflisten von Repository-Verzweigungen](https://docs.gitlab.com/ee/api/branches.html#list-repository-branches) in der [!DNL GitLab] -Dokumentation.

+++

+++**[!UICONTROL Repository-Commits auflisten]**

Dieses Suchmodul ruft eine Liste von Repository-Commits in einem Projekt ab.

Informationen zu Feldern finden Sie unter [Repository-Commits auflisten](https://docs.gitlab.com/ee/api/commits.html#list-repository-commits) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Repository-Mitarbeiter auflisten]**

Dieses Suchmodul ruft eine Repository-Beitragsliste ab.

Informationen zu Feldern finden Sie unter [Mitwirkende](https://docs.gitlab.com/ee/api/repositories.html#contributors) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Repository-Struktur auflisten]**

Dieses Suchmodul ruft eine Liste von Repository-Dateien und -Verzeichnissen in einem Projekt ab.

Informationen zu Feldern finden Sie unter [Repository-Struktur auflisten](https://docs.gitlab.com/ee/api/repositories.html#list-repository-tree) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Markieren Sie einen Todo wie getan]**

Dieses Aktionsmodul markiert ein einzelnes ausstehendes Aufgabenelement, das durch seine Kennung für den aktuellen Benutzer wie erledigt angegeben wird.

Informationen zu Feldern finden Sie unter [Markieren Sie ein Element, um es wie getan auszuführen](https://docs.gitlab.com/ee/api/todos.html#mark-a-todo-as-done) in der [!DNL GitLab] -Dokumentation.

+++

+++**[!UICONTROL Ändern Sie die vorhandene Problembeschreibung]**

Ändert eine vorhandene Anmerkung zu einem Problem.

Informationen zu Feldern finden Sie unter [Vorhandenen Problemvermerk ändern](https://docs.gitlab.com/ee/api/notes.html#modify-existing-issue-note) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Änderung der vorhandenen Notiz für Zusammenführungsanforderungen]**

Ändert die vorhandene Notiz einer Zusammenführungsanforderung.

Informationen zu Feldern finden Sie unter [Notiz vorhandener Zusammenführungsanfragen ändern](https://docs.gitlab.com/ee/api/notes.html#modify-existing-merge-request-note) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Vorhandenen Codefragment-Hinweis ändern]**

Dieses Aktionsmodul ändert eine vorhandene Notiz eines Snippets.

Informationen zu Feldern finden Sie unter [Vorhandenen Codeabschnitt ändern](https://docs.gitlab.com/ee/api/notes.html#modify-existing-snippet-note) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Neues Problem]**

Dieses Aktionsmodul erstellt ein neues Projektproblem.

Informationen zu Feldern finden Sie unter [Neues Problem](https://www.integromat.com/en/help/app/gitlab) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Build abspielen]**

Dieses Aktionsmodul Trigger eine manuelle Aktion zum Starten eines Auftrags.

Informationen zu Feldern finden Sie unter [Auftrag abspielen](https://docs.gitlab.com/ee/api/jobs.html#play-a-job) in der Dokumentation zu [!DNL GitLab] .

+++

+++**[!UICONTROL Kommentar zum Bestätigen posten]**

Dieses Aktionsmodul fügt einem Commit einen Kommentar hinzu.

Informationen zu Feldern finden Sie unter [Kommentar zum Commit posten](https://docs.gitlab.com/ee/api/commits.html#post-comment-to-commit) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Variable entfernen]**

Dieses Aktionsmodul entfernt die -Variable eines Projekts.

Informationen zu Feldern finden Sie unter [Variable entfernen](https://docs.gitlab.com/ee/api/project_level_variables.html#remove-variable) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Erneutes Ausführen eines Builds]**

Dieses Aktionsmodul versucht erneut einen einzelnen Build in einem Commit.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Informationen zum Erstellen einer neuen Verbindung finden Sie unter <a href="#connect-gitlab-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect [!DNL GitLab] to Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID]</td> 
   <td> <p>Wählen Sie das Projekt aus, das den Build enthält, den Sie erneut versuchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Build-ID]</td> 
   <td> Wählen Sie den Build aus, den Sie erneut versuchen möchten. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Wiederholen fehlgeschlagener Aufträge in einer Pipeline]**

Dieses Aktionsmodul versucht erneut fehlgeschlagene Builds in einer Pipeline.

Informationen zu Feldern finden Sie unter [Wiederholen von Aufträgen in einer Pipeline](https://docs.gitlab.com/ee/api/pipelines.html#retry-jobs-in-a-pipeline) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Variable abrufen]**

Dieses Modul ruft Details der spezifischen Variablen eines Projekts ab.

Informationen zu Feldern finden Sie unter [Anzeigen von Variablendetails](https://docs.gitlab.com/ee/api/project_level_variables.html#show-variable-details) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Update einer Version]**

Dieses Aktionsmodul aktualisiert eine Version.

Informationen zu Feldern finden Sie unter [Aktualisieren einer Version](https://docs.gitlab.com/ee/api/releases/#update-a-release) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Aktualisieren der Zusammenführungsanforderung]**

Dieses Aktionsmodul aktualisiert eine vorhandene Zusammenführungsanfrage. Sie können die Zielverzweigung, den Titel oder sogar das MR schließen.

Informationen zu Feldern finden Sie unter [Aktualisierungsanforderung für Zusammenführung](https://docs.gitlab.com/ee/api/merge_requests.html#update-mr) in der Dokumentation zu [!DNL GitLab].

+++

+++**[!UICONTROL Variable aktualisieren]**

Dieses Aktionsmodul aktualisiert die -Variable eines Projekts.

Informationen zu Feldern finden Sie unter [Variable aktualisieren](https://docs.gitlab.com/ee/api/project_level_variables.html#update-variable) in der Dokumentation zu [!DNL GitLab].

+++
