---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 15
description: Adobe Workfront hat die API-Version 14 am 14. Juni 2022 veröffentlicht. API Version 15 enthält die folgenden Änderungen gegenüber Version 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2286'
ht-degree: 0%

---

# Neue Funktionen in API Version 15

Adobe Workfront hat die API-Version 15 am 14. Juni 2022 veröffentlicht. API Version 15 enthält die folgenden Änderungen gegenüber Version 14.

## Hinzugefügte Ressourcen

* [Initiative (INITIV)](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [UserApproval (USRAPV)](#UserAppr)

### Initiative (INITIV)

Das Objekt Initiative erstellt im Workfront-Szenario-Planer Schätzungen für die Art und Anzahl der Arbeitsplatzrollen, die Festkosten und den geplanten Nutzen.

Weitere Informationen zu Initiativen finden Sie unter [Übersicht über Initiativen im Szenario-Planer](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Dies ist ein internes Objekt.</p>
          </li>
          <li>
            <p><b>duration</b>
            </p>
            <p>Die Zeitspanne zwischen endDate und startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>Das geplante Abschlussdatum für die Initiative.</p>
          </li>
          <li>
            <p><b>enterByID</b>
            </p>
            <p>Die ID, die dem Benutzer zugeordnet ist, der die Anfrage gesendet hat.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>Die mit der Aktion verknüpfte ID</p>
          </li>
          <li>
            <p><b>initiativeID</b>
            </p>
            <p>Die mit der Initiative verknüpfte ID.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>Das Datum der letzten Veröffentlichung der Initiative im Workfront-Szenario-Planer.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>Der Name der Initiative</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>Die Kennung des mit der Initiative verknüpften Plans.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>Der Name des mit der Initiative verknüpften Plans.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>Die Kennung des mit der Initiative verknüpften Projekts.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>Die Kennung des Szenarios im Workfront-Szenario-Planer, der mit der Initiative verknüpft ist.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>Das geplante Startdatum der Initiative.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td >
        <ul>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>enterBy</b>
            </p>
          </li>
          <li>
            <p><b>Projekt</b>
            </p>
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
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Vorgänge</td>
      <td>
        <ul>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>BERICHT </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

Das IssueDef -Objekt stellt einen Satz von Daten zum Format von Problemen dar. Dieses Objekt kann an Projekte oder Vorlagen angehängt werden und betrifft die Probleme, die diesem Projekt oder dieser Vorlage hinzugefügt werden.

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
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration -Objekt stellt diese Verknüpfung dar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Dies ist ein internes Objekt.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>Datum und Uhrzeit der Eingabe der ObjectIntegration im Workfront-System.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>Die eindeutige Workfront-ID des bestimmten ObjectIntegration-Objekts.</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>Die externe Software, mit der das ObjectIntegration-Objekt eine Verknüpfung erstellt. Mögliche Werte sind:</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>Das Objekt in Workfront, mit dem die ObjectIntegration verknüpft ist.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>Der Objektcode des Objekts in Workfront, mit dem die ObjectIntegration verknüpft ist.</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td >
        <ul>
          <li>
            <p><b>customer</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

Das TaskDef-Objekt stellt einen Satz von Daten zum Aufgabenformat dar. Dieses Objekt kann an Projekte oder Vorlagen angehängt werden und wirkt sich auf die Aufgaben aus, die diesem Projekt oder dieser Vorlage hinzugefügt werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>Objektkategorien
</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserApproval (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder </td>
      <td>
        <ul>
          <li>
            <p><b>GenehmigerID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td >
        <ul>
          <li>
            <p><b>Genehmiger</b>
            </p>
          </li>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
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
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standardfelder</td>
      <td >
        <ul>
          <li>
            <p><b>GenehmigerID</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>approve</b>
            </p>
          </li>
          <li>
            <p><b>reject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Vorgänge</td>
      <td>
        <ul>
          <li>
            <p><b>ADD</b>
            </p>
          </li>
          <li>
            <p><b>COUNT</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>BERICHT</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Entfernte Ressourcen

Für API Version 15 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen

* [AccessLevel (ACSLVL)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [AccessRequest (ACSREQ)](#AccessRe)

* [AccessRule (ACSRUL)](#AccessRu)

* [Genehmigung (GENEHMIGUNG)](#Approval)

* [Kategorie (KG)](#Category)

* [CategoryParameter (CTGYPA)](#Category2)

* [CustomerPreferences (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Gruppe (GRUPPE)](#Group)

* [JournalEntry (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [OpTask/Problem (OPTASK)](#OpTask)

* [Parameter (PARAM)](#Paramete)

* [Portfolio (HAFEN)](#Portfoli)

* [Programm (PRGM)](#Program)

* [Projekt (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Aufgabe (TASK)](#Task)

* [Vorlage (TMPL)](#Template)

* [Datenblatt (TSHET)](#Timeshee)

* [Anzeigen (UIVIEW)](#View)

* [Aktualisieren (AKTUALISIEREN)](#Update)

* [Benutzer (BENUTZER)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Arbeit (ARBEIT)](#Work)

### AccessLevel (ACSLVL)

Ein AccessLevel -Objekt ist mit Benutzern verknüpft und beschreibt den Satz von AccessLevelPermissions, der bestimmt, auf welchen Benutzer zugreifen können.

Weitere Informationen zu Zugriffsebenen finden Sie unter [Zugriffsebenen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>VTMAWMG (Teams anzeigen, die mit meinen Gruppen verbunden sind)</p>
              </li>
              <li>
                <p>VALLTM (Alle Teams anzeigen)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b>coreAction</b> (string[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
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
            <p><b>action</b> (Zeichenfolge)</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (Zeichenfolge)</p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
            <ul>
              <li>
                <p>WDL</p>
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
            <p><b>coreAction</b> (string[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
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
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td >
        <ul>
          <li>
            <p><b>initiative</b>
            </p>
            <p>Hinzugefügt.</p>
            <p>Das Objekt Initiative erstellt im Workfront-Szenario-Planer Schätzungen für die Art und Anzahl der Arbeitsplatzrollen, die Festkosten und den geplanten Nutzen. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Hinzugefügt.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegrations
</b>
            </p>
            <p style="font-weight: normal;">Hinzugefügt.</p>
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration -Objekt stellt diese Verknüpfung dar.</p>
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
            <p><b>catObjCode</b> (Zeichenfolge)</p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
            <ul>
              <li>
                <p>GRUPPE (Gruppe)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Hinzugefügt.</p>
            <p style="font-weight: normal;">Dieser Parameter ist ein Array möglicher Objekte, an die das benutzerdefinierte Formular angehängt werden kann. Es wurde hinzugefügt, um die Möglichkeit zu unterstützen, ein benutzerdefiniertes Formular an mehrere Objekttypen anzuhängen.</p>
            <p>Mögliche Werte: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Hinzugefügt.</p>
            <p style="font-weight: normal;">Dieser Parameter ist ein Array möglicher Objekte, an die das benutzerdefinierte Formular angehängt werden kann. Es wurde hinzugefügt, um die Möglichkeit zu unterstützen, ein benutzerdefiniertes Formular an mehrere Objekttypen anzuhängen.</p>
            <p>Mögliche Werte: </p>
            <p>CMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>hideFormulaFromDescription</b>
            </p>
            <p>Hinzugefügt.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>Hinzugefügt.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Hinzugefügt.</p>
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
            <p>Die folgenden Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (SharePoint (Graph API)-Integration aktiviert</p>
                <p>Dieser Wert unterstützt die aktualisierte Sharepoint-Integration.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Ermöglichen Sie es Benutzern, Projekte ohne Verwendung einer Vorlage zu erstellen)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

Dokumente können in Ordner unterteilt werden. Sie können persönliche Ordner in Ihrem Bereich &quot;Dokumente&quot;erstellen. Das DocumentFolder-Objekt stellt einen dieser Ordner dar.

Das DocumentFolder-Objekt hat das Flag `SHARABLE` hinzugefügt.

### DocumentVersion (DOCV)

Ein DocumentVersion -Objekt stellt eine bestimmte Version einer Datei dar (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

Weitere Informationen zu Dokumentversionen finden Sie unter [Eine neue Version eines Dokuments hochladen](../../documents/managing-documents/upload-new-document-version.md).

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
            <p>Der folgende Wert wurde hinzugefügt: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph-API)</p>
                <p>Dieser Wert unterstützt die aktualisierte Sharepoint-Integration.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gruppe (GRUPPE)

Ein Group -Objekt stellt eine Gruppe von Benutzern und Teams dar. Gruppen repräsentieren oft die Struktur der Abteilungen.

Weitere Informationen zu Gruppen finden Sie unter Gruppen vs. Teams.

Das Group -Objekt hat das Flag `DATA_EXTENDIBLE` hinzugefügt

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <p>Die folgenden Felder wurden hinzugefügt:</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieser Parameter wurde hinzugefügt, um die Möglichkeit zu unterstützen, benutzerdefinierte Forms zu Gruppenobjekten hinzuzufügen. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Dies ist ein boolescher Parameter mit dem Wert true , wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td >
        <p>Die folgenden Felder wurden hinzugefügt:</p>
        <ul>
          <li>
            <p><b>Genehmiger</b>
            </p>
          </li>
          <li>
            <p><b>customer</b>
            </p>
          </li>
          <li>
            <p><b>requestor</b>
            </p>
          </li>
          <li>
            <p><b>user</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <p>Die folgenden Felder wurden hinzugefügt:</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration -Objekt stellt diese Verknüpfung dar.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Standardfelder</td>
      <td >
        <p>Das folgende Feld wurde hinzugefügt:</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Dies ist ein boolescher Parameter mit dem Wert true , wenn ein Objekt aktiv ist, und false , wenn dies nicht der Fall ist. Objekte, die auf "Aktiv"eingestellt sind, werden in Dropdown-Menüs und Typvorlagenfeldern angezeigt und können an andere Objekte angehängt werden.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <p>Die folgenden Felder wurden hinzugefügt:</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>Durch diese Aktion werden die Ausdrücke in benutzerdefinierten Formularfeldern neu berechnet.</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
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
        <p><b>changeType</b>
        </p>
        <p>Der folgende Wert wurde hinzugefügt: </p>
        <ul>
          <li>
            <p>DW (Download)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

Ein LinkedFolder-Objekt stellt einen Ordner dar, der von einem externen Dokumentenanbieter wie Google Drive oder Dropbox verknüpft ist.

Weitere Informationen zu verknüpften Ordnern finden Sie unter Verknüpfen von Dokumenten aus externen Anwendungen.

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
            <p>Der folgende Wert wurde hinzugefügt: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph-API)</p>
                <p>Dieser Wert unterstützt die aktualisierte Sharepoint-Integration.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask/Problem (OPTASK)

Ein OpTask-Objekt wird häufig als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise anzeigt, dass ein Problem vorliegt, das die Fertigstellung einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungen bei Bestellungen, Anforderungen und Fehlern sind ebenfalls Probleme.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <p>Die folgenden Aktionen wurden hinzugefügt:</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>Die folgende Aktion wurde geändert:</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>Feld hinzugefügt <code>parentID</code></p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Parameter (PARAM)

Ein Parameter -Objekt ist ein benutzerdefiniertes Feld.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <p>Das folgende Feld wurde hinzugefügt:</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>Die folgenden Felder wurden geändert:</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Der mögliche Wert <code>WIDGET </code>(Widget) wurde hinzugefügt. </p>
            <p>Dieser Wert unterstützt die Verwendung von Bildern in benutzerdefinierten Formularen.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Der mögliche Wert <code>WIDGET </code>(Widget) wurde hinzugefügt.</p>
            <p>Dieser Wert unterstützt die Verwendung von Bildern in benutzerdefinierten Formularen.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (HAFEN)

Ein Portfolio-Objekt ist eine Sammlung von Projekten, die um die gleichen Ressourcen konkurrieren, in der Regel um Geld oder Personen, um sie zu vervollständigen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Programm (PRGM)

Ein Programmobjekt ist eine Teilmenge von Projekten in einem Portfolio, in dem ähnliche Projekte gruppiert werden können.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
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
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td >
        <ul>
          <li>
            <p><b>initiative</b>
            </p>
            <p>Das Objekt Initiative erstellt im Workfront-Szenario-Planer Schätzungen für die Art und Anzahl der Arbeitsplatzrollen, die Festkosten und den geplanten Nutzen. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration -Objekt stellt diese Verknüpfung dar.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Ein QueueDef-Objekt stellt eine Warteschlange dar. Hierbei handelt es sich um ein Projekt, das in den Help Desk-Bereich veröffentlicht wurde, um Benutzern die Möglichkeit zu geben, Probleme an sie zu senden.

Weitere Informationen zu Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, in denen ich bin)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Ein ScoreCardQuestion -Objekt stellt eine Frage dar, die einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfolio-Manager bestimmt und ihre Antworten ermöglichen es dem Manager zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

Weitere Informationen zu Scorecard-Fragen finden Sie unter [Erstellen einer Scorecard](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

<table>
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
            <p>Der mögliche Wert <code>WIDGET </code>(Widget) wurde hinzugefügt.</p>
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
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration -Objekt stellt diese Verknüpfung dar.</p>
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
      <td role="rowheader">Referenzfelder</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
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
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <p>Das folgende Feld wurde entfernt:</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Anzeigen (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>Die folgenden möglichen Werte wurden entfernt:</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (Vierspaltenlayout)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Aktualisierungen)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Aktualisierungen)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (Arbeiten am)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (Benutzerdefinierte Daten)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (Benutzerdefinierte Daten aktualisieren)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (Statusaktualisierung)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Statusaktualisierung)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Statusaktualisierung)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Statusaktualisierung)</p>
              </li>
              <li>
                <p><code>DLIST</code> (Detailliste)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (Abschnitt "Detailliste")</p>
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
            <p>Der mögliche Wert <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload) wurde hinzugefügt.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Benutzer (BENUTZER)

Ein User -Objekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Referenzfelder</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
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
            <p><b>eventType</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>DUP </code>(Testversand eines Dokuments angefordert)</p>
              </li>
              <li>
                <p><code>DUV </code>(Zulassen der Anzeige eines Dokuments)</p>
              </li>
            </ul>
          </li>
        </ul>
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
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration -Objekt stellt diese Verknüpfung dar.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
