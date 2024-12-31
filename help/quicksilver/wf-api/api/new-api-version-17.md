---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 17
description: Adobe Workfront hat API Version 17 am 6. April 2022 veröffentlicht. Die API-Version 17 enthält die folgenden Änderungen gegenüber Version 16.
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1353'
ht-degree: 1%

---

# Neue Funktionen in der API-Version 17

Adobe Workfront hat API Version 17 am 12. Oktober 2023 veröffentlicht. Die API-Version 17 enthält die folgenden Änderungen gegenüber Version 16.

## Ressourcen hinzugefügt

<!--

### Booking (BOOKNG)

-->

### Externes Dokument (EXTDOC)

Ein ExternalDocument-Objekt ist ein Dokument oder ein anderes digitales Asset, das sich in einem Dokumentspeicheranbieter außerhalb von Workfront befindet. Diese Assets können mit und von Workfront verknüpft werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>Beschreibung</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>Durchw</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>Pfad</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>Größe</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>Beschreibung</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>Durchw</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>Pfad</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>Größe</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>Wert</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standardfelder</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Abfragen</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Vorgänge</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>
        <ul>
          <li><p><b>Kunde</b></p></li>
          <li><p><b>Benutzer</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## Entfernte Ressourcen

Für API-Version 17 wurden keine Ressourcen entfernt

## Geänderte Ressourcen

Die folgenden Ressourcen wurden für die API-Version 17 geändert.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Baseline (BLIN)

Baselines sind Momentaufnahmen der Leistung eines Projekts zu einem bestimmten Zeitpunkt. Sie speichern wichtige Informationen über das Projekt, wie wichtige Daten, Fortschritt, Kosten und Umsatzwerte.

Das Baseline-Objekt hat das Flag &quot;**_EDITABLE“**.

### Rechnungsnachweis (BILL)

Ein BillingRecord-Objekt zeichnet die Einnahmen, Stunden oder Ausgaben auf, die in Rechnung gestellt werden können. Diese Informationen können zur Erstellung von Rechnungen in einem externen Buchhaltungssystem verwendet werden.

Das BillingRecord-Objekt hat das Flag &quot;**_EDITABLE“**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Firma (COMPY)

Ein Unternehmensobjekt stellt eine Organisation dar, die aus einer Sammlung von Personen besteht.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kundenvoreinstellungen (CUSTPR)

Ein CustomerPreferences-Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Workfront-Instanz festgelegt hat.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>name</b>
            </p>
            <p>Der mögliche Wert „config.defaultToNewHomeDescription“ (customer:config.defaultToNewHome)&gt;/p wurde hinzugefügt?<p>Auf diese Weise kann ein Unternehmen die neue Startseite zum Standard für seine Benutzer machen.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

