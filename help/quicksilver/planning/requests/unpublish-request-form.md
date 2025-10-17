---
title: Veröffentlichung eines Anfrageformulars in Adobe Workfront Planning aufheben
description: Sie können die Veröffentlichung eines Anfrageformulars aufheben, wenn es nicht mehr benötigt wird oder nicht mehr relevant ist. Durch das Rückgängigmachen der Veröffentlichung entfernen Sie die Berechtigungen aller Benutzer für den Zugriff auf das Formular.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: df0686038adb1278339e872e122a311884cb6d29
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 3%

---

# Veröffentlichung eines Anfrageformulars in Adobe Workfront Planning aufheben


<!--take Preview and Production references at Production time-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Sie können die Veröffentlichung eines Anfrageformulars aufheben, wenn es nicht mehr benötigt wird oder nicht mehr relevant ist. Durch das Rückgängigmachen der Veröffentlichung entfernen Sie die Berechtigungen aller Benutzer für den Zugriff auf das Formular.

Sie können auch die Entitäten ändern, für die Sie ein Anfrageformular freigeben, wenn Sie es für eine kleinere Gruppe von Personen verfügbar halten möchten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<p>Jedes Workfront-Paket und jedes Planungspaket</p>
Oder
<p>Beliebiges Workflow-Paket und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und Datensatztyp</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ändern der Freigabe eines Anfrageformulars

Wenn Sie eine Anfrage für öffentlich mit allen Personen teilen, einschließlich Benutzern von außerhalb Ihrer Organisation, sollten Sie diesen Zugriff auf bestimmte Benutzer beschränken, die den Arbeitsbereich, mit dem das Formular verknüpft ist, entweder anzeigen oder verwalten.

So ändern Sie die Freigabe eines Anfrageformulars:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie ein Formular freigeben möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Weitere Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite mit dem Datensatztyp in der Tabellenansicht geöffnet.

1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps in der Seitenkopfzeile und dann auf **Anfrageformulare verwalten**.

   Alle mit dem Datensatztyp verknüpften Anforderungsformulare werden in einer Tabellenansicht angezeigt.
1. Bewegen Sie den Mauszeiger über den Namen eines Anfrageformulars und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben seinem Namen und dann auf **Freigeben**.
1. Aktualisieren Sie die Freigabeoptionen, indem Sie eine der folgenden Optionen auswählen:

   * Jede Person mit Zugriff auf den Arbeitsbereich (Ansicht oder höher)
   * Jede Person mit Zugriff auf den Arbeitsbereich (Beitrag oder höher)
   * Jede Person mit dem Link

   Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Optional) Klicken Sie auf **Link kopieren**, wenn Sie die Freigabe des Anfrageformulars geändert haben und es für die neue Personengruppe über einen neuen Link freigeben möchten.

## Veröffentlichung eines Anfrageformulars für einen Datensatztyp aufheben

Wenn ein Anfrageformular irrelevant wird und Sie nicht mehr möchten, dass jemand darauf zugreift, können Sie die Veröffentlichung aufheben.

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Weitere Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite mit dem Datensatztyp in der Tabellenansicht geöffnet.

1. Klicken Sie auf das **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps in der Seitenkopfzeile und dann auf **Anfrageformulare verwalten**.

   Alle mit dem Datensatztyp verknüpften Anforderungsformulare werden in einer Tabellenansicht angezeigt.
1. Bewegen Sie den Mauszeiger über den Namen eines Anfrageformulars und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben seinem Namen. Klicken Sie dann auf **Veröffentlichung rückgängig machen**

Oder

Klicken Sie auf den Namen des Anfrageformulars, um es zu öffnen **und klicken Sie dann oben rechts** Anfrageformular auf „Veröffentlichung rückgängig machen“.

![Schaltfläche „Veröffentlichung rückgängig machen“ hervorgehoben](assets/unpublish-button-highlighted.png)

Unten im Bildschirm wird eine Bestätigung angezeigt, die Sie darüber informiert, dass die Veröffentlichung des Formulars aufgehoben wurde.

Der **Veröffentlichung aufheben**-Link oder die Schaltfläche ändert sich in **Veröffentlichen**.

1. (Bedingt) Klicken Sie auf **Speichern**, wenn Sie die Veröffentlichung des Formulars nach dem Öffnen aufgehoben haben.

   Benutzende können nicht mehr über einen Link oder über die Anfrage-Warteschlange im Bereich Anfragen von Workfront auf das Anfrageformular zugreifen.

   Alle zuvor über das Anfrageformular hinzugefügten Datensätze verbleiben auf der Seite „Datensatztyp“.

   Alle zuvor hinzugefügten Anfragen verbleiben im Bereich Anfragen von Workfront auf der Registerkarte Planung .
