---
title: Ansichten freigeben
description: Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Verwendung von Adobe Workfront Planning sicherzustellen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: fbf902196c9f5b55ddd1e20516e4237309dff2ed
workflow-type: tm+mt
source-wordcount: '1971'
ht-degree: 0%

---


# Ansichten freigeben

<!--take out preview and production references at production-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit beim Arbeiten mit Datensätzen in Adobe Workfront Planning sicherzustellen.

>[!IMPORTANT]
>
>* Durch das Gewähren von Berechtigungen für einen Arbeitsbereich erhalten andere Benutzer keine Berechtigungen für die Ansichten auf den Datensatztypseiten. Sie müssen einzelnen Ansichten auf einer Datensatztypseite Berechtigungen erteilen, um sie für andere Benutzer freigeben zu können.
>
>* Durch das Gewähren von Berechtigungen für eine Ansicht werden die Berechtigungen zum Anzeigen der Datensätze nicht geändert. Datensatzberechtigungen werden durch die Freigabe von Arbeitsbereichen gewährt.
>
>* Wenn Sie eine Ansicht freigeben, erteilen Sie anderen Berechtigungen für den Zugriff auf alle Elemente der Ansicht. Wenn Sie beispielsweise Berechtigungen zum Verwalten für eine Ansicht erteilen, können diese das Erscheinungsbild von Gruppierung, Filtern, Sortieren oder Balken ändern.


<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Das Unternehmen muss in das einheitliche Adobe-Erlebnis integriert sein, damit Benutzer Berechtigungen für eine Ansicht über eine Berechtigungsanfrage anfordern und erteilen können. </p>
<p>Benutzende müssen zur Adobe Admin Console hinzugefügt werden, um Berechtigungen für Workfront Planning-Ansichten zu erhalten.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard</p>
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
   <td>  <p>Verwalten der Berechtigungen für eine Ansicht</p>  
   <p>Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können eine Ansicht öffentlich freigeben.</p></td> 
  </tr>

</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe von Ansichten

* Sie können eine Ansicht wie folgt freigeben:

   * Intern mit Workfront-Benutzern, -Gruppen, -Teams, -Unternehmen und -Aufgabengebieten
   * Öffentlich, mit Benutzern außerhalb von Workfront
   * Durch Kopieren und anschließendes Freigeben eines Links zu einer Ansicht
   * Durch Exportieren in eine Excel- oder CSV-Datei. Sie können nur die Tabellenansicht in eine Datei exportieren. Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

* Allgemeine Informationen zum Freigeben von Objekten in Workfront Planning finden Sie auch unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Sie können internen Workfront-Benutzern Berechtigungen zum Anzeigen oder Verwalten für eine Ansicht erteilen.

* Benutzer mit der Berechtigung Verwalten können die Anzeigeeinstellungen ändern, freigeben, duplizieren oder löschen.

* Sie können mit Personen außerhalb Ihrer Organisation über einen öffentlichen Link Ansichten austauschen.

* Wenn Sie eine Ansicht öffentlich freigeben, ist der Link für einen begrenzten Zeitraum für alle Personen außerhalb Ihres Unternehmens zugänglich, angegeben durch das Ablaufdatum. Es ist keine Anmeldung erforderlich, um die freigegebene Ansicht anzuzeigen.

* Personen außerhalb Ihrer Organisation, die Zugriff auf eine Ansicht haben, können in der Ansicht keine anderen Ansichten erstellen, die freigegebene Ansicht bearbeiten oder Datensatzinformationen hinzufügen, löschen oder bearbeiten.

## Berechtigungen für eine Ansicht intern freigeben

Sie können von Ihnen erstellte Ansichten oder Ansichten, für die Sie über Verwaltungsberechtigungen verfügen, für Benutzende, Gruppen, Teams, Unternehmen und Aufgabengebiete in Workfront Planning freigeben.

>[!NOTE]
>
>Systemadministratoren können Ansichten, die sie nicht selbst erstellt haben, nicht anzeigen oder freigeben. Sie können nur auf Ansichten zugreifen oder diese freigeben, die für sie freigegeben sind.
>
>Systemadministratoren können nur Verwaltungsberechtigungen für eine Ansicht haben.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz .

   Dadurch wird die Seite „Datensatztyp“ geöffnet.

