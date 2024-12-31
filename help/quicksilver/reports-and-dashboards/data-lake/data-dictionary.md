---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Datenwörterbuch für Workfront Data Connect
description: Diese Seite enthält Informationen zur Struktur und zum Inhalt der Daten in Workfront Data Connect.
author: Nolan
feature: Reports and Dashboards
exl-id: 57985404-554e-4289-b871-b02d3427aa5c
source-git-commit: 4c8b7e7f33ec593b2942725eb9160f7fbe2962e3
workflow-type: tm+mt
source-wordcount: '4294'
ht-degree: 4%

---

# Datenwörterbuch für Workfront Data Connect

Diese Seite enthält Informationen zur Struktur und zum Inhalt der Daten in Workfront Data Connect.

>[!NOTE]
>
>Die Daten in Data Connect werden alle vier Stunden aktualisiert, sodass die letzten Änderungen möglicherweise nicht sofort angezeigt werden.

## Tabellentypen

Es gibt eine Reihe von Tabellentypen, die Sie in Data Connect verwenden können, um Ihre Workfront-Daten auf eine Weise anzuzeigen, die Ihnen die meisten Einblicke bietet.

* **Aktuelle Tabelle**

  Die aktuelle Tabelle spiegelt die Daten ähnlich wie in Workfront wider, jedes Objekt und seinen aktuellen Status. Sie kann jedoch mit einer viel geringeren Latenz als innerhalb von Workfront navigiert werden.

* **Ereignistabelle**

  Die Ereignistabelle erfasst jede Änderung in Workfront: d. h. jedes Mal, wenn ein Objekt den Status wechselt, wird ein Datensatz erstellt, der anzeigt, wann die Änderung stattgefunden hat, wer die Änderung vorgenommen hat und was geändert wurde. Daher ist diese Tabelle für Point-in-Time-Vergleiche nützlich. Diese Tabelle enthält nur Datensätze aus den letzten drei Jahren.

* **Tägliche Verlaufstabelle**

  Die Tägliche Verlaufstabelle bietet eine gekürzte Version der Ereignistabelle, da sie den Status jedes Objekts auf täglicher Basis anzeigt und nicht den Zeitpunkt, zu dem jedes einzelne Ereignis aufgetreten ist. Daher ist diese Tabelle für Trendanalysen nützlich.

<!-- Custom table -->

## Entitätsbeziehungsdiagramm

Objekte in Workfront (und daher im Data Connect-Data Lake) werden nicht nur durch ihre individuellen Werte definiert, sondern auch durch ihre Beziehungen zu anderen Objekten. Das folgende Entitätsbeziehungsdiagramm bietet eine allgemeine Zuordnung von Objektbeziehungen in Data Connect. Das Diagramm kann über den folgenden Link angezeigt und heruntergeladen werden:

[Data Connect-Entitätsbeziehungsdiagramm](/help/quicksilver/reports-and-dashboards/data-lake/assets/Workfront-data-lake_entity-relationship-diagram.pdf)

>[!IMPORTANT]
>
>Das Entitätsbeziehungsdiagramm ist eine laufende Arbeit, die nur zu Referenzzwecken dient und geändert werden kann.

## Datentypen

Es gibt eine Reihe von Datumsobjekten, die Informationen darüber liefern, wann bestimmte Ereignisse auftreten.

* `DL_LOAD_TIMESTAMP`: Dieses Datum wird als interne Referenz verwendet und gibt an, wann die Daten in die Tabelle „Aktuell“, „Ereignis“ oder „Täglicher Verlauf“ geladen wurden. Dieses Datum sollte nicht für die Datenanalyse verwendet werden und soll während der Beta-Phase des Data Lake von Workfront entfernt werden.
* `CALENDAR_DATE`: Dieses Datum ist nur in der Tabelle Tagesverlauf vorhanden. Diese Tabelle enthält eine Aufzeichnung des Aussehens der Daten um 11:59 UTC für jedes in `CALENDAR_DATE` angegebene Datum.
* `BEGIN_EFFECTIVE_TIMESTAMP`: Dieses Datum ist sowohl in der Ereignis- als auch in der täglichen Verlaufstabelle vorhanden und zeichnet genau auf, wann ein Datensatz _auf_ den Wert geändert wurde, den er in der aktuellen Zeile hat.
* `END_EFFECTIVE_TIMESTAMP`: Dieses Datum ist sowohl in der Ereignis- als auch in der täglichen Verlaufstabelle vorhanden und zeichnet genau auf, wann ein Datensatz _von_ den Wert in der aktuellen Zeile in einen Wert in einer anderen Zeile geändert hat. Um zwischen Abfragen von `BEGIN_EFFECTIVE_TIMESTAMP` und `END_EFFECTIVE_TIMESTAMP` zu ermöglichen, ist dieser Wert nie null, auch wenn kein neuer Wert vorhanden ist. Wenn ein Datensatz noch gültig ist (d. h. wenn sich der Wert nicht geändert hat), haben `END_EFFECTIVE_TIMESTAMP` den Wert 2300-01-01.

## Terminologietabelle

In der folgenden Tabelle werden die Objektnamen in Workfront (sowie deren Namen in der Benutzeroberfläche und API) mit den entsprechenden Namen in Data Connect korreliert.

