---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 17
description: Adobe Workfront hat die API-Version 17 am 6. April 2022 veröffentlicht. API Version 17 enthält die folgenden Änderungen gegenüber Version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: 08e90754-5505-424c-ae67-015cc987b5df
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 4%

---

# Neue Funktionen in API Version 17

Adobe Workfront hat die API-Version 17 am 12. Oktober 2023 veröffentlicht. API Version 17 enthält die folgenden Änderungen gegenüber Version 16.

## Hinzugefügte Ressourcen

<!--

### Booking (BOOKNG)

-->

### ExternalDocument (EXTDOC)

Ein ExternalDocument -Objekt ist ein Dokument oder ein anderes digitales Asset, das sich in einem Dokumentenspeicherungsanbieter außerhalb von Workfront befindet. Diese Assets können mit und aus Workfront verknüpft werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>Durchw</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>path</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>description</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>Durchw</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>path</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>size</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>value</b></p></li>
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
          <li><p><b>customer</b></p></li>
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

Die folgenden Ressourcen wurden für API Version 17 geändert.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Grundlinie (BLIN)

Grundlinien sind Momentaufnahmen davon, wie die Leistung eines Projekts zu einem bestimmten Zeitpunkt aussah. Sie speichern wichtige Informationen zum Projekt, wie z. B. Schlüsseldaten, Fortschritt, Kosten und Umsatzwerte.

Das Grundlinien-Objekt hat die Markierung entfernt **INLINE_EDITABLE**.

### BillingRecord (BILL)

Ein BillingRecord -Objekt zeichnet die Einnahmen, Stunden oder Ausgaben auf, die abgerechnet werden können. Diese Informationen können zur Erstellung von Rechnungen in einem externen Buchführungssystem verwendet werden.

Das BillingRecord -Objekt hat die Markierung entfernt **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Unternehmen (CMPY)

Ein Unternehmensobjekt stellt eine Organisation dar, die aus einer Personensammlung besteht.

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
            <p>Entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### CustomerPreferences (CUSTPR)

Ein CustomerPreferences -Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Instanz von Workfront festgelegt hat.

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
            <p>Der mögliche Wert "config.defaultToNewHomeDescription"(customer:config.defaultToNewHome)&gt;/p wurde hinzugefügt.<p>Dadurch kann eine Organisation das neue Starterlebnis zum Standard für ihre Benutzer machen.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### DocumentVersion (DOCV)

