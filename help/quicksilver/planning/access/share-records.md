---
title: Freigeben von Datensätzen
description: Sie können Datensätze mithilfe der Schaltfläche Freigeben freigeben, um die Zusammenarbeit bei der Adobe Workfront-Planung zu verbessern.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 0964ad24535bf43a23c740cd63abcf8fea705b8d
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 3%

---


<!--update metadata with real information at release-->

# Freigeben von Datensätzen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Sie können die Berechtigungen von Personen für einzelne Datensätze in einem Datensatztyp anpassen. O

Sie können einen Adobe Workfront Planning-Datensatz wie folgt freigeben:

* Freigeben eines Links zum Datensatz.

  Weitere Informationen finden Sie unter [Freigeben von Datensätzen über einen Link](/help/quicksilver/planning/records/share-records.md).

* Geben Sie alle Datensätze in einem Arbeitsbereich für andere Benutzer frei, indem Sie den Arbeitsbereich und den Datensatztyp freigeben.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md)

   * [Datensatztyp freigeben](/help/quicksilver/planning/access/share-record-types.md)

* Freigeben eines Datensatzes mithilfe der Option **Freigeben**.

  In diesem Artikel wird beschrieben, wie Sie einen Datensatz mit der Option **Freigeben** freigeben können.

>[!IMPORTANT]
>
>Benutzende mit Zugriff auf einen Arbeitsbereich erhalten automatisch mindestens die Berechtigung Anzeigen für alle Datensätze im Arbeitsbereich.
>Bei der Freigabe von Ansichten erhalten Benutzende keine Berechtigungen für Datensätze. Nur freigegebene Arbeitsbereiche können Benutzern Berechtigungen für Datensatztypen und Datensätze gewähren.
>
>Allgemeine Informationen zum Freigeben von Objekten in Workfront Planning finden Sie auch unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront- und Planungspaket</p> 
Oder
<p>Beliebiges Workflow- und Planungspaket</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Beliebig</p> 
   <p><b>NOTIZ</b></p>
   <p>Nur Personen mit einer Standardlizenz können Berechtigungen zum Verwalten von Datensätzen erhalten. Alle anderen Lizenzen können nur über Anzeigeberechtigungen verfügen und die Option Verwalten ist für sie abgeblendet.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  <p>Verwalten von Berechtigungen für einen Arbeitsbereich, einen Datensatztyp und den Datensatz</p>  
   <p><b>WICHTIG</b></p>
   <p>Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können einen Datensatz freigeben</p></td> 
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> Benutzenden mit einer Light- oder Contributor-Lizenz muss eine Layout-Vorlage zugewiesen werden, die Planning enthält.
   <p>Für Standardbenutzer und Systemadministratoren sind die Planungsbereiche standardmäßig aktiviert.</p></div></li></ul>

</td>
  </tr>

</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe von Datensätzen

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

* Sie können Datensätze für die folgenden Entitäten freigeben: Personen, Gruppen, Teams, Unternehmen oder Aufgabengebiete.
* Wenn Sie einen Arbeitsbereich für Benutzende freigeben, erhalten diese standardmäßig dieselben Berechtigungen für die Datensätze im Arbeitsbereich.
* Wenn Sie eine Entität aus einem Arbeitsbereich entfernen, werden alle Freigabeberechtigungen aus den Datensatztypen und allen darin enthaltenen Datensätzen entfernt.
* Der Zugriff eines Benutzers auf den Datensatz wird durch die Kombination der folgenden drei Einstellungen bestimmt:

   * Berechtigungen, die vom Datensatztyp und Arbeitsbereich übernommen wurden
   * Im Dialogfeld zur Datensatzfreigabe individuell hinzugefügte Berechtigungen
   * Die folgenden Berechtigungen:

      * **Jeder Benutzer im Arbeitsbereich kann Folgendes anzeigen**: Dadurch kann der Datensatz für alle Benutzer im Arbeitsbereich-<!-- is this OK to say "workspace? should it be "record"??--> angezeigt werden
      * **Nur eingeladene Personen können zugreifen**: Dies ist standardmäßig ausgewählt und ermöglicht die Einschränkung des Zugriffs auf den Datensatz auf bestimmte Personen.

* Sie können einem Datensatz die folgenden Berechtigungsebenen gewähren:

   * Ansicht
   * Verwalten

* Wenn Sie einen Datensatz für einen Benutzer freigeben, werden diese standardmäßig mit derselben Berechtigung hinzugefügt, die sie für den Datensatztyp haben.

  Beispiel:

   * Wenn sie über Anzeigeberechtigungen für den Datensatztyp verfügen, erhalten sie Anzeigeberechtigungen für den Datensatz
   * Wenn sie die Berechtigungen Beitragen oder Verwalten für den Datensatztyp besitzen, erhalten sie die Berechtigung Verwalten für den Datensatz

* Als Workspace-Manager können Sie einen Datensatz für Benutzende freigeben, die nicht zum Workspace gehören. In diesem Fall wird neben der hinzugefügten Entität eine Warnung angezeigt, die besagt, dass sie keinen Zugriff auf den Arbeitsbereich haben. Sie können akzeptieren, dass Benutzende sowohl zum Datensatz als auch zum Arbeitsbereich hinzugefügt werden, oder ablehnen, dass sie zum Arbeitsbereich hinzugefügt werden, wodurch sie auch aus dem Datensatz entfernt werden.

* Wenn Sie einen Datensatz für Benutzende freigeben, die über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, erhalten diese standardmäßig auch Verwaltungsberechtigungen für den Datensatz. Die Berechtigung zum Anzeigen ist abgeblendet.

* Wenn Sie nicht über die Berechtigung zum Hinzufügen von Personen zum Arbeitsbereich verfügen, sehen und fügen Sie nur Benutzer, Teams, Gruppen, Rollen und Unternehmen hinzu, die bereits zum Arbeitsbereich hinzugefügt wurden. Sie können keine anderen Entitäten hinzufügen, die noch nicht Teil des Arbeitsbereichs sind.

* Sie können geerbte Berechtigungen für einen einzelnen Datensatz deaktivieren. In diesem Fall können Sie ihnen Berechtigungen einzeln erteilen. Wenn sie zur Option „Alle im Arbeitsbereich“ gehören, können sie Berechtigungen erlangen. <!-- is this OK to say "workspace? should it be "record"??-->

* Wenn für denselben Benutzer mehrere Freigabeberechtigungen gelten, erhalten diese die höchste Berechtigung dieser Berechtigungen.

  Wenn beispielsweise ein Datensatz für einen Benutzer mit Ansichtsberechtigungen und dessen Gruppe mit Verwaltungszugriff freigegeben wird, erhält dieser Benutzer Verwaltungsberechtigungen für den Datensatz.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Wenn ein Formelfeld oder ein Nachschlagefeld aus einem verbundenen Datensatz auf einem Feld für einen Datensatz basiert, für den Sie keine Berechtigungen haben, wird die richtige Berechnung angezeigt, auf welche Faktoren im Datensatz Sie sonst nicht zugreifen können.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Datensatzberechtigungen freigeben