Ein DocumentVersion-Objekt stellt eine bestimmte Version einer Datei dar (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Der mögliche Wert „Frame.io“ (FRAMEIO) wurde hinzugefügt.</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>Der mögliche Wert „enum.filetype.site“ (site) wurde hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Wechselkurs (EXRATE)

Ein ExchangeRate-Objekt stellt einen in Workfront eingerichteten Wechselkurs dar. Wechselkursobjekte sind nicht dynamisch.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt:
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrences</b></p></li>
          <p>hinzugefügt.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kosten (AUSGABEN)

Aufwendungen stellen die sonstigen Kosten dar, die während der Laufzeit eines Projekts anfallen können.

Das Ausgabenobjekt hat das Flag &quot;**_EDITABLE“**.

### Gruppe (GROUP)

Ein Gruppenobjekt steht für eine Gruppe von Benutzern und Teams. Gruppen repräsentieren oft die Abteilungsstruktur.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Stunde (STUNDE)

Ein Stunden -Objekt steht für eine Stunde, die ein Benutzer in einer Arbeitszeittabelle protokolliert.

Das Stunde -Objekt entfernte das Flag **INLINE_EDITABLE**.

### Iteration (ITRN)

Ein Iterationsobjekt stellt eine einzelne Agile-Iteration dar. Iterationen sind diskrete Zeiträume, in denen agile Storys geplant und abgeschlossen werden.

Das Iterationsobjekt hat das Flag &quot;**_EDITABLE“**.


### Tagebucheintrag (JRNLE)

Das JournalEntry-Objekt kann so eingerichtet werden, dass Informationen zu bestimmten Objektfeldern jedes Mal protokolliert werden, wenn diese Felder geändert werden. Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird jedes Mal, wenn dieses Feld geändert wird, ein entsprechender Journaleintrag erstellt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>Genehmigende Person (AAA) hinzugefügt</li>
              <li>Reviewer hinzugefügt (AAR)</li>
              <li>Reviewer entfernt (ARR)</li>
              <li>Genehmigende Person entfernt (ARA)</li>
              <li>Genehmigte Entscheidung (ADA)</li>
              <li>Entscheidung mit Änderungen genehmigt (ADC)</li>
              <li>Entscheidung muss überarbeitet werden (ADN)</li>
              <li>Aufgehobene Entscheidung (ADR)</li>
              <li>Genehmigende Person geändert (AAC)</li>
              <li>Reviewer Changed (ARC)</li>
              <li>Überprüfung abgeschlossen (RDC)</li>
              <li>Überprüfung widerrufen (RDR)</li>
              <li>Publish (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban-Board (KNBNBD)

Ein Kanban-Board wird verwendet, um Aufgaben in einer Agile-Umgebung zu verfolgen.

Das Kanban-Board-Objekt entfernte das Flag **INLINE_EDITABLE**.


### Verknüpfter Ordner (LINKFDR)

Ein LinkedFolder-Objekt stellt einen Ordner dar, der über einen externen Dokumentanbieter verknüpft ist, z. B. Google Drive oder Dropbox.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Der mögliche Wert „Frame.io (FRAMEIO)“ wurde hinzugefügt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Aufgabe/Problem (OPTASK)

Ein OpTask-Objekt wird im Allgemeinen als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise darauf hinweist, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungsanforderungen, -anfragen und -fehler sind ebenfalls Probleme.

Das Anfrageobjekt hat das Flag &quot;**_EDITABLE“**.

### Projekt (PROJ)

Projekte sind Arbeitselemente innerhalb von Workfront und ein wichtiger Baustein in der Art und Weise, wie Workfront Menschen bei der Arbeit unterstützt. Ein Project-Objekt stellt eine Gruppe von Aufgaben mit einem gemeinsamen, spezifischen Ziel dar.

Das Project-Objekt hat das Flag **INLINE_EDITABLE** entfernt.

### Projektbenutzer (PRTU)

Ein ProjectUser-Objekt stellt einen Benutzer dar, der einem bestimmten Projekt zugeordnet ist.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Satz (RATE)

Ein Tarifobjekt stellt einen Abrechnungssatz in Workfront dar.

Das Ratenobjekt hat das Flag &quot;**_EDITABLE“**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>Die folgenden Aktionen wurden hinzugefügt, um die Tarifkartenfunktion zu unterstützen:
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>Die <b>setRatesForRole</b>-Aktion wurde geändert, um die folgenden Felder hinzuzufügen:
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risiko (Risiko)

Ein Risikoobjekt stellt ein mögliches Ereignis dar, das verhindern kann, dass ein Projekt termingerecht oder innerhalb des Budgets abgeschlossen wird. Projekte werden in der Planungsphase mit Risiken versehen, um potenzielle Hindernisse vor der Genehmigung von Arbeiten zu identifizieren.

Das Risikoobjekt hat das Flag &quot;**_EDITABLE“**.

### Funktion/Aufgabengebiet (ROLE)

Ein Rollenobjekt (Aufgabengebiet) stellt eine funktionale Kapazität oder eine Qualifikation dar, die ein Benutzer ausfüllen kann, z. B. Designer oder Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Aufgabe (AUFGABE)

Ein Aufgabenobjekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (Fertigstellen eines Projekts) ausgeführt werden muss.

Das Aufgabenobjekt hat das Flag &quot;**_EDITABLE“**.

### Team (TEAMOB)

Ein Team-Objekt ist eine Sammlung von Benutzern, die einem Arbeitselement zugewiesen werden können.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Teammitglied (TEAMb)

Ein TeamMember-Objekt ist ein einem bestimmten Team zugeordneter Benutzer.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Vorlagenbenutzer (TMTU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Arbeitszeittabelle (TABELLE)

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Aktualisieren (UPDATE)

Arbeitselemente in Workfront können aktualisiert werden, um Benutzende über den aktuellen Status zu informieren. Ein Update -Objekt stellt eine dieser Aktualisierungen dar. Aktualisierungen können von Benutzenden eingegeben oder vom Workfront-System erstellt werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Die folgenden Werte wurden hinzugefügt:</p>
            <ul>
              <li>Genehmigende Person hinzugefügt (assetapprovalAddGenehmigende Person)</li>
              <li>Reviewer hinzugefügt (assetapprovalAddReviewer)</li>
              <li>Genehmigende Person entfernt (assetapprovalRemoveGenehmiger)</li>
              <li>Reviewer entfernt (assetapprovalRemoveReviewer)</li>
              <li>Entscheidung genehmigt (assetapprovalDecisionApproved)</li>
              <li>Entscheidung muss überarbeitet werden (assetapprovalDecisionNeedsWork)</li>
              <li>Entscheidung mit Änderungen genehmigt (assetapprovalDecisionApprovedChanges)</li>
              <li>Entscheidung widerrufen (assetapprovalDecisionRevocked)</li>
              <li>Genehmigende Person geändert (assetapprovalChanged)</li>
              <li>Reviewer changed (assetapprovalReviewerChanged)</li>
              <li>Überprüfung abgeschlossen (assetapprovalReviewerDecisionComplete)</li>
              <li>Überprüfung widerrufen (assetapprovalReviewerDecisionRevocked)</li>
              <li>Fehler beim Senden des externen Dokuments (externalDocumentSendError)</li>
              <li>Dokumentversion veröffentlicht (documentVersionPublish)</li>
              <li>Workflow für verknüpfte Ordner (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Benutzer (USER)

Ein Benutzerobjekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

Das Benutzerobjekt hat das Flag &quot;**_EDITABLE“**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und ist eine Zahl zwischen 0 und 1, die den Prozentsatz der Zeit darstellt, die eine Benutzerin oder ein Benutzer täglich für Projektarbeit (ohne Mehraufwand) aufwenden kann. Der Wert 1 bedeutet, dass der Benutzer 100 % seiner Zeit mit Projektaufgaben verbringen kann.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Benutzergruppen (USRGPS)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserNote (USRNOT)

Ein UserNote-Objekt ist eine Benachrichtigung.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Die folgenden Werte wurden hinzugefügt:</p>
            <ul>
              <li>Dokument muss genehmigt werden (AAA)</li>
              <li>Dokument muss überprüft werden (AAR)</li>
              <li>Das Dokument benötigt keine Zustimmung mehr (ARA)</li>
              <li>Das Dokument muss nicht mehr überprüft werden (ARR)</li>
              <li>Dokument muss von Benutzer genehmigt werden (ATA)</li>
              <li>Dokument muss von (Benutzer) überprüft werden (ATR)</li>
              <li>Das Dokument bedarf keiner Genehmigung (RTA) durch den Benutzer mehr</li>
              <li>Das Dokument muss nicht mehr von (Benutzer) überprüft werden (RTR)</li>
              <li>Dokument genehmigt (ADA)</li>
              <li>Dokument mit Änderungen genehmigt (ADC)</li>
              <li>Dokument muss bearbeitet werden (ADN)</li>
              <li>(Benutzer) hat (Dokument) als genehmigt markiert. Ihre Genehmigung ist nicht mehr erforderlich. (AAN)</li>
              <li>(Benutzer) hat (Dokument) mit Änderungen als genehmigt markiert. Ihre Genehmigung ist nicht mehr erforderlich. (ACN)</li>
              <li>(Benutzer) hat (Dokument) als arbeitsbedürftig markiert. Ihre Genehmigung ist nicht mehr erforderlich. (AWN)</li>
              <li>Das Dokument muss jetzt überprüft und nicht genehmigt werden (AAC).</li>
              <li>Das Dokument muss jetzt von Ihnen genehmigt und nicht überprüft werden (ADN)</li>
              <li>Dokument geprüft (RDC)</li>
              <li>Dokument geprüft (TRC)</li>
              <li>(Benutzer) hat (Dokument) als abgeschlossen geprüft. Ihre Überprüfung ist nicht mehr erforderlich. (TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserRole (USRROL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
