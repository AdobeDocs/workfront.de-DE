---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 19
description: Adobe Workfront hat die API-Version 19 am 6. April 2022 veröffentlicht. API Version 19 enthält die folgenden Änderungen gegenüber Version 18.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: e3f50efa03a43c44e9defd0a724b0516504b0e83
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# Neue Funktionen in API Version 19

Adobe Workfront hat die API-Version 19 am 8. April 2024 veröffentlicht. API Version 19 enthält die folgenden Änderungen gegenüber Version 18.

## Hinzugefügte Ressourcen

Für API Version 19 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API-Version 19 wurden keine Ressourcen entfernt

## Geänderte Ressourcen

### AccessLevel (ACSLVL)

Ein AccessLevel -Objekt ist mit Benutzern verknüpft und beschreibt den Satz von AccessLevelPermissions, der bestimmt, auf welchen Benutzer zugreifen können.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>Die folgenden möglichen Werte wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p>Deaktivieren des Workfront AI-Assistenten (AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Zuweisung (ASSGN)

Ein Zuweisungsobjekt stellt die Verbindung zwischen einem Arbeitselement und dem Benutzer, Team oder der Gruppe dar, der bzw. die für die Bearbeitung zugewiesen ist.

Das Zuweisungsobjekt hat das Flag **DATA_EXTENDIBLE** hinzugefügt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden direkten Felder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>categoryID</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, ein benutzerdefiniertes Formular zu einer Zuweisung hinzuzufügen.
            </p>
          </li>
          <li>
            <p><b>Priorität</b><p>Dieses Feld ermöglicht die folgenden Werte:
            <ul>
              <li>0 (Keine)</li>
              <li>1 (Niedrig)</li>
              <li>2 (Normal)</li>
              <li>3 (Hoch)</li>
              <li>4 (dringend)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>Die folgenden Referenzfelder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>category</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, ein benutzerdefiniertes Formular zu einer Zuweisung hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>Die folgenden Kollektionsfelder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, ein benutzerdefiniertes Formular zu einer Zuweisung hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Kategorie (KG)

Ein Category -Objekt ist ein benutzerdefiniertes Formular.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden Felder wurden hinzugefügt, um das Hinzufügen eines benutzerdefinierten Formulars zu einer Zuweisung zu unterstützen.
        <ul>
          <li>
            <p><b>catObjCode</b><p>Die folgenden möglichen Werte wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p>Zuweisung (ASSGN)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>Die folgenden möglichen Werte wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p>Zuweisung (ASSGN)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Classifier (CLSF)

Ein Klassifizierer ist ein Ort.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>Die folgenden Aktionen wurden hinzugefügt:
        <ul>
          <li>
            <b>activateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Kunde

Ein Kundenobjekt stellt eine Organisation dar, die eine Instanz von Workfront verwendet.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>Die folgenden möglichen Werte wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p>Zuweisungsprioritäten (PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>Das CustomEnum -Objekt unterstützt die Konvertierung von Status-Codes in für Menschen lesbaren Text.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### CustomerPreferences (CUSTPR)

Ein CustomerPreferences -Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Instanz von Workfront festgelegt hat.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>Die folgenden möglichen Werte wurden entfernt:
            </p>
            <ul>
              <li>
                <p>Aktivieren Sie die Zoom-Integration im Aktualisierungsstream (password:zoomIntegrationEnabled)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Dokument (DOCU)

Ein Dokumentobjekt stellt eine Datei dar (z. B. schriftliches Material, Bilder oder andere Informationsformen).

<table>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>Das Feld <code>folderID</code> wurde hinzugefügt.</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### ExchangeRate (EXRATE)

Ein ExchangeRate-Objekt stellt einen in Workfront eingerichteten Wechselkurs dar. ExchangeRate-Objekte sind nicht dynamisch.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
      <ul>
      <li>Die folgenden Felder haben den Validator <code>REQUIRED</code> hinzugefügt:
        <ul>
          <li><p><b>currency</b></li>
          <li><p><b>rate</b></li></ul>
      <li>Die folgenden Felder wurden hinzugefügt:
        <ul>
          <li><p><b>enterByID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>
      <ul>
        <li>Die folgenden Felder wurden hinzugefügt:
        <ul>
          <li><p><b>enterBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gruppe (GRUPPE)

Ein Group -Objekt stellt eine Gruppe von Benutzern und Teams dar. Gruppen repräsentieren oft die Struktur der Abteilungen.

Das Group -Objekt hat die Markierung **SHARABLE** hinzugefügt.

### Stunde (STUNDE)

Ein Hour -Objekt stellt eine Stunde dar, die von einem Benutzer auf einem Timesheet protokolliert wird.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
      Die folgenden Felder wurden hinzugefügt:
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>rejectedByID</b></li>
          <li><p><b>rejectedOnDate</b></li>
          <li><p><b>rejectionComment</b></li>
          <li><p><b>submitByID</b></li>
          </ul>
          <p>Die folgenden Änderungen wurden am Feld <b>Stunden</b> vorgenommen.</p>
          <ul> 
          <li> Validator <b>GREATER_THAN</b> entfernt</li>
          <li> Validator <b>NOT_EQUAL</b> hinzugefügt</li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
      Die folgenden Aktionen wurden hinzugefügt:
        <ul>
          <li><p><b>approve</b></li>
          <li><p><b>unapprove</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

Das JournalEntry -Objekt kann so eingerichtet werden, dass bei jeder Änderung dieser Felder Informationen über bestimmte Objektfelder protokolliert werden. Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird bei jeder Änderung dieses Felds ein entsprechender Journaleintrag erstellt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>Flags</b><p>Die folgenden möglichen Werte wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p>Ist Kostensatz (CR)
                </p>
              </li>
              <li>
                <p>Ist Abrechnungsrate (BR)
                </p>
              </li>
              <li>
                <p>Ist allgemeine Finanzierungen (GF)
                </p>
              </li>
              <li>
                <p>Ist kombinierte Finanzierungen (KF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Parameter (PARAM)

Ein Parameter -Objekt ist ein benutzerdefiniertes Feld.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>Der folgende mögliche Wert wurde hinzugefügt:
            <ul>
            <li>Dauer (DRN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Die folgenden möglichen Werte wurden hinzugefügt:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Bild (BILD)</li>
            <li>PDF (PDF)</li>
            <li>Video (VIDEO)</li>
            <li>Externe Suche (EXTRNL)</li>
            <li>Externe Suche mit Mehrfachauswahl (MULTEXTRNL)</li>
            <li>Natives Feld (WFNATIV)</li>
            <li>Planungsfeld (WFPLANUNG)</li>
            <li>Zeitphasen-KPI (TIMEPHASED)</li>
            <li>Datenaggregation (ROLLUP)</li>
            <li>Dokumente (DOKUMENT)</li>
           </ul>
          </li>
          <li>
            <p><b>Konfigurationen</b><p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Rolle (ROLE)

Ein Rollenobjekt (Auftragsrolle) stellt eine funktionale Kapazität oder eine von einem Benutzer auszufüllende Fähigkeit dar, z. B. Designer oder Produktmanager.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
    Die folgenden Felder wurden hinzugefügt:
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>
        Die folgenden Felder wurden hinzugefügt:
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion {#scorecardquestion}

Ein ScoreCardQuestion -Objekt stellt eine Frage dar, die einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfolio-Manager bestimmt und ihre Antworten ermöglichen es dem Manager zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
            <p><b>displayType</b></p><p>Die folgenden möglichen Werte wurden hinzugefügt:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Bild (BILD)</li>
            <li>PDF (PDF)</li>
            <li>Video (VIDEO)</li>
            <li>Externe Suche (EXTRNL)</li>
            <li>Externe Suche mit Mehrfachauswahl (MULTEXTRNL)</li>
            <li>Natives Feld (WFNATIV)</li>
            <li>Planungsfeld (WFPLANUNG)</li>
            <li>Zeitphasen-KPI (TIMEPHASED)</li>
            <li>Datenaggregation (ROLLUP)</li>
            <li>Dokumente (DOKUMENT)</li>
           </ul>
      </td>
  </tbody>
</table>

### TemplateAssignment (TASSGN)

Ein TemplateAssignment -Objekt stellt die Verbindung zwischen einer Vorlagenaufgabe und dem Benutzer, Team oder der Gruppe dar, der bzw. die für die Bearbeitung zugewiesen ist. Wenn die Vorlage für ein Projekt verwendet wird, wird dieser Benutzer, dieses Team oder diese Gruppe der Aufgabe zugewiesen.

Das TemplateAssignment -Objekt hat das Flag **DATA_EXTENDIBLE** hinzugefügt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden direkten Felder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>categoryID</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, ein benutzerdefiniertes Formular zu einer Zuweisung hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>Die folgenden Referenzfelder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>category</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, ein benutzerdefiniertes Formular zu einer Zuweisung hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>Die folgenden Kollektionsfelder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, ein benutzerdefiniertes Formular zu einer Zuweisung hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Datenblatt (TSHET)

Ein Timesheet-Objekt stellt eine virtuelle Timecard dar, mit der Benutzer die tatsächlichen Arbeitsstunden für Aufgaben, Projekte und Hochtypen eingeben können.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>Entfernt.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


