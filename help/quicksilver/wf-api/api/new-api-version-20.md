---
content-type: api
navigation-topic: api-navigation-topic
title: Neue Funktionen in der API-Version 20
description: Adobe Workfront hat API-Version 20 am 6. April 2022 veröffentlicht. Die API-Version 20 enthält die folgenden Änderungen gegenüber Version 19.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 0%

---

# Neue Funktionen in der API-Version 20

Adobe Workfront hat API Version 20 am 4. Mai 2025 veröffentlicht. Die API-Version 20 enthält die folgenden Änderungen gegenüber Version 19.

## Ressourcen hinzugefügt

Für API-Version 20 wurden keine Ressourcen hinzugefügt.

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## Entfernte Ressourcen

Für API-Version 20 wurden keine Ressourcen entfernt

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
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
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
              <li>
                <p><code>tiff</code> (enum.fileExtension.tiff)</p>
              </li>
            </ul>
          </li>
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
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>Tatsächlicher Gewinn</li>
              <li>actualBillableExpenseCost</li>
              <li>Ist-Kosten</li>
              <li>Ist-Kosten</li>
              <li>Ist-Lohnkosten</li>
              <li>actualNonBillableExpenseCost</li>
              <li>Ist-Einnahmen</li>
              <li>Ist-Risikokosten</li>
              <li>Tatsächlicher Wert</li>
              <li>billedRevenue</li>
              <li>Budget</li>
              <li>Budgetierte Kosten</li>
              <li>budgetierte Stunden</li>
              <li>budgetierte Lohnkosten</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>Fixkosten</li>
              <li>Festeinnahmen</li>
              <li>geplanterGewinn</li>
              <li>scheduledBillableExpenseCost</li>
              <li>Geplante Kosten</li>
              <li>GeplanteAusgabenKosten</li>
              <li>Geplante Lohnkosten</li>
              <li>scheduledNonBillableExpenseCost</li>
              <li>geplante Risikokosten</li>
              <li>scheduledValue</li>
              <li>Verbleibende Kosten</li>
              <li>Verbleibender Umsatz</li>
              <li>Verbleibende Risikokosten</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Ist-Kosten</li>
          <li>Ist-Einnahmen</li>
          <li>Geplante Kosten</li>
          <li>Geplante Einnahmen</li>
          </ul>
          </li>
          <li><p><b>geplanteDauer</b></p> <p>Die Flags <code>DYNAMIC</code>, <code>LAZY_READ</code> und hinzugefügt <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>hat das Flag hinzugefügt <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Der mögliche Wert <code>URH</code> (stündlich für Benutzer und Funktion) wurde hinzugefügt. </li>
          <li><p><b>RevenueType</b></p> <p>Die möglichen Werte <code>URH</code> (Benutzer und Funktion pro Stunde), <code>URC</code> (Benutzer und Funktion pro Stunde mit Obergrenze) und <code>URF</code> (Benutzer und Funktion pro Stunde plus fest) wurden hinzugefügt</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
          <p>Die folgenden Felder wurden hinzugefügt:</p>
             <ul>
              <li><b>Abrechnungssätze</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Zuweisung (ZUWEISUNG)

Ein Arbeitsauftragsobjekt stellt die Verbindung zwischen einem Arbeitselement und dem Benutzer, Team oder der Gruppe dar, der bzw. die für die Bearbeitung zugewiesen ist.

Das Zuweisungsobjekt fügte die Flags `ATTRIBUTE_ATTACHABLE` und `DOMAIN_EXTENDABLE` hinzu.


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### Avatar

Ein Avatar-Objekt ist ein Benutzerfoto.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p><b>attachetobjectCode</b>
            </p>
             <p>Hinzugefügt</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kernfelder</td>
      <td>
        <ul>
          <li>
            <p><b>attachetobjectCode</b>
            </p>
             <p>Hinzugefügt</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Vorgänge</td>
      <td>
        <ul>
          <li>
            <p><b>KOPIEREN</b>
            </p>
             <p>Hinzugefügt</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
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
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>Ist-Kosten</li>
              <li>actualNonBillableExpenseCost</li>
              <li>Budget</li>
              <li>EAC</li>
              <li>scheduledBillableExpenseCost</li>
              <li>Geplante Kosten</li>
              <li>scheduledNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Ist-Kosten</li>
          <li>Geplante Kosten</li>
          </ul>
          </li>
          <li><p><b>EAC</b></p> <p>hat das Flag hinzugefügt <code>CURRENCY</code></li>
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
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>Ist-Kosten</li>
              <li>actualNonBillableExpenseCost</li>
              <li>scheduledBillableExpenseCost</li>
              <li>Geplante Kosten</li>
              <li>scheduledNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Ist-Kosten</li>
          <li>Geplante Kosten</li>
          </ul>
          </li>
          <li><p><b>EAC</b></p> <p>hat das Flag hinzugefügt <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Rechnungsnachweis (BILL)

