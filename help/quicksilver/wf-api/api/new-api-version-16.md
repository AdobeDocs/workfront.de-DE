---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in API Version 16
description: Adobe Workfront hat die API-Version 16 am 6. April 2022 veröffentlicht. API Version 16 enthält die folgenden Änderungen gegenüber Version 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Neue Funktionen in API Version 16

Adobe Workfront hat die API-Version 16 am 6. April 2023 veröffentlicht. API Version 16 enthält die folgenden Änderungen gegenüber Version 15.

## Hinzugefügte Ressourcen

Für API Version 16 wurden keine Ressourcen hinzugefügt.

## Entfernte Ressourcen

Für API-Version 16 wurden keine Ressourcen entfernt

## Geänderte Ressourcen

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Genehmigung (GENEHMIGUNG)](#approval-approval)
* [CustomerPreferences (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [Stunde (STUNDE)](#hour-hour)
* [LayoutTemplate (UITMPL)](#layouttemplate-uitmpl)
* [Hinweis (HINWEIS)](#note-note)
* [OpTask/Problem (OPTASK)](#note-note)
* [Projekt (PROJ)](#project-proj)
* [Rate (RATE)](#rate-rate)
* [RichTextNote (RHNOTE)](#richtextnote-rhnote)
* [Rolle/Auftragsrolle (ROLE)](#role--job-role-role)
* [Aufgabe (TASK)](#task-task)
* [Datenblatt (TSHET)](#timesheet-tshet)
* [UIFilter/Filter (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Grouping (UIGB)](#uigroupby--grouping-uigb)
* [UIView/View (UIVW)](#uiview--view-uivw)
* [Benutzer (BENUTZER)](#user-user)
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
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten pro Tag an, die Sie benötigen. Das Format lautet <code>YYYY-MM-DD: (number of minutes)</code>und berücksichtigt die Zeitzone.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Zuweisung (ASSGN)

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
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten pro Tag an, die Sie benötigen. Das Format lautet <code>YYYY-MM-DD: (number of minutes)</code>und berücksichtigt die Zeitzone.</p>
          </li>
          <li>
            <p><b>isContected</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt. Es ist ein boolescher Wert, der angibt, ob die Zuweisung beibehalten wird. Wenn die Minuten der Zuweisung pro Tag im Lastenausgleich bearbeitet wurden, wurde die Zuweisung beibehalten.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

Das CustomEnum -Objekt unterstützt die Konvertierung von Status-Codes in für Menschen lesbaren Text.

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
            <p>Diese Aktion gibt einen booleschen Wert zurück, der beschreibt, ob der Kunde die Option zur automatischen Aktualisierung von Mitwirkenden-Lizenzinhabern deaktiviert hat.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

Ein ExternalSection -Objekt ist eine externe Webseite, die in einen Workfront-Bericht eingebettet ist.

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
            <p>Dieser wurde hinzugefügt und berechnet die URL eines in einen Bericht eingebetteten iFrame.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>Dieser wurde hinzugefügt und berechnet die URLs der in einen Bericht eingebetteten iFrames.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Stunde (STUNDE)

Ein Hour -Objekt stellt eine Stunde dar, die von einem Benutzer auf einem Timesheet protokolliert wird.

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
            <p>Hinzugefügt. Mit diesem Parameter werden die mit <code>batchSave</code>. </p>
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

### Hinweis (HINWEIS)

Ein Hinweis -Objekt ist ein Kommentar oder eine Aktualisierung, die an einem Workfront-Objekt vorgenommen wird.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
            <p><b>attachDocuments</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und stellt eine Liste von Dokumenten dar, die an den Kommentar angehängt sind.</p>
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
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten pro Tag an, die Sie benötigen. Das Format lautet <code>YYYY-MM-DD: (number of minutes)</code>und berücksichtigt die Zeitzone.</p>
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
            <p>Durch diese Aktion wurde das Feld hinzugefügt. <code>teamIDs</code> , um die Funktion zum Zuweisen mehrerer Teams zu einer Aufgabe oder einem Problem zu unterstützen.</p>
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
            <p>Dieses Feld wurde hinzugefügt und stellt die Summe aller budgetierten Stunden für das Projekt dar.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Rate (RATE)

Ein Rate -Objekt stellt eine Abrechnungsrate in Workfront dar.

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
           <p>Diese Parameter wurden vom Rollenobjekt in das Rate -Objekt verschoben, sodass Rolle- und Benutzerobjekte mehrere Werte aufweisen können (für separate Datumsbereiche).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Diese Parameter stellen die ID und den Objektcode des Objekts dar, an das die Rate angehängt ist.
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
           <p>Diese Aktion wurde hinzugefügt und hängt Rate -Objekte an das angegebene Objekt an. Dieser Endpunkt funktioniert für alle angehängten Ratenobjekte.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (RHNOTE)

Ein RichTextNote -Objekt ist ein Kommentar oder eine Aktualisierung eines Workfront-Objekts, das Rich-Text (z. B. fett gedruckten oder kursiv gedruckten Text) enthält.

Das RichTextNote-Objekt hat das Flag entfernt `REPORTABLE`.

### Rolle/Auftragsrolle (ROLE)

Ein Rollenobjekt (Auftragsrolle) steht für eine funktionale Kapazität oder eine Fachkompetenz, die ein Benutzer ausfüllen kann, z. B. Designer oder Produkt-Manager.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
           <li>
            <p><b>rates</b>
            </p>
            <p>Diese wurde hinzugefügt und stellt die Rate -Objekte dar, die mit dieser Rolle verknüpft sind.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten pro Tag an, die Sie benötigen. Das Format lautet <code>YYYY-MM-DD: (number of minutes)</code>und berücksichtigt die Zeitzone.</p>
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
            <p>Durch diese Aktion wurde das Feld hinzugefügt. <code>teamIDs</code> , um die Funktion zum Zuweisen mehrerer Teams zu einer Aufgabe oder einem Problem zu unterstützen.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>availableActions</b>
            </p>
            <p>Dieser Parameter hat die Markierung entfernt <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Dieser Parameter hat die Markierung entfernt <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Dieser Parameter wurde hinzugefügt und speichert die Timesheets-Dauer in Tagen, unabhängig von den Änderungen zu "Äquivalente Stunden für vollständige Workday".  Wenn beispielsweise "Äquivalente Stunden"auf 6 festgelegt ist und ein Tag protokolliert wird, wird "Äquivalente Stunden"auf 8 Stunden geändert. <code>totalDays</code> hat immer noch den Wert 1.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter/Filter (UIFT)



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
            <p>Diese Aktion wurde hinzugefügt. Sie erstellt eine Filterabfragezuordnung und fügt die <code>allowingnull</code> für nullbare Felder verknüpfen.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Diese Aktionen unterstützen die systemweite Freigabe von Filtern, Ansichten und Gruppierungen.</p><p>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Verfügbar machen von Filtern, Ansichten oder Gruppierungen für alle Benutzer</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Grouping (UIGB)


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
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Diese Aktionen unterstützen die systemweite Freigabe von Filtern, Ansichten und Gruppierungen.</p><p>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Verfügbar machen von Filtern, Ansichten oder Gruppierungen für alle Benutzer</a>.</p>
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
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Diese Aktionen unterstützen die systemweite Freigabe von Filtern, Ansichten und Gruppierungen.</p><p>Weitere Informationen finden Sie unter <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Verfügbar machen von Filtern, Ansichten oder Gruppierungen für alle Benutzer</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Benutzer (BENUTZER)

Ein User -Objekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
           <li>
            <p><b>rates</b>
            </p>
            <p>Diese wurde hinzugefügt und stellt die Rate -Objekte dar, die an diesen Benutzer angehängt sind.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

Ein UserNote -Objekt ist eine Benachrichtigung.

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
            <p><b>workPerDate</b>
            </p>
            <p>Dieses Feld wurde hinzugefügt und zeigt die Anzahl der Minuten pro Tag an, die Sie benötigen. Das Format lautet <code>YYYY-MM-DD: (number of minutes)</code>und berücksichtigt die Zeitzone.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
