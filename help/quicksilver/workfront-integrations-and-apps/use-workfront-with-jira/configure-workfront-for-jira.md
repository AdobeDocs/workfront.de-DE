---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Konfigurieren von  [!DNL Adobe Workfront for Jira]
description: Sie können [!DNL Adobe Workfront for Jira] zur Integration Ihrer [!DNL Jira] und [!DNL Workfront] Systeme verwenden.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 43afa8136e51332a0970b01fff36113d5bf42294
workflow-type: tm+mt
source-wordcount: '2384'
ht-degree: 0%

---

# Konfigurieren von [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->

Sie können [!DNL Adobe Workfront for Jira] verwenden, um Ihre [!DNL Jira]- und [!DNL Workfront]-Systeme zu integrieren.

Nach der Installation des Add-ons können Sie Workflows definieren, die bei der Erstellung von [!DNL Workfront] Arbeitselementen automatisch [!DNL Jira] Probleme verursachen. Die Elemente in beiden Anwendungen werden verknüpft und einige ihrer Informationen werden automatisch in beiden Systemen aktualisiert.

Alle Benutzer in [!DNL Workfront] und [!DNL Jira] können von dieser Integration profitieren. Sie benötigen nur eine Lizenz für das System, in dem sie am besten funktionieren, und nicht für beide Systeme.

Dieses Add-on ist sowohl für die [!UICONTROL Server]- als auch für die [!UICONTROL OnDemand]- (oder [!UICONTROL Cloud]-) Version der [!DNL Jira] -Software verfügbar.

