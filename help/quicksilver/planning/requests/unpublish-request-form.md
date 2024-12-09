---
title: Rückgängigmachen der Veröffentlichung eines Anforderungsformulars in der Adobe Workfront-Planung
description: Sie können die Veröffentlichung eines Anfrageformulars rückgängig machen, wenn es nicht mehr benötigt oder relevant ist. Wenn Sie die Veröffentlichung rückgängig machen, entfernen Sie die Berechtigungen aller Benutzer für den Zugriff auf das Formular.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: b42436ad660642bd23638a8a44d9561513d748ed
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---


# Veröffentlichung eines Anfrageformulars in der Adobe Workfront-Planung rückgängig machen


<!--take Preview and Production references at Production time-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

Sie können die Veröffentlichung eines Anfrageformulars rückgängig machen, wenn es nicht mehr benötigt oder relevant ist. Wenn Sie die Veröffentlichung rückgängig machen, entfernen Sie die Berechtigungen aller Benutzer für den Zugriff auf das Formular.

Sie können auch die Entitäten ändern, für die Sie ein Anfrageformular freigeben, wenn Sie es für eine kleinere Personengruppe verfügbar halten möchten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
<p>Die folgenden Workfront-Pläne:</p>
<ul><li>Auswählen</li>
<li>Erstklassig</li>
<li>Ultimativ</li></ul>
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td>
   <td>
<p>Alle </p>  
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td>
   <td>
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Standard</p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <ul>
   <li><p>Berechtigungen für einen Arbeitsbereich verwalten</p></li>
    <li><p>Systemadministratoren können nicht erstellte Arbeitsbereiche verwalten. </p></li>
    </ul>
   <p>Informationen zum Freigeben von Berechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Überblick über die Freigabe von Berechtigungen in der Adobe Workfront-Planung</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ändern der Freigabe eines Anfrageformulars

Wenn Sie eine Anfrage für die Öffentlichkeit mit allen Benutzern, einschließlich Benutzern aus Nicht-Unternehmen, teilen, sollten Sie in Erwägung ziehen, diesen Zugriff auf bestimmte Benutzer zu beschränken, die den Arbeitsbereich, mit dem das Formular verknüpft ist, anzeigen oder verwalten.

So ändern Sie die Freigabe eines Anfrageformulars:

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in den Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite mit dem Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite vom Typ Datensatz in der Tabellenansicht geöffnet.

1. Klicken Sie auf das Menü **Mehr** rechts neben dem Namen des Datensatztyps in der Kopfzeile der Seite und klicken Sie dann auf **Anforderungsformular aktualisieren**.![](assets/more-menu.png)
1. Klicken Sie oben rechts im Bildschirm auf **Freigabe** und aktualisieren Sie dann die Freigabeoptionen. Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anforderungsformulars in der Adobe Workfront-Planung](/help/quicksilver/planning/requests/create-request-form.md).
1. (Optional) Klicken Sie auf **Link kopieren**, wenn Sie die Freigabe des Anfrageformulars geändert haben und es für die neue Personengruppe mit einem neuen Link freigeben möchten.

## Veröffentlichung eines Anfrageformulars für einen Datensatztyp rückgängig machen

Wenn ein Anfrageformular irrelevant wird und Sie nicht möchten, dass jemand mehr darauf zugreifen kann, können Sie die Veröffentlichung rückgängig machen.

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in den Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite mit dem Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite vom Typ Datensatz in der Tabellenansicht geöffnet.

1. Klicken Sie auf das Menü **Mehr** rechts neben dem Namen des Datensatztyps in der Kopfzeile der Seite und klicken Sie dann auf **Anforderungsformular aktualisieren**.![](assets/more-menu.png)
1. Klicken Sie oben rechts auf **Veröffentlichung rückgängig machen** .

   ![](assets/unpublish-button-highlighted.png)

   Unten im Bildschirm wird eine Bestätigung angezeigt, die Sie darüber informiert, dass die Veröffentlichung des Formulars rückgängig gemacht wurde.

   Die Schaltfläche **Veröffentlichung rückgängig machen** ändert sich in **Publish**.

1. Klicken Sie auf **Speichern**.

   Der Zugriff auf das Formular über einen Link <!--or from the request queue in the Requests area of Workfront--> ist nicht mehr möglich.

   Alle Datensätze, die zuvor über das Anfrageformular hinzugefügt wurden, verbleiben auf der Seite vom Typ Datensatz .

   <span class="preview">Alle zuvor hinzugefügten Anforderungen verbleiben auf der Registerkarte &quot;Planung&quot;im Bereich &quot;Anforderungen&quot;von Workfront.</span>