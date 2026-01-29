---
title: Hinzufügen einer Genehmigung zu einem Anforderungsformular in Adobe Workfront Planning
description: Sie können einem Adobe Workfront Planning-Anforderungsformular einen Genehmigungsprozess hinzufügen, um für jede gesendete Anforderung eine Genehmigung zu starten, bevor ein Datensatz erstellt wird.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: 2ffd06f2f50d14b6d33bc79c92616ebed1d58fed
workflow-type: tm+mt
source-wordcount: '1195'
ht-degree: 1%

---

# Hinzufügen einer Genehmigung zu einem Anforderungsformular in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können einem Adobe Workfront Planning-Anforderungsformular einen Genehmigungsprozess hinzufügen, um für jede gesendete Anforderung eine Genehmigung zu starten, bevor ein Datensatz erstellt wird.

In diesem Artikel wird beschrieben, wie ein Workspace-Manager einem Anfrageformular, das mit einem Datensatztyp verknüpft ist, eine Genehmigung hinzufügen kann.

Informationen zum Erstellen eines Anfrageformulars in Workfront Planning finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Weitere Informationen zum Senden einer Anfrage an einen Datensatztyp zum Erstellen eines Datensatzes finden Sie unter [Senden von Adobe Workfront Planning-Anfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<p>Jedes Workfront-Paket und jedes Planungspaket</p>
ODER
<p>Beliebiges Workflow-Paket und beliebiges Planungspaket</p>

<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und Datensatztyp</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Hinzufügen von Genehmigungen zu einem Anfrageformular

* Sie können einem Anfrageformular eine oder mehrere genehmigende Personen hinzufügen. Sie können nur Benutzer als genehmigende Personen hinzufügen.
* Sie können Genehmigungsinformationen zu einem Datensatz anzeigen, der durch Senden eines Anforderungsformulars in den Feldern Genehmigt von und Genehmigt am erstellt wurde. Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).
* Wenn Sie einem Anfrageformular mehrere genehmigende Personen hinzufügen, müssen alle genehmigenden Personen die Anfrage akzeptieren, bevor in Workfront Planning ein Datensatz erstellt wird.
* Wenn alle genehmigenden Personen die Anfrage genehmigen, wird ein Datensatz für den mit dem Anfrageformular verknüpften Datensatztyp erstellt.
* Wenn mindestens eine genehmigende Person die Anforderung ablehnt und alle anderen sie genehmigen, wird eine Anforderung für den Bereich Anfragen in Workfront erstellt, aber es wird kein Datensatz für den Datensatztyp erstellt, der mit dem Anfrageformular verknüpft ist.
* Das Hinzufügen von Genehmigungen zu einem Anfrageformular ist optional. Workfront Planning erstellt beim Senden einer Anfrage sofort einen Datensatz, wenn das Anforderungsformular nicht mit einer Genehmigung verknüpft ist.

## Hinzufügen einer Genehmigung zu einem Anfrageformular in der Produktionsumgebung

1. Erstellen Sie zunächst ein Anfrageformular für einen Datensatztyp, wie in [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md) beschrieben.
1. Klicken Sie **Konfiguration**.

   Der **Konfiguration** wird angezeigt.

   ![Registerkarte „Konfiguration“](assets/configuration-tab.png)
1. Beginnen Sie **Feld** Genehmigende Person“, den Namen einer Person oder eines Teams einzugeben, die bzw. das Sie als genehmigende Person festlegen möchten, und wählen Sie ihn aus, wenn er bzw. es in der Liste angezeigt wird.
1. (Optional und bedingt) Wenn Sie mehr als eine genehmigende Person eingerichtet haben und nur eine genehmigende Person benötigen, um eine Entscheidung zu treffen, aktivieren Sie die Option **Nur eine Entscheidung ist erforderlich**.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Sie können einem Anfrageformular eine oder mehrere genehmigende Personen hinzufügen.
   >
   >* Wenn Sie mehr als eine genehmigende Person hinzufügen und die Option Nur eine Entscheidung ist erforderlich nicht aktiviert ist, müssen alle genehmigenden Personen die Anfrage genehmigen, bevor Workfront Planning einen Datensatz erstellt.
   >
   >* Wenn mindestens eine genehmigende Person die Anforderung ablehnt, wird die Anforderung abgelehnt und der Datensatz nicht erstellt. Die Anfrage verbleibt im Bereich Anfragen von Workfront.
   >
   >* Wenn Sie mehr als eine genehmigende Person hinzufügen und die Option Nur eine Entscheidung ist erforderlich nicht aktiviert ist, müssen alle genehmigenden Personen eine Entscheidung treffen, bevor eine Anfrage entweder genehmigt oder abgelehnt wird.
   >
   >* Wenn ein Team als genehmigende Person festgelegt ist, ist nur eine Entscheidung vom Team erforderlich.


1. (Optional) Klicken Sie auf **Veröffentlichen**, wenn Sie das Anfrageformular noch nie freigegeben haben.

   ODER

   Klicken Sie auf **Freigeben**, um das Formular freizugeben, und **Link kopieren**.