1. Führen Sie auf der Registerkarte der Ansicht eine der folgenden Aktionen aus:

   * Führen Sie je nach Umgebung, von der aus Sie auf die Ansicht zugreifen, die folgenden Schritte aus:

      * Bewegen Sie in der Produktionsumgebung den Mauszeiger über den Namen der Registerkarte der Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen der Ansicht und klicken Sie dann auf **Freigeben**.

      * <span class="preview"> Klicken Sie in der Vorschau-Umgebung auf die Registerkarte der Ansicht, bewegen Sie den Mauszeiger über die Ansicht im Dropdown-Menü, klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und klicken Sie dann auf **Freigeben**.</span>

     ![Menü „Mehr“ für eine Ansicht](assets/more-menu-for-views-expanded-with-share-option.png)

   * Klicken Sie **Freigeben** > **Aktuelle Ansicht freigeben**

     ![Freigabeschaltfläche mit Datensatztyp- und Ansichtsfreigabeoptionen](assets/share-button-with-record-type-and-view-sharing-options.png)

   Das Feld **Ansicht freigeben** wird geöffnet und die Registerkarte **Interne Freigabe** sollte standardmäßig ausgewählt sein.

1. (Optional) Wählen Sie im Bereich **Wer hat Zugriff** eine der folgenden Optionen aus:

   * **Nur eingeladene Personen können zugreifen**: Sie müssen Benutzer, Gruppen, Teams, Unternehmen oder Aufgabengebiete angeben, für die Sie die Ansicht freigeben möchten. Dies ist die Standardoption.

   >[!NOTE]
   >
   >Zusätzlich zu Teams, Gruppen, Unternehmen und Aufgabengebieten können Sie nur für Benutzende freigeben, die der Adobe Admin Console hinzugefügt wurden. Benutzende, die nur Workfront unterstützen, können nicht hinzugefügt werden. Weitere Informationen finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).


   * **Jeder Benutzer im Arbeitsbereich kann Folgendes anzeigen** Alle Benutzer mit Ansichts- oder höheren Berechtigungen für Arbeitsbereiche können auf die Ansicht zugreifen.

