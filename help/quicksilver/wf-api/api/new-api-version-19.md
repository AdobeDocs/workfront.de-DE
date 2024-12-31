---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 19
description: Adobe Workfront hat API Version 19 am 6. April 2022 veröffentlicht. Die API-Version 19 enthält die folgenden Änderungen gegenüber Version 18.
author: Becky
feature: Workfront API
role: Developer
exl-id: 84909dea-7ce1-4ad3-90f5-9dbdb354eaa4
source-git-commit: 8428bfba81fa988cf370581af0692e4ff595c0ae
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Neue Funktionen in der API-Version 19

Adobe Workfront hat API Version 19 am 8. April 2024 veröffentlicht. Die API-Version 19 enthält die folgenden Änderungen gegenüber Version 18.

## Ressourcen hinzugefügt

Für API-Version 19 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API-Version 19 wurden keine Ressourcen entfernt

## Geänderte Ressourcen

### Zugriffsebene (ACSLV)

Ein AccessLevel-Objekt ist Benutzern zugeordnet und beschreibt den Satz von AccessLevelPermissions, die bestimmen, auf was Benutzer zugreifen können.

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
                <p>Deaktivieren des Workfront-KI-Assistenten (AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Zuweisung (ZUWEISUNG)

Ein Arbeitsauftragsobjekt stellt die Verbindung zwischen einem Arbeitselement und dem Benutzer, Team oder der Gruppe dar, der bzw. die für die Bearbeitung zugewiesen ist.

Das Zuweisungsobjekt hat das Flag **DATA_EXTENDIBLE** hinzugefügt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden direkten Felder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>categoryID</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, einem Arbeitsauftrag ein benutzerdefiniertes Formular hinzuzufügen.
            </p>
          </li>
          <li>
            <p><b>Priorität</b><p>Dieses Feld lässt die folgenden Werte zu:
            <ul>
              <li>0 (keine)</li>
              <li>1 (Niedrig)</li>
              <li>2 (normal)</li>
              <li>3 (Hoch)</li>
              <li>4 (Dringend)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>Die folgenden Referenzfelder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>Kategorie</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, einem Arbeitsauftrag ein benutzerdefiniertes Formular hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>Die folgenden Sammlungsfelder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, einem Arbeitsauftrag ein benutzerdefiniertes Formular hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Kategorie (CTG)

Ein Kategorieobjekt ist ein benutzerdefiniertes Formular.

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
                <p>Zuweisung (ZUWEISUNG)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>Die folgenden möglichen Werte wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p>Zuweisung (ZUWEISUNG)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Klassifikator (CLSF)

Ein Klassifikator ist ein Speicherort.

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
            <b>DeaktivierenClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Kunde

Ein Customer-Objekt stellt eine Organisation dar, die eine Instanz von Workfront verwendet.

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
              <p>Das CustomEnum-Objekt unterstützt Sie beim Konvertieren von Status-Codes in für Menschen lesbaren Text.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Kundenvoreinstellungen (CUSTPR)

Ein CustomerPreferences-Objekt stellt den Satz von Voreinstellungen dar, die ein Kunde für seine Workfront-Instanz festgelegt hat.

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
                <p>Zoom-Integration im Updates-Stream aktivieren (Kennwort:zoomIntegrationEnabled)
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

Ein Dokumentobjekt, das eine Datei darstellt (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

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
            <p><b>sendDocumentsToExternalProvider</b><p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### Wechselkurs (EXRATE)

Ein ExchangeRate-Objekt stellt einen in Workfront eingerichteten Wechselkurs dar. Wechselkursobjekte sind nicht dynamisch.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
      <ul>
      <li>Die folgenden Felder haben den Validator-<code>REQUIRED</code> hinzugefügt:
        <ul>
          <li><p><b>Währung</b></li>
          <li><p><b>Satz</b></li></ul>
      <li>Die folgenden Felder wurden hinzugefügt:
        <ul>
          <li><p><b>enteredByID</b></li>
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
          <li><p><b>enteredBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gruppe (GROUP)

Ein Gruppenobjekt steht für eine Gruppe von Benutzern und Teams. Gruppen repräsentieren oft die Abteilungsstruktur.

Das Gruppenobjekt hat das Flag **SHARABLE** hinzugefügt.

### Stunde (STUNDE)

Ein Stunden -Objekt steht für eine Stunde, die ein Benutzer in einer Arbeitszeittabelle protokolliert.

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
          <li><p><b>failedByID</b></li>
          <li><p><b>failedOnDate</b></li>
          <li><p><b>Zurückweisungskommentar</b></li>
          <li><p><b>submitByID</b></li>
          </ul>
          <p>Folgende Änderungen wurden am Feld <b>Stunden</b> vorgenommen.</p>
          <ul> 
          <li> Validator entfernt <b>GREATER_THAN</b></li>
          <li> Validator hinzugefügt <b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
      Die folgenden Aktionen wurden hinzugefügt:
        <ul>
          <li><p><b>genehmigen</b></li>
          <li><p><b>Genehmigung aufheben</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tagebucheintrag (JRNLE)

Das JournalEntry-Objekt kann so eingerichtet werden, dass Informationen zu bestimmten Objektfeldern jedes Mal protokolliert werden, wenn diese Felder geändert werden. Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird jedes Mal, wenn dieses Feld geändert wird, ein entsprechender Journaleintrag erstellt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>Markierungen</b><p>Die folgenden möglichen Werte wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p>Ist Kostensatz (CR)
                </p>
              </li>
              <li>
                <p>Ist Abrechnungssatz (BR)
                </p>
              </li>
              <li>
                <p>Ist die allgemeine Finanzierung (GF)
                </p>
              </li>
              <li>
                <p>Ist kombinierte Finanzierung (KF)
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

Ein Parameter-Objekt ist ein benutzerdefiniertes Feld.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>Der folgende mögliche Wert wurde hinzugefügt:
            <ul>
            <li>Dauer (DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Um ein benutzerfreundlicheres und flexibleres System zu erstellen, wird der <b>Widget (WIDGET</b>-Feldtyp nicht mehr unterstützt und in die folgenden Feldtypen unterteilt:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Bild (IMAGE)</li>
            <li>PDF PDF</li>
            <li>Video (VIDEO)</li>
            <li>Externe Suche (EXTRNL)</li>
            <li>Externe Suche mit Mehrfachauswahl (MULTEXTRNL)</li>
            <li>Natives Feld (WFNATIVE)</li>
            <li>Feld „Planung“ (WFPLANNING)</li>
            <li>Zeitphasen-KPI (TIMEPHASED)</li>
            <li>Datenaggregation (ROLLUP)</li>
            <li>Dokumente (DOKUMENT)</li>
           </ul>
          </li>
          <li>
            <p><b>Konfigurationen</b><p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Rolle (ROLE)

Ein Rollenobjekt (Aufgabengebiet) stellt eine funktionale Kapazität oder eine Qualifikation dar, die ein Benutzer ausfüllen kann, z. B. Designer oder Product Manager.

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

Ein ScoreCardQuestion-Objekt stellt eine Frage dar, die zu einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfoliomanager bestimmt und ihre Antworten geben dem Portfolio die Möglichkeit zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
            <p><b>displayType</b></p><p>Um ein benutzerfreundlicheres und flexibleres System zu erstellen, wird der <b>Widget (WIDGET</b>-Feldtyp nicht mehr unterstützt und in die folgenden Feldtypen unterteilt:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Bild (IMAGE)</li>
            <li>PDF PDF</li>
            <li>Video (VIDEO)</li>
            <li>Externe Suche (EXTRNL)</li>
            <li>Externe Suche mit Mehrfachauswahl (MULTEXTRNL)</li>
            <li>Natives Feld (WFNATIVE)</li>
            <li>Feld „Planung“ (WFPLANNING)</li>
            <li>Zeitphasen-KPI (TIMEPHASED)</li>
            <li>Datenaggregation (ROLLUP)</li>
            <li>Dokumente (DOKUMENT)</li>
           </ul>
      </td>
  </tbody>
</table>

### Vorlagenzuweisung (TASSGN)

Ein TemplateAssignment-Objekt stellt die Verbindung zwischen einer Vorlagenaufgabe und dem Benutzer, dem Team oder der Gruppe dar, der bzw. die für die Bearbeitung zugewiesen ist. Wenn die Vorlage für ein Projekt verwendet wird, wird dieser Benutzer, dieses Team oder diese Gruppe der Aufgabe zugewiesen.

Das TemplateAssignment-Objekt hat das Flag **DATA_EXTENDIBLE** hinzugefügt.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>Die folgenden direkten Felder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>categoryID</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, einem Arbeitsauftrag ein benutzerdefiniertes Formular hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>Die folgenden Referenzfelder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>Kategorie</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, einem Arbeitsauftrag ein benutzerdefiniertes Formular hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>Die folgenden Sammlungsfelder wurden hinzugefügt:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieses Feld unterstützt die Möglichkeit, einem Arbeitsauftrag ein benutzerdefiniertes Formular hinzuzufügen.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Arbeitszeittabelle (TABELLE)

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>entfernt.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>
