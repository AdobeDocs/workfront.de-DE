---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen und bereitstellen
description: Standardmäßig können Benutzende nur die Objekte in einem Bericht sehen, für die sie über die Berechtigung zum Anzeigen verfügen.
author: Nolan
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: 12e8bc389c42510b5adbb0190eb71c9f6a9f52a7
workflow-type: tm+mt
source-wordcount: '1179'
ht-degree: 0%

---

# Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen und bereitstellen

<!-- Audited: 11/2024 -->

Standardmäßig können Benutzende nur die Objekte in einem Bericht sehen, für die sie über die Berechtigung zum Anzeigen verfügen.

Sie können allen Benutzenden ermöglichen, dieselben Ergebnisse in einem Bericht wie allen anderen Benutzenden anzuzeigen, unabhängig von ihrer Zugriffsebene oder Berechtigungsstufe für die Objekte innerhalb des Berichts.

Wenn Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers ausführen, der über höhere Zugriffsrechte verfügt (z. B. die Zugriffsrechte eines Adobe Workfront-Administrators), können alle Benutzer, die über die Berechtigung zum Anzeigen des Berichts verfügen, die Informationen im Bericht so anzeigen, wie der in Report Builder angegebene Benutzer. Sie können dies für Berichte einrichten, die Benutzende in der Workfront-Benutzeroberfläche finden, oder für Berichte, die Benutzenden als Anhang einer E-Mail zugestellt werden.

>[!TIP]
>
>Sie sollten das Feld **Diesen Bericht ausführen durch die Zugriffsrechte von:** nur dann durch einen aktiven Benutzer ersetzen, wenn Sie möchten, dass der Bericht mit den Zugriffsrechten dieses Benutzers angezeigt wird. Beispielsweise verfügt ein Benutzer mit Arbeitslizenz möglicherweise nicht über die Berechtigungen zum Anzeigen aller Elemente in einem Bericht, der von einem Benutzer mit Planlizenz oder einem Systemadministrator erstellt wurde, es sei denn, der Bericht wird mit den Zugriffsrechten eines Planers oder Systemadministrators angezeigt.\
>Wenn der Bericht für Benutzer mit ähnlichem Zugriff wie der im Feld **Diesen Bericht mit den Zugriffsrechten von ausführen:** angegebene Benutzer freigegeben wird, können Sie dieses Feld leer lassen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
      <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen der Berechtigungen für einen Bericht (zum Anzeigen des bereitgestellten Berichts)</p><p>Berechtigungen für einen Bericht verwalten (um den Bericht auszuführen)</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen eines Berichts mit den Zugriffsrechten eines anderen Benutzers

Durch das Ausfüllen des Felds **Diesen Bericht ausführen mit den Zugriffsrechten von:** wird sichergestellt, dass ein Bericht dieselben Daten enthält, unabhängig davon, welcher Benutzer auf den Bericht zugreift. Der Bericht wird so angezeigt, wie es für den angegebenen Benutzer der Fall wäre.

Die Benutzer, die auf den Bericht zugreifen, müssen mindestens über Anzeigeberechtigungen für den Bericht verfügen, damit sie ihn anzeigen können. Wenn der in der Liste **Diesen Bericht ausführen mit den Zugriffsrechten von:** aufgeführte Benutzer deaktiviert ist, wird der Bericht für keine anderen Benutzer mehr angezeigt, für die der Bericht freigegeben ist.

So führen Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers aus:

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **[!UICONTROL Berichte]**.

1. Wählen Sie den Bericht aus, den Sie mit den Zugriffsrechten eines anderen Benutzers anzeigen möchten.
1. Klicken Sie **Berichtsaktionen** und dann auf **Bearbeiten**.

1. Klicken Sie **Berichteinstellungen**.

1. Geben **im Feld „Diesen Bericht ausführen mit Zugriffsrechten von:**&quot; den Namen des Benutzers ein, als den der Bericht angezeigt werden soll, und wählen Sie ihn aus, wenn Sie ihn in der Liste sehen.\
   ![](assets/unshimmed-access-rights-of.png)

   >[!NOTE]
   >
   >Benutzer mit einer niedrigeren Zugriffsebene, die Berichte erstellen dürfen, können für das Feld **Diesen Bericht ausführen mit Zugriffsrechten von:** nicht einen anderen Benutzer als sich selbst auswählen.

1. Klicken Sie **Fertig**.
1. Klicken Sie auf **Speichern + schließen**.\
   Der Bericht wird nun für alle Benutzer angezeigt, für die der Bericht freigegeben ist, als ob er von dem im Feld **Diesen Bericht mit Zugriffsrechten ausführen von:** angegebenen Benutzer angezeigt worden wäre.