<table>
  <thead>
    <tr>
        <th>Workfront-Entitätsname</th>
        <th>Schnittstellenverweise</th>
        <th>API-Referenz | Bezeichnung</th>
        <th>Data-Lake-Tabellen</th>
        <th>Feld „Beziehungen“</th>
        <th>Beziehungstabelle und -feld</th>
    </tr>
  </thead>
  <tbody>
    <tr>
        <td>Zugriffsebene</td>
        <td>Zugriffsebene</td>
        <td>GENEHMIGEN | Zugriffsebene</td>
        <td>ACCESSLEVELS_CURRENT<br>ACCESSLEVELS_DAILY_HISTORY<br>ACCESSLEVELS_EVENT</td>
        <td>ACCESSLEVELID (self)<br>APPGLOBALID<br>LASTUPDATEDBYID<br>LEGACYACCESSLEVELID<br>OBJID<br>SYSID</td>
        <td>Self<br>Not a relation; für interne Anwendungszwecke verwendet<br>USER_CURRENT | USERID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>Die ID des im OBJCODE-Feld identifizierten Objekts<br>Keine Beziehung; für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Zugriffsregel</td>
        <td>Freigeben</td>
        <td>VERSIERT | Freigeben</td>
        <td>ACCESSRULES_CURRENT<br>ACCESSRULES_DAILY_HISTORY<br>ACCESSRULES_EVENT</td>
        <td>ACCESSORID <br>ACCESSRULEID (SELBST) <br>ANCESTORID <br>LASTUPDATEDBYID <br>SECURITYOBJID <br>SYSID</td>
        <td>Die ID des -Objekts, das in ACCESSOROBJCODE field<br>Self<br> identifiziert wird. Die ID des -Objekts, das in dem ANCESTOROBJCODE field<br>USERS_CURRENT identifiziert wird | USERID<br>Die ID des im Feld SECURITYOBJCODE identifizierten Objekts<br>keine Beziehung; für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Genehmigungspfad</td>
        <td>Genehmigungspfad</td>
        <td>ARVPTH | Validierung</td>
        <td>APPROVALPATHS_CURRENT<br>APPROVALPATHS_DAILY_HISTORY<br>APPROVALPATHS_EVENT</td>
        <td>APPROVALPATHID (SELF) <br>APPROVALPROCESSID <br>ENTEREDBYID <br>GLOBALPATHID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td><br>_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | USERID<br>Keine Beziehung; für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Genehmigungsprozess</td>
        <td>Genehmigungsprozess</td>
        <td>ARVPRC | Genehmigungsprozess</td>
        <td>APPROVALPROCESSES_CURRENT<br>APPROVALPROCESSES_DAILY_HISTORY_<br>_EVENT</td>
        <td>APPROVALPROCESSID (self) <br>ENTEREDBYID <br>LASTUPDATEDBYID<br>SYSID</td>
        <td>self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID<br>Keine Beziehung; für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Genehmigungsschritt</td>
        <td>Genehmigungsschritt</td>
        <td>ARVSTP | Genehmigungsphase</td>
        <td>APPROVALSTEPS_CURRENT<br>APPROVALSTEPS_DAILY_HISTORY<br>APPROVALSTEPS_EVENT</td>
        <td>APPROVALPATHID <br>APPROVALSTEPID (self) <br>SYSID</td>
        <td>APPROVALPATHS_CURRENT | APPROVALPATHID<br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Status der genehmigenden Person</td>
        <td>Status der genehmigenden Person</td>
        <td>ARVSTS | Status der genehmigenden Person</td>
        <td>APPROVERSTATUSES_CURRENT<br>APPROVERSTATUSES_DAILY_HISTORY_<br>_EVENT</td>
        <td>APPROVERSTATUSID (SELF)<br>APPROVABLEOBJID<br>APPROVALSTEPID<br>APPROVEDBYID <br>DELEGATEUSERID<br>LASTUPDATEDBYID <br>OPTASKID<br>OVERRIDDENUSERID<br>PROJECTID<br>STEPAPPROVERID<br>SYSID<br>TASKID<br>WILDCARDUSERID</td>
        <td>Self<br>Die ID des im Feld APPROVABLEOBJCODE_<br>_CURRENT identifizierten Objekts | APPROVALSTEPID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>OPTASKS_CURRENT | OPTASKID<br>USERS_CURRENT | USERID<br>PROJECTS_CURRENT | PROJECTID<br>USERS_CURRENT | USERID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>Zuweisung</td>
        <td>Zuweisung</td>
        <td>ZUWEISEN | Zuweisung</td>
        <td>ASSIGNMENTS_CURRENT<br>ASSIGNMENTS_DAILY_HISTORY<br>ASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDBYID<br>ASSIGNEDTOID<br>ASSIGNMENTID (SELF)<br>CATEGORYID<br>CLASSIFIERID<br>OPTASKID<br>PRIVATERATECARDID<br>PROJECTID<br>ROLEID<br>TASKID<br>TEAMID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>SELF<br>CATEGORIES_CURRENT | CATEGORYID<br>Classifier-Tabelle wird derzeit nicht unterstützt<br>OPTASK_CURRENT | OPTASKID<br>RATECARD_CURRENT | RATECARDID<br>PROJECT_CURRENT | PROJECTID<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TEAM_CURRENT | TEAMFÄNGER</td>
    </tr>
    <tr>
        <td>Warten auf Genehmigungen</td>
        <td>Warten auf Genehmigungen</td>
        <td>AWAPVL | Warten auf Genehmigung</td>
        <td>AWAITINGAPPROVALS_CURRENT<br>AWAITINGAPPROVALS_DAILY_HISTORY<br>AWAITINGAPPROVALS_EVENT</td>
        <td>ACCESSREQUESTID<br>APPROVABLEID <br>APPROVERID <br>AWAITINGAPPROVALID (SELF) <br>DOCUMENTID <br>DOCUMENTVERSIONID<br>OPTASKID <br>PROJECTID <br>ROLEID <br>SUBMITTEDBYID <br>SYSID<br>TASKID <br>TEAMID <br>TIMESHEETID<br>USERID</td>
        <td>Tabelle für Zugriffsanfragen wird derzeit nicht unterstützt<br>Keine Beziehung; wird für interne Anwendungszwecke verwendet<br>USERS_CURRENT | USERID<br>SELF<br>DOCUMENTS_CURRENT | DOCUMENTID<br>DOCUMENTVERSIONS_CURRENT | DOCUMENTVERSIONID<br>OPTASKS_CURRENT | OPTASKID<br>PROJECTS_CURRENT | PROJECTID<br>ROLES_CURRENT | ROLEID<br>USERS_CURRENT | USERID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | TASKID<br>TEAMS_CURRENT | TEAMID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>USERS_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>Ausgangsbasis</td>
        <td>Ausgangsbasis</td>
        <td>BLIND | Baseline</td>
        <td>BASELINES_CURRENT_<br>_DAILY_HISTORY<br>BASELINES_EVENT</td>
        <td>BASELINEID (self)<br>EXCHANGERATEID <br>PROJECTID <br>SYSID</td>
        <td><br>_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Keine Beziehung; für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Baseline-Aufgabe</td>
        <td>Baseline-Aufgabe</td>
        <td>BSTSK | Baseline-Aufgabe</td>
        <td>BASELINETASKS_CURRENT<br>BASELINETASKS_DAILY_HISTORY<br>BASELINETASKS_EVENT</td>
        <td>BASELINEID<br>BASELINETASKID (self) <br>EXCHANGERATEID <br>PROJECTID <br>SYSID<br>TASKID</td>
        <td>BASELINES_CURRENT | BASELINEID<br>SELF<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>PROJECTS_CURRENT | PROJECTID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | AUFGABEN-ID</td>
    </tr>
    <tr>
        <td>Abrechnungssatz</td>
        <td>Abrechnungssatz</td>
        <td>RATE | Abrechnungssatz</td>
        <td>RATES_CURRENT<br>RATES_DAILY_HISTORY<br>RATES_EVENT</td>
        <td>ASSIGNMENTID<br>CLASSIFIERID<br>EXCHANGERATEID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID <br>RATECARDID<br>RATEID (SELF)<br>ROLEID <br>SOURCERATECARDID <br>SYSID <br>TEMPLATEID<br>USERID</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID<br>Classifier-Tabelle wird derzeit nicht unterstützt<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Non-Labor Resource Category-Tabelle wird derzeit nicht unterstützt<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>Die ID des im OBJCODE-Feld identifizierten Objekts <br>PROJECTS_CURRENT | PROJECTID <br>RATECARD_CURRENT | RATECARDID<br>SELF<br>ROLES_CURRENT | ROLEID <br>RATECARD_CURRENT | RATECARDID <br>Keine Beziehung; für interne Anwendungszwecke verwendet <br>TEMPLATES_CURRENT | TEMPLATEID<br>USERS_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>Abrechnungseintrag</td>
        <td>Abrechnungseintrag</td>
        <td>RECHNUNG | Rechnungsnachweis</td>
        <td>BILLINGRECORDS_CURRENT<br>BILLINGRECORDS_DAILY_HISTORY<br>BILLINGRECORDS_EVENT</td>
        <td>BILLINGRECORDID (self)<br>CATEGORYID<br>EXCHANGERATEID <br>INVOICEID <br>LASTUPDATEDBYID <br>PROJECTID <br>SYSID</td>
        <td>self<br>CATEGORIES_CURRENT | CATEGORYID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>Rechnungstabelle wird derzeit nicht unterstützt <br>USERS_CURRENT | USERID <br>PROJECTS_CURRENT | PROJEKT-ID   <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Buchung</td>
        <td>Buchung</td>
        <td>BUCHUNG | Buchung</td>
        <td>BOOKINGS_CURRENT_<br>_DAILY_HISTORY<br>BOOKINGS_EVENT</td>
        <td>BOOKINGID (SELBST)<br>ENTEREDBYID<br>LASTUPDATEDBYID<br>NLBRCATEGORYID<br>NONLABORRESOURCEID<br>OBJID<br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>self<br>USERS_CURRENT | USERID<br>USERS_CURRENT | Die Tabelle <br>USERID-Non-Labor-Ressourcenkategorie“ wird derzeit nicht unterstützt<br>NONLABORRESOURCES_CURRENT | NONLABORRESOURCEID<br>Die ID des im OBJOBJCODE-Feld identifizierten Objekts <br>PROJECTS_CURRENT | PROJECTID <br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | AUFGABEN-ID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Die ID des im Feld TOPOBJCODE identifizierten Objekts</td>
    </tr>
    <tr>
        <td>Kategorie</td>
        <td>Benutzerdefiniertes Formular</td>
        <td>CTGY | Kategorie</td>
        <td>CATEGORIES_CURRENT<br>CATEGORIES_DAILY_HISTORY<br>CATEGORIES_EVENT</td>
        <td>CATEGORYID (self)<br>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID</td>
        <td>self<br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Kategorieparameter</td>
        <td>Benutzerdefinierte Formularfelder</td>
        <td>CTGYPA | Kategorieparameter</td>
        <td>CATEGORIESPARAMETERS_CURRENT<br>CATEGORIESPARAMETERS_DAILY_HISTORY<br>CATEGORIESPARAMETERS_EVENT</td>
        <td>CATEGORIESPARAMETERID (self)<br>CATEGORYID<br>PARAMETERGROUPID<br>PARAMETERID    <br>SYSID</td>
        <td>self<br>CATEGORIES_CURRENT | CATEGORYID<br>Parameter Group-Tabelle wird derzeit nicht unterstützt<br>PARAMETERS_CURRENT | PARAMETERID    <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Firma</td>
        <td>Firma</td>
        <td>COMPY | Firma</td>
        <td>COMPANIES_CURRENT<br>COMPANIES_DAILY_HISTORY<br>COMPANIES_EVENT</td>
        <td>CATEGORYID<br>COMPANYID (SELF)<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>PRIVATERATECARDID<br>SYSID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>SELF<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>Keine Beziehung; für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Benutzerdefiniertes Quartal</td>
        <td>Benutzerdefiniertes Quartal</td>
        <td>CSTART | Benutzerdefiniertes Quartal</td>
        <td>CUSTOMQUARTERS_CURRENT<br>CUSTOMQUARTERS_DAILY_HISTORY<br>CUSTOMQUARTERS_EVENT</td>
        <td>CUSTOMQUARTERID (self) <br>SYSID</td>
        <td>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Benutzerdefinierte Enumeration</td>
        <td>Bedingung, Priorität, Schweregrad, Status</td>
        <td>SYSTEM | Benutzerdefinierte Enumeration</td>
        <td>CUSTOMENUMS_CURRENT<br>CUSTOMENUMS_DAILY_HISTORY<br>CUSTOMENUMS_EVENT<br>* Die Art des Datensatzes wird durch die Eigenschaft „enumClass“ identifiziert. Die folgenden Typen werden erwartet:<br>CONDITION_OPTASK<br>CONDITION_PROJ<br>CONDITION_TASK<br>PRIORITY_OPTASK<br>PRIORITY_PROJ<br>PRIORITY_TASK<br>SEVERITY_OPTASK<br>STATUS_OPTASK<br>STATUS_PROJ<br>_TASK</td>
        <td>ENTEREDBYID<br>GROUPID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID</td>
    </tr>
    <tr>
        <td>Dokument</td>
        <td>Dokument</td>
        <td>DOKU | Dokument</td>
        <td>DOCUMENTS_CURRENT<br>DOCUMENTS_DAILY_HISTORY<br>DOCUMENTS_EVENT<br>DOCUMENTS_CUSTOM_VALUE_CURRENT<br>DOCUMENTS_CUSTOM_VALUE_DAILY_HISTORY<br>DOCUMENTS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>CHECKEDOUTBYID<br>DOCUMENTID<br>DOCUMENTREQUESTID<br>EXCHANGERATEID<br>ITERATIONID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>RELEASEVERSIONID<br>TASKID<br>TEMPLATEID<br> TEMPLATETASKID<br>TOPOBJID<br>USERID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | Tabelle <br>USERID Self<br>Document-Anfrage“ wird derzeit nicht unterstützt<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Variable abhängig von DOCOBJCODE value<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Release-Versionstabelle wird derzeit nicht <br>. | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Variable abhängig vom TOPOBJCODE-Wert<br>USER_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>Dokumentengenehmigung</td>
        <td>Dokumentengenehmigung</td>
        <td>DOCAPL | Dokumentengenehmigung</td>
        <td>DOCAPPROVALS_CURRENT<br>DOCAPPROVALS_DAILY_HISTORY<br>DOCAPPROVALS_EVENT</td>
        <td>APPROVERID<br>DOCAPPROVALID (self)<br>DOCUMENTID<br>NOTEID<br>REQUESTORID<br>SYSID</td>
        <td>USERS_CURRENT | USERID <br>SELF<br>DOCUMENTS_CURRENT | DOCUMENTID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Dokumentenordner</td>
        <td>Dokumentenordner</td>
        <td>DOCFLD | DocsFolders</td>
        <td>DOCFOLDERS_CURRENT<br>DOCFOLDERS_DAILY_HISTORY<br>DOCFOLDERS_EVENT</td>
        <td>DOCFOLDERID (self)<br>ENTEREDBYID<br>ISSUEID<br>ITERATIONID    <br>LINKEDFOLDERID<br>PARENTID<br>PORTFOLIOID <br>PROGRAMID    <br>PROJECTID<br>SYSID<br>TASKID     <br>TEMPLATEID<br>TEMPLATETASKID<br>USERID</td>
        <td>self<br>USERS_CURRENT | USERID<br>OPTASKS_CURRENT | OPTASKID<br>ITERATIONS_CURRENT | ITERATIONID<br>LINKEDFOLDER_CURRENT | LINKEDFOLDERID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>PORTFOLIO_CURRENT | PORTFOLIOID <br>PROGRAM_CURRENT | PROGRAMM-ID    <br>PROJECTS_CURRENT | PROJECTID <br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | AUFGABEN-ID     <br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>USERS_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>DocumentProvideMetadata</td>
        <td>Dokument stellt Metadaten bereit</td>
        <td>DOKUMENT | DocumentProviderMetadata</td>
        <td>DOCPROVIDERMETA_CURRENT<br>DOCPROVIDERMETA_DAILY_HISTORY<br>DOCPROVIDERMETA_EVENT</td>
        <td>DOCPROVIDERMETAID (self) <br>SYSID</td>
        <td>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>DocumentProvider</td>
        <td>Dokumentanbieter</td>
        <td>DOCPRO | Dokumentanbieter</td>
        <td>DOCPROVIDERS_CURRENT<br>DOCPROVIDERS_DAILY_HISTORY<br>DOCPROVIDERS_EVENT</td>
        <td>DOCPROVIDERCONFIGID<br>DOCPROVIDERID (Self)<br>OWNERID    <br>SYSID</td>
        <td>DOCPROVIDERCONFIG_CURRENT | DOCPROVIDERCONFIGID<br>SELF<br>USERS_CURRENT | BENUTZER-ID    <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>DocumentProviderConfig</td>
        <td>Konfiguration des Dokumentanbieters</td>
        <td>DOCCFG | DocumentProviderConfig</td>
        <td>DOCPROVIDERCONFIG_CURRENT<br>DOCPROVIDERCONFIG_DAILY_HISTORY<br>DOCPROVIDERCONFIG_EVENT</td>
        <td>DOCPROVIDERCONFIGID (self)<br>SYSID</td>
        <td>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>DocumentVersion</td>
        <td>Dokumentversion</td>
        <td>DOCV | Dokumentversion</td>
        <td>DOCUMENTVERSIONS_CURRENT<br>DOCUMENTVERSIONS_DAILY_HISTORY<br>DOCUMENTVERSIONS_EVENT</td>
        <td>DOCUMENTID<br>DOCUMENTPROVIDERID<br>DOCUMENTVERSIONID<br>ENTEREDBYID<br>EXTERNALSTORAGEID<br>PROOFAPPROVALSTATUSID<br>PROOFEDBYUSERID<br>PROOFID<br>PROOFOWNERID<br>PROOFSTAGEID</td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>DOCPROVIDERS_CURRENT | DOCUMENTPROVIDERID<br>SELF<br>USER_CURRENT | USERID<br>External ID<br>Proof Approval Status-Tabelle wird derzeit nicht unterstützt<br>USER_CURRENT | USERID<br>Proof-Tabelle wird derzeit nicht unterstützt<br>USER_CURRENT | USERID<br>Proof-Staging-Tabelle wird derzeit nicht unterstützt</td>
    </tr>
    <tr>
        <td>Wechselkurs</td>
        <td>Wechselkurs</td>
        <td>EXTRAHIEREN | Wechselkurs</td>
        <td>EXCHANGERATES_CURRENT<br>EXCHANGERATES_DAILY_HISTORY<br>EXCHANGERATES_EVENT</td>
        <td>EXCHANGERATEID (self)<br>PROJECTID<br>SYSID <br>TEMPLATEID  </td>
        <td>SELF<br>PROJECTS_CURRENT | PROJECTID <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet <br>TEMPLATES_CURRENT | TEMPLATEID  </td>
    </tr>
    <tr>
        <td>Ausgabe</td>
        <td>Ausgabe</td>
        <td>AUSGABEN | Ausgabe</td>
        <td>EXPENSES_CURRENT<br>EXPENSES_DAILY_HISTORY<br>EXPENSES_EVENT</td>
        <td>BILLINGRECORDID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID <br>EXPENSEID (SELBST) <br>EXPENSETYPEID <br>LASTUPDATEDBYID <br>OBJID <br>PROJECTID<br>SYSID<br>TASKID<br>TEMPLATEID<br>TEMPLATETASKID<br>TOPOBJID</td>
        <td>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID <br>SELF <br>EXPENSETYPES_CURRENT | EXPENSETYPEID <br>USERS_CURRENT | USERID <br>Die ID des im OBJCODE-Feld identifizierten Objekts <br>PROJECTS_CURRENT | PROJECTID <br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>Die ID des im Feld TOPOBJCODE identifizierten Objekts</td>
    </tr>
    <tr>
        <td>Ausgabentyp</td>
        <td>Ausgabentyp</td>
        <td>EXPTYP | Ausgabentyp</td>
        <td>EXPENSETYPES_CURRENT<br>EXPENSETYPES_DAILY_HISTORY<br>EXPENSETYPES_EVENT</td>
        <td>APPGLOBALID<br>EXPENSETYPEID (self)<br>OBJID <br>SYSID  </td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet<br>Selbst<br>Die ID des im OBJCODE-Feld identifizierten Objekts <br>Keine Beziehung; für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Gruppe</td>
        <td>Gruppe</td>
        <td>GRUPPE | Gruppe</td>
        <td>GROUPS_CURRENT<br>GROUPS_DAILY_HISTORY<br>GROUPS_EVENT</td>
        <td>BUSINESSLEADERID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>PARENTID<br>ROOTID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>Self<br>Layout-Vorlagentabelle wird nicht unterstützt<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>UITEMPLATES_CURRENT | UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Stunde</td>
        <td>Stunde</td>
        <td>STUNDE | Stunde</td>
        <td>HOURS_CURRENT<br>HOURS_DAILY_HISTORY<br>HOURS_EVENT</td>
        <td>APPROVEDBYID<br>BILLINGRECORDID<br>CATEGORYID<br>CLASSIFIERID<br>DUPID<br>EXCHANGERATEID<br>EXTERNALTIMESHEETID<br>HOURID<br>HOURTYPEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>PROJECTOVERHEADID<br>ROLEID<br>TASKID<br>TIMESTIMESHEETIMESHEETIMESHEETIMESHEETIMESHEETIMESHEETIMESHEETIME</td>
        <td>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>Classifier-Tabelle wird derzeit nicht unterstützt<br>Keine Beziehung; wird für interne Anwendungszwecke verwendet<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>Keine Workfront-Beziehung; wird für die Integration in externe Systeme verwendet<br>Self<br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>ROLE_CURRENT | ROLEID<br>TASK_CURRENT | TASKID<br>TIMESHEET_CURRENT | ARBEITSZEITTABELLEN-ID</td>
    </tr>
    <tr>
        <td>Stundentyp</td>
        <td>Stundentyp</td>
        <td>STUNDE | Stundentyp</td>
        <td>HOURTYPES_CURRENT</td>
        <td>APPGLOBALID<br>HOURTYPEID<br>OBJID</td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet<br>Selbst<br>Keine Beziehung; für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Wiederholung</td>
        <td>Wiederholung</td>
        <td>ZURÜCK | Wiederholung</td>
        <td>ITERATIONS_CURRENT<br>ITERATIONS_DAILY_HISTORY<br>ITERATIONS_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>ITERATIONID (SELF)<br>LASTUPDATEDBYID<br>OWNERID<br>SYSID<br>TEAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID <br>SELF<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TEAMS_CURRENT | TEAMFÄNGER</td>
    </tr>
    <tr>
        <td>Journaleintrag</td>
        <td>Journaleintrag</td>
        <td>KNURREN | Tagebucheintrag</td>
        <td>JOURNALENTRIES_CURRENT<br>JOURNALENTRIES_DAILY_HISTORY<br>JOURNALENTRIES_EVENT</td>
        <td>APPROVERSTATUSID<br>ASSIGNMENTID<br>AUDITRECORDID<br>BASELINEID <br>BILLINGRECORDID<br>COMPANYID <br>DOCUMENTID <br>DOCUMENTSHAREID <br>EDITEDBYID<br>EXPENSEID<br>HOURID<br>INITIATIVEID<br>JOURNALENTRIEID (Self)<br>OBJID<br>OPTASKID<br>PORTFOLIOID<br>PROGRAMID<br>SUBOBJID<br>SUBSCRIBEID<br>SYSID<br>TASKID<br>TEMPLATETID<br><br> <br> <br> TOPOBJIDMESHEETID</td>
        <td>APPROVERSTATUSES_CURRENT | APPROVERSTATUSID<br>ASSIGNMENTS_CURRENT | Tabelle <br>ASSIGNMENTID-Audit-Einträge“ wird derzeit nicht unterstützt<br>BASELINES_CURRENT | BASELINEID <br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENTS_CURRENT | DOCUMENTID <br>Tabelle für Dokumentfreigabe wird derzeit nicht unterstützt <br>USERS_CURRENT | USERID<br>EXPENSES_CURRENT | EXPENSEID<br>HOURS_CURRENT | HOURID<br>Initiative-Tabelle wird derzeit nicht unterstützt<br>Self<br>Die ID des im OBJCODE-Feld identifizierten Objekts<br>OPTASKS_CURRENT | OPTASKID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECTS_CURRENT | PROJECTID <br>Die ID des im Feld SUBOBJCODE identifizierten Objekts "<br>" wird derzeit nicht unterstützt<br>keine Beziehung; wird für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TIMESHEETS_CURRENT | TIMESHEETID<br>Die ID des im Feld TOPOBJCODE_<br>_CURRENT identifizierten Objekts | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>LinkedFolder</td>
        <td>LinkedFolder</td>
        <td>LINKFDR | LinkedFolder</td>
        <td>LINKEDFOLDERS_CURRENT<br>LINKEDFOLDERS_DAILY_HISTORY_<br>_EVENT</td>
        <td>DOCUMENTPROVIDERID<br>EXTERNALSTORAGEID<br>FOLDERID<br>LINKEDBYID<br>LINKEDFOLDERID (SELF)<br>SYSID</td>
        <td>DOCPROVIDERS_CURRENT | DOCPROVIDERID<br>EXTERNAL ID<br>DOCFOLDERS_CURRENT | DOCFOLDERID<br>USERS_CURRENT | USERID <br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Meilenstein</td>
        <td>Meilenstein</td>
        <td>MEILE | Meilenstein</td>
        <td>MILESTONES_CURRENT<br>MILESTONES_DAILY_HISTORY_<br>_EVENT</td>
        <td>LASTUPDATEDBYID<br>MILESTONEID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>SELF<br>MILESTONEPATH_CURRENT | MEILENSTEIN-ID</td>
    </tr>
    <tr>
        <td>Meilensteinpfad</td>
        <td>Meilensteinpfad</td>
        <td>MPATH | Meilensteinpfad</td>
        <td>MILESTONEPATHS_CURRENT<br>MILESTONEPATHS_DAILY_HISTORY<br>MILESTONEPATHS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID<br>MILESTONEPATHID</td>
        <td>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Sonstige Ressource</td>
        <td>Sonstige Ressource</td>
        <td>NLBR | Sonstige Ressource</td>
        <td>NONLABORRESOURCES_CURRENT<br>NONLABORRESOURCES_DAILY_HISTORY<br>NONLABORRESOURCES_EVENT</td>
        <td>CATEGORYID<br>NONLABORRESOURCEID (SELF)<br>ENTEREDBYID<br>HOMEGROUPID<br>LASTUPDATEDBYID<br>NONLABORRESOURCECATEGORYID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>SELF<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>USERS_CURRENT | USERID <br>Tabelle der sonstigen Ressourcenkategorie wird derzeit nicht unterstützt <br>Keine Beziehung; für interne Anwendungszwecke verwendet    </td>
    </tr>
    <tr>
        <td>arbeitsfreier Tag</td>
        <td>Zeitplanausnahme</td>
        <td>NONWKD | Arbeitsfreier Tag</td>
        <td>NONWORKDAYS_CURRENT<br>NONWORKDAYS_DAILY_HISTORY<br>NONWORKDAYS_EVENT</td>
        <td>NONWORKDAYID (self)<br>OBJID <br>SCHEDULEID <br>SYSID <br>USERID  </td>
        <td>Self<br>Die ID des im OBJCODE-Feld identifizierten Objekts <br>SCHEDULES_CURRENT | SCHEDULEID <br>Keine Beziehung; für interne Anwendungszwecke verwendet <br>USERS_CURRENT | BENUTZER-ID  </td>
    </tr>
    <tr>
        <td>Notiz</td>
        <td>Notiz</td>
        <td>HINWEIS | Hinweis</td>
        <td>NOTES_CURRENT<br>NOTES_DAILY_HISTORY<br>NOTES_EVENT</td>
        <td>ATTACHDOCUMENTID<br>ATTACHOBJID<br>ATTACHOPTASKID<br>ATTACHWORKID<br>ATTACHWORKUSERID<br>AUDITRECORDID<br>COMPANYID<br>DOCUMENTID<br>EXTERNALSERVICEID<br>ITERATIONID<br>NOTEID<br>OBJID<br>OPTASKID<br>OWNERID<br>PARENTENDORSEMENTID<br>PARENTJOURNALENTRYID<br><br> TEID<br>PORTFOLIOID<br>PROGRAMID<br>PROJECTID<br>PROOFACTIONIDPROOFIDRICHTETEXTNOTEID<br> <br> <br> <br> <br> <br> <br> <br></td>
        <td>DOCUMENT_CURRENT | DOCUMENTID<br>Variable abhängig von ATTACHOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>WORKITEMS_CURRENT<br>USER_CURRENT | Die Tabelle <br>USERID-Audit-Einträge“ wird derzeit nicht unterstützt<br>COMPANIES_CURRENT | COMPANYID <br>DOCUMENT_CURRENT | DOCUMENTID<br>Keine Workfront-Beziehung; wird für die Integration in externe Systeme verwendet<br>ITERATIONS_CURRENT | ITERATIONID<br>Self<br>Variable abhängig von NOTEOBJCODE<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | Die Tabelle <br>USERID_Endorsement“ wird derzeit nicht unterstützt<br>JOURNALENTRIES_CURRENT | JOURNALENTRYID<br>NOTE_CURRENT | NOTEID<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>PROGRAM_CURRENT | PROGRAMID<br>PROJECT_CURRENT | PROJECTID<br>Proof-Aktionstabelle wird derzeit nicht unterstützt<br>Proof-Tabelle wird derzeit nicht unterstützt<br>RESERVEDTEXTNOTES_CURRENT | RICHTEXTNOTEID<br>TASK_CURRENT | TASKID<br>TEMPLATES_CURRENT | TEMPLATEID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID<br>NOTE_CURRENT | NOTEID<br>TIMESHEET_CURRENT | TIMESHEETID<br>Variable abhängig von TOPOBJCODE<br>USER_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>Objektintegration</td>
        <td>Objektintegration</td>
        <td>EINWENDEN | ObjectIntegration</td>
        <td>OBJECTINTEGRATION_CURRENT<br>OBJECTINTEGRATION_DAILY_HISTORY<br>OBJECTINTEGRATION_EVENT</td>
        <td>LINKEDOBJECTID<br>OBJECTINTEGRATIONID   (self)<br>OBJID <br>SYSID  </td>
        <td>Die ID des im Feld LINKEDOBJECTCODE identifizierten Objekts <br>Self<br>Die ID des im Feld OBJCODE identifizierten Objekts <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Objektkategorie</td>
        <td>Objektkategorien</td>
        <td>OBJEKT | Objektkategorie</td>
        <td>OBJECTSCATEGORIES_CURRENT<br>OBJECTSCATEGORIES_DAILY_HISTORY<br>OBJECTSCATEGORIES_EVENT</td>
        <td>CATEGORYID<br>OBJECTSCATEGORYID (self)<br>OBJID <br>SYSID  </td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>Self<br>Die ID des im Feld OBJCODE identifizierten Objekts <br>keine Beziehung; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>OpTask</td>
        <td>Problem, Anfrage</td>
        <td>OPTASK | Problem</td>
        <td>OPTASKS_CURRENT<br>OPTASKS_DAILY_HISTORY<br>OPTASKS_EVENT<br>OPTASKS_CUSTOM_VALUE_CURRENT<br>OPTASKS_CUSTOM_VALUE_DAILY_HISTORY<br>OPTASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>OPTASKID<br>OWNERID<br>PROJECTID<br>QUEUEDEFID<br>QUEUETOPICID<br> RESOLVEOPTASKID<br>RESOLVEPROJECTID<br>RESOLVETASKID<br>RESOLVINGOBJID<br>ROLEID<br>SOURCEOBJID<br><br> <br> SOURCETASKIDSUBMITTEDBYIDTEAMID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>ITERATIONS_CURRENT | ITERATIONID<br>Kanban-Board-Tabelle wird derzeit nicht unterstützt<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>SELF<br>USER_CURRENT | USERID<br>PROJECT_CURRENT | PROJECTID<br>Queue-Definitionstabelle wird derzeit nicht unterstützt<br>Queue-Thementabelle wird derzeit nicht unterstützt<br>OPTASK_CURRENT | OPTASKID<br>PROJECT_CURRENT | PROJECTID<br>TASK_CURRENT | TASKID<br>Variable abhängig von RESOLVINGOBJCODE<br>ROLE_CURRENT | ROLEID<br>Variable abhängig von SOURCEOBJCODE<br>TASK_CURRENT | TASKID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMFÄNGER</td>
    </tr>
    <tr>
        <td>Parameter</td>
        <td>Benutzerdefiniertes Feld</td>
        <td>PARAMETER | Parameter</td>
        <td>PARAMETERS_CURRENT<br>PARAMETERS_DAILY_HISTORY_<br>_EVENT</td>
        <td>LASTUPDATEDBYID<br>PARAMETERFILTERID<br>PARAMETERID (SELF)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID<br>Parameter-Filtertabelle wird derzeit nicht unterstützt<br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Parameteroption</td>
        <td>Parameteroption</td>
        <td>POPT | Parameteroption</td>
        <td>PARAMETEROPTIONS_CURRENT<br>PARAMETEROPTIONS_DAILY_HISTORY<br>PARAMETEROPTIONS_EVENT</td>
        <td>PARAMETERID<br>PARAMETEROPTIONID (self) <br>SYSID  </td>
        <td>PARAMETERS_CURRENT | PARAMETERID <br>Self <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Portalabschnitt</td>
        <td>Bericht</td>
        <td>PTLSEC | Bericht</td>
        <td>PORTALSECTIONS_CURRENT<br>PORTALSECTIONS_DAILY_HISTORY<br>PORTALSECTIONS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID<br>FILTERID<br>GROUPBYID<br>LASTUPDATEDBYID<br>LASTVIEWEDBYID<br>OBJID<br>PORTALSECTIONID (SELBST)<br>PREFERENCEID<br>PUBLICRUNASUSERID<br>REPORTFOLDERID<br>RUNASUSERID<br>SCHEDULEDREPORTID<br>SYSID<br>VIEWID</td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet <br>USERS_CURRENT | USERID <br>UIFILTERS_CURRENT | FILTERID<br>UIGROUPBYS_CURRENT | GROUPBYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Die ID des im OBJOBJCODE-Feld identifizierten Objekts<br>Self<br>PREFERENCES_CURRENT | PREFERENCEID<br>USERS_CURRENT | USERID <br>REPORTFOLDERS_CURRENT | REPORTFOLDERID<br>USERS_CURRENT | USERID <br>Geplante Berichtstabelle wird derzeit nicht unterstützt<br>Keine Beziehung; wird für interne Anwendungszwecke verwendet (<br>_CURRENT | VIEWID</td>
    </tr>
    <tr>
        <td>Registerkarte „Portal“</td>
        <td>Dashboard</td>
        <td>PTLTAB | Dashboard</td>
        <td>PORTALTABS_CURRENT<br>PORTALTABS_DAILY_HISTORY<br>PORTALTABS_EVENT</td>
        <td>DOCID<br>LASTUPDATEDBYID<br>PORTALPROFILEID<br>PORTALTABID (SELF)<br>SYSID<br>USERID</td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet <br>USERS_CURRENT | USERID <br>Portalprofiltabelle wird nicht unterstützt <br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet <br>USERS_CURRENT | BENUTZER-ID  </td>
    </tr>
    <tr>
        <td>Portal-Registerkarten-Abschnitt</td>
        <td>Dashboard-Abschnitt</td>
        <td>PRTBSC | Portalregisterkarten-Abschnitt</td>
        <td>PORTALTABSPORTALSECTIONS_CURRENT<br>PORTALTABSPORTALSECTIONS_DAILY_HISTORY<br>PORTALTABSPORTALSECTIONS_EVENT</td>
        <td>CALENDARPORTALSECTIONID<br>EXTERNALSECTIONID<br>INTERNALSECTIONID <br>PORTALSECTIONOBJID <br>PORTALTABID<br>PORTALTABSECTIONID (SELF)<br>SYSID</td>
        <td>Kalenderportalabschnitt wird derzeit nicht unterstützt <br>Tabelle der externen Abschnitte wird derzeit nicht unterstützt<br>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>Die ID des im PORTALSECTIONOBJCODE-Feld identifizierten Objekts<br>PORTALTABS_CURRENT | PORTALTABID<br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>PortalSectionLastViewer</td>
        <td>Letzte Betrachter des Berichts</td>
        <td>PLSV | PortalSectionLastViewer</td>
        <td>REPORTLASTVIEWERS_CURRENT<br>REPORTLASTVIEWERS_DAILY_HISTORY<br>REPORTLASTVIEWERS_EVENT</td>
        <td>REPORTID<br>REPORTLASTVIEWERID (self)<br>SYSID<br>VIEWERID</td>
        <td>PORTALSECTIONS_CURRENT | PORTALSECTIONID <br>REPORTLASTVIEWERID (self)<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | BENUTZER-ID  </td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Portfolio</td>
        <td>PORT | Portfolio</td>
        <td>PORTFOLIOS_CURRENT<br>PORTFOLIOS_DAILY_HISTORY<br>PORTFOLIOS_EVENT<br>PORTFOLIOS_CUSTOM_VALUE_CURRENT<br>PORTFOLIOS_CUSTOM_VALUE_DAILY_HISTORY<br>PORTFOLIOS_CUSTOM_VALUE_EVENT</td>
        <td>ALIGNMENTSCORECARDID<br>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID</td>
        <td>Scorecard-Tabelle wird derzeit nicht unterstützt<br>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>Self</td>
    </tr>
    <tr>
        <td>Voreinstellung</td>
        <td>Anzeigen, Filtern, Gruppieren, Berichtsdefinition</td>
        <td>PROSET | Voreinstellung</td>
        <td>PREFERENCES_CURRENT<br>PREFERENCES_DAILY_HISTORY<br>PREFERENCES_EVENT</td>
        <td>APPGLOBALID<br>PREFERENCEID (self) <br>SYSID  </td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet<br>Selbst <br>Keine Beziehung; für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Programm</td>
        <td>Programm</td>
        <td>PRGM | Programm</td>
        <td>PROGRAMS_CURRENT<br>PROGRAMS_DAILY_HISTORY<br>PROGRAMS_EVENT<br>PROGRAMS_CUSTOM_VALUE_CURRENT<br>PROGRAMS_CUSTOM_VALUE_DAILY_HISTORY<br>PROGRAMS_CUSTOM_VALUE_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>GROUPID<br>LASTUPDATEDBYID<br>OWNERID<br>PORTFOLIOID<br>PROGRAMID</td>
        <td>CATEGORIES_CURRENT | CATEGORYID<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>PORTFOLIO_CURRENT | PORTFOLIOID-<br></td>
    </tr>
    <tr>
        <td>Projekt</td>
        <td>Projekt</td>
        <td>PROJ | Projekt</td>
        <td>PROJECTS_CURRENT<br>PROJECTS_DAILY_HISTORY<br>PROJECTS_EVENT<br>PROJECTS_CUSTOM_VALUE_CURRENT<br>PROJECTS_CUSTOM_VALUE_DAILY_HISTORY<br>PROJECTS_CUSTOM_VALUE_EVENT</td>
        <td>AEMNATIVEFOLDERTREESREFID<br>ALIGNMENTSCORECARDID<br>APPROVALPROCESSID<br>ATTACHEDRATECARDID<br>CATEGORYID<br>COMPANYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>DELIVERABLESCORECARDID<br>ENTEREDBYID<br>GROUPID<br>LASTCONDITIONNOTEID<br>LASTASTASTASTASTASTASTASTASTASTASTE TEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID<br>OWNERID<br>POPACCOUNTID<br>PORTFOLIOID<br>PRIVATERATECARDID<br>PROGRAMID<br>PROJECTID<br>QUEUEDEFIED<br>ID<br>REJECTIONISSUID<br>RECOURCEPOID<br>SCHEDULEID<br>SPONSORID<br>SUBTEDBYIDEDED<br>TEAMID</td>
        <td>Keine Workfront-Beziehung; wird für die Integration in externe Systeme verwendet<br>Scorecard-Tabelle wird derzeit nicht unterstützt<br>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>RATECARD_CURRENT | RATECARDID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | Die Tabelle APPROVALSTEPID<br>Scorecard wird derzeit nicht unterstützt<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID<br>USER_CURRENT | Die Kontotabelle USERID<br>POP wird derzeit nicht unterstützt<br>PORTFOLIO_CURRENT | PORTFOLIOID<br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | Die <br> PROGRAMID<br>Self-Queue Definition wird derzeit nicht unterstützt<br>OPTASK_CURRENT | OPTASKID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>SCHEDULE_CURRENT | SCHEDULEID<br>USER_CURRENT | USERID<br>USER_CURRENT | USERID<br>TEAM_CURRENT | TEAMID<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Tarifkarte</td>
        <td>Tarifkarte</td>
        <td>RTCRD |Tarifkarte</td>
        <td>RATECARD_CURRENT<br>RATECARD_DAILY_HISTORY_<br>_EVENT</td>
        <td>CATEGORYID<br>ENTEREDBYID<br>LASTUPDATEDBYID <br>RATECARDID (SELF) <br>SECURITYROOTID <br>SOURCEID<br>SYSID</td>
        <td>CATEGORYID<br>USERS_CURRENT | USERID <br>USERS_CURRENT | BENUTZER-ID    <br>Self<br>Die ID des im Feld SECURITYOBJCODE identifizierten Objekts <br>Die ID des im Feld SOURCEOBJCODE identifizierten Objekts<br>Keine Beziehung; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Berichtordner</td>
        <td>Berichtordner</td>
        <td>RPTFDR | Berichtsordner</td>
        <td>REPORTFOLDERS_CURRENT<br>REPORTFOLDERS_DAILY_HISTORY_<br>_EVENT</td>
        <td>REPORTFOLDERID (self) <br>SYSID  </td>
        <td>Self <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Reservierte Zeit</td>
        <td>(Privat) Ausfallzeit</td>
        <td>RESVT | Ausfallzeit</td>
        <td>RESERVEDTIMES_CURRENT<br>RESERVEDTIMES_DAILY_HISTORY<br>RESERVEDTIMES_EVENT</td>
        <td>RESERVEDTIMEID (self) <br>SYSID<br>TASKID<br>USERID  </td>
        <td>Self<br>Not a relation; für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | TASKID<br>USERS_CURRENT | BENUTZER-ID  </td>
    </tr>
    <tr>
        <td>Ressourcen-Pool</td>
        <td>Ressourcen-Pool</td>
        <td>RSPL | Ressourcenpool</td>
        <td>RSRCPOOLS_CURRENT<br>RSRCPOOLS_DAILY_HISTORY<br>RSRCPOOLS_EVENT</td>
        <td>ENTEREDBYID<br>LASTUPDATEDBYID <br>RESOURCEPOOLID (self)<br>SYSID  </td>
        <td>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Rich-Text-Notiz</td>
        <td>Rich-Text-Notiz</td>
        <td>RHNOTE | Rich-Text-Notiz</td>
        <td>RESERVEDTEXTNOTES_CURRENT<br>RESERVEDTEXTNOTES_DAILY_HISTORY<br>RESERVEDTEXTNOTES_EVENT</td>
        <td>RICHTEXTNOTEID (self) <br>SYSID  </td>
        <td>Self <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Rich-Text-Parameterwert</td>
        <td>Rich-Text-Parameterwert</td>
        <td>ARCHVAL | RichTextParameterValue</td>
        <td>RICHTEXTPARAMETERVALUES_CURRENT<br>RICHTEXTPARAMETERVALUES_DAILY_HISTORY<br>RICHTEXTPARAMETERVALUES_EVENT</td>
        <td>PARAMETERVALUEID<br>RICHTEXTPARAMETERVALUEID (SELBST) <br>SYSID  </td>
        <td>Parameterwerttabelle wird derzeit nicht unterstützt<br>Selbst <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet  </td>
    </tr>
    <tr>
        <td>Risiko</td>
        <td>Risiko</td>
        <td>RISIKO | Risiko</td>
        <td>RISKS_CURRENT<br>RISKS_DAILY_HISTORY<br>RISKS_EVENT</td>
        <td>ENTEREDBYID<br>EXCHANGERATEID<br>LASTUPDATEDBYID <br>PROJECTID <br>RISKID (SELF)<br>RISKTYPEID<br>SYSID<br>TEMPLATEID</td>
        <td>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>USERS_CURRENT | USERID <br>PROJECTS_CURRENT | PROJEKT-ID   <br>SELF<br>RISKTYPES_CURRENT | RISKTYPEID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TEMPLATES_CURRENT | TEMPLATEID</td>
    </tr>
    <tr>
        <td>Risikotyp</td>
        <td>Risikotyp</td>
        <td>RSKTYP | Risikotyp</td>
        <td>RISKTYPES_CURRENT<br>RISKTYPES_DAILY_HISTORY<br>RISKTYPES_EVENT</td>
        <td>RISKTYPEID<br>SYSID</td>
        <td>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Funktion</td>
        <td>Aufgabengebiet</td>
        <td>ROLLE | Aufgabengebiet</td>
        <td>ROLES_CURRENT<br>ROLES_DAILY_HISTORY<br>ROLES_EVENT</td>
        <td>ENTEREDBYID<br>LAYOUTTEMPLATEID<br>PRIVATERATECARDID<br>ROLEID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>Layout-Vorlagentabelle wird nicht unterstützt<br>RATECARD_CURRENT | RATECARDID<br>SELF<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Zeitplan</td>
        <td>Zeitplan</td>
        <td>SCHEDEN | Zeitplan</td>
        <td>SCHEDULES_CURRENT<br>SCHEDULES_DAILY_HISTORY<br>SCHEDULES_EVENT</td>
        <td>ENTEREDBYID.<br>.<br>.HOMEGROUPID<br>SCHEDULEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>GROUP_CURRENT | GROUPID<br>Self</td>
    </tr>
    <tr>
        <td>Genehmigende Person für Schritt</td>
        <td>Genehmigende Person für Schritt</td>
        <td>SPAPER | Genehmigende Person für Phase</td>
        <td>STEPAPPROVERS_CURRENT<br>STEPAPPROVERS_DAILY_HISTORY<br>STEPAPPROVERS_EVENT</td>
        <td>APPROVALSTEPID<br>ROLEID<br>STEPAPPROVERID (self)<br>SYSID <br>TEAMID<br>USERID</td>
        <td>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>ROLES_CURRENT | ROLEID<br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet <br>TEAMS_CURRENT | TEAMID<br>USERS_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>Aufgabe</td>
        <td>Aufgabe</td>
        <td>AUFGABE | Aufgabe</td>
        <td>TASKS_CURRENT<br>TASKS_DAILY_HISTORY<br>TASKS_EVENT<br>TASKS_CUSTOM_VALUE_CURRENT<br>TASKS_CUSTOM_VALUE_DAILY_HISTORY<br>TASKS_CUSTOM_VALUE_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>BILLINGRECORDID<br>CATEGORYID<br>CONVERTEDOPTASKID<br>CONVERTEDOPTASKORIGINATORID<br>CURRENTAPPROVALSTEPID<br>ENTEREDBYID<br>EXCHANGERATEID<br>GROUPID<br>ITERATIONID<br>KANBANBOARDID<br>LASTCONDITIONNOTEID<br>LASTNOTEID<br>LASTUPDATEDBYID <br>MILESTONEID<br>PARENTID<br>PROJECTID<br>RECURRENCERULEID<br>REJECTIONISSUEID<br>RESERVEDTIMED<br><br> <br> <br> <br> SUBMITTEDBYIDTASKID</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USER_CURRENT | USERID<br>BILLINGRECORDS_CURRENT | BILLINGRECORDID<br>CATEGORIES_CURRENT | CATEGORYID<br>OPTASK_CURRENT | OPTASKID<br>USER_CURRENT | USERID<br>APPROVALSTEPS_CURRENT | APPROVALSTEPID<br>USER_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>GROUP_CURRENT | GROUPID<br>ITERATIONS_CURRENT | ITERATIONID<br>Kanban-Board-Tabelle wird derzeit nicht unterstützt<br>NOTE_CURRENT | NOTEID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TASK_CURRENT | TASKID<br>PROJECT_CURRENT | PROJECTID<br>Recurrence-Regeltabelle wird derzeit nicht unterstützt<br>OPTASK_CURRENT | OPTASKID<br>RESERVEDTIMES_CURRENT | RESERVEDTIMEID<br>ROLE_CURRENT | ROLEID<br>USER_CURRENT | USERID<br>SELF<br>TEAM_CURRENT | TEAMID<br>TEMPLATETASKS_CURRENT | TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Vorgänger der Aufgabe</td>
        <td>Vorgänger</td>
        <td>PRED | Vorgänger</td>
        <td>PREDECESSORS_CURRENT<br>PREDECESSORS_DAILY_HISTORY<br>PREDECESSORS_EVENT</td>
        <td>ID (self)<br>PREDECESSORID<br>SUCCESSORID <br>SYSID</td>
        <td>SELF<br>TASKS_CURRENT | TASKID<br>TASKS_CURRENT | TASKID <br>Keine Beziehung; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Team</td>
        <td>Team</td>
        <td>MANNSCHAFT | Team</td>
        <td>TEAMS_CURRENT<br>TEAMS_DAILY_HISTORY<br>TEAMS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID<br>LAYOUTTEMPLATEID<br>MYWORKVIEWID<br>OWNERID<br>REQUESTSVIEWID<br>SCHEDULEID<br>TEAMID<br>UITEMPLATEID</td>
        <td>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>Layout-Vorlagentabelle wird nicht unterstützt<br>UIVIEWS_CURRENT | UIVIEWID<br>USER_CURRENT | USERID<br>UIVIEWS_CURRENT | UIVIEWID<br>SCHEDULE_CURRENT | SCHEDULEID<br>SELF<br>UITEMPLATES_CURRENT |UITEMPLATEID</td>
    </tr>
    <tr>
        <td>Teammitglied</td>
        <td>Andere Teams, Teammitglied</td>
        <td>TEAM | Teammitglied</td>
        <td>TEAMMEMBERS_CURRENT<br>TEAMMEMBERS_DAILY_HISTORY<br>TEAMMEMBERS_EVENT</td>
        <td>SYSID <br>TEAMID<br>TEAMMEMBERID (self)<br>USERID</td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet <br>TEAMS_CURRENT | TEAMID<br>SELF<br>USERS_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>TeamMemberRole</td>
        <td>Teammitglied-Funktion</td>
        <td>TEAM | Teammitglied-Funktion</td>
        <td>TEAMMEMBERROLES_CURRENT<br>TEAMMEMBERROLES_DAILY_HISTORY<br>TEAMMEMBERROLES_EVENT</td>
        <td>ROLEID <br>TEAMID<br>TEAMMEMBERROLEID (self)<br>USERID</td>
        <td>ROLES_CURRENT | ROLEID <br>TEAMS_CURRENT | TEAMID<br>SELF<br>USERS_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>Vorlage</td>
        <td>Vorlage</td>
        <td>TMPL | Vorlage</td>
        <td>TEMPLATES_CURRENT<br>TEMPLATES_DAILY_HISTORY<br>TEMPLATES_EVENT</td>
        <td>APPROVALPROCESSID<br>CATEGORYID<br>COMPANYID <br>DELIVERABLESCORECARDID <br>ENTEREDBYID<br>GROUPID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEPATHID <br>OWNERID <br>PRIVATERATECARDID<br>PROGRAMID<br>QUEUEDEFID<br>SCHEDULEID <br>SYSID <br>TEAMID<br>TEMPLATEID (Self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID   <br>DELIVERABLESCORECARDID <br>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONEPATH_CURRENT | MILESTONEPATHID <br>USERS_CURRENT | USERID <br>RATECARD_CURRENT | RATECARDID<br>PROGRAM_CURRENT | Tabelle <br>PROGRAMID-Queue-Definition“ wird derzeit nicht unterstützt<br>SCHEDULES_CURRENT | SCHEDULEID <br>Keine Beziehung; für interne Anwendungszwecke verwendet <br>TEAMS_CURRENT | TEAMID<br>Self</td>
    </tr>
    <tr>
        <td>Vorlagenzuweisung</td>
        <td>Vorlagenzuweisung</td>
        <td>TAG-TAG | Vorlagenzuweisung</td>
        <td>TEMPLATEASSIGNMENTS_CURRENT<br>TEMPLATEASSIGNMENTS_DAILY_HISTORY<br>TEMPLATEASSIGNMENTS_EVENT</td>
        <td>ASSIGNEDTOID<br>CATEGORYID<br>LASTUPDATEDBYID<br>OBJID<br>ROLEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEASSIGNMENTID (SELF)<br>TEMPLATETASKID</td>
        <td>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>Die ID des im OBJCODE-Feld identifizierten Objekts <br>ROLES_CURRENT | ROLEID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TEAMS_CURRENT | TEAMID<br>Team Timelineable-Tabelle wird derzeit nicht unterstützt<br>Self<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID</td>
    </tr>
    <tr>
        <td>Vorlagenaufgabe</td>
        <td>Vorlagenaufgabe</td>
        <td>TTSK | Vorlagenaufgabe</td>
        <td>TEMPLATETASKS_CURRENT<br>TEMPLATETASKS_DAILY_HISTORY<br>TEMPLATETASKS_EVENT</td>
        <td>APPROVALPROCESSID<br>ASSIGNEDTOID<br>CATEGORYID<br>ENTEREDBYID<br>EXCHANGERATEID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>MILESTONEID<br>PARENTID<br><br> RECURRENCERULEID<br>SYSID<br>TEAMID<br>TEAMTIMELINEABLEID<br>TEMPLATEID<br>TEMPLATETASKID (Self)</td>
        <td>APPROVALPROCESSES_CURRENT | APPROVALPROCESSID<br>USERS_CURRENT | USERID<br>CATEGORIES_CURRENT | CATEGORYID<br>USERS_CURRENT | USERID<br>EXCHANGERATES_CURRENT | EXCHANGERATEID<br>NOTES_CURRENT | NOTEID<br>USERS_CURRENT | USERID<br>MILESTONE_CURRENT | MILESTONEID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID_<br>-Regeltabelle wird derzeit nicht unterstützt<br>ROLES_CURRENT | ROLEID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TEAMS_CURRENT | TEAMID<br>Team Timelineable-Tabelle wird derzeit nicht unterstützt<br>TEMPLATES_CURRENT | TEMPLATEID<br>Self</td>
    </tr>
    <tr>
        <td>Vorlagenaufgabe - Vorgänger</td>
        <td>Vorgängervorlage</td>
        <td>TPRED | Vorgänger</td>
        <td>TEMPLATEPREDECESSORS_CURRENT<br>TEMPLATEPREDECESSORS_DAILY_HISTORY<br>TEMPLATEPREDECESSORS_EVENT</td>
        <td>PREDECESSORID<br>SUCCESSORID <br>TEMPLATEPREDECESSORID (SELF)<br>SYSID</td>
        <td>TEMPLATETASKS_CURRENT |TEMPLATETASKID<br>TEMPLATETASKS_CURRENT |TEMPLATETASKID <br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Arbeitszeittabelle</td>
        <td>Arbeitszeittabelle</td>
        <td>TSHET | Arbeitszeittabelle</td>
        <td>TIMESHEETS_CURRENT<br>TIMESHEETS_DAILY_HISTORY<br>TIMESHEETS_EVENT</td>
        <td>APPROVERID<br>LASTNOTEID<br>LASTUPDATEDBYID<br>TIMESHEETID<br>TIMESHEETPROFILEID<br>USERID</td>
        <td>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>SELF<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>USER_CURRENT | BENUTZER-ID</td>
    </tr>
    <tr>
        <td>Arbeitszeittabellen-Profil</td>
        <td>Arbeitszeittabellen-Profil</td>
        <td>TSPRO | Arbeitszeittabellen-Profil</td>
        <td>TIMESHEETPROFILES_CURRENT<br>TIMESHEETPROFILES_DAILY_HISTORY<br>TIMESHEETPROFILES_EVENT</td>
        <td>APPROVERID<br>ENTEREDBYID <br>GROUPID<br>SYSID<br>TIMESHEETPROFILEID (SELF)</td>
        <td>USERS_CURRENT | USERID<br>USERS_CURRENT | USERID <br>GROUPS_CURRENT | GROUPID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>Selbst</td>
    </tr>
    <tr>
        <td>UI-Filter</td>
        <td>Filter</td>
        <td>VERSCHIEBEN | Filter</td>
        <td>UIFILTERS_CURRENT<br>UIFILTERS_DAILY_HISTORY_<br>_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIFILTERID (SELF)</td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Die ID des im OBJCODE-Feld identifizierten Objekts<br>PREFERENCES_CURRENT | PREFERENCEID<br>Keine Beziehung; für interne Anwendungszwecke verwendet <br>Selbst</td>
    </tr>
    <tr>
        <td>Benutzeroberfläche gruppieren nach</td>
        <td>Gruppierung</td>
        <td>UIGB | Gruppierung</td>
        <td>UIGROUPBYS_CURRENT<br>UIGROUPBYS_DAILY_HISTORY<br>UIGROUPBYS_EVENT</td>
        <td>ENTEREDBYID<br>GROUPID <br>LASTUPDATEDBYID <br>SYSID <br>UITEMPLATEID (self)</td>
        <td>USERS_CURRENT | USERID<br>GROUPS_CURRENT | GROUPID <br>USERS_CURRENT | USERID <br>Keine Beziehung; für interne Anwendungszwecke verwendet <br>Selbst</td>
    </tr>
    <tr>
        <td>UI-Vorlage</td>
        <td>Layoutvorlage</td>
        <td>UTIMPL | Layoutvorlage</td>
        <td>UITEMPLATES_CURRENT<br>UITEMPLATES_DAILY_HISTORY<br>UITEMPLATES_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIGROUPBYID (SELF)</td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Die ID des im OBJCODE-Feld identifizierten Objekts<br>PREFERENCES_CURRENT | PREFERENCEID<br>Keine Beziehung; für interne Anwendungszwecke verwendet <br>Selbst</td>
    </tr>
    <tr>
        <td>UI-Ansicht</td>
        <td>Anzeigen</td>
        <td>UIVIEW | anzeigen</td>
        <td>UIVIEWS_CURRENT<br>UIVIEWS_DAILY_HISTORY<br>UIVIEWS_EVENT</td>
        <td>APPGLOBALID<br>ENTEREDBYID <br>LASTUPDATEDBYID <br>OBJID<br>PREFERENCEID<br>SYSID <br>UIVIEWID (SELF)</td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | USERID <br>USERS_CURRENT | USERID <br>Die ID des im OBJCODE-Feld identifizierten Objekts<br>PREFERENCES_CURRENT | PREFERENCEID<br>Keine Beziehung; für interne Anwendungszwecke verwendet <br>Selbst</td>
    </tr>
    <tr>
        <td>Benutzerin oder Benutzer</td>
        <td>Benutzerin oder Benutzer</td>
        <td>BENUTZER | Benutzer</td>
        <td>USERS_CURRENT<br>USERS_DAILY_HISTORY<br>USERS_EVENT<br>USERS_CUSTOM_VALUE_CURRENT<br>USERS_CUSTOM_VALUE_DAILY_HISTORY<br>USERS_CUSTOM_VALUE_EVENT</td>
        <td>ACCESSLEVELID<br>CATEGORYID<br>COMPANYID<br>DEFAULTHOURTYPEID<br>DELEGATIONTOID<br>EAUTHUSERID<br>ENTEREDBYID<br>HOMEGROUPID<br>HOMETEAMID<br>LASTENTEREDNOTEID<br>LASTUPDATEDBYID<br>LATESTUPDATENOTEID<br>LAYOUTTEMPLATEID<br>MANAGERID<br>PORTALPROFILEID<br> D<br>PRIVATERATECARDID<br>RESOURCEPOOLID<br>ROLEID<br>SCHEDULEID<br>TIMESHEETPROFILEID<br>UUMUSERID<br> <br></td>
        <td>ACCESSLEVELS_CURRENT |ACCESSLEVELID<br>CATEGORIES_CURRENT | CATEGORYID<br>COMPANIES_CURRENT | COMPANYID <br>HOURTYPE_CURRENT | HOURTYPEID<br>USER_CURRENT | USERID<br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USER_CURRENT | USERID<br>GROUP_CURRENT | GROUPID<br>TEAM_CURRENT | TEAMID<br>NOTE_CURRENT | NOTEID<br>USER_CURRENT | USERID<br>NOTE_CURRENT | NOTEID<br>Layout-Vorlagentabelle wird nicht unterstützt<br>USER_CURRENT | Die <br> USERID-Portal wird nicht unterstützt<br>keine Beziehung; wird für interne Anwendungszwecke verwendet<br>RATECARD_CURRENT | RATECARDID<br>RESOURCEPOOLS_CURRENT | RESOURCEPOOLID<br>ROLE_CURRENT | ROLEID<br>SCHEDULE_CURRENT | SCHEDULEID<br>TIMESHEETPROFILES_CURRENT | TIMESHEETPROFILEID<br>UITEMPLATES_CURRENT |UITEMPLATEID<br>Self<br>Not a relation; wird für interne Anwendungszwecke verwendet</td>
    </tr>
    <tr>
        <td>Benutzerdelegierung</td>
        <td>Benutzerdelegierung</td>
        <td>USRDEL | Benutzerdelegierung</td>
        <td>USERDELEGATIONS_CURRENT<br>USERDELEGATIONS_DAILY_HISTORY<br>USERDELEGATIONS_EVENT</td>
        <td>FROMUSERID<br>SYSID <br>TOUSERID <br>USERDELEGATIONID (self)</td>
        <td>USERS_CURRENT | USERID<br>Keine Beziehung; für interne Anwendungszwecke verwendet <br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Benutzergruppe</td>
        <td>Andere Gruppen</td>
        <td>USRGPS | Benutzergruppe</td>
        <td>USERSGROUPS_CURRENT<br>USERSGROUPS_DAILY_HISTORY<br>USERSGROUPS_EVENT</td>
        <td>GROUPID <br>SYSID<br>USERID <br>USERSGROUPID (self)</td>
        <td>GROUPS_CURRENT | GROUPID <br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Benutzerfunktion</td>
        <td>Weitere Funktionen</td>
        <td>USRROL | Benutzerrolle</td>
        <td>USERSROLES_CURRENT<br>USERSROLES_DAILY_HISTORY<br>USERSROLES_EVENT</td>
        <td>ROLEID <br>SYSID<br>USERID    <br>USERROLESETID<br>USERSROLEID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | BENUTZER-ID    <br>USERROLESET_CURRENT | USERROLESETID<br>SELF</td>
    </tr>
    <tr>
        <td>UserPrefValue</td>
        <td>UserPrefValue</td>
        <td>USERPF | Benutzerpräferenz</td>
        <td>USERPREFVALUES_CURRENT<br>USERPREFVALUES_DAILY_HISTORY_<br>_EVENT</td>
        <td>SYSID    <br>USERID <br>USERPREFVALUEID (self)</td>
        <td>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | BENUTZER-ID    <br>Selbst</td>
    </tr>
    <tr>
        <td>UserRoleSet</td>
        <td>UserRoleSet</td>
        <td>MISSBRAUCH | UserRoleSet</td>
        <td>USERROLESET_CURRENT<br>USERROLESET_DAILY_HISTORY<br>USERROLESET_EVENT</td>
        <td>PRIMARYROLEID <br>SYSID<br>USERID    <br>USERROLESETID (self)</td>
        <td>ROLES_CURRENT | ROLEID <br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>USERS_CURRENT | USERID <br>Self</td>
    </tr>
    <tr>
        <td>Benutzerentscheidungen</td>
        <td>Benutzerentscheidungen</td>
        <td>USRDEC | Benutzerentscheidungen</td>
        <td>USERSDECISIONS_CURRENT<br>USERSDECISIONS_DAILY_HISTORY<br>USERSDECISIONS_EVENT</td>
        <td>USERDECISIONID (self)<br>SYSID <br>USERID  </td>
        <td>Self<br>Not a relation; für interne Anwendungszwecke verwendet <br>USERS_CURRENT | BENUTZER-ID </td>
    </tr>
    <tr>
        <td>Arbeitselement</td>
        <td>Arbeitselement</td>
        <td>WORKITM | Arbeitselement</td>
        <td>WORKITEMS_CURRENT_<br>_DAILY_HISTORY<br>WORKITEMS_EVENT</td>
        <td>ASSIGNMENTID <br>OBJID<br>OPTASKID    <br>PROJECTID <br>SYSID<br>TASKID    <br>USERID <br>WORKITEMID (self)</td>
        <td>ASSIGNMENTS_CURRENT | ASSIGNMENTID <br>Die ID des im OBJOBJCODE-Feld identifizierten Objekts<br>OPTASK_CURRENT | OPTASKID    <br>PROJECTS_CURRENT | PROJECTID <br>Keine Beziehung; für interne Anwendungszwecke verwendet<br>TASKS_CURRENT | AUFGABEN-ID    <br>USERS_CURRENT | BENUTZER-ID    <br>Selbst </td>
    </tr>
  </tbody>
</table>