Ein DocumentVersion -Objekt stellt eine bestimmte Version einer Datei dar (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

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
            <p>Der mögliche Wert "Frame.io"(FRAMEIO) wurde hinzugefügt.</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>Der mögliche Wert "enum.filetype.site"(Site) wurde hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### ExchangeRate (EXRATE)

Ein ExchangeRate-Objekt stellt einen in Workfront eingerichteten Wechselkurs dar. ExchangeRate-Objekte sind nicht dynamisch.

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
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>Hinzugefügt.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Ausgaben (EXPNS)

Ausgaben stellen die Nichtarbeitskosten dar, die während der Laufzeit eines Projekts anfallen könnten.

Das Spesenobjekt entfernte das Flag **INLINE_EDITABLE**.

### Gruppe (GRUPPE)

Ein Group -Objekt stellt eine Gruppe von Benutzern und Teams dar. Gruppen repräsentieren oft die Struktur der Abteilungen.

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
            <p>Entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Stunde (STUNDE)

Ein Hour -Objekt stellt eine Stunde dar, die von einem Benutzer auf einem Timesheet protokolliert wird.

Das Objekt Stunde entfernt die Markierung **INLINE_EDITABLE**.

### Iteration (ITRN)

Ein Iteration -Objekt stellt eine einzelne Agile Iteration dar. Iterationen sind diskrete Zeiträume, die zur Planung und Ergänzung von Agile-Geschichten verwendet werden.

Das Iterationsobjekt entfernte das Flag **INLINE_EDITABLE**.


### JournalEntry (JRNLE)

Das JournalEntry -Objekt kann so eingerichtet werden, dass bei jeder Änderung dieser Felder Informationen über bestimmte Objektfelder protokolliert werden. Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird bei jeder Änderung dieses Felds ein entsprechender Journaleintrag erstellt.

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
              <li>Genehmiger hinzugefügt (AAA)</li>
              <li>Überprüfer hinzugefügt (AAR)</li>
              <li>Überprüfer entfernt (ARR)</li>
              <li>Genehmiger (ARA) entfernt</li>
              <li>Genehmigte Entscheidung (ADA)</li>
              <li>Mit Änderungen genehmigte Entscheidung (ADC)</li>
              <li>Entscheidungsbedarf (ADN)</li>
              <li>Entscheidung aufgehoben (ADR)</li>
              <li>Genehmiger geändert (AAC)</li>
              <li>Überprüfer geändert (ARC)</li>
              <li>Abschluss der Überprüfung (RDC)</li>
              <li>Rückgängig gezogene Überprüfung (RDR)</li>
              <li>Veröffentlichen (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kanban Board (KNBNBD)

Ein Kanban-Board wird verwendet, um Aufgaben in einer Agile-Umgebung zu verfolgen.

Das Objekt des Kanban-Boards hat die Flagge entfernt **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

Ein LinkedFolder-Objekt stellt einen Ordner dar, der von einem externen Dokumentenanbieter wie Google Drive oder Dropbox verknüpft ist.

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
            <p>Möglicher Wert "Frame.io (FRAMEIO)"hinzugefügt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask/Problem (OPTASK)

Ein OpTask-Objekt wird häufig als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise anzeigt, dass ein Problem vorliegt, das die Fertigstellung einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungen bei Bestellungen, Anforderungen und Fehlern sind ebenfalls Probleme.

Das Problem -Objekt hat die Markierung entfernt **INLINE_EDITABLE**.

### Projekt (PROJ)

Projekte sind Arbeitselemente in Workfront und stellen einen Hauptbaustein dar, wie Workfront Menschen bei der Arbeit unterstützt. Ein Projektobjekt stellt eine Gruppe von Aufgaben mit einem gemeinsamen, spezifischen Ziel dar.

Das Projektobjekt hat die Markierung entfernt **INLINE_EDITABLE**.

### ProjectUser (PRTU)

Ein ProjectUser -Objekt stellt einen Benutzer dar, der einem bestimmten Projekt zugeordnet ist.

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
            <p>Hinzugefügt.</p>
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
            <p>Hinzugefügt.</p>
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

### Rate (RATE)

Ein Rate -Objekt stellt eine Abrechnungsrate in Workfront dar.

Das Objekt Rate entfernt die Markierung **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>Die folgenden Aktionen wurden hinzugefügt, um die Funktion der Ratenkarte zu unterstützen:
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>Die <b>setRatesForRole</b> -Aktion wurde geändert, um die folgenden Felder hinzuzufügen:
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risiko (RISIKO)

Ein Risikoobjekt stellt ein mögliches Ereignis dar, das verhindern kann, dass ein Projekt rechtzeitig oder innerhalb des Budgets beendet wird. In der Planungsphase werden den Projekten Risiken hinzugefügt, um potenzielle Hindernisse vor der Genehmigung von Arbeiten zu ermitteln.

Das Risikoobjekt hat die Markierung entfernt **INLINE_EDITABLE**.

### Rolle/Auftragsrolle (ROLE)

Ein Rollenobjekt (Auftragsrolle) steht für eine funktionale Kapazität oder eine Fachkompetenz, die ein Benutzer ausfüllen kann, z. B. Designer oder Produkt-Manager.

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
            <p>Entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Aufgabe (TASK)

Ein Task -Objekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (zum Abschließen eines Projekts) ausgeführt werden muss.

Das Task-Objekt hat die Markierung entfernt **INLINE_EDITABLE**.

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
            <p>Entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TeamMember (TEAMB)

Ein TeamMember-Objekt ist ein Benutzer, der einem bestimmten Team zugeordnet ist.

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
            <p>Hinzugefügt.</p>
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
            <p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser (TMTU)

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
            <p>Hinzugefügt.</p>
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
            <p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Datenblatt (TSHET)

Ein Timesheet-Objekt stellt eine virtuelle Timecard dar, mit der Benutzer die tatsächlichen Arbeitsstunden für Aufgaben, Projekte und Hochtypen eingeben können.

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
            <p>Entfernt</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Aktualisieren (AKTUALISIEREN)

Arbeitselemente in Workfront können aktualisiert werden, damit Benutzer über den aktuellen Status informiert werden. Ein Update -Objekt stellt eine dieser Aktualisierungen dar. Aktualisierungen können von Benutzern eingegeben oder vom Workfront-System erstellt werden.

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
              <li>Genehmiger hinzugefügt (assetapprovalAddApprover)</li>
              <li>Überprüfer hinzugefügt (assetapprovalAddReviewer)</li>
              <li>Genehmiger entfernt (assetapprovalRemoveApprover)</li>
              <li>Überprüfer entfernt (assetapprovalRemoveReviewer)</li>
              <li>Entscheidung genehmigt (assetapprovalDecisionApproved)</li>
              <li>Entscheidungsbedarf funktioniert (assetapprovalDecisionNeedsWork)</li>
              <li>Mit Änderungen genehmigte Entscheidung (assetapprovalDecisionApprovedChanges)</li>
              <li>Entscheidung widerrufen (assetapprovalDecisionRevoked)</li>
              <li>Genehmiger geändert (assetapprovalApproverChanged)</li>
              <li>Überprüfer geändert (assetapprovalReviewerChanged)</li>
              <li>Review abgeschlossen (assetapprovalReviewerDecisionComplete)</li>
              <li>Überprüfung gesperrt (assetapprovalReviewerDecisionRevoked)</li>
              <li>Fehler beim Senden eines externen Dokuments (externalDocumentSendError)</li>
              <li>Veröffentlichte Dokumentversion (documentVersionPublish)</li>
              <li>Workflow für verknüpfte Ordner (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Benutzer (BENUTZER)

Ein User -Objekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

Das User -Objekt hat die Markierung entfernt **INLINE_EDITABLE**.

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
            <p>Dieses Feld wurde hinzugefügt. Es ist eine Zahl zwischen 0 und 1, die den Prozentsatz der Zeit darstellt, die ein Benutzer täglich für die Projektarbeit (ohne Overhead) verbringen kann. Der Wert 1 bedeutet, dass der Benutzer 100 % seiner Zeit mit Projektarbeit verbringen kann.</p>
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

### UserGroups (USRGPS)

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
            <p>Hinzugefügt.</p>
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
            <p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### UserNote (USRNOT)

Ein UserNote -Objekt ist eine Benachrichtigung.

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
              <li>Dokument erfordert Ihre Genehmigung (AAA)</li>
              <li>Dokument benötigt Ihre Überprüfung (AAR)</li>
              <li>Dokument benötigt Ihre Genehmigung nicht mehr (ARA).</li>
              <li>Dokument benötigt Ihre Überprüfung nicht mehr (ARR)</li>
              <li>Validierung (ATA) für Dokumentanforderungen (Benutzer)</li>
              <li>Überprüfung der Dokumentenanforderungen (Benutzer) (ATR)</li>
              <li>Dokument muss nicht mehr genehmigt werden (Benutzer) (RTA)</li>
              <li>Dokument muss nicht mehr (Benutzer) überprüft werden (RTR).</li>
              <li>Dokument genehmigt (ADA)</li>
              <li>Dokument mit Änderungen genehmigt (ADC)</li>
              <li>Arbeit für Dokument erforderlich (ADN)</li>
              <li>(Benutzer) hat (Dokument) als genehmigt markiert. Ihre Genehmigung ist nicht mehr erforderlich. (AN)</li>
              <li>(Benutzer) hat (Dokument) mit den Änderungen als genehmigt markiert. Ihre Genehmigung ist nicht mehr erforderlich. (ACN)</li>
              <li>(Benutzer) hat markiert (Dokument), da es funktioniert. Ihre Genehmigung ist nicht mehr erforderlich. (AWN)</li>
              <li>Dokument erfordert Ihre Überprüfung jetzt anstatt der Genehmigung (AAC)</li>
              <li>Dokument erfordert Ihre Genehmigung jetzt anstatt einer Überprüfung (ADN)</li>
              <li>Dokument geprüft (RDC)</li>
              <li>Dokument geprüft (TRC)</li>
              <li>(Benutzer) hat als abgeschlossen geprüft (Dokument). Ihre Überprüfung ist nicht mehr erforderlich. TRN</li>
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
            <p>Hinzugefügt.</p>
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
            <p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
