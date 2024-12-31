---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 18
description: Adobe Workfront hat API Version 18 am 6. April 2022 veröffentlicht. Die API-Version 18 enthält die folgenden Änderungen gegenüber Version 17.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: 842b26177a11225049ef42f779ca77dd81926b74
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Neue Funktionen in der API-Version 18

Adobe Workfront hat API Version 18 am 8. April 2024 veröffentlicht. Die API-Version 18 enthält die folgenden Änderungen gegenüber Version 17.

## Ressourcen hinzugefügt

Für API-Version 18 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API-Version 18 wurden keine Ressourcen entfernt

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
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
              </li>
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
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
              </li>
            </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
              </li>
            </ul>
          </li>
        </ul>
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
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
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

### Warten auf Genehmigung (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Vorgänge</td>
      <td>
        <ul>
          <li>
            <p>Folgende Vorgänge wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>HINZUFÜGEN</b>
                </p>
              </li>
              <li>
                <p><b>DELETE </b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Baseline (BLIN)

Baselines sind Momentaufnahmen der Leistung eines Projekts zu einem bestimmten Zeitpunkt. Sie speichern wichtige Informationen über das Projekt, wie wichtige Daten, Fortschritt, Kosten und Umsatzwerte.

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
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
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

### Baseline-Aufgabe (BSTSK)

Baselines sind Momentaufnahmen der Leistung eines Projekts zu einem bestimmten Zeitpunkt. Sie speichern wichtige Informationen über das Projekt, wie wichtige Daten, Fortschritt, Kosten und Umsatzwerte. Wenn Sie eine Baseline erstellen, werden die Aufgabeninformationen auch in den Baseline-Aufgaben dieser Baseline erfasst.

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
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
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
            <p><b>catObjCode</b>:
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Sonstige Ressourcenkategorie)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Stunde)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Tarifkarte)
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
                <p><code>NLBRCY</code> (Sonstige Ressourcenkategorie)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Stunde)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Tarifkarte)
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

Ein Dokumentobjekt, das eine Datei darstellt (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

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
            <p>hinzugefügt. Diese neue Aktion erfordert die folgenden Parameter:
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
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
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
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
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
              <li>
                <p><code>AAO</code> (enum.actionTypeEnum.AssetApproval.Opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actionTypeEnum.AssetApproval.locked.all.decisions.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actionTypeEnum.AssetApproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actionTypeEnum.AssetApproval.locked.manual)</p>
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
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
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
             <p>hinzugefügt.
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
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>RequestorForbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Kostensätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Abrechnungssätze anzeigen)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Allgemeine Finanzen anzeigen)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Kostensätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Abrechnungssätze bearbeiten)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Allgemeine Finanzen bearbeiten)</p>
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
          <p><b>displayName</b></p><p>hinzugefügt.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


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
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
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

Ein Vorlagenobjekt stellt ein Muster für ein Projekt dar. Projekte können aus Vorlagen erstellt werden, um Zeit zu sparen. Eine Vorlage enthält ein Team und Aufgaben, die in jedes aus der Vorlage erstellte Projekt kopiert werden.

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


### Vorlagenaufgabe (TTSK)

Ein TemplateTask-Objekt stellt eine Aufgabe dar, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, in dem die Vorlage verwendet wird.<table>
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

### TemplateUserRole (TEAM)

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

### Arbeitszeittabelle (TABELLE)

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

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
            <p>hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

Ein UserPrefValue-Objekt, das eine Benutzervoreinstellung darstellt.

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
            <p>Die folgenden Felder wurden hinzugefügt:
            </p>
            <ul>
              <li>
                <p><b>actualBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>actualNonBillableExpenseCost</b>
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