Eine Liste der [!DNL Jira] Versionen, die [!DNL Workfront for Jira] derzeit unterstützt, finden Sie unter [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) unter [!DNL Atlassian Marketplace].

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] plan]</td> 
   <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: [!UICONTROL Pro] oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Neu: [!UICONTROL Standard] </p>
       <p>oder</p> 
       <p>Aktuell: [!UICONTROL Plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in [!DNL Jira] und [!DNL Workfront] zu erstellen, um diese Integration zu widmen, anstatt vorhandene zu Benutzern gehörende Konten zu verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie [!DNL Workfront for Jira] konfigurieren können, müssen Sie:

* Installieren Sie [!DNL Workfront for Jira].
Anweisungen zum Installieren von [!DNL Workfront for Jira] finden Sie unter [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Konfigurieren von [!DNL Workfront for Jira]

Durch die Konfiguration von [!DNL Workfront for Jira] können Sie:

* Definieren Sie Trigger, die [!DNL Jira] Elemente erstellen, wenn [!DNL Workfront] Elemente erstellt werden.
* Geben Sie an, welche Felder zwischen den zwischen [!DNL Jira] und [!DNL Workfront] verknüpften Elementen synchronisiert werden sollen.

>[!NOTE]
>
>* Nachdem Sie [!DNL Workfront for Jira] in Ihrer [!DNL Jira] -Umgebung konfiguriert haben, sehen alle [!DNL Jira] -Benutzer ein [!DNL Workfront] rechtes Bedienfeld für alle [!DNL Jira] -Elemente. Das Bedienfeld enthält Informationen zu den Elementen, die möglicherweise mit [!DNL Workfront] verknüpft sind, oder gibt an, dass keine [!DNL Workfront] Elemente mit [!DNL Jira] Elementen verknüpft sind.
>* Bei Verwendung der Installation von [!DNL Jira Server] wird nur das Bedienfeld Workfront angezeigt, wenn Probleme im Zusammenhang mit Projekten auftreten, die als Trigger für die Workfront-Integration identifiziert wurden. Weitere Informationen zum Einrichten von Triggern für den Workflow [!DNL Workfront to Jira] finden Sie unter [Konfigurieren von Triggern für die automatische Verknüpfung von Elementen zwischen  [!DNL Jira]  und  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

So konfigurieren Sie [!DNL Workfront for Jira]:

1. Melden Sie sich bei [!DNL Jira] als [!DNL Jira] -Administrator an.
1. Klicken Sie im Hauptmenü von [!DNL Jira] auf **[!UICONTROL Einstellungen]** .
1. Klicken Sie auf **[!UICONTROL Add-ons]** und dann auf **[!UICONTROL Add-ons verwalten]**.

1. Erweitern Sie das Add-on **[!DNL Workfront]** .
1. Klicken Sie auf **[!UICONTROL Konfigurieren]**.
1. Befolgen Sie die Anweisungen zum Anmelden bei [!DNL Workfront].

   >[!NOTE]
   >
   >Der Benutzer muss über einen gültigen `apiKey` in [!UICONTROL Workfront] verfügen, um eine erfolgreiche Verbindung herzustellen.

   Sie müssen sich als [!DNL Workfront] -Administrator bei [!DNL Workfront] anmelden, um die Konfiguration fortzusetzen.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] stellt mithilfe von OAuth 2.0 eine Verbindung zu [!DNL Jira] her, einem Standard, der von den meisten webbasierten Integrationen für die Authentifizierung und Autorisierung von Benutzern verwendet wird.
   >* Wenn Sie aufgefordert werden, die Domäne Ihres [!DNL Workfront]-Kontos einzugeben, geben Sie es in folgendem Format ein: *sDomain.my.workfront.com* Ihres Unternehmens. Die Domäne Ihres Unternehmens ist normalerweise der Name Ihres Unternehmens.
   >* Die erweiterte Authentifizierung ist erst verfügbar, wenn ein [!DNL Workfront] -Administrator sie für diese Integration aktiviert hat.

1. Wählen Sie in Jira die Registerkarte **[!UICONTROL Trigger]** aus, um die automatische Erstellung von [!DNL Jira] Elementen zu konfigurieren, während neue [!DNL Workfront] Elemente erstellt werden.

   Weitere Informationen zum Einrichten von Triggern für den Workflow Workfront auf [!DNL Jira] finden Sie unter [Konfigurieren von Triggern für die automatische Verknüpfung von Elementen zwischen  [!DNL Jira]  und  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Wählen Sie die Registerkarte **[!UICONTROL Einrichtung]** aus, um die Synchronisierung der Felder zwischen verknüpften [!DNL Jira] - und [!DNL Workfront] -Elementen zu konfigurieren.

   Weitere Informationen zum Einrichten der Synchronisierung von Feldern zwischen [!DNL Jira] und [!DNL Workfront] finden Sie unter [Konfigurieren der Feldsynchronisierung zwischen  [!DNL Jira] und [!DNL Workfront] Elementen](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Nachdem Sie die Trigger und die Synchronisation der Felder zwischen den beiden Anwendungen definiert haben, kann jeder [!DNL Workfront]-Benutzer, der Aufgaben oder Probleme erstellen kann, möglicherweise die Erstellung eines Elements in [!DNL Jira] Trigger haben. Der Benutzer kann ein Element erstellen, wenn die Kriterien für das Element, das er erstellt, mit den Triggern in [!DNL Jira] übereinstimmen, selbst wenn der Benutzer nicht über eine [!DNL Jira] -Lizenz verfügt. Außerdem kann jeder [!DNL Jira] -Benutzer sofort mit der Arbeit am [!DNL Jira] -Element beginnen, und seine Aktualisierungen sind in [!DNL Workfront] sichtbar, ohne dass er über eine [!DNL Workfront] -Lizenz verfügt. Alle Aktualisierungen in [!DNL Workfront] sind auch in den [!DNL Jira] -Elementen sichtbar.

1. (Optional) Wählen Sie die Registerkarte **[!UICONTROL Aktivitätsprotokoll]** aus, um etwaige Fehler zu überprüfen, die während der Integration aufgetreten sind.

   Weitere Informationen zum [!UICONTROL Aktivitätsprotokoll] finden Sie unter [Anzeigen des [!DNL Jira] [!UICONTROL Aktivitätsprotokolls]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Konfigurieren von Triggern für die automatische Verknüpfung von Elementen zwischen [!DNL Jira] und [!DNL Workfront]

Als Systemadministrator von [!DNL Jira] können Sie Trigger definieren, die in [!DNL Jira] automatisch Probleme verursachen, wenn ein Element in [!DNL Workfront] bestimmte Kriterien erfüllt.

>[!NOTE]
>
>Es kann bis zu 10 Minuten dauern, bis die Integration neue Probleme in [!DNL Jira] erstellt.

Beachten Sie Folgendes bei der Konfiguration, die die Erstellung von [!DNL Jira] -Elementen auslöst, da [!DNL Workfront] -Elemente erstellt werden:

* Die Integration ist unidirektional: Sie können nur Elemente, die Sie in [!DNL Workfront] erstellen, in [!DNL Jira] automatisch erstellen lassen. Es ist nicht möglich, Elemente, die Sie in [!DNL Jira] erstellen, automatisch in [!DNL Workfront] zu erstellen.
* Es gibt keine Beschränkung für die Anzahl der Trigger, die Sie haben können.
* Wenn ein Element, das Sie in [!DNL Workfront] erstellen, mehr als einem der Trigger entspricht, wird nur ein Element in [!DNL Jira] erstellt. Das Element wird in [!DNL Jira] gemäß dem ersten Trigger erstellt (in der Reihenfolge, in der sie in [!DNL Jira] definiert wurden). Alle anderen Trigger werden ignoriert.
* Nur ein Element in [!DNL Workfront] kann mit einem Element in Jira verknüpft werden. Sie können nie ein [!DNL Workfront] Element mit mehreren [!DNL Jira] Problemen oder ein [!DNL Jira] Problem mit mehreren [!DNL Workfront] Elementen verknüpfen.

So konfigurieren Sie Trigger für das automatische Erstellen von Elementen in [!DNL Jira]:

1. Melden Sie sich bei [!DNL Jira] als Systemadministrator an.
1. Klicken Sie im Hauptmenü von [!DNL Jira] auf **[!UICONTROL Einstellungen]** .
1. Klicken Sie auf **[!UICONTROL Add-ons]** und dann auf **[!UICONTROL Add-ons verwalten]**.
1. Erweitern Sie das Add-on **[!DNL Workfront]** .
1. Klicken Sie auf **[!UICONTROL Konfigurieren]**.
1. Melden Sie sich bei [!DNL Workfront] als Systemadministrator an.

   Die Registerkarte **[!UICONTROL Trigger]** ist in Jira standardmäßig ausgewählt.

1. Klicken Sie auf **[!UICONTROL Trigger hinzufügen]** , um einen neuen Trigger hinzuzufügen.
1. Geben Sie im Feld **[!UICONTROL Workfront-Team/Benutzer/Rolle]** den Namen eines [!DNL Workfront]-Teams, Benutzers oder einer Rolle an und klicken Sie dann auf , um die Rolle auszuwählen, wenn sie in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie können nicht mehrere Trigger für dasselbe Team, denselben Benutzer oder dieselbe Rolle haben.

   Wenn jemand eine Aufgabe oder ein Problem erstellt und sie einer dieser Entitäten zuweist, wird automatisch ein Problem in [!DNL [!DNL Jira]] erstellt.

1. Geben Sie im Feld **[!UICONTROL [!DNL Jira]Projekt]** den Namen eines [!DNL Jira] -Projekts ein und klicken Sie dann auf , um es auszuwählen, wenn es in der Liste angezeigt wird.

   Wenn das Problem [!DNL Jira] erstellt wird, wird es in das hier ausgewählte Projekt eingefügt.

1. Wählen Sie einen **I[!UICONTROL sicheren Typ]** aus dem Dropdownmenü aus.

   Dies gibt den Ausgabetyp an, der in [!DNL Jira] erstellt wird, wenn die Bedingungen dieses Triggers erfüllt sind, basierend auf Ihren Einstellungen für dieses spezifische Projekt in [!DNL Jira].

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Mit dieser Konfiguration wird jedes Mal, wenn ein [!DNL Workfront] -Benutzer ein Element erstellt, das den angegebenen Triggern entspricht, ein neues Problem in [!DNL Jira] erstellt.

## Konfigurieren der Feldsynchronisierung zwischen [!DNL Jira] und [!DNL Workfront] Elementen

Als Administrator von [!DNL Jira] können Sie definieren, welche Felder automatisch für Elemente synchronisiert werden sollen, die zwischen [!DNL Workfront] und Jira verknüpft sind. Bestimmte Felder können vom Element [!DNL Workfront] mit dem Element [!DNL Jira] synchronisiert werden, andere von Jira mit Workfront.

So definieren Sie, welche Felder automatisch für Elemente synchronisiert werden sollen, die zwischen den beiden Anwendungen verknüpft sind:

1. Melden Sie sich bei [!DNL Jira] als Jira-Administrator an.
1. Klicken Sie im Hauptmenü von [!DNL Jira] auf **[!UICONTROL Einstellungen]** .
1. Klicken Sie auf **[!UICONTROL Add-ons]** und dann auf **[!UICONTROL Add-ons verwalten]**.
1. Erweitern Sie das Add-on **[!DNL Workfront]** .
1. Klicken Sie auf **[!UICONTROL Konfigurieren]**.
1. Melden Sie sich bei [!DNL Workfront] als Workfront-Administrator an.
1. Klicken Sie in Jira auf die Registerkarte **[!UICONTROL Einrichtung]** .
1. Wählen Sie im Abschnitt **[!UICONTROL Von Workfront zu Jira synchronisieren]** die Felder aus, die Sie in [!DNL Jira] aktualisieren möchten, wenn sie in Workfront aktualisiert werden.

   1. Wählen Sie eine der folgenden Frequenzen aus, mit denen die Felder synchronisiert werden:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Bei Erstellung]</td>
              <td>Die von Ihnen angegebenen Felder werden bei der Erstellung des Elements in Workfront zwischen den verknüpften Workfront- und [!DNL Jira]-Elementen synchronisiert.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Immer]</td>
              <td>Die von Ihnen angegebenen Felder werden zwischen den verknüpften Workfront- und [!DNL Jira]-Elementen synchronisiert, wenn die Felder in Workfront aktualisiert werden. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Nie]</td>
              <td>Die Felder, die Sie angeben, werden nie zwischen den verknüpften [!DNL Workfront] - und [!DNL Jira] -Elementen synchronisiert. In [!DNL Jira] gibt es keinen Hinweis darauf, dass das Feld in [!DNL Workfront] aktualisiert wurde. </td>
          </tr>
      </table>

   1. Wählen Sie eine der folgenden Optionen aus, um die Felder von [!DNL Workfront] auf [!DNL Jira] zu synchronisieren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Der Name einer Aufgabe oder eines Problems in [!DNL Workfront] wird zum Namen des Problems, mit dem es in [!DNL Jira] verknüpft ist.</p><p>Hinweis: Wenn neue Elemente in [!DNL Jira] automatisch erstellt werden, wird der [!DNL Workfront] Name immer für das Element [!DNL Jira] aktualisiert, unabhängig davon, ob dieses Feld hier aktiviert ist oder nicht. Wenn ein Element [!DNL Jira] manuell mit einem Element [!DNL Workfront] verknüpft wird, wird der Name des Elements [!DNL Workfront] nur in [!DNL Jira] aktualisiert, wenn Sie auf <strong>Immer</strong> klicken, um dieses Feld zu synchronisieren. Weitere Informationen zum manuellen oder automatischen Verknüpfen von Elementen finden Sie unter <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Elemente zwischen [!DNL Adobe Workfront] und [!DNL Jira]</a> verknüpfen.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Beschreibung]</td>
         <td>Die Beschreibung einer Aufgabe oder eines Problems in [!DNL Workfront] wird zur Beschreibung des Problems, mit dem sie in [!DNL Jira] verknüpft ist.</td>
        </tr>
        <tr>
         <td role="rowheader">Dokumente</td>
         <td><p>Dokumente, die mit einer Aufgabe oder einem Problem in [!DNL Workfront] verknüpft sind, sind ebenfalls an das Problem angehängt, mit dem sie in Jira verknüpft ist. Neue Dokumentversionen von [!DNL Workfront] werden Jira als separate Dokumente hinzugefügt und mit <i>_v&lt;Versionsnummer&gt;</i> angehängt, um die nummerierte Version in Workfront anzugeben. </p><p>Wenn beispielsweise der Name eines Dokuments in [!DNL Workfront] "<strong>Hauptanzeige</strong>"lautet und Sie ihm eine neue Version in [!DNL Workfront] hinzufügen, wird die neue Version als neues Dokument mit dem Namen "<strong>Hauptanzeige_v2</strong>"in "[!DNL Jira]"übertragen.</p><p>Wichtig: <p>Beachten Sie beim Synchronisieren von Dokumenten Folgendes:</p>
           <ul>
            <li><p>Dokumente, die größer als 5 MB sind, werden nicht synchronisiert. Wenn die Dokumentsynchronisierung fehlschlägt, weil das Dokument zu groß ist, wird ein Fehler im Aktivitätsprotokoll protokolliert. </p><p>Weitere Informationen zum Aktivitätsprotokoll finden Sie unter <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Anzeigen des Jira-Aktivitätsprotokolls</a>.</p></li>
            <li><p>Dokumente, die mit Aufgaben und Problemen von externen Servern verknüpft sind, werden nicht in die [!DNL Jira] -Elemente übertragen. Nur Dokumente, die direkt in die Aufgabe oder das Problem in [!DNL Workfront] hochgeladen wurden, werden in das verknüpfte Problem in [!DNL Jira] übertragen.</p></li>
            <li><p>Um einen Testversand aus einem Dokument zu erstellen, müssen Sie den Testversand in [!DNL Workfront] generieren. </p><p>Weitere Informationen zum Generieren eines Testversands finden Sie unter <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Erstellen eines Testversands für ein vorhandenes Dokument </a> in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Erstellen eines Testversands für ein Dokument</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Geplantes Abschlussdatum]</td>
         <td><p>Das geplante [!UICONTROL Abschlussdatum] einer Aufgabe oder eines Problems in [!DNL Workfront] wird zum [!UICONTROL Fälligkeitsdatum] des Problems, mit dem sie in [!DNL Jira] verknüpft ist.</p><p>Hinweis: Stellen Sie sicher, dass Sie "<strong>[!UICONTROL Fälligkeitsdatum]</strong>" bei [!DNL Jira] -Problemen anzeigen, damit dieser Wert synchronisiert wird.</p></td>
        </tr>
       </tbody>
      </table>