1. Beginnen Sie im Feld **Zugriff auf diese Ansicht gewähren** mit der Eingabe des Namens eines Benutzers, einer Gruppe, eines Teams, eines Unternehmens oder eines Aufgabengebiets und klicken Sie dann auf das Feld, wenn es in der Liste angezeigt wird.

   ![Freigeben einer Ansicht für Gruppen](assets/sharing-a-view-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Ansicht
   * Verwalten

     Informationen zu Berechtigungsebenen und den Aktionen, die Benutzende für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systemadministratoren erhalten immer Verwaltungsberechtigungen für Ansichten, die für sie freigegeben wurden.

1. Klicken Sie auf **Speichern**.

   Die Ansicht wird mit dem Symbol Personen ![Mit anderen Benutzern geteilt anzeigen](assets/view-shared-with-others-people-icon.png) aktualisiert, um anzugeben, dass die Ansicht jetzt für andere Benutzer freigegeben ist.

   Die Benutzenden, für die Sie die Ansicht freigegeben haben, erhalten sowohl eine In-App- als auch eine E-Mail-Benachrichtigung über die entsprechenden Berechtigungen.

   >[!TIP]
   >
   >Ansichten ohne Personen- oder Globalsymbol sind von Ihnen erstellte Ansichten und werden nicht für andere freigegeben. Nicht freigegebene Ansichten sind nur für Sie sichtbar.

1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite für den Datensatztyp zugreifen und sie in der ausgewählten Ansicht anzeigen zu können.

## Berechtigungen für eine Ansicht öffentlich freigeben

Sie können von Ihnen erstellte Ansichten oder Ansichten, für die Sie Verwaltungsberechtigungen haben, für Personen freigeben, die keine Workfront-Lizenz haben und die möglicherweise nicht zu Ihrem Unternehmen gehören.

>[!IMPORTANT]
>
>Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können die Ansichten des Arbeitsbereichs öffentlich freigeben.


So geben Sie eine Ansicht in Workfront Planning öffentlich frei:

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz .

   Dadurch wird die Seite „Datensatztyp“ geöffnet.

1. Führen Sie auf der Registerkarte Ansicht eine der folgenden Aktionen aus:

   * Bewegen Sie den Mauszeiger über den Namen der Registerkarte der Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** ![Mehr ](assets/more-menu.png) rechts neben dem Namen der Ansicht und klicken Sie dann auf **Freigeben**.

   ![Mehr Menü für Ansichten mit Freigabeoption erweitert](assets/more-menu-for-views-expanded-with-share-option.png)
   * Klicken Sie **Freigeben** > **Aktuelle Ansicht freigeben**

   Das **Ansicht freigeben** wird geöffnet.

1. Klicken Sie auf **Öffentliche Freigabe**.

   ![Registerkarte „Öffentliche Freigabe“ für Ansichten](assets/public-sharing-tab-for-views.png)

1. Aktivieren Sie die Einstellung **Öffentlichen Link erstellen**.

   Ein Link wird verfügbar. Dies ist ein öffentlicher Link. Bei der Freigabe kann jeder Benutzer mit dem Link, einschließlich Personen von außerhalb Ihres Unternehmens, auf die Seite „Datensatztyp“ zugreifen und Datensätze und Felder auf der Seite anzeigen.

1. Klicken Sie auf das **Link kopieren**-Symbol ![Link-Ansicht kopieren](assets/copy-link-view.png), um den Link in die Zwischenablage zu kopieren.

1. Geben Sie manuell ein Datum ein oder verwenden Sie den Kalender im Feld **Link-**), um ein Ablaufdatum für den öffentlichen Link auszuwählen. Die Datensatz-Seitenansicht ist nach dem ausgewählten Datum nicht mehr zugänglich.

1. Klicken Sie auf **Speichern**.

   Die Ansicht wird mit dem globalen Symbol ![Symbol „Öffentliche freigegebene Ansicht“ hervorgehoben](assets/public-shared-view-icon-highlighted.png) um anzugeben, dass die Ansicht öffentlich freigegeben ist.

   >[!TIP]
   >
   >Ansichten ohne Personen- oder Globalsymbol sind von Ihnen erstellte Ansichten und werden nicht für andere freigegeben. Nicht freigegebene Ansichten sind nur für Sie sichtbar.


1. (Optional) Fügen Sie den Link ein, den Sie in eine E-Mail, eine Chat-Nachricht, ein Dokument oder einen Workfront-Kommentar kopiert haben, um ihn für andere freizugeben.

## Kopieren eines Links in eine Ansicht

Sie können einen Link zu einer Ansicht in die Zwischenablage kopieren und in andere Anwendungen einfügen oder für andere freigeben.

