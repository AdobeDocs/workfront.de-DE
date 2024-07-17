---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 18
description: Adobe Workfront hat die API-Version 18 am 6. April 2022 veröffentlicht. API Version 18 enthält die folgenden Änderungen gegenüber Version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Neue Funktionen in API Version 18

Adobe Workfront hat die API-Version 18 am 8. April 2024 veröffentlicht. API Version 18 enthält die folgenden Änderungen gegenüber Version 15.

## Hinzugefügte Ressourcen

Für API Version 18 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API-Version 18 wurden keine Ressourcen entfernt

## Geänderte Ressourcen

### AccessLevelPermissions (ALVPER)

Ein AccessLevelPermissions -Objekt stellt eine spezifische Berechtigung zum Zugreifen auf, Erstellen oder Ändern eines Workfront-Objekts dar. Diese Berechtigungen können dann einer Zugriffsebene zugeordnet werden.

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
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Wenn ein Benutzer keinen Zugriff auf ein Objekt in Workfront hat, das er benötigt, kann er den Zugriff auf dieses Objekt anfordern. Das AccessRequest -Objekt stellt diese Anforderung dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>action</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Ein AccessRule -Objekt stellt einen Regelsatz in benutzerdefinierten Zugriffsebenen dar, der bestimmt, wie Benutzer erstellte Projekte freigeben können.

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
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Genehmigung (GENEHMIGUNG)

Ein bestimmtes Arbeitselement, wie z. B. eine Aufgabe, ein Dokument oder ein Timesheet, kann vorschreiben, dass ein Supervisor oder ein anderer Benutzer das Arbeitselement abzeichnet. Ein Approval-Objekt stellt die Aktion zum Abmelden eines Arbeitselements dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ISTBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>ISTNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### WartenGenehmigung (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Vorgänge</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Vorgänge wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ADD</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Grundlinie (BLIN)

Grundlinien sind Momentaufnahmen davon, wie die Leistung eines Projekts zu einem bestimmten Zeitpunkt aussah. Sie speichern wichtige Informationen zum Projekt, wie z. B. Schlüsseldaten, Fortschritt, Kosten und Umsatzwerte.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ISTBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>ISTNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### BaselineTask (BSTSK)

Grundlinien sind Momentaufnahmen davon, wie die Leistung eines Projekts zu einem bestimmten Zeitpunkt aussah. Sie speichern wichtige Informationen zum Projekt, wie z. B. Schlüsseldaten, Fortschritt, Kosten und Umsatzwerte. Wenn Sie eine Grundlinie erstellen, werden die Aufgabeninformationen auch in den Grundaufgaben dieser Grundlinie erfasst.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ISTBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>ISTNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Kategorie (KG)

Ein Category -Objekt ist ein benutzerdefiniertes Formular.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>:
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Nicht-Arbeitskräfte-Ressourcentyp)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Stunde)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Karte Rate)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Nicht-Arbeitskräfte-Ressourcentyp)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Stunde)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Karte Rate)
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Dokument (DOCU)

Ein Dokumentobjekt stellt eine Datei dar (z. B. schriftliches Material, Bilder oder andere Informationsformen).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>Der folgende Parameter wurde hinzugefügt:
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>:
            </p>
            <p>Hinzugefügt. Diese neue Aktion akzeptiert die folgenden Parameter:
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### FinancialData (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ISTBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>ISTNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
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
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ISTBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>ISTNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.entscheidungen.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask (OPTASK)

Ein OpTask-Objekt wird häufig als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise anzeigt, dass ein Problem vorliegt, das die Fertigstellung einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungen bei Bestellungen, Anforderungen und Fehlern sind ebenfalls Probleme.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>Die folgenden Felder wurden hinzugefügt:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>Die folgenden Felder wurden hinzugefügt:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Projekt (PROJ)

Projekte sind Arbeitselemente in Workfront und stellen einen Hauptbaustein dar, wie Workfront Menschen bei der Arbeit unterstützt. Ein Projektobjekt stellt eine Gruppe von Aufgaben mit einem gemeinsamen, spezifischen Ziel dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ISTBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>ISTNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
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
            <p><b>createProjectWithOverride</b>
            </p>
             <p>Hinzugefügt.
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ProjectUserRole (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Das folgende Feld wurde hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p>Das folgende Feld wurde hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Ein QueueDef-Objekt stellt eine Warteschlange dar. Hierbei handelt es sich um ein Projekt, das in den Help Desk-Bereich veröffentlicht wurde, um Benutzern die Möglichkeit zu geben, Probleme an sie zu senden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Anzeigen von Kostensätzen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Rechnungsraten anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzinformationen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Rechnungsgebühren bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzverwaltung bearbeiten)</p>
              </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Rate (RATE)

Ein Rate -Objekt stellt eine Abrechnungsrate in Workfront dar.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>Die folgenden Flags wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DYNAMISCH
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>Hinzugefügt.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Aufgabe (TASK)

Ein Task -Objekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (zum Abschließen eines Projekts) ausgeführt werden muss.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ISTBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>ISTNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
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
            <p><b>convertToProject</b>
            </p>
             <p>Das folgende Feld wurde hinzugefügt:
             <ul><li><code>copyCategories</code></li></ul>
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Vorlage (TMPL)

Ein Template -Objekt stellt ein Muster für ein Projekt dar. Projekte können aus Vorlagen erstellt werden, um Zeit zu sparen. Eine Vorlage enthält ein Team und Aufgaben, die in jedes aus der Vorlage erstellte Projekt kopiert werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### TemplateTask (TTSK)

Ein TemplateTask -Objekt stellt eine Aufgabe dar, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, in dem die Vorlage verwendet wird.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole (TTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Das folgende Feld wurde hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p>Das folgende Feld wurde hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
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
            <p>Das folgende Feld wurde entfernt:
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
              </li>
             </ul>
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
            <p><b>updateType</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
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
            <p><b>recentUpdatesObjIDs</b>
            </p>
            <p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

Ein UserPrefValue -Objekt stellt eine Benutzervoreinstellung dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>value</b>
            </p>
            <p>Validator hinzugefügt <code>MAX_LENGTH</code></p>
      </td>
    </tr>
  </tbody>
</table>

### Arbeit (ARBEIT)

Ein Work-Objekt ist eine gemeinsame Schnittstelle, die sowohl von Task als auch von OpTask übernommen wird und gemeinsamen Code für beide verwendet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>ISTBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>ISTNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>scheduledNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

