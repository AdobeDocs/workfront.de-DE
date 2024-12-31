---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 15
description: Adobe Workfront hat API Version 14 am 14. Juni 2022 veröffentlicht. Die API-Version 15 enthält die folgenden Änderungen gegenüber Version 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2286'
ht-degree: 0%

---

# Neue Funktionen in der API-Version 15

Adobe Workfront hat API Version 15 am 14. Juni 2022 veröffentlicht. Die API-Version 15 enthält die folgenden Änderungen gegenüber Version 14.

## Ressourcen hinzugefügt

* [Initiative (INITIV)](#Initiati)

* [Anfrage-Def (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [Benutzerzustimmung (USRAPV)](#UserAppr)

### Initiative (INITIV)

Das Objekt Initiative erstellt im Workfront-Szenarioplaner Schätzungen für die Art und Anzahl der Aufgabengebiete, die Fixkosten und den geplanten Nutzen.

Weitere Informationen zu Initiativen finden Sie unter [Initiativen - Übersicht im Szenario-Planer](../../scenario-planner/initiatives-overview.md).

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
            <p>Dies ist ein internes -Objekt.</p>
          </li>
          <li>
            <p><b>duration</b>
            </p>
            <p>Die Zeit zwischen endDate und startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>Das geplante Abschlussdatum für die Initiative.</p>
          </li>
          <li>
            <p><b>enteredByID</b>
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
            <p>Das Datum, an dem die Initiative zuletzt im Workfront Scenario Planner veröffentlicht wurde.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>Der Name der Initiative</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>Die ID des Plans, der mit der Initiative verknüpft ist.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>Der Name des Plans, der mit der Initiative verknüpft ist.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>Die ID des Projekts, das der Initiative zugeordnet ist.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>Die ID des Szenarios im Workfront-Szenarioplaner, das mit der Initiative verknüpft ist.</p>
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
            <p><b>Kunde</b>
            </p>
          </li>
          <li>
            <p><b>enteredBy</b>
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
            <p><b>ANZAHL</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>REPORT </b>
            </p>
          </li>
          <li>
            <p><b>SUCHE</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Anfrage-Def (ISSDEF)

Das IssueDef-Objekt stellt einen Satz von Daten zum Format von Anfragen dar. Dieses Objekt kann an Projekte oder Vorlagen angehängt werden und wirkt sich auf die Probleme aus, die diesem Projekt oder dieser Vorlage hinzugefügt werden.

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

In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration-Objekt stellt diese Relation dar.

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
            <p>Dies ist ein internes -Objekt.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>Datum und Uhrzeit der Eingabe der ObjectIntegration in das Workfront-System.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>Die eindeutige Workfront-ID des spezifischen ObjectIntegration-Objekts.</p>
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
            <p>Das -Objekt in Workfront, mit dem die ObjectIntegration verknüpft ist.</p>
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
            <p><b>Kunde</b>
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

Das TaskDef-Objekt stellt einen Satz von Daten zum Format von Aufgaben dar. Dieses Objekt kann an Projekte oder Vorlagen angehängt werden und wirkt sich auf die Aufgaben aus, die diesem Projekt oder dieser Vorlage hinzugefügt werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours-</b>
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
            <p><b>objectCategory
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

### Benutzerzustimmung (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
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
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>RequestorID</b>
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
            <p><b>Kunde</b>
            </p>
          </li>
          <li>
            <p><b>Antragsteller</b>
            </p>
          </li>
          <li>
            <p><b>Benutzer</b>
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
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>RequestorID</b>
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
            <p><b>Genehmigen</b>
            </p>
          </li>
          <li>
            <p><b>Ablehnen</b>
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
            <p><b>HINZUFÜGEN</b>
            </p>
          </li>
          <li>
            <p><b>ANZAHL</b>
            </p>
          </li>
          <li>
            <p><b>DELETE </b>
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
            <p><b>SUCHE</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Entfernte Ressourcen

Für API-Version 15 wurden keine Ressourcen entfernt.

## Geänderte Ressourcen

* [Zugriffsebene (ACSLV)](#AccessLe)

* [AccessLevelPermissions (ALVPER)](#AccessLe2)

* [Zugriffsanforderung (ACSREQ)](#AccessRe)

* [Zugriffsregel (ACSRUL)](#AccessRu)

* [Validierung (VALIDIERUNG)](#Approval)

* [Kategorie (CTG)](#Category)

* [Kategorieparameter (CTGYPA)](#Category2)

* [Kundenvoreinstellungen (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [DocumentVersion (DOCV)](#Document2)

* [Gruppe (GROUP)](#Group)

* [Tagebucheintrag (JRNLE)](#JournalE)

* [Verknüpfter Ordner (LINKFDR)](#LinkedFo)

* [Aufgabe/Problem (OPTASK)](#OpTask)

* [Parameter (PARAM)](#Paramete)

* [Portfolio (PORT)](#Portfoli)

* [Programm (PRGM)](#Program)

* [Projekt (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Aufgabe (AUFGABE)](#Task)

* [Vorlage (TMPL)](#Template)

* [Arbeitszeittabelle (TABELLE)](#Timeshee)

* [Anzeigen (UIVIEW)](#View)

* [Aktualisieren (UPDATE)](#Update)

* [Benutzer (USER)](#User)

* [UserNote (USRNOT)](#UserNote)

* [Arbeit (ARBEIT)](#Work)

### Zugriffsebene (ACSLV)

Ein AccessLevel-Objekt ist Benutzern zugeordnet und beschreibt den Satz von AccessLevelPermissions, die bestimmen, auf was Benutzer zugreifen können.

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
                <p>VTMAWMG (Meinen Gruppen zugeordnete Teams anzeigen)</p>
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
            <p><b>coreAction</b> (Zeichenfolge[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
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
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (Zeichenfolge[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
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
            <p><b>action</b> (Zeichenfolge)</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
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
            <p><b>coreAction</b> (Zeichenfolge[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
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
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (Zeichenfolge[])</p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
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
            <p><b>resourcePlannerBudgetedHours-</b>
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
            <p><b>Initiative</b>
            </p>
            <p>hinzugefügt.</p>
            <p>Das Objekt Initiative erstellt im Workfront-Szenarioplaner Schätzungen für die Art und Anzahl der Aufgabengebiete, die Fixkosten und den geplanten Nutzen. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>hinzugefügt.</p>
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
            <p style="font-weight: normal;">hinzugefügt.</p>
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration-Objekt stellt diese Relation dar.</p>
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
            <p><b>catObjCode</b> (Zeichenfolge)</p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
            <ul>
              <li>
                <p>GROUP (Gruppe)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (Zeichenfolge[])</p>
            <p>hinzugefügt.</p>
            <p style="font-weight: normal;">Dieser Parameter ist ein Array möglicher Objekte, an die das benutzerdefinierte Formular angehängt werden kann. Es wurde hinzugefügt, um die Möglichkeit zu unterstützen, ein benutzerdefiniertes Formular an mehrere Objekttypen anzuhängen.</p>
            <p>Mögliche Werte: </p>
            <p>KOPIEREN, PORT, PRGM, PROJ, AUFGABE, OPTASK, BENUTZER, DOKUMENT, AUSGABEN, INTERN, RECHNUNG, GRUPPE</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (Zeichenfolge[])</p>
            <p>hinzugefügt.</p>
            <p style="font-weight: normal;">Dieser Parameter ist ein Array möglicher Objekte, an die das benutzerdefinierte Formular angehängt werden kann. Es wurde hinzugefügt, um die Möglichkeit zu unterstützen, ein benutzerdefiniertes Formular an mehrere Objekttypen anzuhängen.</p>
            <p>Mögliche Werte: </p>
            <p>KOPIEREN, PORT, PRGM, PROJ, AUFGABE, OPTASK, BENUTZER, DOKUMENT, AUSGABEN, INTERN, RECHNUNG, GRUPPE</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Kategorieparameter (CTGYPA)

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
            <p>hinzugefügt.</p>
          </li>
          <li>
            <p><b>journalizedObjCodes</b>
            </p>
            <p>hinzugefügt.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>hinzugefügt.</p>
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
            <p>Die folgenden Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (Integration der SharePoint (Graph API) aktiviert)</p>
                <p>Dieser Wert unterstützt die aktualisierte SharePoint-Integration.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Benutzern erlauben, Projekte ohne Vorlage zu erstellen)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskIssue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

Dokumente können in Ordnern organisiert werden. Sie können persönliche Ordner in Ihrem Bereich für persönliche Dokumente erstellen. Das DocumentFolder-Objekt stellt einen dieser Ordner dar.

Das DocumentFolder-Objekt hat die `SHARABLE` hinzugefügt.

### DocumentVersion (DOCV)

Ein DocumentVersion-Objekt stellt eine bestimmte Version einer Datei dar (z. B. geschriebenes Material, Bilder oder andere Informationsformen).

Weitere Informationen zu Dokumentversionen finden Sie unter [Hochladen einer neuen Version eines Dokuments](../../documents/managing-documents/upload-new-document-version.md).

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
            <p>Folgender Wert wurde hinzugefügt: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API)</p>
                <p>Dieser Wert unterstützt die aktualisierte SharePoint-Integration.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Gruppe (GROUP)

Ein Gruppenobjekt steht für eine Gruppe von Benutzern und Teams. Gruppen repräsentieren oft die Abteilungsstruktur.

Weitere Informationen zu Gruppen finden Sie unter Gruppen im Vergleich zu Teams .

Das Gruppenobjekt hat die `DATA_EXTENDIBLE` hinzugefügt

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
            <p>Eine Kategorie ist ein benutzerdefiniertes Formular. Dieser Parameter wurde hinzugefügt, um das Hinzufügen benutzerdefinierter Forms zu Gruppenobjekten zu unterstützen. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Dies ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt „Active“ ist, und den Wert „false“, wenn es nicht ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden.</p>
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
            <p><b>Kunde</b>
            </p>
          </li>
          <li>
            <p><b>Antragsteller</b>
            </p>
          </li>
          <li>
            <p><b>Benutzer</b>
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
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration-Objekt stellt diese Relation dar.</p>
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
            <p>Dies ist ein boolescher Parameter, der den Wert „true“ hat, wenn ein Objekt „Active“ ist, und den Wert „false“, wenn es nicht ist. Objekte, die als Aktiv festgelegt sind, werden in Dropdown-Menüs und Feldern mit automatischer Textvervollständigung angezeigt und können an andere Objekte angehängt werden.</p>
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
            <p>Diese Aktion berechnet die Ausdrücke in benutzerdefinierten Formularfeldern neu.</p>
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

### Tagebucheintrag (JRNLE)

Das JournalEntry-Objekt kann so eingerichtet werden, dass Informationen zu bestimmten Objektfeldern jedes Mal protokolliert werden, wenn diese Felder geändert werden. Wenn ein Feld so eingerichtet ist, dass es als Teil des Journaleintragsobjekts protokolliert wird, wird jedes Mal, wenn dieses Feld geändert wird, ein entsprechender Journaleintrag erstellt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <p><b>changeType</b>
        </p>
        <p>Folgender Wert wurde hinzugefügt: </p>
        <ul>
          <li>
            <p>DW (Download)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Verknüpfter Ordner (LINKFDR)

Ein LinkedFolder-Objekt stellt einen Ordner dar, der über einen externen Dokumentanbieter verknüpft ist, z. B. Google Drive oder Dropbox.

Weitere Informationen zu verknüpften Ordnern finden Sie unter Verknüpfen von Dokumenten aus externen Programmen.

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
            <p>Folgender Wert wurde hinzugefügt: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API)</p>
                <p>Dieser Wert unterstützt die aktualisierte SharePoint-Integration.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aufgabe/Problem (OPTASK)

Ein OpTask-Objekt wird im Allgemeinen als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise darauf hinweist, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungsanforderungen, -anfragen und -fehler sind ebenfalls Probleme.

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

Ein Parameter-Objekt ist ein benutzerdefiniertes Feld.

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
            <p>Der mögliche Wert <code>WIDGET </code>(Widget) wurde hinzugefügt </p>
            <p>Dieser Wert unterstützt die Verwendung von Bildern in benutzerdefinierten Formularen.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Der mögliche Wert <code>WIDGET </code>(Widget) wurde hinzugefügt</p>
            <p>Dieser Wert unterstützt die Verwendung von Bildern in benutzerdefinierten Formularen.</p>
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

Ein Programmobjekt ist eine Teilmenge von Projekten innerhalb eines Portfolios, in dem ähnliche Projekte gruppiert werden können.

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
            <p><b>Initiative</b>
            </p>
            <p>Das Objekt Initiative erstellt im Workfront-Szenarioplaner Schätzungen für die Art und Anzahl der Aufgabengebiete, die Fixkosten und den geplanten Nutzen. </p>
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
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration-Objekt stellt diese Relation dar.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Ein QueueDef -Objekt stellt eine Warteschlange dar. Dabei handelt es sich um ein Projekt, das im Helpdesk-Bereich veröffentlicht wurde, um Benutzenden die Übermittlung von Problemen zu ermöglichen.

Weitere Informationen zu Anfrage-Warteschlangen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

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
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Teams in von mir verwalteten Gruppen bearbeiten (nur Gruppenadministratoren))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>RequestorForbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Teams bearbeiten, an denen ich mitwirke)</p>
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

Ein ScoreCardQuestion-Objekt stellt eine Frage dar, die zu einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfoliomanager bestimmt und ihre Antworten geben dem Portfolio die Möglichkeit zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

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
            <p>Der mögliche Wert <code>WIDGET </code>(Widget) wurde hinzugefügt</p>
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
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration-Objekt stellt diese Relation dar.</p>
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

### Arbeitszeittabelle (TABELLE)

Ein Arbeitszeittabellen-Objekt stellt eine virtuelle Arbeitszeitkarte dar, mit der Benutzende tatsächliche Arbeitsstunden für Aufgaben, Projekte und allgemeine Stundentypen eingeben können.

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
                <p><code>FOUR_COL</code> (Vierspaltiges Layout)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Aktualisierungen)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Aktualisierungen)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (in Arbeit)</p>
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
                <p><code>DLIST_SECTION</code> (Abschnitt Detailliste)</p>
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
            <p>Der mögliche Wert <code>documentVersionDownload </code>(enum.updateTypeEnum.DocumentVersionDownload) wurde hinzugefügt.</p>
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
            <p><b>eventType</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>DUP </code>(hat Sie um den Korrekturabzug eines Dokuments gebeten)</p>
              </li>
              <li>
                <p><code>DUV </code>(Ermöglicht die Anzeige eines Dokuments)</p>
              </li>
            </ul>
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
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegrations</b>
            </p>
            <p>In einigen Fällen ist es möglich, Workfront-Arbeitselemente direkt mit Objekten in einem externen Softwareprodukt zu verknüpfen. Das ObjectIntegration-Objekt stellt diese Relation dar.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
