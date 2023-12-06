---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Konfigurieren [!DNL Adobe Workfront for Jira]
description: Sie können [!DNL Adobe Workfront for Jira] zur Integration Ihrer [!DNL Jira] und [!DNL Workfront] Systeme.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 4ade799ff735183f83f045e7eaa876961d266208
workflow-type: tm+mt
source-wordcount: '2424'
ht-degree: 0%

---

# Konfigurieren [!DNL Adobe Workfront for Jira]

Sie können [!DNL Adobe Workfront for Jira] zur Integration Ihrer [!DNL Jira] und [!DNL Workfront] Systeme.

Nach der Installation des Add-ons können Sie Workflows definieren, die [!DNL Jira] automatisch Probleme bei [!DNL Workfront] Arbeitselemente werden erstellt. Die Elemente in beiden Anwendungen werden verknüpft und einige ihrer Informationen werden automatisch in beiden Systemen aktualisiert.

Alle Benutzer in [!DNL Workfront] und [!DNL Jira] kann von dieser Integration profitieren. Sie benötigen nur eine Lizenz für das System, in dem sie am besten funktionieren, und nicht für beide Systeme.

Dieses Add-on ist für beide [!UICONTROL Server] und [!UICONTROL OnDemand] (oder [!UICONTROL Cloud]) Versionen von [!DNL Jira] Software.

Für eine Liste von [!DNL Jira] Versionen [!DNL Workfront for Jira] unterstützt derzeit, siehe [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) im [!DNL Atlassian Marketplace].

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] plan]*</td> 
   <td><p>Neuer Plan: Beliebig</p>
       <p>oder</p>
       <p>Aktueller Plan: [!UICONTROL Pro] oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>Neuer Plan: [!UICONTROL Standard] </p>
       <p>oder</p> 
       <p>Aktueller Plan: [!UICONTROL Plan] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] access</td> 
   <td> <p>Systemadministratorzugriff</p> <p>Wichtig: Es wird empfohlen, separate Systemadministratorkonten in der [!DNL Jira] und [!DNL Workfront] , um dieser Integration zu widmen, anstatt vorhandene zu verwenden, die möglicherweise mit Benutzern verbunden sind.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Vor der Konfiguration [!DNL Workfront for Jira]müssen Sie:

