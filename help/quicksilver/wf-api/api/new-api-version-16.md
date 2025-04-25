---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 16
description: Adobe Workfront hat API Version 16 am 6. April 2022 veröffentlicht. Die API-Version 16 enthält die folgenden Änderungen gegenüber Version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: acd1fe5500776b8f16c67b05048a88d0c8107079
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# Neue Funktionen in der API-Version 16

Adobe Workfront hat API Version 16 am 6. April 2023 veröffentlicht. Die API-Version 16 enthält die folgenden Änderungen gegenüber Version 15.

## Ressourcen hinzugefügt

Für API-Version 16 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API-Version 16 wurden keine Ressourcen entfernt

## Geänderte Ressourcen

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Validierung (VALIDIERUNG)](#approval-approval)
* [Kundenvoreinstellungen (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTEC)](#externalsection-extsec)
* [Stunde (STUNDE)](#hour-hour)
* [Layout-Vorlage (UTIMPL)](#layouttemplate-uitmpl)
* [Notiz (HINWEIS)](#note-note)
* [Aufgabe/Problem (OPTASK)](#note-note)
* [Projekt (PROJ)](#project-proj)
* [Satz (RATE)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Funktion/Aufgabengebiet (ROLE)](#role--job-role-role)
* [Aufgabe (AUFGABE)](#task-task)
* [Arbeitszeittabelle (TABELLE)](#timesheet-tshet)
* [UIFilter / Filter (UIFT)](#uifilter--filter-uift)
* [UIGroupBy/Gruppierung (UIGB)](#uigroupby--grouping-uigb)
* [UIView/View (UIVW)](#uiview--view-uivw)
* [Benutzer (USER)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

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
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten Arbeit pro Tag an, die Sie ausführen müssen. Es hat das Format <code>YYYY-MM-DD: (number of minutes)</code> und berücksichtigt die Zeitzone.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Zuweisung (ZUWEISUNG)

Ein Zuweisungsobjekt stellt die Verbindung zwischen einem Arbeitselement und dem Benutzer, Team oder der Gruppe dar, der bzw. die für die Bearbeitung zugewiesen ist.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten Arbeit pro Tag an, die Sie ausführen müssen. Es hat das Format <code>YYYY-MM-DD: (number of minutes)</code> und berücksichtigt die Zeitzone.</p>
          </li>
          <li>
            <p><b>isContured</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und ist ein boolescher Wert, der angibt, ob die Zuweisung konturiert ist. Wenn die Minuten der Zuweisung pro Tag im Workload Balancer bearbeitet wurden, wurde für die Zuweisung ein Konturverfahren erstellt.</p>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
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
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
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
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>Diese Aktion gibt einen booleschen Wert zurück, der beschreibt, ob die Kundin oder der Kunde die Option zum automatischen Upgrade von Mitwirkenden-Lizenzinhabern deaktiviert hat.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTEC)

Ein ExternalSection-Objekt ist eine externe Webseite, die in einen Workfront-Bericht eingebettet ist.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>Dieser wurde hinzugefügt und berechnet die URL eines in einen Bericht eingebetteten iFrames.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>Dieser wurde hinzugefügt und berechnet die URLs von iFrames, die in einen Bericht eingebettet sind.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

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
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>hinzugefügt. Dieser Parameter wird verwendet, um die mit <code>batchSave</code> erstellten Stunden zu identifizieren. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Notiz (HINWEIS)

Ein Notizobjekt ist ein Kommentar oder eine Aktualisierung eines Workfront-Objekts.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>attachedDocuments</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und stellt eine Liste von Dokumenten dar, die an den Kommentar angehängt sind.</p>
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
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten Arbeit pro Tag an, die Sie ausführen müssen. Es hat das Format <code>YYYY-MM-DD: (number of minutes)</code> und berücksichtigt die Zeitzone.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Durch diese Aktion wurde die <code>teamIDs</code> hinzugefügt, um die Funktion zum Zuweisen mehrerer Teams zu einer Aufgabe oder einem Problem zu unterstützen.</p>
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
            <p>Dieses Feld wurde hinzugefügt und stellt die Summe aller budgetierten Stunden für das Projekt dar.</p>
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
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>Diese Parameter wurden aus dem Role-Objekt in das Rate-Objekt verschoben, sodass Role- und User-Objekte mehrere Werte haben können (für separate Datumsbereiche).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Diese Parameter stellen die ID und den Objekt-Code des Objekts dar, mit dem die Rate verknüpft ist.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>Diese Aktion wurde hinzugefügt und fügt Rate -Objekte an das angegebene Objekt an. Dieser Endpunkt funktioniert für alle „Rate Attachable“-Objekte.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

Ein RichTextNote-Objekt ist ein Kommentar oder eine Aktualisierung eines Workfront-Objekts, das bzw. die Rich-Text wie fett oder kursiv gedruckten Text enthält.

Das RichTextNote-Objekt hat das `REPORTABLE` entfernt.

### Funktion/Aufgabengebiet (ROLE)

Ein Rollenobjekt (Aufgabengebiet) stellt eine funktionale Kapazität oder eine Qualifikation dar, die ein Benutzer ausfüllen kann, z. B. Designer oder Product Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
           <li>
            <p><b>Tarife</b>
            </p>
            <p>Dies wurde hinzugefügt und stellt die mit dieser Rolle verknüpften Tarifobjekte dar.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten Arbeit pro Tag an, die Sie ausführen müssen. Es hat das Format <code>YYYY-MM-DD: (number of minutes)</code> und berücksichtigt die Zeitzone.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Durch diese Aktion wurde die <code>teamIDs</code> hinzugefügt, um die Funktion zum Zuweisen mehrerer Teams zu einer Aufgabe oder einem Problem zu unterstützen.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>availableActions</b>
            </p>
            <p>Dieser Parameter entfernte den <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Dieser Parameter entfernte den <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Dieser Parameter wurde hinzugefügt und speichert die Arbeitszeittabellen-Dauer in Tagen, unabhängig von Änderungen an „Entsprechende Stunden für vollständige Workday".  Wenn beispielsweise die äquivalenten Stunden auf 6 gesetzt sind und ein Tag protokolliert wird, werden die äquivalenten Stunden in 8 Stunden geändert, wobei <code>totalDays</code> immer noch den Wert 1 hat.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filter (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>Diese Aktion wurde hinzugefügt und verwendet eine Filterabfragezuordnung und fügt den <code>allowingnull</code>-Join für Felder hinzu, für die NULL-Werte zulässig sind.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility-</b>
            </p>
            <p>Diese Aktionen unterstützen die Möglichkeit, Filter, Ansichten und Gruppierungen systemweit freizugeben.</p><p>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E">Alle Benutzer Zugriff auf Filter, Ansichten oder Gruppierungen gewähren</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy/Gruppierung (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Aktionen</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility-</b>
            </p>
            <p>Diese Aktionen unterstützen die Möglichkeit, Filter, Ansichten und Gruppierungen systemweit freizugeben.</p><p>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E">Alle Benutzer Zugriff auf Filter, Ansichten oder Gruppierungen gewähren</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView/View (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
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
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility-</b>
            </p>
            <p>Diese Aktionen unterstützen die Möglichkeit, Filter, Ansichten und Gruppierungen systemweit freizugeben.</p><p>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs#make-filters-views-or-groupings-available-to-users%22%3E">Alle Benutzer Zugriff auf Filter, Ansichten oder Gruppierungen gewähren</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Benutzer (USER)

Ein Benutzerobjekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
           <li>
            <p><b>Tarife</b>
            </p>
            <p>Dies wurde hinzugefügt und stellt die mit diesem Benutzer verbundenen Rate-Objekte dar.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

Ein UserNote-Objekt ist eine Benachrichtigung.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Abfragen</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>Der folgende mögliche Wert wurde hinzugefügt:
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten Arbeit pro Tag an, die Sie ausführen müssen. Es hat das Format <code>YYYY-MM-DD: (number of minutes)</code> und berücksichtigt die Zeitzone.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