>[!IMPORTANT]
>
>Die Eingabe eines anderen Benutzers als des angemeldeten Benutzers für das Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** wirkt sich auf die im Bericht angezeigten Informationen aus, wenn der Bericht einen Filter enthält, der einen Platzhalter verwendet, der auf den angemeldeten Benutzer verweist. Der Bericht wird entsprechend dem Wert im Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** statt gemäß dem im Platzhalterfilter definierten Wert angezeigt.
>
>Weitere Informationen zu Platzhaltern für Benutzerfelder finden Sie im Abschnitt „Benutzerbasierte Variablen“ in der [Übersicht über Platzhalterfiltervariablen](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Bereitstellen eines Berichts mit den Zugriffsrechten eines anderen Benutzers

Sie können Berichte so einrichten, dass sie als Anhang an eine E-Mail gesendet werden. Sie können festlegen, dass diese bereitgestellten Berichte so angezeigt werden, wie sie für Benutzer mit einer höheren Zugriffsebene angezeigt werden, damit alle Benutzer dieselben Informationen in den bereitgestellten Berichten sehen können. Die Benutzer, die den in der E-Mail zugestellten Bericht sehen werden, müssen zur Empfängerliste „Senden an“ im Berichtsversand hinzugefügt werden. Weitere Informationen zum Einrichten eines Berichts für den Versand finden Sie im Artikel [Übersicht über den Versand von Berichten](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

So stellen Sie einen Bericht mit den Zugriffsrechten eines anderen Benutzers bereit:

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Workfront und dann auf **Berichte**.

1. Wählen Sie den Bericht aus, den Sie mit den Zugriffsrechten eines anderen Benutzers bereitstellen möchten.
1. Klicken Sie auf den Namen des Berichts, um ihn auszuwählen.
1. Klicken Sie **Berichtsaktionen**.
1. Klicken Sie **Bericht senden**.

1. Beginnen Sie im Feld **Diesen Bericht mit den Zugriffsrechten von bereitstellen:** mit der Eingabe des Benutzernamens, den der Bericht anzeigen soll, als ob er in einer E-Mail zugestellt wird, und wählen Sie ihn aus, wenn Sie ihn in der Liste sehen. Der Standardwert ist der Name des Benutzers, der den Bericht erstellt.\
   ![](assets/unshimmed-send-report-access-rights-of.png)

   >[!NOTE]
   >
   >Benutzer mit einer niedrigeren Zugriffsebene, die Berichte erstellen dürfen, können für das Feld **Diesen Bericht mit Zugriffsrechten bereitstellen von:** keinen anderen Benutzer als sich selbst auswählen.

1. Wählen Sie **Format**, den Bericht in der E-Mail anzuzeigen:

   * HTML
   * PDF
   * Excel
   * Excel (.xlsx)
   * TSV

1. Klicken Sie **Jetzt senden**, um es sofort zu senden.\
   Oder\
   Klicken Sie **Sich wiederholenden Versand durchführen**, um einen wiederkehrenden Versand für den Bericht zu planen.\
   Weitere Informationen zu Berichtssendungen finden Sie im Artikel [Übersicht über die Berichtsbereitstellung](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Einschränkungen für Berichte mit einer Source-Spalte

Die folgenden Berichte zeigen eine Source-Spalte an, in der Sie Informationen zum übergeordneten Objekt anzeigen können:

* Problemberichte
* Stundenberichte
* Dokumentieren von Berichten

Wenn Benutzende keine Berechtigungen für das übergeordnete Objekt eines Problems, einer Stunde oder eines Dokuments haben, wird die Source-Spalte des Berichts leer angezeigt, selbst wenn der Bericht so konfiguriert ist, dass er angezeigt wird oder mit den Zugriffsrechten eines anderen Benutzers bereitgestellt werden soll.

Um Informationen über das übergeordnete Objekt im Bericht anzuzeigen, empfehlen wir, eine Spalte für das übergeordnete Objekt hinzuzufügen, in der Sie den Namen des übergeordneten Objekts anzeigen können.

Sie können beispielsweise einen der folgenden Punkte zu einem Bericht mit einer Source-Spalte hinzufügen:

* Die Spalten „Projektname“, „Aufgabenname“ oder „Problemname“ für ein Dokument oder einen Stundenbericht.
* Die Spalten „Projektname“ oder „Aufgabenname“ für einen Problembericht.
* Eine Spalte mit Textmodusausdrücken, die auf alle drei Objekte verweist. Im Folgenden finden Sie ein Beispiel für einen Stundenbericht:

  ```
  displayname=Custom Source
  
  linkedname=opTask
  
  namekey=view.relatedcolumn
  
  namekeyargkey.0=opTask
  
  namekeyargkey.1=name
  
  textmode=true
  
  valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))
  
  valueformat=HTML
  ```

  Weitere Informationen zu Textmodusansichten finden Sie unter [Bearbeiten einer Ansicht im Textmodus](../text-mode/edit-text-mode-in-view.md).