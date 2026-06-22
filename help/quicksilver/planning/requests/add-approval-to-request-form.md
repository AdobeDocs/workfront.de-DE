---
title: Hinzufügen einer Genehmigung zu einem Anforderungsformular in Adobe Workfront Planning
description: Sie können einem Adobe Workfront Planning-Anforderungsformular einen Genehmigungsprozess hinzufügen, um für jede gesendete Anforderung eine Genehmigung zu starten, bevor ein Datensatz erstellt wird.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/E9LEGJ8T822JuvIO3s8nn6UkLbX-j4ffwaKSviKxl0o
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 930
ht-degree: 3%

---

# Hinzufügen einer Genehmigung zu einem Anfrageformular in Adobe Workfront-Planung

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

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

* Sie können einem Anfrageformular eine oder mehrere genehmigende Personen hinzufügen. Sie können Benutzer und Teams als genehmigende Personen hinzufügen.
* Sie können Genehmigungsinformationen zu einem Datensatz anzeigen, der durch Senden eines Anforderungsformulars in den Feldern Genehmigt von und Genehmigt am erstellt wurde. Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).
* Wenn Sie einem Anfrageformular mehrere genehmigende Personen hinzufügen, müssen alle genehmigenden Personen die Anfrage akzeptieren, bevor in Workfront Planning ein Datensatz erstellt wird.
* Wenn alle genehmigenden Personen die Anfrage genehmigen, wird ein Datensatz für den mit dem Anfrageformular verknüpften Datensatztyp erstellt.
* Wenn mindestens eine genehmigende Person die Anforderung ablehnt und alle anderen sie genehmigen, wird eine Anforderung für den Bereich Anfragen in Workfront erstellt, aber es wird kein Datensatz für den Datensatztyp erstellt, der mit dem Anfrageformular verknüpft ist.
* Das Hinzufügen von Genehmigungen zu einem Anfrageformular ist optional. Workfront Planning erstellt beim Senden einer Anfrage sofort einen Datensatz, wenn das Anforderungsformular nicht mit einer Genehmigung verknüpft ist.

<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->

## Hinzufügen von Genehmigungsregeln zu einem Anfrageformular

Genehmigungsregeln definieren den Genehmigungsprozess basierend auf den Feldwerten in den gesendeten Anfragen.

Wenn beispielsweise ein Anfrageformular das Feld „Kampagnentyp“ aufweist, kann eine Regel erstellt werden, die die Anfrage an eine Person sendet, wenn das Feld den Wert „Digital“ hat, und an eine andere Person, wenn es den Wert „Drucken“ hat.

Beachten Sie beim Hinzufügen von Genehmigungsregeln Folgendes:

* Sie können einer Genehmigungsregel eine oder mehrere genehmigende Personen hinzufügen.
* Wenn mindestens eine genehmigende Person die Anforderung ablehnt, wird die Anforderung abgelehnt und der Datensatz nicht erstellt. Die Anfrage verbleibt im Bereich Anfragen von Workfront.
* Wenn Sie mehr als eine genehmigende Person hinzufügen und die Option Nur eine Entscheidung ist erforderlich nicht aktiviert ist, müssen alle genehmigenden Personen eine Entscheidung treffen, bevor eine Anfrage entweder genehmigt oder abgelehnt wird.
* Wenn ein Team als genehmigende Person festgelegt ist, ist von einem Teammitglied nur eine Entscheidung erforderlich.

So legen Sie Genehmigungsregeln für ein Anfrageformular fest:

1. Erstellen Sie zunächst ein Anfrageformular für einen Datensatztyp, wie im Artikel [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md) beschrieben.
1. Wenn das Anfrageformular geöffnet wird, klicken Sie auf **Einstellungen**.

   Die **Einstellungen** wird geöffnet.

1. Um mit der Konfiguration von Genehmigungsregeln zu beginnen, klicken Sie **Genehmigungen** ![Genehmigungssymbol](assets/approvals-icon-on-form.png) im linken Bereich.

1. (Optional) Wenn Sie einen standardmäßigen Genehmigungsprozess festlegen möchten, fügen Sie mindestens einen Benutzer oder ein Team zum Feld **Genehmigende Personen** im Bereich **Standardgenehmigungsregel** hinzu und klicken Sie dann auf das Kontrollkästchen **Nur eine Entscheidung ist erforderlich**, wenn Sie möchten, dass der Datensatz erstellt wird, nachdem eine der standardmäßigen genehmigenden Personen ihn genehmigt hat.

   ![Standardmäßiger Bereich für Genehmigungsregeln](assets/default-approvers.png)

1. (Optional) Beginnen Sie mit dem Hinzufügen von Genehmigungsregeln. Gehen Sie für jede benutzerdefinierte Genehmigungsregel wie folgt vor:

   1. Klicken Sie **Genehmigungsregel hinzufügen**
   1. Klicken Sie auf den Platzhaltertitel **Nicht benannte Genehmigungsregel** und geben Sie einen Namen für die Genehmigungsregel ein.
   1. Klicken Sie **Feld auswählen** und wählen Sie das Feld aus, das die Regel aktiviert.
   1. Wählen Sie den Operator für die Regel aus. Die Operatoren variieren je nach Feldtyp.
   1. Wenn der ausgewählte Operator einen Wert benötigt, klicken Sie auf das Pluszeichen und fügen Sie einen oder mehrere Werte hinzu.
   1. (Optional) Klicken Sie auf **Bedingung hinzufügen**, um weitere Bedingungen hinzuzufügen und sie durch **Und**- oder **Oder**-Anweisungen zu verbinden, indem Sie die zusätzlichen Bedingungen wie in den Schritten C-E konfigurieren.
   1. Fügen Sie im Bereich **Aktionen** der Genehmigungsregel im Feld **Genehmigende Personen** mindestens einen Benutzer oder ein Team hinzu, der bzw. das bei der genehmigenden Person festgelegt werden soll, wenn die Bedingung erfüllt ist.
   1. (Bedingt und optional) Wenn der Datensatz erstellt werden soll, nachdem eine der genehmigenden Personen ihn genehmigt hat, aktivieren Sie das Kontrollkästchen **Nur eine Entscheidung ist erforderlich**. Andernfalls müssen alle genehmigenden Personen über die Genehmigung entscheiden, bevor die Anforderung akzeptiert oder abgelehnt wird.

   >[!NOTE]
   >
   >   Beachten Sie beim Hinzufügen von Genehmigungsregeln Folgendes:
   >
   >   * Wenn nur eine Standardregel eingerichtet ist, gilt sie für jede gesendete Anfrage.
   >   * Wenn eine benutzerdefinierte Regel erfüllt ist, wird die Standardeinstellung nicht auf den Workflow für die Anfragegenehmigung angewendet. Für Genehmigungen gelten nur die passenden benutzerdefinierten Regeln, und die Standardregel wird ignoriert.
   >   * Wenn mehrere benutzerdefinierte Regeln erfüllt sind, gilt die erste in der Reihenfolge. In diesem Fall gilt die Standardgenehmigung nicht, falls eine solche vorhanden ist.

1. Klicken Sie **Speichern**, um die Genehmigungsregeln zu speichern.
1. (Optional) Klicken Sie auf **Veröffentlichen**, wenn Sie das Anfrageformular noch nie freigegeben haben.