Ein BillingRecord-Objekt zeichnet die Einnahmen, Stunden oder Ausgaben auf, die in Rechnung gestellt werden können. Diese Informationen können zur Erstellung von Rechnungen in einem externen Buchhaltungssystem verwendet werden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>Stärke</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>Hinzugefügt</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

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
            <p><b>Konfigurationen</b>
            </p>
             <p>Hinzugefügt</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Firma (COMPY)

Ein Unternehmensobjekt stellt eine Organisation dar, die aus einer Sammlung von Personen besteht.

Das Unternehmensobjekt hat die `SHARABLE` hinzugefügt.

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

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
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (singleAssignmentSchedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedTaskIssueMove)</p></li>
            </ul>
          </li>
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
      <td>
           <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Satz</li>
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
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>Ist-Kosten</li>
              <li>Ist-Festeinnahmen</li>
              <li>Ist-Lohnkosten</li>
              <li>actualLabourCostHours</li>
              <li>Ist-Arbeitseinnahmen</li>
              <li>actualNonBillableExpenseCost</li>
              <li>Fixkosten</li>
              <li>scheduledBillableExpenseCost</li>
              <li>GeplanteAusgabenKosten</li>
              <li>GeplanterFesteinnahmen</li>
              <li>Geplante Lohnkosten</li>
              <li>GeplanteArbeitskostenStunden</li>
              <li>Geplante Arbeitseinnahmen</li>
              <li>scheduledNonBillableExpenseCost</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalGeplanterUmsatz</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLabourRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Gruppe (GROUP)

Ein Gruppenobjekt steht für eine Gruppe von Benutzern und Teams. Gruppen repräsentieren oft die Abteilungsstruktur.

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
      </td>
    </tr>
  </tbody>
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
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>Ist-Kosten</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
              <li>Ist-Kosten</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>Hinzugefügt</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask (OPTASK)

Ein OpTask-Objekt wird im Allgemeinen als Problem bezeichnet. Ein Problem ist ein Arbeitselement, das normalerweise darauf hinweist, dass ein Problem vorliegt, das den Abschluss einer Aufgabe oder eines Projekts verhindert. Ein Problem kann auch eine Helpdesk-Anfrage sein. Änderungsanforderungen, -anfragen und -fehler sind ebenfalls Probleme.

Das OpTask-Objekt hat das Flag DOMAIN_EXTENDABLE hinzugefügt

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>Ist-Kosten</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
              <li>Ist-Kosten</li>
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
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (Interne Suche)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (Interne Suche mit Mehrfachauswahl)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterDisplayTypeEnum.UIEXTENSION)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio (PORT)

Ein Portfolio-Objekt ist eine Sammlung von Projekten, die um dieselben Ressourcen konkurrieren, normalerweise Geld oder Personen, um sie abzuschließen.

Das Portfolio-Objekt hat die `DOMAIN_EXTENDABLE` hinzugefügt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>Abgestimmt</li>
              <li>Budget</li>
              <li>Währung</li>
              <li>nettoValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioROI</li>
              <li>ROI</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Programm (PRGM)

Ein Programmobjekt ist eine Teilmenge von Projekten innerhalb eines Portfolios, in dem ähnliche Projekte gruppiert werden können.