Informationen zum Kopieren eines Links in eine öffentlich freigegebene Ansicht finden Sie im Abschnitt [Freigeben von Berechtigungen für eine öffentliche Ansicht](#share-permissions-to-a-view-publicly) in diesem Artikel.

In diesem Abschnitt wird beschrieben, wie Sie eine Ansicht intern freigeben.

>[!IMPORTANT]
>
>Zunächst müssen Sie die Ansicht für Benutzer freigeben, bevor Sie den Link zur Ansicht freigeben, damit sie sie anzeigen können.


{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, in dessen Ansicht Sie den Link kopieren und freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz .

   Dadurch wird die Seite „Datensatztyp“ geöffnet.

1. Führen Sie auf der Registerkarte einer Ansicht einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Registerkarte der Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Ansichtsnamen. Klicken Sie dann **Freigeben** > **Link kopieren** im **** Ansicht freigeben.
   * Klicken Sie **Freigeben** > **Link „Ansicht kopieren** auf der Seite „Datensatztyp“.

   Ein Link zur Ansicht wird in die Zwischenablage kopiert und Sie erhalten eine Bestätigung am unteren Bildschirmrand.

   Sie können den Link jetzt in ein anderes Programm einfügen oder an andere senden.

## Erteilen von Berechtigungen für eine Ansicht über eine Berechtigungsanfrage

Benutzende, die auf einen Link zu einer Ansicht zugreifen, für die sie keine Berechtigungen haben, können Berechtigungen für die Ansicht anfordern. Alle Benutzenden mit der Berechtigung Verwalten für die Ansicht erhalten die Berechtigungsanfrage und können die Berechtigungen erteilen oder verweigern.

1. (Bedingt) Wenn Sie der Manager einer Ansicht sind, erhalten Sie möglicherweise eine Anfrage eines anderen Benutzers, in den folgenden Bereichen auf die Ansicht zuzugreifen:

   * In-App-Benachrichtigung
     ![In-App-Benachrichtigung über Zugriffsanfrage für Ansicht](assets/in-app-notification-for-access-request-for-view.png)
   * Eine E-Mail-Benachrichtigung
     ![In-App-Benachrichtigung über Zugriffsanfrage für Ansicht](assets/in-app-notification-for-access-request-for-view.png)
1. (Bedingt) Klicken Sie im Benachrichtigungsbereich in Workfront auf die In-App-Benachrichtigung
oder
Klicken Sie in der E-Mail-Benachrichtigung **Alle Benachrichtigungen anzeigen** und klicken Sie dann auf die Benachrichtigung in der Liste.

   Das **Ausstehende**&quot; wird angezeigt.

   ![Benachrichtigungslisten-Genehmigungsfeld](assets/notifications-list-approval-box.png)
1. (Optional) Wählen Sie für den Benutzer, dessen Berechtigungen Sie genehmigen möchten, eine der folgenden Optionen aus dem Dropdown-Menü rechts neben dem Namen des Benutzers aus:
   * **Anzeigen**
   * **Verwalten**
1. Wählen Sie den Benutzer aus, für den Sie die Berechtigung genehmigen oder ablehnen möchten, und klicken Sie dann auf **Alle genehmigen** oder **Alle ablehnen**.
1. Klicken Sie auf den nach links zeigenden Pfeil links neben **Ausstehende**) und dann auf **Speichern**.

   Wenn Sie die Anfrage genehmigt haben, werden die Benutzer zum Freigabefeld der Ansicht hinzugefügt. Der Benutzer, der die Berechtigung anfordert, erhält eine E-Mail-Bestätigung, dass seine Anforderung genehmigt wurde. <!--will they also get an in-app notification??-->

## Entfernen von Berechtigungen für eine Ansicht

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie nicht mehr freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz . Dadurch wird die Seite „Datensatztyp“ geöffnet.
1. Führen Sie auf der Registerkarte Ansicht eine der folgenden Aktionen aus:

   * Bewegen Sie den Mauszeiger über den Namen der Registerkarte der Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** ![Mehr ](assets/more-menu.png) rechts neben dem Namen der Ansicht und klicken Sie dann auf **Freigeben**.

   * Klicken Sie **Freigeben** > **Aktuelle Ansicht freigeben**

   Das **Ansicht freigeben** wird geöffnet.
1. Gehen Sie wie folgt vor, um die interne Freigabe einer Ansicht zu entfernen:

   1. Stellen Sie sicher **dass die Registerkarte** Interne Freigabe“ ausgewählt ist.
   1. Suchen Sie den/die Benutzende(n), die/die Gruppe, das Team, das Unternehmen oder das Aufgabengebiet, das/die Sie entfernen möchten, erweitern Sie das Dropdown-Menü Berechtigungen rechts neben dem Namen der Entität, für die Sie die Ansicht freigeben, und klicken Sie dann auf **Entfernen**.

1. Gehen Sie wie folgt vor, um die öffentliche Freigabe einer Ansicht zu entfernen:

   1. Klicken Sie auf die **Öffentliche Freigabe**.
   1. Deaktivieren Sie die Option **Öffentlichen Link erstellen**.

1. Klicken Sie auf **Speichern**.

   Die Personen haben keinen Zugriff mehr auf die Ansicht. Es gibt keine Benachrichtigung für die Benutzer, die vom Zugriff auf entfernt wurden, dass sie diesen Zugriff nicht mehr haben.
