---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 21
description: Adobe Workfront hat API Version 21 am 23. Oktober 2025 veröffentlicht. Die API-Version 21 enthält die folgenden Änderungen gegenüber Version 20.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 7166a6b51a45b744a33df697c2bc8080427908a8
workflow-type: tm+mt
source-wordcount: '932'
ht-degree: 3%

---

# Neue Funktionen in der API-Version 21

>[!IMPORTANT]
>
>Diese API-Versionsänderung beinhaltet eine grundlegende Änderung, die sich auf Ihre vorhandenen API-Aufrufe auswirken kann. Dies liegt daran, dass die API-Version 21 die Ereignisabonnements-Version 2 verwendet.
>
> Bei Feldern mit Mehrfachauswahl werden Ereignisabonnements in Version 2 immer als Array gesendet. Version 1 hat ein Array gesendet, wenn mehr als ein Wert ausgewählt ist. Wenn nur ein Wert ausgewählt war, wurde eine Zeichenfolge gesendet.

Adobe Workfront hat API Version 21 am 23. Oktober 2025 veröffentlicht. Die API-Version 21 enthält die folgenden Änderungen gegenüber Version 20.

## Ressourcen hinzugefügt

### OriginalRequest (ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>entryDate</li>
          <li>ID</li>
          <li>requestID</li>
          <li>requestName</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>ID</li>
          <li>objCode</li>
        </ul>
      </td>
 </tbody>
</table>

<!--

### StaffingPlanTemplate (SPTMPL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li>ADD</li>
          <li>COUNT</li>
          <li>DELETE</li>
          <li>EDIT</li>
          <li>GET</li>
          <li>REPORT</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

## Entfernte Ressourcen

### ZuweisungBillingRole (ASBURL)

Das AssignmentBillingRole-Objekt und alle zugehörigen Felder wurden entfernt.

## Geänderte Ressourcen

### AccessLevelPermissions (ALVPER)

Ein AccessLevelPermissions-Objekt stellt eine bestimmte Berechtigung zum Zugreifen auf, Erstellen oder Ändern eines Workfront-Objekts dar. Diese Berechtigungen können dann mit einer Zugriffsebene verknüpft werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
            </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>Aktion</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Anhang zur Ankündigung (ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Validierung (VALIDIERUNG)

Für ein bestimmtes Arbeitselement, z. B. eine Aufgabe, ein Dokument oder eine Arbeitszeittabelle, kann es erforderlich sein, dass ein Verantwortlicher oder ein anderer Benutzer das Arbeitselement abzeichnet. Ein Validierungsobjekt stellt die Aktion des Abzeichnens eines Arbeitselements dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>TeamAssignments</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Zuweisung (ZUWEISUNG)

Ein Arbeitsauftragsobjekt stellt die Verbindung zwischen einem Arbeitselement und dem Benutzer, Team oder der Gruppe dar, der bzw. die für die Bearbeitung zugewiesen ist.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>Entfernt</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>TEAMOB</code> (Team)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Kunde (CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (Deaktiviert die Verwendung eines Java-Applets für Zeitleistenberechnungen)
            </p>
            <p>Hinzugefügt</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Dokument (DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>Hinzugefügt</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder

Das DocumentFolder-Objekt hat die `RESTORABLE` hinzugefügt.

### Stunde (STUNDE)

Ein Stunden -Objekt steht für eine Stunde, die ein Benutzer in einer Arbeitszeittabelle protokolliert.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>getTerejectionCommentmporaryCloudURL</b>
            </p>
            <p>Validator hinzugefügt <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
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
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Hinzugefügt</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (lexikalischer Rich-Text)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Einzeilige Datenaggregation)</p>
              </li></ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Hinzugefügt</p>
           </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standardfelder</td>
      <td>
        <ul>
         <li>
            <p><b>isActive</b>
            </p>
            <p>Hinzugefügt</p>
           </li>
           </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>Hinzugefügt</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>Währung</b>
            </p>
            <p>Hinzugefügt</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Hinzugefügt</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Ein QueueDef -Objekt stellt eine Warteschlange dar. Dabei handelt es sich um ein Projekt, das im Helpdesk-Bereich veröffentlicht wurde, um Benutzenden die Übermittlung von Problemen zu ermöglichen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>RequestorCoreAction</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>RequestorForbiddenActions</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Kontaktinformationen bearbeiten)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>helpDeskProjects</b>
            </p>
            <p>Hinzugefügt</p>
            </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Satz (RATE)

Ein Tarifobjekt stellt einen Abrechnungssatz in Workfront dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>localBillingPerHour</b>
            </p>
            <p>Entfernt</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>Entfernt</p>
              </li>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Rolle (ROLE)

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
            <p><b>Währung überschreiben</b>
            </p>
            <p>Entfernt</p>
              </li>
          <li>
            <p><b>Kostensatz überschreiben</b>
            </p>
            <p>Entfernt</p>
              </li>
          <li>
            <p><b>Abrechnungssatz überschreiben</b>
            </p>
            <p>Entfernt</p>
              </li>
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
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Ein ScoreCardQuestion-Objekt stellt eine Frage dar, die zu einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfolio-Manager bestimmt, und die Antworten geben dem Manager die Möglichkeit zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Einzeilige Datenaggregation)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### StaffingPlan

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

<!--

### StaffingPlanResource

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>totalEstimatedCost</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Added</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Added</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

-->

### Aufgabe (AUFGABE)

Ein Aufgabenobjekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (Fertigstellen eines Projekts) ausgeführt werden muss.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>TeamAssignments</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Team

Das Team-Objekt fügte die Flags `DATA_EXTENDIBLE` und `SHARABLE` hinzu.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>
        <ul>
          <li>
            <p><b>Kategorie</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### Vorlagenzuweisung

Das TemplateAssignment-Objekt hat die `ATTRIBUTE_ATTACHABLE` hinzugefügt.

### Arbeitszeittabelle (TABELLE)

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Kernfelder</td>
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

### Arbeit (ARBEIT)

Ein Arbeitsobjekt ist eine gemeinsame Schnittstelle, die sowohl von Task als auch von OpTask erbt wird und gemeinsamen Code zwischen den beiden verwendet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>actualWorkRequiredDouble</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>TeamAssignments</b>
            </p>
            <p>Hinzugefügt</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