Das Programmobjekt hat die `DOMAIN_EXTENDABLE` hinzugefügt.

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
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>Tatsächlicher Gewinn</li>
              <li>actualBillableExpenseCost</li>
              <li>Ist-Kosten</li>
              <li>Ist-Kosten</li>
              <li>Ist-Lohnkosten</li>
              <li>actualNonBillableExpenseCost</li>
              <li>Ist-Einnahmen</li>
              <li>Ist-Risikokosten</li>
              <li>Tatsächlicher Wert</li>
              <li>BCWP</li>
              <li>BCWS</li>
              <li>billedRevenue</li>
              <li>Budget</li>
              <li>Budgetierte Kosten</li>
              <li>budgetierte Stunden</li>
              <li>budgetierte Lohnkosten</li>
              <li>EAC</li>
              <li>Fixkosten</li>
              <li>Festeinnahmen</li>
              <li>geplanterGewinn</li>
              <li>scheduledBillableExpenseCost</li>
              <li>Geplante Kosten</li>
              <li>GeplanteAusgabenKosten</li>
              <li>Geplante Lohnkosten</li>
              <li>scheduledNonBillableExpenseCost</li>
              <li>Geplante Einnahmen</li>
              <li>geplante Risikokosten</li>
              <li>scheduledValue</li>
              <li>Verbleibende Kosten</li>
              <li>Verbleibender Umsatz</li>
              <li>Verbleibende Risikokosten</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Ist-Kosten</li>
          <li>Ist-Einnahmen</li>
          <li>Geplante Kosten</li>
          <li>Geplante Einnahmen</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>hat das Flag hinzugefügt <code>CURRENCY</code></li>
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
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>RequestorForbiddenActions</b>
            </p>
            <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (aus benutzerdefinierten Daten entfernen)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Unterprojekte hinzufügen)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Satz (RATE)

Ein Tarifobjekt stellt einen Abrechnungssatz in Workfront dar.

Das Ratenobjekt hat die `ATTRIBUTE_ATTACHABLE` hinzugefügt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>Die folgenden Felder wurden hinzugefügt:
          <ul>
          <li>Währung</li>
          <li>gesperrt</li>
          <li>Typ</li>
          <li>Wert</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Rolle (ROLE)

Ein Rollenobjekt (Aufgabengebiet) stellt eine funktionale Kapazität oder eine Qualifikation dar, die ein Benutzer ausfüllen kann, z. B. Designer oder Product Manager.

Das Role-Objekt hat die `DOMAIN_EXTENDABLE` hinzugefügt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
        <ul>
          <li>
          <p>Die folgenden Felder wurden hinzugefügt:
          <ul>
          <li>Abrechnungssätze</li>
          <li>costRates</li>
          </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
             <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileExtension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Ein ScoreCardQuestion-Objekt stellt eine Frage dar, die zu einer Scorecard hinzugefügt wurde. Diese Fragen werden in der Regel vom Portfolio-Manager bestimmt, und die Antworten geben dem Manager die Möglichkeit zu verstehen, wie gut ein Projekt mit den Portfoliozielen übereinstimmt.

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
             <p>Die folgenden möglichen Werte wurden hinzugefügt:</p>
             <ul>
              <li><p><code>INTRNL</code> (Interne Suche)</p></li>
              <li><p><code>MULTINTRNL</code> (Interne Suche mit Mehrfachauswahl)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterDisplayTypeEnum.UIEXTENSION)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aufgabe (AUFGABE)

Ein Aufgabenobjekt stellt ein Arbeitselement dar, das als Schritt zum Erreichen eines endgültigen Ziels (Fertigstellen eines Projekts) ausgeführt werden muss.

Das Aufgabenobjekt hat die `DOMAIN_EXTENDABLE` hinzugefügt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>Ist-Kosten</li>
              <li>Ist-Kosten</li>
              <li>Ist-Lohnkosten</li>
              <li>actualNonBillableExpenseCost</li>
              <li>Ist-Einnahmen</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>Geplante Kosten/LI&gt;
              <li>GeplanteAusgabenKosten</li>
              <li>Geplante Lohnkosten</li>
              <li>scheduledNonBillableExpenseCost</li>
              <li>Geplante Einnahmen</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Ist-Kosten</li>
          <li>Ist-Einnahmen</li>
          <li>Geplante Kosten</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Die folgenden möglichen Werte wurden hinzugefügt:<ul><li><code>URH</code> (Benutzer und Funktion stündlich)</li></ul></li>
          <li><p><b>RevenueType</b></p> <p>Die folgenden möglichen Werte wurden hinzugefügt:<ul><li><code>URH</code> (Benutzer und Funktion stündlich)</li><li><code>URC</code> (Benutzer und Funktion stündlich mit Obergrenze)</li><li><code>URF</code> (Stündlich für Benutzer und Funktionen plus fest)</li></ul></li>
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
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>Budget</li>
              <li>Fixkosten</li>
              <li>Festeinnahmen</li>
              <li>geplanterGewinn</li>
              <li>scheduledBillableExpenseCost</li>
              <li>Geplante Kosten</li>
              <li>GeplanteAusgabenKosten</li>
              <li>Geplante Lohnkosten</li>
              <li>scheduledNonBillableExpenseCost</li>
              <li>Geplante Einnahmen</li>
              <li>geplante Risikokosten</li>
              <li>WorkRequired</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Geplante Kosten</li>
          <li>Geplante Einnahmen</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
          <p>Die folgenden Felder wurden hinzugefügt:</p>
             <ul>
              <li><b>Abrechnungssätze</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Vorlagenaufgabe (TTSK)