* Installieren [!DNL Workfront for Jira].
Anweisungen zur Installation [!DNL Workfront for Jira], siehe [Installieren [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Konfigurieren [!DNL Workfront for Jira]

Durch Konfiguration [!DNL Workfront for Jira]können Sie:

* Definieren Sie die erstellten Trigger [!DNL Jira] Elemente, wenn [!DNL Workfront] -Elemente erstellt werden.
* Geben Sie an, welche Felder zwischen den verknüpften Elementen synchronisiert werden sollen [!DNL Jira] und [!DNL Workfront].

>[!NOTE]
>
>* Nach der Konfiguration [!DNL Workfront for Jira] auf [!DNL Jira] Umgebung, alle [!DNL Jira] -Benutzer sehen [!DNL Workfront] Rechtes Bedienfeld auf allen [!DNL Jira] Elemente. Das Bedienfeld enthält Informationen zu den Elementen, die verknüpft werden können von [!DNL Workfront] oder gibt an, dass [!DNL Workfront] -Elemente [!DNL Jira] Elemente.
>* Bei Verwendung von [!DNL Jira Server] -Installation werden nur die Probleme angezeigt, die mit den als Trigger für die Workfront-Integration identifizierten Projekten verknüpft sind. Weitere Informationen zum Einrichten von Triggern für die [!DNL Workfront to Jira] Workflow, siehe [Trigger für die automatische Verknüpfung von Elementen zwischen [!DNL Jira] und [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

So konfigurieren Sie [!DNL Workfront for Jira]:

1. Anmelden bei [!DNL Jira] as a [!DNL Jira] Administrator.
1. Klicks **[!UICONTROL Einstellungen]** im Hauptteil [!DNL Jira] Menü.
1. Klicks **[!UICONTROL Add-ons]** Klicken Sie auf **[!UICONTROL Verwalten von Add-ons]**.

1. Erweitern Sie die **[!DNL Workfront]** -Add-on.
1. Klicks **[!UICONTROL Konfigurieren]**.
1. Befolgen Sie die Anweisungen zum Anmelden bei [!DNL Workfront].

   >[!NOTE]
   >
   >Der Benutzer muss über eine gültige `apiKey` in [!UICONTROL Workfront] , um eine erfolgreiche Verbindung herzustellen.

   Sie müssen sich bei [!DNL Workfront] as a [!DNL Workfront] Administrator , um die Konfiguration fortzusetzen.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] verbindet [!DNL Jira] mit OAuth 2.0, einem Standard, der von den meisten webbasierten Integrationen für die Authentifizierung und Autorisierung von Benutzern verwendet wird.
   >* Wenn Sie aufgefordert werden, die Domäne Ihrer [!DNL Workfront] -Konto angeben, geben Sie es in folgendem Format ein: *yourCompany&#39;sDomain.my.workfront.com*. Die Domäne Ihres Unternehmens ist normalerweise der Name Ihres Unternehmens.
   >* Die erweiterte Authentifizierung ist erst verfügbar, wenn eine [!DNL Workfront] -Administrator aktiviert sie für diese Integration.

1. Wählen Sie in Jira die **[!UICONTROL Trigger]** zur Konfiguration der automatischen Erstellung von [!DNL Jira] Elemente als neue [!DNL Workfront] -Elemente erstellt werden.

   Weitere Informationen zum Einrichten von Triggern für die Workfront finden Sie unter [!DNL Jira] Workflow, siehe [Trigger für die automatische Verknüpfung von Elementen zwischen [!DNL Jira] und [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Wählen Sie die **[!UICONTROL Einrichtung]** Registerkarte zur Konfiguration der Synchronisierung von Feldern zwischen verknüpften Feldern [!DNL Jira] und [!DNL Workfront] Elemente.

   Weitere Informationen zum Einrichten der Synchronisierung von Feldern zwischen [!DNL Jira] und [!DNL Workfront], siehe [Konfigurieren der Feldsynchronisierung zwischen [!DNL Jira] und [!DNL Workfront] Elemente](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Nachdem Sie die Trigger und die Synchronisation der Felder zwischen den beiden Anwendungen definiert haben, können Sie alle [!DNL Workfront] Benutzer, die Aufgaben oder Probleme erstellen können, können möglicherweise Trigger auf die Erstellung eines Elements in [!DNL Jira]. Der Benutzer kann ein Element erstellen, wenn die Kriterien für das Element, das er erstellt, mit den Triggern in [!DNL Jira], auch wenn der Benutzer nicht über eine [!DNL Jira] -Lizenz. Darüber hinaus werden alle [!DNL Jira] Der Benutzer kann sofort mit der Arbeit an der [!DNL Jira] -Element und deren Aktualisierungen sind sichtbar in [!DNL Workfront], ohne dass sie [!DNL Workfront] -Lizenz. Jegliche Aktualisierungen in [!DNL Workfront] sind auch auf der [!DNL Jira] Elemente.

1. (Optional) Wählen Sie die **[!UICONTROL Aktivitätsprotokoll]** um etwaige Fehler zu überprüfen, die während der Integration aufgetreten sind.

   Weitere Informationen zum [!UICONTROL Aktivitätsprotokoll], siehe [Anzeigen der [!DNL Jira] [!UICONTROL Aktivitätsprotokoll]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Trigger für die automatische Verknüpfung von Elementen zwischen [!DNL Jira] und [!DNL Workfront]

Als [!DNL Jira] Systemadministrator können Sie Trigger definieren, die automatisch Probleme in [!DNL Jira] wenn ein Element in [!DNL Workfront] bestimmte Kriterien erfüllt.

>[!NOTE]
>
>Es kann bis zu 10 Minuten dauern, bis die Integration neue Probleme in [!DNL Jira].

Beachten Sie beim Konfigurieren des Auslösens der Erstellung von [!DNL Jira] Elemente als [!DNL Workfront] -Elemente werden erstellt:

* Die Integration ist unidirektional: Sie können nur Elemente Trigger haben, die Sie in erstellen. [!DNL Workfront] automatisch in [!DNL Jira]. Es ist nicht möglich, Elemente Trigger, die Sie in [!DNL Jira] automatisch in [!DNL Workfront].
* Es gibt keine Beschränkung für die Anzahl der Trigger, die Sie haben können.
* Wenn ein Element, das Sie in [!DNL Workfront] mehr als einem der Trigger entspricht, wird nur ein Element in erstellt. [!DNL Jira]. Das Element wird in [!DNL Jira] nach dem ersten Trigger (in der Reihenfolge, in der sie definiert wurden in [!DNL Jira]). Alle anderen Trigger werden ignoriert.
* Nur ein Element in [!DNL Workfront] kann mit einem Element in Jira verknüpft werden. Sie können nie eine [!DNL Workfront] Element zu mehreren [!DNL Jira] Probleme oder eines [!DNL Jira] Problem bei mehreren [!DNL Workfront] Elemente.

So konfigurieren Sie Trigger für das automatische Erstellen von Elementen in [!DNL Jira]:

1. Anmelden bei [!DNL Jira] als Systemadministrator.
1. Klicks **[!UICONTROL Einstellungen]** im Hauptteil [!DNL Jira] Menü.
1. Klicks **[!UICONTROL Add-ons]**, dann **[!UICONTROL Verwalten von Add-ons]**.
1. Erweitern Sie die **[!DNL Workfront]** -Add-on.
1. Klicks **[!UICONTROL Konfigurieren]**.
1. Anmelden bei [!DNL Workfront] als Systemadministrator.

   Die **[!UICONTROL Trigger]** ist in Jira standardmäßig ausgewählt.

1. Klicks **[!UICONTROL Trigger hinzufügen]** , um einen neuen Trigger hinzuzufügen.
1. Im **[!UICONTROL Workfront-Team/Benutzer/Rolle]** -Feld den Namen eines [!DNL Workfront] Team-, Benutzer- oder Auftragsrolle aus und klicken Sie dann auf , um sie auszuwählen, wenn sie in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie können nicht mehrere Trigger für dasselbe Team, denselben Benutzer oder dieselbe Rolle haben.

   Wenn jemand eine Aufgabe oder ein Problem erstellt und sie einer dieser Entitäten zuweist, wird automatisch ein Problem in [!DNL [!DNL Jira]].

1. Im **[!UICONTROL [!DNL Jira]Projekt]** ein, beginnen Sie mit der Eingabe des Namens eines [!DNL Jira] und klicken Sie dann auf , um es auszuwählen, wenn es in der Liste angezeigt wird.

   Wenn die Variable [!DNL Jira] -Problem erstellt wurde, wird es in das hier ausgewählte Projekt eingefügt.

1. Wählen Sie eine **I[!UICONTROL Sicherungstyp]** aus dem Dropdown-Menü.

   Dies zeigt den Problemtyp an, der in [!DNL Jira] wenn die Bedingungen dieses Triggers erfüllt sind, basierend auf Ihren Einstellungen für dieses spezifische Projekt in [!DNL Jira].

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Mit dieser Konfiguration wird jedes Mal [!DNL Workfront] -Benutzer erstellt ein Element, das den angegebenen Triggern entspricht, ein neues Problem wird in erstellt. [!DNL Jira].

## Konfigurieren der Feldsynchronisierung zwischen [!DNL Jira] und [!DNL Workfront] Elemente

Als [!DNL Jira] Administrator können Sie festlegen, welche Felder automatisch für Elemente synchronisiert werden sollen, die zwischen [!DNL Workfront] und Jira. Bestimmte Felder können über die [!DNL Workfront] der [!DNL Jira] und andere Elemente werden von Jira nach Workfront synchronisiert.

So definieren Sie, welche Felder automatisch für Elemente synchronisiert werden sollen, die zwischen den beiden Anwendungen verknüpft sind:

1. Anmelden bei [!DNL Jira] als Jira-Administrator
1. Klicks **[!UICONTROL Einstellungen]** im Hauptteil [!DNL Jira] Menü.
1. Klicks **[!UICONTROL Add-ons]**, dann **[!UICONTROL Verwalten von Add-ons]**.
1. Erweitern Sie die **[!DNL Workfront]** -Add-on.
1. Klicks **[!UICONTROL Konfigurieren]**.
1. Anmelden bei [!DNL Workfront] als Workfront-Administrator.
1. Klicken Sie in Jira auf die **[!UICONTROL Einrichtung]** Registerkarte.
1. Im **[!UICONTROL Synchronisieren von Workfront mit Jira]** auswählen Sie die Felder, die Sie aktualisieren möchten in [!DNL Jira] wenn sie in Workfront aktualisiert werden.

   1. Wählen Sie eine der folgenden Frequenzen aus, mit denen die Felder synchronisiert werden:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Bei Erstellung]</td>
              <td>Die von Ihnen angegebenen Felder werden zwischen der verknüpften Workfront und [!DNL Jira] Elemente, wenn das Element in Workfront erstellt wird.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Immer]</td>
              <td>Die von Ihnen angegebenen Felder werden zwischen der verknüpften Workfront und [!DNL Jira] Elemente, wenn die Felder in Workfront aktualisiert werden. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Nie]</td>
              <td>Die von Ihnen angegebenen Felder werden nie zwischen den verknüpften [!DNL Workfront] und [!DNL Jira] Elemente. Es gibt keine Hinweise für [!DNL Jira] dass das Feld in aktualisiert wurde [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Wählen Sie eine der folgenden Optionen aus, um die Felder zu synchronisieren [!DNL Workfront] nach [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>Der Name einer Aufgabe oder eines Problems in [!DNL Workfront] wird zum Namen des Problems, mit dem es verknüpft ist [!DNL Jira].</p><p>Hinweis: Wenn neue Elemente in erstellt werden [!DNL Jira] automatisch die [!DNL Workfront] Der Name aktualisiert immer auf dem [!DNL Jira] -Element, unabhängig davon, ob dieses Feld hier aktiviert ist oder nicht. Wenn eine [!DNL Jira] Element manuell mit einer [!DNL Workfront] item, der Name des [!DNL Workfront] Aktualisierungen nur für Elemente in [!DNL Jira] bei Auswahl von <strong>Immer</strong> Synchronisieren Sie dieses Feld. Weitere Informationen zum manuellen oder automatischen Verknüpfen von Elementen finden Sie unter <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Elemente verknüpfen zwischen [!DNL Adobe Workfront] und [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Beschreibung]</td>
         <td>Die Beschreibung einer Aufgabe oder eines Problems in [!DNL Workfront] wird zur Beschreibung des Problems, mit dem es verknüpft ist in [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Dokumente</td>
         <td><p>Dokumente, die an eine Aufgabe oder ein Problem in [!DNL Workfront] sind auch mit der Frage verbunden, mit der sie in Jira verbunden ist. Neue Dokumentversionen von [!DNL Workfront] werden als separate Dokumente zu Jira hinzugefügt und mit <i>_v&lt;version number=""&gt;</i> um die nummerierte Version in Workfront anzugeben. </p><p>Wenn beispielsweise der Name eines Dokuments in [!DNL Workfront] is <strong>Hauptanzeige</strong>und fügen Sie ihr eine neue Version hinzu in [!DNL Workfront], wird die neue Version in [!DNL Jira] als neues Dokument mit dem Namen <strong>Main Ad_v2</strong>.</p><p>Wichtig: <p>Beachten Sie beim Synchronisieren von Dokumenten Folgendes:</p>
           <ul>
            <li><p>Dokumente, die größer als 5 MB sind, werden nicht synchronisiert. Wenn die Dokumentsynchronisierung fehlschlägt, weil das Dokument zu groß ist, wird ein Fehler im Aktivitätsprotokoll protokolliert. </p><p>Weitere Informationen zum Aktivitätsprotokoll finden Sie unter <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Jira-Aktivitätsprotokoll anzeigen</a>.</p></li>
            <li><p>Dokumente, die mit Aufgaben und Problemen von externen Servern verknüpft sind, werden nicht an die [!DNL Jira] Elemente. Nur Dokumente, die direkt zur Aufgabe oder zum Problem in hochgeladen wurden [!DNL Workfront] auf die damit verbundene Ausgabe in [!DNL Jira].</p></li>
            <li><p>Um einen Testversand aus einem Dokument zu erstellen, müssen Sie den Testversand in [!DNL Workfront]. </p><p>Weitere Informationen zum Generieren eines Testversands finden Sie unter <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Erstellen eines Testversands für ein vorhandenes Dokument </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Erstellen eines Testversands für ein Dokument</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Geplantes Abschlussdatum]</td>
         <td><p>Das geplante Abschlussdatum einer Aufgabe oder eines Problems in [!DNL Workfront] wird zum [!UICONTROL Fälligkeitsdatum] des Problems, mit dem es verknüpft ist in [!DNL Jira].</p><p>Hinweis: Stellen Sie sicher, dass Sie <strong>[!UICONTROL Fälligkeitsdatum]</strong> on [!DNL Jira] -Probleme, damit dieser Wert synchronisiert werden kann.</p></td>
        </tr>
       </tbody>
      </table>

1. Im **[!UICONTROL Synchronisieren von [!DNL Jira] nach[!DNL Workfront]]** auswählen Sie die Felder, die Sie aktualisieren möchten in [!DNL Workfront] wann sie in aktualisiert wurden [!DNL Jira].

   1. Wählen Sie eine der folgenden Frequenzen aus, mit denen die Felder synchronisiert werden:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Immer]</td>
         <td>Die von Ihnen angegebenen Felder werden immer zwischen den verknüpften [!DNL Workfront] und [!DNL Jira] Elemente, wenn die Felder in [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Nie]</td>
         <td><p>Die von Ihnen angegebenen Felder werden nie zwischen den verknüpften [!DNL Workfront] und [!DNL Jira] Elemente. Es gibt keine Hinweise für [!DNL Workfront] dass das Feld in aktualisiert wurde [!DNL Jira]. </p><p>Hinweis: Wenn Sie Nie auswählen, [!DNL Workfront] Felder können weiterhin manuell aktualisiert werden über [!DNL Jira] links [!DNL Workfront] -Bedienfeld der [!DNL Jira] Problem. Diese Aktualisierungen werden nur in [!DNL Workfront] Elemente in [!DNL Jira] und [!DNL Workfront] und nicht [!DNL Jira] Elemente.</p></td>
        </tr>
       </tbody>
      </table>

   1. Wählen Sie aus, um eines der folgenden Felder zu synchronisieren [!DNL Jira] nach [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>Der [!UICONTROL Status] eines Problems in [!DNL Jira] wird zum [!UICONTROL Status] der Aufgabe oder des Problems, mit der/dem sie verknüpft ist. [!DNL Workfront].<br>Weitere Informationen finden Sie unter [!DNL Workfront] Status, siehe <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Erstellen oder Bearbeiten eines Status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Zuweisung]</td>
         <td><p>Der [!UICONTROL Verantwortliche] eines Problems in [!DNL Jira] wird zum [!UICONTROL Verantwortlichen] der Aufgabe oder des Problems, mit der/dem sie verknüpft ist. [!DNL Workfront].</p><p>Wichtig: Wenn Sie ein Element in [!DNL Jira] für einen Benutzer, der keine [!DNL Workfront] -Konto erstellen, erstellt die Integration einen neuen aktiven Benutzer in [!DNL Workfront] nur bei <strong>Benutzer automatisch erstellen in [!DNL Workfront] wenn die [!DNL Jira] Der Benutzer verfügt nicht über eine [!DNL Workfront] account</strong> auf <strong>[!UICONTROL Immer]</strong>. Dieser Benutzer belegt keine [!DNL Workfront] -Lizenz. Aktive Benutzer können Arbeitselementen in [!DNL Workfront], können jedoch nicht in Aktualisierungen einbezogen werden. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Attachments]</td>
         <td>Anlagen eines Problems in [!DNL Jira] auch mit der Aufgabe oder dem Problem verbunden sind, mit der sie verknüpft ist [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Kommentare]</td>
         <td><p>Ein Kommentar zu [!DNL Jira] -Problem wird auch auf der verknüpften [!DNL Workfront] im Bereich [!UICONTROL Updates]. Umgekehrt wird ein Kommentar im Bereich [!UICONTROL Updates] für eine [!DNL Workfront] Aufgabe oder Problem synchronisieren mit [!DNL Jira]Nativer Kommentar-Stream für das verknüpfte Problem. </p><p>Dies ist auf <strong>[!UICONTROL Immer]</strong> Standardmäßig. Wenn Sie <strong>[!UICONTROL Nie]</strong> Hier können Sie Kommentare weiterhin manuell für ein verknüpftes Element veröffentlichen, entweder in [!DNL Workfront] oder [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. Im **[!UICONTROL SONSTIGE]** auswählen, welche zusätzlichen Felder zwischen verknüpften Elementen aktualisiert werden sollen.

   1. Wählen Sie eine Option aus, um zu bestimmen, ob die von Ihnen angegebenen Felder **[!UICONTROL Immer]** oder **[!UICONTROL Nie]** Aktualisieren in [!DNL Jira] oder [!DNL Workfront] wenn sie geändert werden.

   1. Wählen Sie aus den folgenden Feldern und Updates aus:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Benutzerdefinierte Daten im rechten Bereich in [!DNL Jira]]</td>
         <td><p>Zeigt die [!DNL Workfront] Benutzerdefinierte Daten eines Elements im [!DNL Workfront] rechts.</p><p>Hinweis: Die Abschnitte Benutzerdefiniertes Formular werden im Abschnitt [!DNL Workfront] rechter Bereich mit der Zugriffsebene der [!DNL Workfront] Systemadministrator.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copy [!DNL Workfront] Priorität im rechten Bereich in [!DNL Jira]]</td>
         <td>Zeigt die [!DNL Workfront] Priorität eines Elements im [!DNL Workfront] rechts.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Hinzufügen eines Updates im [!DNL Workfront] Registerkarte "Aktualisierungen"zu Änderungen am Fälligkeitsdatum in [!DNL Jira]]</td>
         <td>Fügt auf der Registerkarte [!UICONTROL Update] im [!DNL Workfront] Element, wenn sich das [!UICONTROL Fälligkeitsdatum] in einem verknüpften [!DNL Jira] -Element.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Benutzer automatisch in [!DNL Workfront] wenn die [!DNL Jira] Der Benutzer verfügt nicht über eine [!DNL Workfront] account]</td>
         <td><p>Die folgenden Szenarien existieren:</p>
          <ul>
           <li>Wenn Sie <strong>[!UICONTROL Immer]</strong>, aktivieren Sie die Integration, um jedes Mal einen neuen Workfront-Benutzer zu erstellen. [!DNL Jira] Benutzer ohne [!DNL Workfront] -Konto führt die folgenden Aktionen für einen verknüpften [!DNL Jira] Problem:
            <ul>
             <li>Wird einem [!DNL Jira] Problem</li>
             <li><p>Protokolliert die Zeit auf einen [!DNL Jira] Problem</p><p>Dieser neue Benutzer hat keine [!DNL Workfront] -Lizenz. Die Standardeinstellung ist "Immer". Der Benutzer hat auf diese Weise in [!DNL Workfront] hat "[!UICONTROL Jira]" zu ihrem Namen hinzugefügt.</p></li>
            </ul></li>
           <li>Wenn Sie <strong>[!UICONTROL Nie]</strong>, geschieht Folgendes:
            <ul>
             <li>Sie können keine [!DNL Jira] Zuweisungen für die [!DNL Workfront] Elemente. In diesem Fall werden nur Zuweisungen in [!DNL Workfront] auf der [!DNL Workfront] Elemente.</li>
             <li>Die in einem Link protokollierte Zeit [!DNL Jira] Problem durch einen Benutzer ohne [!DNL Workfront] wird nicht automatisch auf das verknüpfte Konto übertragen [!DNL Workfront] -Element. Sie können die Protokollzeit weiterhin auf der [!DNL Workfront] -Element im rechten Bereich des [!DNL Jira] Problem.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Jedes Mal, wenn ein Benutzer eines der in dieser Konfiguration angegebenen Felder für ein Element in [!DNL Jira] oder [!DNL Workfront], wird auch das verknüpfte Element in der anderen Anwendung aktualisiert.

## Fehlerbehebung

### Elemente können nicht in erstellt werden [!DNL Jira] aufgrund von Trigger-Feldern, die mit &quot;[!UICONTROL Nicht gefunden]&quot;

#### Problem

Wenn ein Fehler mit der [!DNL Workfront for Jira] Anwendung, [!DNL Workfront] deaktiviert die Trigger zur Vermeidung weiterer Komplikationen. Wenn diese Trigger deaktiviert sind, werden sie als[!UICONTROL Nicht gefunden].&quot;

#### Lösung

Suchen Sie den Fehler, der die Trigger deaktiviert hat. Sie finden den Fehler im [!DNL Workfront for Jira] [!UICONTROL Aktivitätsprotokoll].

Die häufigste Ursache für dieses Verhalten ist der Fehler &quot;[!UICONTROL Das Feld &quot;Standardwert&quot;kann nicht festgelegt werden. Sie befindet sich nicht auf dem entsprechenden Bildschirm oder ist unbekannt.]&quot;

Dieser Fehler bedeutet, dass Sie versuchen, die[!UICONTROL Geplantes Abschlussdatum]&quot; von [!DNL Workfront] nach [!DNL Jira]. Dazu müssen Sie sicherstellen, dass Ihre [!DNL Jira] Objekte haben ein Feld namens[!UICONTROL Fälligkeitsdatum].&quot; Wenn sie dieses Feld nicht haben, [!DNL Workfront] kann das geplante Abschlussdatum nicht synchronisieren von [!DNL Workfront] und deaktiviert Ihre Trigger.

Um diesen Fehler zu beheben, führen Sie einen der folgenden Schritte aus:

* Fragen Sie Ihre [!DNL Jira] Administrator zum Aktualisieren der betroffenen [!DNL Jira] -Objekte, um sicherzustellen, dass sie über ein Fälligkeitsfeld verfügen.
* Deaktivierung der Synchronisierung von [!DNL Workfront]Voraussichtlicher Abschlussdatum in der Workfront [!UICONTROL Einrichtung] Seite.
