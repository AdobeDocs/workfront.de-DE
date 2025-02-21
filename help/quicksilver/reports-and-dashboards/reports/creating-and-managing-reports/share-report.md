---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Freigeben eines Berichts in Adobe Workfront
description: Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff zum Anzeigen oder Bearbeiten von Berichten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Probleme finden Sie unter Gewähren des Zugriffs auf Berichte, Dashboards und Kalender.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '823'
ht-degree: 0%

---

# Freigeben eines Berichts in Adobe Workfront

<!-- Audited: 11/2024 -->

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff zum Anzeigen oder Bearbeiten von Berichten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Probleme finden Sie unter [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Berichte erteilen, auf die Sie Zugriff haben. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Funktionsweise von Zugriffsebenen und Berechtigungen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Berechtigungen sind für ein Element in Workfront spezifisch und definieren, welche Aktionen man für dieses Element ausführen kann.

>[!NOTE]
>
>Ein Workfront-Administrator kann für alle Benutzenden Berechtigungen zu Elementen im System hinzufügen oder entfernen, ohne Besitzer dieser Elemente zu sein.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
      <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Licht oder höher</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Überprüfen oder höher</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Anzeigen des Zugriffs auf Berichte, Dashboards, Kalender oder höher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen oder höher im Bericht</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe von Berichten

Zusätzlich zu den unten stehenden Überlegungen finden Sie weitere Informationen unter [Freigeben von Berichten, Dashboards und Kalendern](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Sie können von Ihnen erstellte Berichte für andere Personen, Teams, Gruppen, Aufgabengebiete oder Unternehmen freigeben. Sie können auch von anderen erstellte Berichte, die für Sie freigegeben wurden, freigeben.
* Sie können sie auch für Ihr gesamtes Unternehmen freigeben oder veröffentlichen. Wenn Sie einen Bericht veröffentlichen, wird eine URL generiert, die für andere freigegeben werden kann.
* Sie können einen einzelnen Bericht freigeben oder mehrere Berichte aus einer Berichtsliste freigeben.

## Möglichkeiten zum Freigeben von Berichten

Sie können Berichte in Workfront wie folgt freigeben:

* Manuell, wie im Abschnitt [Freigeben eines Berichts](#share-a-report) unten beschrieben.
* Automatisch durch Vererbung der Ansichtsberechtigungen von einem Dashboard, das den freigegebenen Bericht enthält. Weitere Informationen zum Anzeigen geerbter Berechtigungen für Objekte finden Sie unter [Anzeigen geerbter Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Freigeben eines Berichts {#share-a-report}

Die Freigabe eines Berichts oder mehrerer Berichte aus einer Liste ist identisch.

1. Gehen Sie zu einer Liste von Berichten und wählen Sie einen oder mehrere Berichte aus und klicken Sie dann auf **Freigeben**.

   Oder

   Klicken Sie auf den Namen eines Berichts und dann auf **Berichtsaktionen >****Freigabe**.

   ![](assets/unshimmed-report-actions-sharing.png)

1. Geben Sie im angezeigten Feld im Feld **Personen, Teams, Rollen, Gruppen oder Firmen hinzufügen…** den Namen des Benutzers, Teams, Aufgabengebiets, der Gruppe oder des Unternehmens ein, für den bzw. das Sie den Bericht freigeben möchten, und drücken Sie dann die **Eingabetaste** wenn der Name angezeigt wird.

1. Um die Zugriffsebene für einen hinzugefügten Namen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und wählen Sie dann eine der folgenden Optionen aus.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Ermöglicht es dem Empfänger, den Bericht im Bereich <strong>Berichte</strong> anzuzeigen und auszuführen.</p> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> klicken, um anzugeben, ob die Benutzerin bzw. der Benutzer sie für </strong> im System <strong>freigeben“ kann.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Ermöglicht dem Empfänger vollen Bearbeitungszugriff auf den Bericht.</p> <p>Sie können auf <strong>Erweiterte Einstellungen</strong> klicken, um anzugeben, ob der/die Benutzende den Bericht aus dem System <strong>löschen</strong> und für </strong> im System <strong>freigeben können soll.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die beiden vorherigen Schritte, um weitere Namen zur Liste hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Klicken Sie auf das **Nur eingeladene Personen können zugreifen** Dropdown-Menü im Freigabefeld und wählen Sie dann eine der folgenden Optionen:

   * **Nur eingeladene Personen können darauf zugreifen** Wählen Sie diese Option aus, damit nur Benutzer, denen Zugriff auf den Bericht gewährt wurde, ihn anzeigen können.

   * **Alle im System können anzeigen** Wählen Sie diese Option aus, damit jeder in Workfront mit Zugriff auf Berichte den Bericht anzeigen kann.

1. (Optional) Klicken Sie auf **Zahnrad**-Symbol ![Zahnradsymbol-Einstellungen](assets/gear-icon-settings-with-dn-arrow.jpg) in der oberen rechten Ecke des Freigabefelds und wählen Sie dann optional die folgende Option:

   * **Für externe Benutzer veröffentlichen: Wählen** diese Option aus, um eine URL zu generieren, die für andere freigegeben werden kann. Jeder Benutzer mit der URL kann auf den Bericht zugreifen, ohne über eine Adobe Workfront-Lizenz zu verfügen.

     >[!CAUTION]
     >
     >Es wird empfohlen, bei der Freigabe eines Objekts mit vertraulichen Informationen an externe Benutzer Vorsicht walten zu lassen. Auf diese Weise können sie Informationen anzeigen, ohne ein Workfront-Benutzer oder Teil Ihres Unternehmens zu sein.

     >[!NOTE]
     >
     >Wenn für den Bericht eine Eingabeaufforderung vorhanden ist und Sie ihn öffentlich freigeben, können Benutzende, die den Bericht über den öffentlichen Freigabe-Link ausführen, den Bericht nicht über die Eingabeaufforderung ausführen. Der Bericht wird ohne Eingabeaufforderung angezeigt, es sei denn, der Benutzer meldet sich bei Workfront an und greift auf den Bericht zu, ohne den öffentlichen Freigabe-Link zu verwenden. Weitere Informationen zu den Einschränkungen bei der Freigabe von Berichten mit Eingabeaufforderungen finden Sie im Abschnitt [Einschränkungen bei der Freigabe ](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) Berichten) im Artikel [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf **Speichern**.