Ein TemplateTask-Objekt stellt eine Aufgabe dar, die Teil einer Vorlage ist. Vorlagenaufgaben werden zu Aufgaben im Projekt, in dem die Vorlage verwendet wird.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>billingAmount</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>Geplante Kosten/LI&gt;
              <li>GeplanteAusgabenKosten</li>
              <li>Geplante Lohnkosten</li>
              <li>scheduledNonBillableExpenseCost</li>
              <li>Geplante Einnahmen</li>
              <li>RevenueType</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Geplante Kosten</li>
          <li>Geplante Einnahmen</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Die folgenden möglichen Werte wurden hinzugefügt:<ul><li><code>URH</code> (Benutzer und Funktion stündlich)</li></ul></li>
          <li><p><b>RevenueType</b></p> <p>Die folgenden möglichen Werte wurden hinzugefügt:<ul><li><code>URH</code> (Benutzer und Funktion stündlich)</li><li><code>URC</code> (Benutzer und Funktion stündlich mit Obergrenze)</li><li><code>URF</code> (Stündlich für Benutzer und Funktionen plus fest)</li></ul></li>
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
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>Entfernt</p>
          </li>
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
                <p><code>externalFolderMetadataError</code> (enum.updateTypeEnum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Benutzer (USER)

Ein Benutzerobjekt stellt eine Person mit einem Konto in Workfront dar, die sich anmelden und mit dem System interagieren kann.

Das Benutzerobjekt hat die Felder `ATTRIBUTE_ATTACHABLE` und `DOMAIN_EXTENDABLE` hinzugefügt.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direkte Felder</td>
      <td>
        <ul>
          <li>
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Sammlungsfelder</td>
      <td>
          <p>Die folgenden Felder wurden hinzugefügt:</p>
             <ul>
              <li><b>Abrechnungssätze</b></li>
              <li><b>costRates</b></li>
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
            <p>Die folgenden Felder haben das <code>RESTRICTABLE</code> hinzugefügt:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>Ist-Kosten</li>
              <li>Ist-Kosten</li>
              <li>Ist-Lohnkosten</li>
              <li>actualNonBillableExpenseCost</li>
              <li>Ist-Einnahmen</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>scheduledBillableExpenseCost</li>
              <li>Geplante Kosten</li>
              <li>GeplanteAusgabenKosten</li>
              <li>Geplante Lohnkosten</li>
              <li>scheduledNonBillableExpenseCost</li>
              <li>Geplante Einnahmen</li>
            </ul>
          </li>
          <li>
          <p>Die folgenden Felder haben ihren Typ von <code>double</code> in <code>class java.math.BigDecimal</code> geändert:
          <ul>
          <li>Ist-Kosten</li>
          <li>Ist-Einnahmen</li>
          <li>Geplante Kosten</li>
          <li>Geplante Einnahmen</li>
          </ul>
          </li>
          <li><p><b>geplanteDauer</b></p> <p>Die Flags <code>DYNAMIC</code>, <code>LAZY_READ</code> und hinzugefügt <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>hat das Flag hinzugefügt <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Der mögliche Wert <code>URH</code> (stündlich für Benutzer und Funktion) wurde hinzugefügt. </li>
          <li><p><b>RevenueType</b></p> <p>Die möglichen Werte <code>URH</code> (Benutzer und Funktion pro Stunde), <code>URC</code> (Benutzer und Funktion pro Stunde mit Obergrenze) und <code>URF</code> (Benutzer und Funktion pro Stunde plus fest) wurden hinzugefügt</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



