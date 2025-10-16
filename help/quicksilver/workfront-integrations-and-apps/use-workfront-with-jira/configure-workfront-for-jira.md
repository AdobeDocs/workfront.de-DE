---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Konfigurieren Sie [!DNL Adobe Workfront for Jira]
description: Sie können verwenden [!DNL Adobe Workfront for Jira]  um Ihre  [!DNL Jira] -Systeme  [!DNL Workfront]  integrieren.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '2454'
ht-degree: 0%

---

# Konfigurieren von [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>Um stabilere und skalierbarere Integrationen bereitzustellen, wechseln wir mithilfe von Workfront Automation and Integration (Fusion) zu einem modernen, flexiblen Integrationsansatz. Im Rahmen dieses Übergangsprozesses wird die Integration von Workfront für Jira nach dem 28. **2026 nicht mehr**.
>
>Es wird empfohlen, Workfront-Automatisierung und -Integration für die Integrationsanforderungen Ihres Unternehmens mit Jira zu verwenden.
>
>Einen Überblick über die Automatisierung und Integration von Workfront finden Sie unter [Übersicht über Adobe Workfront Fusion](https://experienceleague.adobe.com/de/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Informationen zu den spezifischen Funktionen der Workfront-Automatisierungs- und Integrationsmodule für Jira finden Sie unter [Jira-Softwaremodule](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Sie können [!DNL Adobe Workfront for Jira] verwenden, um Ihre [!DNL Jira]- und [!DNL Workfront] zu integrieren.

Nach der Installation des Add-ons können Sie Workflows definieren, die beim Erstellen von [!DNL Jira] automatisch [!DNL Workfront] Probleme verursachen. Die Elemente in beiden Anwendungen werden verknüpft, und einige ihrer Informationen werden automatisch in beiden Systemen aktualisiert.

Von dieser Integration können alle Anwender in [!DNL Workfront] und [!DNL Jira] profitieren. Sie benötigen lediglich eine Lizenz für das System, in dem sie am meisten arbeiten, und nicht für beide Systeme.

Dieses Add-on ist sowohl für die [!UICONTROL Server]- als auch für [!UICONTROL OnDemand]-Versionen (oder [!UICONTROL Cloud]) [!DNL Jira] Software verfügbar.

Eine Liste der [!DNL Jira] Versionen, die [!DNL Workfront for Jira] derzeit unterstützt, finden Sie unter [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) auf der [!DNL Atlassian Marketplace].

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard </p>
       <p>Plan </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Jira-Zugriff</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in Jira und Workfront zu erstellen, um diese Integration zu ermöglichen, anstatt vorhandene Konten zu verwenden, die an Benutzende angehängt sein könnten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie [!DNL Workfront for Jira] konfigurieren können, müssen Sie:

* Installieren Sie [!DNL Workfront for Jira].
Anweisungen zur Installation von [!DNL Workfront for Jira] finden Sie unter [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Konfigurieren von [!DNL Workfront for Jira]

Durch die Konfiguration von [!DNL Workfront for Jira] haben Sie folgende Möglichkeiten:

* Trigger definieren, die [!DNL Jira] Elemente erstellen, wenn [!DNL Workfront] Elemente erstellt werden.
* Geben Sie an, welche Felder zwischen Elementen synchronisiert werden sollen, die zwischen [!DNL Jira] und [!DNL Workfront] verknüpft sind.

>[!NOTE]
>
>* Nachdem Sie [!DNL Workfront for Jira] in Ihrer [!DNL Jira] konfiguriert haben, wird allen [!DNL Jira] Benutzern ein [!DNL Workfront] rechter Bereich für alle [!DNL Jira] Elemente angezeigt. Das Bedienfeld enthält Informationen zu den Elementen, die von [!DNL Workfront] aus verknüpft werden können, oder gibt an, dass keine [!DNL Workfront] Elemente mit [!DNL Jira] Elementen verknüpft sind.
>* Bei Verwendung der [!DNL Jira Server]-Installation wird das Bedienfeld Workfront nur für Probleme angezeigt, die mit Projekten verbunden sind, die als Trigger für die Workfront-Integration identifiziert wurden. Weitere Informationen zum Einrichten von Triggern für den [!DNL Workfront to Jira]-Workflow finden Sie unter [Konfigurieren von Triggern für die automatische Verknüpfung von Elementen zwischen  [!DNL Jira]  und  [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

So konfigurieren Sie [!DNL Workfront for Jira]:

1. Melden Sie sich bei [!DNL Jira] als [!DNL Jira] an.
1. Klicken Sie **[!UICONTROL Hauptmenü auf]** Einstellungen[!DNL Jira].
1. Klicken Sie **[!UICONTROL Add-ons]** und dann auf **[!UICONTROL Add-ons verwalten]**.

1. Erweitern Sie das Add-on **[!DNL Workfront]** .
1. Klicken Sie **[!UICONTROL Konfigurieren]**.
1. Befolgen Sie die Anweisungen, um sich bei [!DNL Workfront] anzumelden.

   >[!NOTE]
   >
   >Die Benutzerin bzw. der Benutzer muss über eine gültige `apiKey` in [!UICONTROL Workfront] verfügen, um eine erfolgreiche Verbindung herzustellen.

   Sie müssen sich bei [!DNL Workfront] als [!DNL Workfront] anmelden, um die Konfiguration fortzusetzen.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] stellt mithilfe von OAuth 2.0 eine Verbindung zu [!DNL Jira] her. Dies ist ein Standard, der von den meisten Web-basierten Integrationen zur Authentifizierung und Autorisierung von Benutzern verwendet wird.
   >* Wenn Sie aufgefordert werden, die Domain Ihres [!DNL Workfront] Kontos einzugeben, geben Sie sie in folgendem Format ein: *yourCompany&#39;sDomain.my.workfront.com*. Die Domain Ihres Unternehmens ist normalerweise der Name Ihres Unternehmens.
   >* Die erweiterte Authentifizierung ist erst verfügbar, wenn sie von einem [!DNL Workfront]-Administrator für diese Integration aktiviert wurde.

1. Wählen Sie in Jira die Registerkarte **[!UICONTROL Trigger]** aus, um die automatische Erstellung [!DNL Jira] Elemente zu konfigurieren, wenn neue [!DNL Workfront] erstellt werden.

   Weitere Informationen zum Einrichten von Triggern für den Workflow &quot;Workfront to [!DNL Jira]&quot; finden Sie unter [Konfigurieren von Triggern für die automatische Verknüpfung von Elementen zwischen  [!DNL Jira]  und [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Wählen Sie die **[!UICONTROL Setup]**, um die Synchronisierung von Feldern zwischen verknüpften [!DNL Jira] und [!DNL Workfront] zu konfigurieren.

   Weitere Informationen zum Einrichten der Feldsynchronisierung zwischen [!DNL Jira] und [!DNL Workfront] finden Sie unter [Konfigurieren der Feldsynchronisierung zwischen  [!DNL Jira]  und  [!DNL Workfront] Elementen](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Nachdem Sie die Trigger und die Synchronisierung von Feldern zwischen den beiden Anwendungen definiert haben, kann jeder [!DNL Workfront], der Aufgaben oder Probleme erstellen kann, möglicherweise Trigger bei der Erstellung eines Elements in [!DNL Jira] verursachen. Der/die Benutzende kann ein Element erstellen, wenn die Kriterien des von ihm/ihr erstellten Elements mit den Triggern in [!DNL Jira] übereinstimmen, auch wenn der/die Benutzende keine [!DNL Jira] hat. Außerdem kann jeder [!DNL Jira] Benutzer sofort mit der Arbeit am [!DNL Jira] beginnen, und seine Aktualisierungen sind in [!DNL Workfront] sichtbar, ohne dass er über eine [!DNL Workfront]-Lizenz verfügt. Alle Aktualisierungen in [!DNL Workfront] sind auch in den [!DNL Jira] Elementen sichtbar.

1. (Optional) Wählen Sie die Registerkarte **[!UICONTROL Aktivitätsprotokoll]**, um alle Fehler zu überprüfen, die während der Integration aufgetreten sein könnten.

   Weitere Informationen zum [!UICONTROL Aktivitätsprotokoll] finden Sie unter [Anzeigen  [!DNL Jira] [!UICONTROL Aktivitätsprotokolls]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Konfigurieren von Triggern für die automatische Verknüpfung von Elementen zwischen [!DNL Jira] und [!DNL Workfront]

Als [!DNL Jira] können Sie Trigger definieren, die automatisch Probleme in [!DNL Jira] verursachen, wenn ein Element in [!DNL Workfront] bestimmte Kriterien erfüllt.

>[!NOTE]
>
>Es kann bis zu 10 Minuten dauern, bis die Integration in [!DNL Jira] neue Probleme verursacht.

Beachten Sie beim Konfigurieren des Auslösers für die Erstellung von [!DNL Jira] beim Erstellen [!DNL Workfront] Elemente Folgendes:

* Trigger Die Integration ist unidirektional: Sie können nur Elemente, die Sie in erstellen, [!DNL Workfront] automatisch in [!DNL Jira] erstellt werden. Sie können Elemente, die Sie in erstellen, nicht [!DNL Jira], dass sie automatisch in [!DNL Workfront] erstellt werden, in Trigger setzen.
* Es gibt keine Begrenzung dafür, wie viele Trigger Sie haben können.
* Wenn ein Element, das Sie in [!DNL Workfront] erstellen, mit mehr als einem der Trigger übereinstimmt, wird nur ein Element in [!DNL Jira] erstellt. Das Element wird in [!DNL Jira] gemäß dem ersten Trigger erstellt (in der Reihenfolge, in der sie in [!DNL Jira] definiert wurden). Alle anderen Trigger werden ignoriert.
* Nur ein Element in [!DNL Workfront] kann mit einem Element in Jira verknüpft werden. Sie können niemals ein [!DNL Workfront] mit mehreren [!DNL Jira] oder ein [!DNL Jira] mit mehreren [!DNL Workfront] verknüpfen.

So konfigurieren Sie Trigger für die automatische Erstellung von Elementen in [!DNL Jira]:

1. Melden Sie sich bei [!DNL Jira] als Systemadministrator an.
1. Klicken Sie **[!UICONTROL Hauptmenü auf]** Einstellungen[!DNL Jira].
1. Klicken Sie **[!UICONTROL Add-ons]** und dann **[!UICONTROL Add-ons verwalten]**.
1. Erweitern Sie das Add-on **[!DNL Workfront]** .
1. Klicken Sie **[!UICONTROL Konfigurieren]**.
1. Melden Sie sich bei [!DNL Workfront] als Systemadministrator an.

   Die Registerkarte **** Trigger&quot; ist in Jira standardmäßig ausgewählt.

1. Klicken Sie **[!UICONTROL Trigger hinzufügen]**, um einen neuen Trigger hinzuzufügen.
1. Geben Sie im Feld **[!UICONTROL Workfront-Team/Benutzer/Rolle]** den Namen eines [!DNL Workfront]-Teams, eines Benutzers oder eines Aufgabengebiets an und klicken Sie dann auf das gewünschte Team, um es auszuwählen, wenn es in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie können nicht mehrere Trigger für dasselbe Team, denselben Benutzer oder dieselbe Rolle haben.

   Wenn jemand eine Aufgabe oder ein Problem erstellt und sie bzw. es einer dieser Entitäten zuweist, wird in [!DNL [!DNL Jira]] automatisch ein Problem erstellt.

1. Beginnen Sie im Feld **[!UICONTROL [!DNL Jira]Projekt]** mit der Eingabe des Namens eines [!DNL Jira] Projekts und klicken Sie dann, um es auszuwählen, wenn es in der Liste angezeigt wird.

   Wenn das [!DNL Jira] Problem erstellt wird, wird es in dem hier ausgewählten Projekt platziert.

1. Wählen Sie **Dropdown[!UICONTROL Menü einen]** Problemtyp) aus.

   Dies zeigt den Problemtyp an, der in [!DNL Jira] erstellt wird, wenn die Bedingungen dieses Triggers erfüllt sind, und zwar basierend auf Ihren Einstellungen für dieses spezifische Projekt in [!DNL Jira].

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Mit dieser Konfiguration wird jedes Mal, wenn ein [!DNL Workfront] ein Element erstellt, das den angegebenen Triggern entspricht, ein neues Problem in [!DNL Jira] erstellt.

## Konfigurieren der Feldsynchronisierung zwischen [!DNL Jira] und [!DNL Workfront] Elementen

Als [!DNL Jira] können Sie festlegen, welche Felder automatisch für Elemente synchronisiert werden sollen, die zwischen [!DNL Workfront] und Jira verknüpft sind. Bestimmte Felder können vom [!DNL Workfront] zum [!DNL Jira] synchronisiert werden, andere können von Jira zu Workfront synchronisiert werden.

So definieren Sie, welche Felder automatisch für Elemente synchronisiert werden sollen, die zwischen den beiden Anwendungen verknüpft sind:

1. Melden Sie sich bei [!DNL Jira] als Jira-Administrator an.
1. Klicken Sie **[!UICONTROL Hauptmenü auf]** Einstellungen[!DNL Jira].
1. Klicken Sie **[!UICONTROL Add-ons]** und dann **[!UICONTROL Add-ons verwalten]**.
1. Erweitern Sie das Add-on **[!DNL Workfront]** .
1. Klicken Sie **[!UICONTROL Konfigurieren]**.
1. Melden Sie sich bei [!DNL Workfront] als Workfront-Administrator an.
1. Klicken Sie in Jira auf die Registerkarte **[!UICONTROL Setup]**.
1. Wählen **[!UICONTROL im Abschnitt „Synchronisieren von Workfront mit Jira]** die Felder aus, die Sie in [!DNL Jira] aktualisieren möchten, wenn sie in Workfront aktualisiert werden.

   1. Wählen Sie eine der folgenden Frequenzen, mit denen die Felder synchronisiert werden sollen:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL bei Erstellung]</td>
              <td>Die angegebenen Felder werden zwischen den verknüpften Workfront- und [!DNL Jira]-Elementen synchronisiert, wenn das Element in Workfront erstellt wird.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Immer]</td>
              <td>Die angegebenen Felder werden zwischen den verknüpften Workfront- und [!DNL Jira]-Elementen synchronisiert, wenn die Felder in Workfront aktualisiert werden. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Never]</td>
              <td>Die angegebenen Felder werden nie zwischen den verknüpften [!DNL Workfront] und [!DNL Jira] Elementen synchronisiert. In [!DNL Jira] gibt es keinen Hinweis darauf, dass das Feld in [!DNL Workfront] aktualisiert wurde. </td>
          </tr>
      </table>

   1. Wählen Sie eine der folgenden Optionen aus, um die Felder von [!DNL Workfront] nach [!DNL Jira] zu synchronisieren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Der Name einer Aufgabe oder eines Problems in [!DNL Workfront] wird zum Namen des Problems, mit dem es bzw. es in [!DNL Jira] verknüpft ist.</p><p>Hinweis: Wenn neue Elemente in [!DNL Jira] automatisch erstellt werden, wird der [!DNL Workfront] immer für das [!DNL Jira] Element aktualisiert, unabhängig davon, ob dieses Feld hier aktiviert ist oder nicht. Wenn ein [!DNL Jira] Element manuell mit einem [!DNL Workfront] Element verknüpft wird, wird der Name des [!DNL Workfront] Elements nur in [!DNL Jira] aktualisiert, wenn Sie dieses Feld <strong>Immer</strong> synchronisieren. Weitere Informationen zum manuellen oder automatischen Verknüpfen von Elementen finden Sie unter <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Verknüpfen von Elementen zwischen [!DNL Adobe Workfront] und [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Beschreibung]</td>
         <td>Die Beschreibung einer Aufgabe oder eines Problems in [!DNL Workfront] wird zur Beschreibung des Problems, mit dem es bzw. es in [!DNL Jira] verknüpft ist.</td>
        </tr>
        <tr>
         <td role="rowheader">Dokumente</td>
         <td><p>Dokumente, die an eine Aufgabe oder ein Problem in [!DNL Workfront] angehängt sind, sind auch an das Problem angehängt, mit dem es in Jira verknüpft ist. Neue Dokumentversionen von [!DNL Workfront] werden Jira als separate Dokumente hinzugefügt und mit <i>_v&lt;Versionsnummer&gt;</i> angehängt, um die nummerierte Version in Workfront anzugeben. </p><p>Wenn beispielsweise der Name eines Dokuments in [!DNL Workfront] "<strong>" lautet </strong> Sie ihm in [!DNL Workfront] eine neue Version hinzufügen, wird die neue Version als neues Dokument mit dem Namen "[!DNL Jira]" in <strong> übertragen</strong>.</p><p>Wichtig: <p>Beachten Sie beim Synchronisieren von Dokumenten Folgendes:</p>
           <ul>
            <li><p>Dokumente mit mehr als 5 MB werden nicht synchronisiert. Wenn die Synchronisierung eines Dokuments fehlschlägt, weil das Dokument zu groß ist, wird ein Fehler im Aktivitätsprotokoll protokolliert. </p><p>Weitere Informationen zum Aktivitätsprotokoll finden Sie unter <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Jira-Aktivitätsprotokoll anzeigen</a>.</p></li>
            <li><p>Dokumente, die mit Aufgaben und Problemen von externen Servern verknüpft sind, werden nicht an die [!DNL Jira] Elemente übertragen. Nur Dokumente, die direkt auf die Aufgabe oder das Problem in [!DNL Workfront] hochgeladen werden, werden auf die verknüpfte Anfrage in [!DNL Jira] übertragen.</p></li>
            <li><p>Um einen Korrekturabzug aus einem Dokument zu erstellen, müssen Sie den Korrekturabzug in [!DNL Workfront] generieren. </p><p>Weitere Informationen zum Erstellen eines Korrekturabzugs finden Sie unter <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Erstellen eines Korrekturabzugs für ein vorhandenes Dokument </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Erstellen eines Korrekturabzugs für ein Dokument</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Geplantes Abschlussdatum]</td>
         <td><p>Das [!UICONTROL Geplantes Abschlussdatum] einer Aufgabe oder eines Problems in [!DNL Workfront] wird zum [!UICONTROL Fälligkeitsdatum] des Problems, mit dem es in [!DNL Jira] verknüpft ist.</p><p>Hinweis: Stellen Sie sicher, dass bei <strong> Problemen </strong>[!UICONTROL Due Date][!DNL Jira] angezeigt wird, damit dieser Wert synchronisiert werden kann.</p></td>
        </tr>
       </tbody>
      </table>

1. Wählen **[!UICONTROL im Abschnitt „Synchronisieren von [!DNL Jira] nach[!DNL Workfront]]**&quot; die Felder aus, die Sie in [!DNL Workfront] aktualisieren möchten, wenn sie in [!DNL Jira] aktualisiert werden.

   1. Wählen Sie eine der folgenden Frequenzen, mit denen die Felder synchronisiert werden sollen:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Immer]</td>
         <td>Die angegebenen Felder werden immer zwischen den verknüpften [!DNL Workfront] und [!DNL Jira] Elementen synchronisiert, wenn die Felder in [!DNL Jira] aktualisiert werden. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Never]</td>
         <td><p>Die angegebenen Felder werden nie zwischen den verknüpften [!DNL Workfront] und [!DNL Jira] Elementen synchronisiert. In [!DNL Workfront] gibt es keinen Hinweis darauf, dass das Feld in [!DNL Jira] aktualisiert wurde. </p><p>Hinweis: Wenn Sie Nie auswählen, können [!DNL Workfront] Felder weiterhin manuell aus [!DNL Jira] im linken [!DNL Workfront] des [!DNL Jira] aktualisiert werden. Diese Aktualisierungen werden nur für [!DNL Workfront] Elemente in [!DNL Jira] und [!DNL Workfront] und nicht für [!DNL Jira] Elemente angezeigt.</p></td>
        </tr>
       </tbody>
      </table>

   1. Wählen Sie diese Option aus, um eines der folgenden Felder von [!DNL Jira] nach [!DNL Workfront] zu synchronisieren:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>Der [!UICONTROL Status] eines Problems in [!DNL Jira] wird zum [!UICONTROL Status] der Aufgabe oder des Problems, mit der bzw. dem es in [!DNL Workfront] verknüpft ist.<br>Weitere Informationen zum [!DNL Workfront] finden Sie unter <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Bevollmächtigter]</td>
         <td><p>Der [!UICONTROL Bevollmächtigte] eines Problems in [!DNL Jira] wird zum [!UICONTROL Bevollmächtigten] der Aufgabe oder des Problems, mit der bzw. dem es in [!DNL Workfront] verknüpft ist.</p><p>Wichtig: Wenn Sie einem Benutzer, der kein [!DNL Jira] Konto hat, ein Element in [!DNL Workfront] zuweisen, erstellt die Integration nur dann einen neuen aktiven Benutzer in [!DNL Workfront], wenn <strong>Automatisch einen Benutzer in [!DNL Workfront] erstellen, wenn der [!DNL Jira] Benutzer kein [!DNL Workfront] Konto hat</strong> auf <strong>[!UICONTROL Always]</strong> gesetzt ist. Dieser Benutzer ist nicht im Besitz einer [!DNL Workfront]. Aktive Benutzende können Arbeitselementen in [!DNL Workfront] zugewiesen werden, können jedoch nicht in Aktualisierungen eingeschlossen werden. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Anlagen]</td>
         <td>Anlagen eines Problems in [!DNL Jira] sind auch an die Aufgabe oder das Problem angehängt, mit der bzw. dem es in [!DNL Workfront] verknüpft ist. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Kommentare]</td>
         <td><p>Ein Kommentar zu einem [!DNL Jira] Problem wird auch über das verknüpfte [!DNL Workfront] im Bereich [!UICONTROL Updates] veröffentlicht. Umgekehrt wird ein Kommentar, der im Bereich [!UICONTROL Aktualisiert] für eine [!DNL Workfront] Aufgabe oder ein Problem gepostet wird, mit dem nativen Kommentar-Stream von [!DNL Jira] für das verknüpfte Problem synchronisiert. </p><p>Standardmäßig ist dies auf <strong>[!UICONTROL Always]</strong> festgelegt. Wenn Sie hier <strong>[!UICONTROL Never]</strong> auswählen, können Sie dennoch manuell Kommentare zu einem verknüpften Element entweder in [!DNL Workfront] oder in [!DNL Jira] posten.</p></td>
        </tr>
       </tbody>
      </table>

