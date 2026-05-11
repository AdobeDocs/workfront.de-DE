---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 22
description: Adobe Workfront veröffentlichte API-Version 22 am 11. Mai 2026. Die API-Version 22 enthält die folgenden Änderungen gegenüber Version 21.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 4%

---

# Neue Funktionen in der API-Version 22

Adobe Workfront veröffentlichte API-Version 22 am 8. Mai 2026. Die API-Version 22 enthält die folgenden Änderungen gegenüber Version 21.

## Ressourcen hinzugefügt

Die folgenden Ressourcen wurden für die API-Version 22 hinzugefügt.

### ReportSharableFolder (RPSHFD)

Sie können freigebbare Berichtsordner verwenden, um Berichte zu organisieren und diese Ordner für andere Benutzer freizugeben. Diese Funktion wurde für Teams entwickelt, die große Mengen an Berichten verwalten und eine skalierbare, konsistente Zugriffskontrolle benötigen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Standardfelder</td>
      <td>
        <ul>
          <li>name</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">Vorgänge</td>
      <td>
        <ul>
          <li>HINZUFÜGEN</li>
          <li>ANZAHL</li>
          <li>LÖSCHEN</li>
          <li>BEARBEITEN</li>
          <li>GET</li>
          <li>BERICHT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## Entfernte Ressourcen

Die folgenden Ressourcen wurden aus API-Version 22 entfernt.

### UserLocation (USRLOC)

Dieses Objekt wurde entfernt.

## Geänderte Ressourcen

Die folgenden Ressourcen wurden für die API-Version 22 geändert.

### Zugriffsebene (ACSLV)

Ein AccessLevel-Objekt ist Benutzern zugeordnet und beschreibt den Satz von AccessLevelPermissions, die bestimmen, auf was Benutzer zugreifen können.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Das folgende Feld wurde mit Änderungen an möglichen Werten geändert. Weitere Informationen finden Sie in der Entwicklerdokumentation .
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessLevelPermissions (ALVPER)

Ein AccessLevelPermissions-Objekt stellt eine bestimmte Berechtigung zum Zugreifen auf, Erstellen oder Ändern eines Workfront-Objekts dar. Diese Berechtigungen können dann mit einer Zugriffsebene verknüpft werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden mit Änderungen an möglichen Werten geändert. Weitere Informationen finden Sie in der Entwicklerdokumentation .
        <ul>
          <li><b>CoreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>sekundäre Aktionen</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Zugriffsanforderung (ACSREQ)

Wenn ein(e) Benutzende(r) keinen Zugriff auf ein Objekt in Workfront hat, das er/sie benötigt, kann er/sie Zugriff auf dieses Objekt anfordern. Das AccessRequest-Objekt stellt diese Anforderung dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Das folgende Feld wurde mit Änderungen an möglichen Werten geändert. Weitere Informationen finden Sie in der Entwicklerdokumentation .
        <ul>
          <li><b>Aktion</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Zugriffsregel (ACSRUL)

Ein AccessRule-Objekt stellt einen Regelsatz in benutzerdefinierten Zugriffsebenen dar, der bestimmt, wie Benutzer erstellte Projekte freigeben können.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden mit Änderungen an möglichen Werten geändert. Weitere Informationen finden Sie in der Entwicklerdokumentation .
        <ul>
          <li><b>CoreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>sekundäre Aktionen</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Validierung (VALIDIERUNG)

Für ein bestimmtes Arbeitselement, z. B. eine Aufgabe, ein Dokument oder eine Arbeitszeittabelle, kann es erforderlich sein, dass eine verantwortliche Person oder ein anderer Benutzer bzw. eine andere Benutzerin das Arbeitselement abzeichnet. Ein Validierungsobjekt stellt die Aktion des Abzeichnens eines Arbeitselements dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Kategorie (CTG)

Ein Kategorieobjekt ist ein benutzerdefiniertes Formular.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Das folgende Feld wurde hinzugefügt.
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Firma (COMPY)

Ein Unternehmensobjekt stellt eine Organisation dar, die aus einer Sammlung von Personen besteht.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmProjectID</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

Das CustomEnum-Objekt unterstützt Sie beim Konvertieren von Status-Codes in für Menschen lesbaren Text.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>Hinzugefügt
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Abfragen</td>
      <td>Hinzugefügt
        <ul>
          <li><p><b>assignstatus</b></p></li>
          <li><p><b>bookingStatus</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### Kunde (CUST)

Ein Customer-Objekt stellt eine Organisation dar, die eine Instanz von Workfront verwendet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Das folgende Feld wurde geändert.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt.</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> (Buchungsstatus)</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> (Zuweisungsstatus)</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
         <ul>
         <li><b>isLegacyCustomerEsmStorageEnabled</b></li>
         <li><b>isLegacyCustomerSystemFileMigrationEnabled</b></li>
         <li><b>LegacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>LegacyCustomerSystemFileMigrationDate</b></li>
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
      <td>Das folgende Feld wurde geändert.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt, um Enterprise Storage Management zu unterstützen:</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>


### Dokument (DOCU)