1. (Optional) Nachdem ein(e) Benutzende(r) den von Ihnen freigegebenen Link verwendet und eine Anfrage gesendet hat, sendet Workfront Planning eine In-App-Benachrichtigung über die Genehmigung und eine E-Mail an die genehmigenden Personen.

   >[!NOTE]
   >
   >   Damit Benutzerinnen und Benutzer E-Mail- und In-App-Benachrichtigungen empfangen können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.


   Informationen zum Genehmigen von Anfragen finden Sie unter [Genehmigen einer Anfrage](/help/quicksilver/planning/requests/approve-request.md).

<div class="preview">

## Hinzufügen von Genehmigungsregeln zu einem Anfrageformular

>[!NOTE]
>
>Diese Funktion ist nur in der Vorschau-Umgebung verfügbar.

Genehmigungsregeln definieren den Genehmigungsprozess basierend auf den Feldwerten in den gesendeten Anfragen.

Wenn beispielsweise ein Anfrageformular das Feld „Kampagnentyp“ aufweist, kann eine Regel erstellt werden, die die Anfrage an eine Person sendet, wenn das Feld den Wert „Digital“ hat, und an eine andere Person, wenn es den Wert „Drucken“ hat.

Beachten Sie beim Hinzufügen von Genehmigungsregeln Folgendes:

* Sie können einer Genehmigungsregel eine oder mehrere genehmigende Personen hinzufügen.
* Wenn mindestens eine genehmigende Person die Anforderung ablehnt, wird die Anforderung abgelehnt und der Datensatz nicht erstellt. Die Anfrage verbleibt im Bereich Anfragen von Workfront.
* Wenn Sie mehr als eine genehmigende Person hinzufügen und die Option Nur eine Entscheidung ist erforderlich nicht aktiviert ist, müssen alle genehmigenden Personen eine Entscheidung treffen, bevor eine Anfrage entweder genehmigt oder abgelehnt wird.
* Wenn ein Team als genehmigende Person festgelegt ist, ist nur eine Entscheidung vom Team erforderlich.

Weitere Informationen zum Hinzufügen von Genehmigungen finden Sie [Genehmigung zu einem Anfrageformular hinzufügen](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

So legen Sie Genehmigungsregeln für ein Anfrageformular fest:

1. Erstellen Sie zunächst ein Anfrageformular für einen Datensatztyp, wie in [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md) beschrieben.
1. Klicken Sie auf **Einstellungen**.

   Die Registerkarte Einstellungen wird angezeigt.

1. Um mit der Konfiguration von Genehmigungsregeln zu beginnen, klicken Sie ![&#x200B; der linken Navigationsleiste auf Genehmigungen &#x200B;](assets/approvals-icon-on-form.png)Genehmigungssymbol).

1. (Optional) Wenn Sie einen Standardgenehmigungsprozess festlegen möchten, fügen Sie mindestens einen Benutzer oder ein Team zum Feld **Genehmigende Person** im Bereich Standardgenehmigungsregel hinzu. Aktivieren Sie dann das Kontrollkästchen **Nur eine Entscheidung ist erforderlich**, wenn der Datensatz erstellt werden soll, nachdem eine der Standardgenehmigenden ihn genehmigt hat.

   ![Standardmäßiger Bereich für Genehmigungsregeln](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (Optional) Gehen Sie für jede zusätzliche Genehmigungsregel wie folgt vor:

   1. Klicken Sie **Genehmigungsregel hinzufügen**
   1. Klicken Sie auf den Platzhaltertitel „Nicht benannte Genehmigungsregel“ und geben Sie einen Namen für die Genehmigungsregel ein.
   1. Klicken Sie **Feld auswählen** und wählen Sie das Feld aus, das die Regel aktiviert.
   1. Wählen Sie den Operator für die Regel aus. Die Operatoren variieren je nach Feldtyp.
   1. Wenn der ausgewählte Operator einen Wert benötigt, klicken Sie auf das Pluszeichen und fügen Sie einen oder mehrere Werte hinzu.
   1. (Optional) Fügen Sie weitere Bedingungen mit UND oder hinzu, indem Sie auf Bedingung hinzufügen klicken und die zusätzliche Bedingung wie in den Schritten C-E konfiguriert wird.
   1. Fügen Sie im Bereich Aktionen der Genehmigungsregel im Feld **Genehmigende Personen** mindestens einen Benutzer oder ein Team hinzu, der bzw. das bei der genehmigenden Person eingestellt werden soll, wenn die Bedingung erfüllt ist.
   1. &#x200B;
      1. (Bedingt) Wenn der Datensatz erstellt werden soll, nachdem eine der genehmigenden Personen ihn genehmigt hat, aktivieren Sie das Kontrollkästchen **Nur eine Entscheidung ist erforderlich**.

1. Klicken Sie **Speichern**, um die Genehmigungsregeln zu speichern.
1. (Optional) Klicken Sie auf **Veröffentlichen**, wenn Sie das Anfrageformular noch nie freigegeben haben.

</div>