1. Wählen Sie im Abschnitt **[!UICONTROL SONSTIGE]** aus, welche zusätzlichen Felder zwischen verknüpften Elementen aktualisiert werden sollen.

   1. Wählen Sie eine Option aus, um festzulegen, ob die von Ihnen angegebenen Felder **[!UICONTROL Immer]** oder **[!UICONTROL Nie]** in [!DNL Jira] oder [!DNL Workfront] aktualisiert werden sollen, wenn sie geändert werden.

   1. Wählen Sie aus den folgenden Feldern und Aktualisierungen aus:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL [!DNL Workfront] Benutzerdefinierte Daten im rechten Bedienfeld in [!DNL Jira] kopieren]</td>
         <td><p>Zeigt die [!DNL Workfront] benutzerdefinierten Daten eines Elements im [!DNL Workfront] rechten Bedienfeld an.</p><p>Hinweis: Benutzerdefinierte Formularabschnitte werden im rechten [!DNL Workfront] Bereich mit der Zugriffsebene des [!DNL Workfront] angezeigt.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL [!DNL Workfront] Priorität im rechten Bedienfeld in [!DNL Jira] kopieren]</td>
         <td>Zeigt die [!DNL Workfront] eines Elements im [!DNL Workfront] rechten Bedienfeld an.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Fügen Sie auf der Registerkarte [!DNL Workfront]-Updates eine Aktualisierung zu den Änderungen des Fälligkeitsdatums in [!DNL Jira] hinzu]</td>
         <td>Fügt einen Kommentar in die Registerkarte [!UICONTROL Update] des [!DNL Workfront] ein, wenn sich das [!UICONTROL Due Date] im verknüpften [!DNL Jira] ändert.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Automatisches Erstellen eines Benutzers in [!DNL Workfront], wenn der [!DNL Jira] Benutzer kein [!DNL Workfront] Konto hat]</td>
         <td><p>Die folgenden Szenarien sind vorhanden:</p>
          <ul>
           <li>Wenn Sie <strong>[!UICONTROL Always]</strong> auswählen, aktivieren Sie die Integration so, dass jedes Mal, wenn ein [!DNL Jira] ohne [!DNL Workfront]-Konto die folgenden Aktionen für ein verknüpftes [!DNL Jira] ausführt, ein neuer Workfront-Benutzer erstellt wird:
            <ul>
             <li>Ist einem [!DNL Jira] Problem zugewiesen</li>
             <li><p>Protokolliert die Zeit für ein [!DNL Jira] Problem</p><p>Dieser neue Benutzer ist nicht im Besitz einer [!DNL Workfront]. Die Standardeinstellung ist Immer . Dem auf diese Weise in erstellten Benutzer wurde [!DNL Workfront] "[!UICONTROL Jira]" hinzugefügt.</p></li>
            </ul></li>
           <li>Wenn Sie <strong>[!UICONTROL Never]</strong> auswählen, passiert Folgendes:
            <ul>
             <li>Es werden keine [!DNL Jira] Zuweisungen für die [!DNL Workfront] Elemente angezeigt. In diesem Fall werden in [!DNL Workfront] nur Zuweisungen auf den [!DNL Workfront] Elementen angezeigt.</li>
             <li>Die Zeit, die ein Benutzer ohne ein [!DNL Jira]-Konto für ein verknüpftes [!DNL Workfront]-Problem protokolliert hat, wird nicht automatisch auf das verknüpfte [!DNL Workfront]-Element übertragen. Sie können weiterhin Zeit für das [!DNL Workfront] Element im rechten Bedienfeld des [!DNL Jira] Problems protokollieren.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Jedes Mal, wenn ein Benutzer eines der in dieser Konfiguration für ein Element in [!DNL Jira] oder [!DNL Workfront] angegebenen Felder aktualisiert, wird jetzt auch das verknüpfte Element in der anderen Anwendung aktualisiert.