1. Wählen Sie im Abschnitt **[!UICONTROL Von [!DNL Jira] zu[!DNL Workfront]]** synchronisieren die Felder aus, die Sie in [!DNL Workfront] aktualisieren möchten, wenn sie in [!DNL Jira] aktualisiert werden.

   1. Wählen Sie eine der folgenden Frequenzen aus, mit denen die Felder synchronisiert werden:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Immer]</td>
         <td>Die von Ihnen angegebenen Felder werden immer zwischen den verknüpften [!DNL Workfront] - und [!DNL Jira] -Elementen synchronisiert, wenn die Felder in [!DNL Jira] aktualisiert werden. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Nie]</td>
         <td><p>Die Felder, die Sie angeben, werden nie zwischen den verknüpften [!DNL Workfront] - und [!DNL Jira] -Elementen synchronisiert. In [!DNL Workfront] gibt es keinen Hinweis darauf, dass das Feld in [!DNL Jira] aktualisiert wurde. </p><p>Hinweis: Wenn Sie Nie auswählen, können die Felder [!DNL Workfront] weiterhin manuell von [!DNL Jira] im linken Bereich [!DNL Workfront] des Problems [!DNL Jira] aktualisiert werden. Diese Aktualisierungen werden nur für [!DNL Workfront] Elemente in [!DNL Jira] und [!DNL Workfront] und nicht für [!DNL Jira] Elemente angezeigt.</p></td>
        </tr>
       </tbody>
      </table>

   1. Wählen Sie diese Option, um eines der folgenden Felder von [!DNL Jira] auf [!DNL Workfront] zu synchronisieren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>Der [!UICONTROL Status] eines Problems in [!DNL Jira] wird zum [!UICONTROL Status] der Aufgabe oder des Problems, mit der/dem es in [!DNL Workfront] verknüpft ist.<br>Weitere Informationen zu [!DNL Workfront] -Status finden Sie unter <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Zuweisung]</td>
         <td><p>Der [!UICONTROL Verantwortliche] eines Problems in [!DNL Jira] wird zum [!UICONTROL Verantwortlichen] der Aufgabe oder des Problems, mit der/dem es in [!DNL Workfront] verknüpft ist.</p><p>Wichtig: Wenn Sie ein Element in [!DNL Jira] einem Benutzer zuweisen, der kein [!DNL Workfront] -Konto hat, erstellt die Integration einen neuen aktiven Benutzer nur dann in [!DNL Workfront], wenn <strong>automatisch einen Benutzer in [!DNL Workfront] erstellt, wenn der [!DNL Jira] -Benutzer kein [!DNL Workfront] -Konto</strong> auf <strong>[!UICONTROL Immer]</strong> gesetzt ist. Dieser Benutzer besitzt keine [!DNL Workfront] -Lizenz. Aktive Benutzer können Arbeitselementen in [!DNL Workfront] zugewiesen werden, können jedoch nicht in Aktualisierungen einbezogen werden. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Anlagen eines Problems in [!DNL Jira] sind auch an die Aufgabe oder das Problem angehängt, mit der es in [!DNL Workfront] verknüpft ist. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Kommentare]</td>
         <td><p>Ein Kommentar zu einem [!DNL Jira] -Problem wird auch auf dem verknüpften [!DNL Workfront] -Element im Bereich [!UICONTROL Updates] veröffentlicht. Umgekehrt wird ein Kommentar, der im Bereich [!UICONTROL Updates] für eine [!DNL Workfront] -Aufgabe oder ein Problem veröffentlicht wird, mit dem nativen Kommentar-Stream von [!DNL Jira] für das verknüpfte Problem synchronisiert. </p><p>Standardmäßig ist dies auf <strong>[!UICONTROL Immer]</strong> gesetzt. Wenn Sie hier <strong>[!UICONTROL Nie]</strong> auswählen, können Sie Kommentare manuell für ein verknüpftes Element entweder in [!DNL Workfront] oder in [!DNL Jira] posten.</p></td>
        </tr>
       </tbody>
      </table>

