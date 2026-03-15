---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Freigeben eines Berichts in Adobe Workfront
description: Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff zum Anzeigen oder Bearbeiten von Berichten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Probleme finden Sie unter Gewähren des Zugriffs auf Berichte, Dashboards und Kalender.
author: Courtney
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 7%

---

# Freigeben eines Berichts in Adobe Workfront

<!-- Audited: 11/2024 -->

Ihr Adobe Workfront-Administrator gewährt Benutzern Zugriff zum Anzeigen oder Bearbeiten von Berichten, wenn sie Zugriffsebenen zuweisen. Weitere Informationen zum Gewähren des Zugriffs auf Probleme finden Sie unter [Gewähren des Zugriffs auf Berichte, Dashboards und Kalender](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen oder Verwalten bestimmter Berichte erteilen, auf die Sie Zugriff haben, um sie freizugeben. Weitere Informationen zu Zugriffsebenen und Berechtigungen finden Sie unter [Zusammenwirken von Zugriffsebenen und Berechtigungen](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

Berechtigungen gelten für ein Element in Workfront und definieren, welche Aktionen für dieses Element ausgeführt werden können.

>[!NOTE]
>
>Ein Workfront-Administrator kann Berechtigungen für alle Elemente im System hinzufügen oder entfernen, ohne der Eigentümer dieser Elemente zu sein.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
      <p>Leicht</p>
      <p>Überprüfung</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender oder höher anzeigen</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für den Bericht anzeigen oder höher</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Freigeben von Berichten

Zusätzlich zu den folgenden Überlegungen finden Sie weitere Informationen unter [Berichte, Dashboards und Kalender freigeben](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Sie können Berichte, die Sie erstellen, mit anderen Personen, Teams, Gruppen, Arbeitsrollen oder Unternehmen teilen. Sie können auch Berichte freigeben, die andere erstellt haben und die für Sie freigegeben wurden.
* Sie können Berichte für Ihr gesamtes Unternehmen freigeben oder sie veröffentlichen. Wenn Sie einen Bericht veröffentlichen, wird eine URL generiert, die für andere freigegeben werden kann.
* Sie können einen einzelnen Bericht freigeben oder mehrere Berichte aus einer Berichtsliste freigeben.

## Möglichkeiten zur Weitergabe von Berichten

Sie können Berichte in Workfront auf folgende Weise freigeben:

* Manuell, wie im Abschnitt [Bericht freigeben](#share-a-report) unten beschrieben.
* Automatisch, indem Sie Anzeigeberechtigungen von einem Dashboard erben, das den freigegebenen Bericht enthält. Informationen zum Anzeigen von geerbten Berechtigungen für Objekte finden Sie unter [Anzeigen von geerbten Berechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Einen Bericht freigeben {#share-a-report}

Das Freigeben eines oder mehrerer Berichte in einer Liste ist identisch.

1. Wechseln Sie zu einer Liste von Berichten, wählen Sie einen oder mehrere Berichte aus, klicken Sie dann auf das Symbol **Freigeben** ![Freigeben](assets/share-icon.png).

   ODER

   Klicken Sie auf den Namen eines Berichts und dann auf **Berichtsaktionen** > **Freigabe**. Das **Freigeben [BERICHTSNAME]** wird geöffnet.

   ![Freigabeoption](assets/unshimmed-report-actions-sharing.png)

1. Geben Sie im Feld **Berichtszugriff auf** gewähren den Namen des Benutzers, des Teams, der Rolle des Jobs, der Gruppe oder des Unternehmens ein, für den bzw. das Sie den Bericht freigeben möchten, und wählen Sie ihn dann aus, wenn er angezeigt wird.

1. Um die Zugriffsebene für einen hinzugefügten Namen anzupassen, klicken Sie auf das Dropdown-Menü rechts neben dem Namen und wählen Sie dann eine der folgenden Optionen aus.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ansicht</td> 
      <td> <p>Ermöglicht es Ihrem Empfänger, den Bericht im Bereich <strong>Berichte</strong> anzuzeigen und auszuführen.</p> <p>Sie können rechts auf das Symbol <strong>Erweiterte Einstellungen</strong> klicken, um anzugeben, ob der Benutzer oder die Benutzer die <strong>Erweiterte Einstellungen</strong> für andere Benutzer im System freigeben können sollen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verwalten</td> 
      <td> <p>Der Empfänger hat vollständigen Zugriff auf den Bericht.</p> <p>Sie können auf das Symbol <strong>Erweiterte Einstellungen</strong> rechts klicken, um anzugeben, ob der/die Benutzende den Bericht aus dem System <strong>Löschen</strong> und für <strong> im System </strong> können soll.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wiederholen Sie die beiden vorherigen Schritte, um weitere Namen zur Liste hinzuzufügen und ihre Optionen zu konfigurieren.
1. (Optional) Klicken Sie auf das **Nur eingeladene Personen können zugreifen** Dropdown-Menü im Freigabefeld und wählen Sie dann eine der folgenden Optionen:

   * **Nur eingeladene Personen können zugreifen**: Wählen Sie diese Option, damit nur Benutzer, denen Zugriff auf den Bericht gewährt wurde, ihn anzeigen können.

   * **Jeder im System kann anzeigen**: Wählen Sie diese Option aus, damit jeder in Workfront mit Zugriff auf Berichte den Bericht anzeigen kann.

1. (Optional) Klicken Sie auf **Zahnrad**-Symbol ![Zahnradsymbol-Einstellungen](assets/gear-icon-settings-with-dn-arrow.jpg) in der oberen rechten Ecke des Freigabefelds und wählen Sie dann optional die folgende Option:

   * **Für externe Benutzer veröffentlichen**: Wählen Sie diese Option, um eine URL zu generieren, die für andere freigegeben werden kann. Jeder Benutzer mit der URL kann auf den Bericht zugreifen, ohne über eine Adobe Workfront-Lizenz zu verfügen.

     >[!CAUTION]
     >
     >Es wird empfohlen, bei der Freigabe eines Objekts mit vertraulichen Informationen an externe Benutzer Vorsicht walten zu lassen. Auf diese Weise können sie Informationen anzeigen, ohne ein Workfront-Benutzer oder Teil Ihres Unternehmens zu sein.

     >[!NOTE]
     >
     >Wenn für den Bericht eine Eingabeaufforderung vorhanden ist und Sie ihn öffentlich freigeben, können Benutzende, die den Bericht über den öffentlichen Freigabe-Link ausführen, den Bericht nicht über die Eingabeaufforderung ausführen. Sie sehen den Bericht ohne die darauf angewendete Aufforderung, es sei denn, sie melden sich bei Workfront an und greifen auf den Bericht zu, ohne den öffentlichen Freigabelink zu verwenden. Weitere Informationen zu den Einschränkungen bei der Freigabe von Berichten mit Eingabeaufforderungen finden Sie im Abschnitt [Einschränkungen bei der Freigabe von Berichten mit Eingabeaufforderung](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) im Artikel [Hinzufügen einer Eingabeaufforderung zu einem Bericht](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicken Sie auf **Speichern**.