## Fehlerbehebung

### Elemente können in [!DNL Jira] nicht erstellt werden, da Trigger-Felder mit der Kennzeichnung &quot;[!UICONTROL  nicht gefunden ]&quot;

#### Problem

Wenn bei der [!DNL Workfront for Jira] Anwendung ein Fehler auftritt, deaktiviert [!DNL Workfront] die Trigger, um weitere Komplikationen zu vermeiden. Wenn diese Trigger deaktiviert sind, werden sie als &quot;[!UICONTROL  nicht gefunden“ ].

#### Lösung

Suchen Sie den Fehler, der die Trigger deaktiviert hat. Den Fehler finden Sie im [!DNL Workfront for Jira] [!UICONTROL Aktivitätsprotokoll].

Die häufigste Ursache für dieses Verhalten ist der Fehler &quot;[!UICONTROL Feld &#39;duedate&#39; kann nicht festgelegt werden. Es ist nicht auf dem entsprechenden Bildschirm oder unbekannt.]&quot;

Dieser Fehler bedeutet, dass Sie versuchen, das &quot;[!UICONTROL  Abschlussdatum“ ] von [!DNL Workfront] nach [!DNL Jira] zu synchronisieren. Dazu müssen Sie sicherstellen, dass Ihre [!DNL Jira] ein Feld namens „Fälligkeitsdatum[!UICONTROL  aufweisen]. Wenn dieses Feld nicht vorhanden ist, kann [!DNL Workfront] das geplante Abschlussdatum nicht mit [!DNL Workfront] synchronisieren und deaktiviert Ihre Trigger.

Um diesen Fehler zu beheben, führen Sie einen der folgenden Schritte aus:

* Bitten Sie Ihren [!DNL Jira], die betroffenen [!DNL Jira] zu aktualisieren, um sicherzustellen, dass sie ein Feld für das Fälligkeitsdatum haben.
* Deaktivieren Sie die Synchronisierung des geplanten Abschlussdatums von [!DNL Workfront] auf der Seite „Setup[!UICONTROL  von Workfront].