1. Wählen Sie im Abschnitt **[!UICONTROL SONSTIGES]** aus, welche zusätzlichen Felder zwischen verknüpften Elementen aktualisiert werden sollen.

   1. Wählen Sie eine Option aus, um zu bestimmen, ob die Felder, die Sie für **[!UICONTROL Always]** oder **[!UICONTROL Nie]** angeben, in [!DNL Jira] oder [!DNL Workfront] aktualisiert werden, wenn sie geändert werden.

   1. Wählen Sie aus den folgenden Feldern und Updates aus:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Kopieren [!DNL Workfront] Benutzerdefinierte Daten im rechten Bereich in [!DNL Jira]]</td>
         <td><p>Zeigt die [!DNL Workfront] benutzerdefinierten Daten eines Elements im rechten Bereich [!DNL Workfront] an.</p><p>Hinweis: Die Abschnitte "Benutzerdefiniertes Formular"werden im rechten Bereich von [!DNL Workfront] mit der Zugriffsebene des [!DNL Workfront] Systemadministrators angezeigt.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Kopieren [!DNL Workfront] Priorität im rechten Bereich in [!DNL Jira]]</td>
         <td>Zeigt die [!DNL Workfront] Priorität eines Elements im rechten Bereich [!DNL Workfront] an.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Fügen Sie auf der Registerkarte [!DNL Workfront] Aktualisierungen ein Update über die Änderungen am Fälligkeitsdatum in [!DNL Jira] hinzu.]</td>
         <td>Fügt auf der Registerkarte [!UICONTROL Update] des Elements [!DNL Workfront] einen Kommentar hinzu, wenn sich das Fälligkeitsdatum von [!UICONTROL in dem verknüpften Element [!DNL Jira] ändert.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Benutzer in [!DNL Workfront] automatisch erstellen, wenn der [!DNL Jira]-Benutzer kein [!DNL Workfront]-Konto hat]</td>
         <td><p>Die folgenden Szenarien existieren:</p>
          <ul>
           <li>Wenn Sie "<strong>[!UICONTROL Immer]</strong>"auswählen, aktivieren Sie die Integration, damit jedes Mal ein neuer Workfront-Benutzer erstellt wird, wenn ein [!DNL Jira] Benutzer ohne ein [!DNL Workfront] -Konto die folgenden Aktionen für ein verknüpftes [!DNL Jira] -Problem durchführt:
            <ul>
             <li>Wird einem [!DNL Jira] -Problem zugewiesen</li>
             <li><p>Protokolliert die Zeit auf ein [!DNL Jira] -Problem</p><p>Dieser neue Benutzer besitzt keine [!DNL Workfront] -Lizenz. Die Standardeinstellung ist "Immer". Der auf diese Weise in [!DNL Workfront] erstellte Benutzer hat den Namen "[!UICONTROL Jira]"hinzugefügt.</p></li>
            </ul></li>
           <li>Wenn Sie <strong>[!UICONTROL Nie]</strong> auswählen, passiert Folgendes:
            <ul>
             <li>Sie können keine [!DNL Jira]-Zuweisungen für die [!DNL Workfront]-Elemente sehen. In diesem Fall werden nur in [!DNL Workfront] vorgenommene Zuweisungen für die Elemente [!DNL Workfront] angezeigt.</li>
             <li>Die Zeit, die ein Benutzer ohne [!DNL Workfront] -Konto bei einem verknüpften [!DNL Jira]-Problem protokolliert, wird nicht automatisch auf das verknüpfte [!DNL Workfront]-Element übertragen. Sie können die Zeit für das Element [!DNL Workfront] im rechten Bereich des Problems [!DNL Jira] protokollieren.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Jedes Mal, wenn ein Benutzer eines der in dieser Konfiguration angegebenen Felder für ein Element in [!DNL Jira] oder [!DNL Workfront] aktualisiert, wird das verknüpfte Element in der anderen Anwendung ebenfalls aktualisiert.

