---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Bericht in Adobe Workfront freigeben
description: Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Berichten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zur Gewährung des Zugriffs auf Probleme finden Sie unter Zugriff auf Berichte, Dashboards und Kalender gewähren .
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Bericht in Adobe Workfront freigeben

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Berichten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zur Gewährung des Zugriffs auf Probleme finden Sie unter [Zugriff auf Berichte, Dashboards und Kalender gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Neben der Zugriffsebene, auf die Benutzer zugreifen können, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Berichte erteilen, auf die Sie Zugriff haben. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Wie Zugriffsebenen und Berechtigungen zusammenarbeiten](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Berechtigungen beziehen sich auf ein Element in Workfront und legen fest, welche Aktionen für dieses Element durchgeführt werden können.

>[!NOTE]
>
>Ein Workfront-Administrator kann allen Elementen im System Berechtigungen hinzufügen oder entfernen, ohne Eigentümer dieser Elemente zu sein.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um Objekte freizugeben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender oder höher anzeigen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen oder höher für den Bericht</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zur Freigabe von Berichten

Zusätzlich zu den unten stehenden Überlegungen siehe [Berichte, Dashboards und Kalender freigeben](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Sie können von Ihnen erstellte Berichte für andere Personen, Teams, Gruppen, Rollen oder Unternehmen freigeben. Sie können auch Berichte freigeben, die erstellt und für Sie freigegeben wurden.
* Sie können sie auch für Ihre gesamte Organisation freigeben oder veröffentlichen. Wenn Sie einen Bericht öffentlich machen, wird eine URL generiert, die für andere freigegeben werden kann.
* Sie können einen einzelnen Bericht freigeben oder mehrere Berichte aus einer Liste von Berichten freigeben.

## Möglichkeiten zum Freigeben von Berichten

Sie können Berichte in Workfront wie folgt freigeben:

* Manuell, wie im Abschnitt [Bericht freigeben](#share-a-report) unten.
* automatisch durch Vererben der Anzeigeberechtigungen von einem Dashboard, das den freigegebenen Bericht enthält. Informationen zum Anzeigen von geerbten Berechtigungen für Objekte finden Sie unter [Vererbte Berechtigungen für Objekte anzeigen](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Bericht freigeben {#share-a-report}

Die Freigabe eines oder mehrerer Berichte aus einer Liste ist identisch.

1. Markieren Sie eine Liste von Berichten und wählen Sie einen oder mehrere Berichte aus. Klicken Sie dann auf **Freigeben**.

   Oder

   Klicken Sie auf den Namen eines Berichts und dann auf **Berichtaktionen >****Freigabe**.

   ![](assets/qs-report-actions-sharing.png)

1. Im angezeigten Feld wird im **Hinzufügen von Personen, Teams, Rollen, Gruppen oder Unternehmen ...** ein Feld eingeben, in das Sie den Namen des Benutzers, Teams, der Rolle, der Gruppe oder des Unternehmens eingeben möchten, für den/die Sie den Bericht freigeben möchten, und drücken Sie dann die Eingabetaste **Eingabe** wenn der Name angezeigt wird.

1. Um die Zugriffsebene für einen von Ihnen hinzugefügten Namen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und wählen Sie dann eine der folgenden Optionen aus.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Ermöglicht es Ihrem Empfänger, den Bericht im <strong>Berichte</strong> <img src="assets/reports-in-main-menu.png"> und führen Sie es aus.</p> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> , um anzugeben, ob der Benutzer oder die Benutzer in der Lage sein sollen <strong>Freigeben</strong> mit jedem im System.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Ermöglicht dem Empfänger die vollständige Bearbeitung des Berichts.</p> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> , um anzugeben, ob der Benutzer oder die Benutzer in der Lage sein sollen <strong>Löschen</strong> den Bericht des Systems und <strong>Freigeben</strong> mit jedem im System.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die beiden vorherigen Schritte, um der Liste weitere Namen hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Klicken Sie auf die **Fanggerät** icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) Wählen Sie oben rechts im Freigabefeld eine der folgenden Optionen aus:

   * **Veröffentlichen Sie dies für externe Benutzer:** Wählen Sie diese Option aus, um eine URL zu generieren, die für andere freigegeben werden kann. Jeder mit der URL kann auf den Bericht zugreifen, ohne über eine Adobe Workfront-Lizenz zu verfügen.

      >[!CAUTION]
      >
      >Es wird empfohlen, bei der Freigabe eines Objekts mit vertraulichen Informationen für externe Benutzer Vorsicht walten zu lassen. Dadurch können sie Informationen anzeigen, ohne Workfront-Benutzer oder Teil Ihres Unternehmens zu sein.

      >[!NOTE]
      >
      >Wenn der Bericht eine Eingabeaufforderung enthält und Sie ihn öffentlich freigeben, müssen die Benutzer, die den Bericht ausführen, bei Workfront angemeldet sein, damit der Bericht über die Eingabeaufforderung ausgeführt werden kann. Wenn sie sich nicht bei Workfront anmelden können, wird der Bericht angezeigt, ohne dass eine Eingabeaufforderung darauf angewendet wird. Weitere Informationen zu Einschränkungen bei der Freigabe von Berichten für Eingabeaufforderungen finden Sie im Abschnitt [Einschränkungen bei der Freigabe erforderlicher Berichte](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) im Artikel [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **Machen Sie dies systemweit sichtbar:** Wählen Sie diese Option aus, damit jeder in Workfront mit Zugriff auf Berichte den Bericht sehen kann.

1. Klicken Sie auf **Speichern**.
