---
title: Veröffentlichung eines Anfrageformulars in Adobe Workfront Planning aufheben
description: Sie können die Veröffentlichung eines Anfrageformulars aufheben, wenn es nicht mehr benötigt wird oder nicht mehr relevant ist. Durch das Rückgängigmachen der Veröffentlichung entfernen Sie die Berechtigungen aller Benutzer für den Zugriff auf das Formular.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: df8c4926-e258-49c0-ab9d-563ccaf7a6aa
source-git-commit: ba17bd824717f61e72fb9a73c8b90fbe755e20d8
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 1%

---

# Veröffentlichung eines Anfrageformulars in Adobe Workfront Planning aufheben


<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie können die Veröffentlichung eines Anfrageformulars aufheben, wenn es nicht mehr benötigt wird oder nicht mehr relevant ist. Durch das Rückgängigmachen der Veröffentlichung entfernen Sie die Berechtigungen aller Benutzer für den Zugriff auf das Formular.

Sie können auch die Entitäten ändern, für die Sie ein Anfrageformular freigeben, wenn Sie es für eine kleinere Gruppe von Personen verfügbar halten möchten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkte</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront-Planung<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td>
   <td>
<p>Einer der folgenden Workfront-Pläne:</p>
<ul><li>Auswählen</li>
<li>Erstklassig</li>
<li>Ultimativ</li></ul>
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td>
   <td>
<p>Beliebig </p>  
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td>
   <td>
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience für Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <ul>
   <li><p>Verwalten von Berechtigungen für einen Arbeitsbereich</p></li>
    <li><p>Systemadministratoren können Arbeitsbereiche verwalten, die sie nicht erstellt haben. </p></li>
    </ul>
   <p>Informationen zu Freigabeberechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Übersicht über Freigabeberechtigungen in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutvorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ändern der Freigabe eines Anfrageformulars

Wenn Sie eine Anfrage für öffentlich mit allen Personen teilen, einschließlich Benutzern von außerhalb Ihrer Organisation, sollten Sie diesen Zugriff auf bestimmte Benutzer beschränken, die den Arbeitsbereich, mit dem das Formular verknüpft ist, entweder anzeigen oder verwalten.

So ändern Sie die Freigabe eines Anfrageformulars:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Weitere Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite mit dem Datensatztyp in der Tabellenansicht geöffnet.

1. Klicken Sie auf das **Mehr**-Menü ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps in der Kopfzeile der Seite und dann auf **Anfrageformular aktualisieren**.
1. Klicken **oben rechts** Bildschirm auf „Freigeben“ und aktualisieren Sie dann die Freigabeoptionen. Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. (Optional) Klicken Sie auf **Link kopieren**, wenn Sie die Freigabe des Anfrageformulars geändert haben und es für die neue Personengruppe über einen neuen Link freigeben möchten.

## Veröffentlichung eines Anfrageformulars für einen Datensatztyp aufheben

Wenn ein Anfrageformular irrelevant wird und Sie nicht mehr möchten, dass jemand darauf zugreift, können Sie die Veröffentlichung aufheben.

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Weitere Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite mit dem Datensatztyp in der Tabellenansicht geöffnet.

1. Klicken Sie auf das **Mehr**-Menü ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps in der Kopfzeile der Seite und dann auf **Anfrageformular aktualisieren**.
1. Klicken **oben** auf „Veröffentlichung rückgängig machen“.

   ![](assets/unpublish-button-highlighted.png)

   Unten im Bildschirm wird eine Bestätigung angezeigt, die Sie darüber informiert, dass die Veröffentlichung des Formulars aufgehoben wurde.

   Die Schaltfläche **Veröffentlichung aufheben** ändert sich in **Publish**.

1. Klicken Sie auf **Speichern**.

   Der Zugriff auf das Formular ist über einen Link <!--or from the request queue in the Requests area of Workfront--> nicht mehr möglich.

   Alle zuvor über das Anfrageformular hinzugefügten Datensätze verbleiben auf der Seite „Datensatztyp“.

   Alle zuvor hinzugefügten Anfragen verbleiben im Bereich Anfragen von Workfront auf der Registerkarte Planung .