## Fehlerbehebung

### Elemente können nicht in [!DNL Jira] erstellt werden, da Trigger-Felder mit der Markierung &quot;[!UICONTROL konnte nicht gefunden werden]&quot;

#### Problem

Wenn bei der [!DNL Workfront for Jira] -Anwendung ein Fehler auftritt, deaktiviert [!DNL Workfront] die Trigger, um weitere Komplikationen zu vermeiden. Wenn diese Trigger deaktiviert sind, werden sie als &quot;[!UICONTROL konnte nicht gefunden werden]&quot; angezeigt.

#### Lösung

Suchen Sie den Fehler, der die Trigger deaktiviert hat. Sie finden den Fehler im [!DNL Workfront for Jira] [!UICONTROL Aktivitätsprotokoll].

Die häufigste Ursache für dieses Verhalten ist der Fehler &quot;[!UICONTROL Feld &#39;edate&#39; kann nicht festgelegt werden. Er befindet sich nicht auf dem entsprechenden Bildschirm oder ist unbekannt.]&quot;

Dieser Fehler bedeutet, dass Sie versuchen, das &quot;[!UICONTROL geplante Abschlussdatum]&quot; von [!DNL Workfront] mit [!DNL Jira] zu synchronisieren. Dazu müssen Sie sicherstellen, dass Ihre [!DNL Jira] -Objekte über ein Feld mit dem Namen &quot;[!UICONTROL Fälligkeitsdatum]&quot;verfügen. Wenn das Feld nicht ausgefüllt ist, kann [!DNL Workfront] das geplante Abschlussdatum nicht mit [!DNL Workfront] synchronisieren und Ihre Trigger deaktivieren.

Um diesen Fehler zu beheben, führen Sie einen der folgenden Schritte aus:

* Bitten Sie Ihren [!DNL Jira] -Administrator, die betroffenen [!DNL Jira] -Objekte zu aktualisieren, um sicherzustellen, dass sie über ein Fälligkeitsfeld verfügen.
* Deaktivieren Sie die Synchronisierung des geplanten Abschlussdatums von [!DNL Workfront] auf der Workfront-Seite [!UICONTROL Einrichtung] .