Ein Dokumentobjekt, das eine Datei darstellt (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>Die folgende Aktion wurde geändert.
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>objID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder (DOCFDR)

Dokumente können in Ordnern organisiert werden. Sie können persönliche Ordner in Ihrem Bereich für persönliche Dokumente erstellen. Das DocumentFolder-Objekt stellt einen dieser Ordner dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
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
      <td>Das folgende Feld wurde hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      Das folgende Feld wurde geändert.
        <ul>
          <li><b>version</b><p>Validator „REQUIRED“ entfernt.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>Die folgende Aktion wurde hinzugefügt.
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Vorgänge</td>
      <td>Der folgende Vorgang wurde hinzugefügt.
        <ul>
          <li><p><b>BEARBEITEN</b></p>
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
      <td>Die folgenden Felder wurden hinzugefügt.
        <ul>
          <li><b>portfolioID</b></li>
          <li><b>programID
          </b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tagebucheintrag (JRNLE)

Das JournalEntry-Objekt kann so eingerichtet werden, dass Informationen zu bestimmten Objektfeldern jedes Mal protokolliert werden, wenn diese Felder geändert werden. Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird jedes Mal, wenn dieses Feld geändert wird, ein entsprechender Journaleintrag erstellt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden geändert.
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Ordner verschieben)</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>Flags</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt.</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.journalEntryFlagenum.isContactInfoEntry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### Journalfeld (JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden geändert.
        <ul>
          <li>
            <p><b>Aktion</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Ordner verschieben)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask (OPTASK)

Ein OpTask-Objekt wird im Allgemeinen als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise darauf hinweist, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungsanforderungen, -anfragen und -fehler sind ebenfalls Probleme.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li><b>actualWorkRequired</b><p>Die folgenden Flags wurden hinzugefügt:
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Felder suchen</td>
      <td>
        <ul>
          <li><b>Tatsächliche Arbeit</b><p>Typ von <code>null</code> in <code>double</code> geändert.</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest(ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Vorgänge</td>
      <td>Die folgenden Vorgänge wurden hinzugefügt.
        <ul>
          <li><p><b>ANZAHL</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>BERICHT</b></p>
          <li><p><b>SEARCH</b></p>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### Parameter (PARAM)

Ein Parameter-Objekt ist ein benutzerdefiniertes Feld.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Parametergruppe (PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### PortalSection (PTLSEC)

Ein PortalSection-Objekt ist ein Bericht.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Das folgende Feld wurde hinzugefügt.
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>Das folgende Feld wurde hinzugefügt.
        <ul>
          <li><b>reportShareableFolder</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Portfolio (PORT)

Ein Portfolio-Objekt ist eine Sammlung von Projekten, die um dieselben Ressourcen konkurrieren, normalerweise Geld oder Personen, um sie abzuschließen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Programm (PRGM)

Ein Programmobjekt ist eine Teilmenge von Projekten innerhalb eines Portfolios, in dem ähnliche Projekte gruppiert werden können.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      Das folgende Feld wurde geändert.
        <ul>
          <li><b>portfolioID</b><p>Validator „REQUIRED“ hinzugefügt.</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Projekt (PROJ)

Projekte sind Arbeitselemente innerhalb von Workfront und ein wichtiger Baustein in der Art und Weise, wie Workfront Menschen bei der Arbeit unterstützt. Ein Project-Objekt stellt eine Gruppe von Aufgaben mit einem gemeinsamen, spezifischen Ziel dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef (QUED)

Ein QueueDef-Objekt stellt eine Anforderungswarteschlangendefinition in Workfront dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden mit Änderungen an möglichen Werten geändert. Weitere Informationen finden Sie in der Entwicklerdokumentation .
        <ul>
          <li><b>RequestorCoreAction</b></li>
          <li><b>RequestorForbiddenActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Geplanter Bericht (SCHREP)

Ein ScheduledReport-Objekt stellt einen Bericht dar, der für die Bereitstellung geplant wurde.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Das folgende Feld wurde mit umfangreichen Änderungen an möglichen Werten geändert. Weitere Informationen finden Sie in der Entwicklerdokumentation .
        <ul>
          <li><b>Format</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Aufgabe (AUFGABE)

Ein Aufgabenobjekt stellt ein Arbeitselement dar, das zum Erreichen eines endgültigen Ziels (Abschließen eines Projekts) abgeschlossen werden muss.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>Hinzugefügt</p></li>
          <li><p><b>actualWorkRequired</b></p><p>Es wurden Flags <code>AUTO_LOAD</code> und <code>DYNAMIC</code> hinzugefügt.</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>
        <ul>
          <li>
            <p><b>convertedOpTask</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
        </ul> 
      </td>
    </tr>
  </tbody>
</table>

### Vorlage (TMPL)

Ein Vorlagenobjekt stellt ein Muster für ein Projekt dar. Projekte können aus Vorlagen erstellt werden, um Zeit zu sparen. Eine Vorlage enthält ein Team und Aufgaben, die in jedes aus der Vorlage erstellte Projekt kopiert werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um Enterprise Storage Management zu unterstützen.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>Das folgende Feld wurde geändert.
        <ul>
          <li>
            <p><b>Aktion</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt.</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### Benutzer (USER)

Ein Benutzerobjekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Das folgende Feld wurde hinzugefügt.
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>Das folgende Feld wurde entfernt.
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





