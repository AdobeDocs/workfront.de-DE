---
title: Freigeben von Arbeitsbereichen
description: Sie können einen Arbeitsbereich für andere freigeben, um die Zusammenarbeit bei der Arbeit in Adobe Workfront Planning sicherzustellen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
source-git-commit: ddcefb0baf10df9ae9ac3b29d7da1e2a070101c8
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 1%

---

# Freigeben von Arbeitsbereichen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können einen Arbeitsbereich für andere freigeben, um die Zusammenarbeit bei der Arbeit in Adobe Workfront Planning sicherzustellen.

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

>[!NOTE]
>
>Durch das Gewähren von Berechtigungen für einen Arbeitsbereich erhalten andere Benutzer keine Berechtigungen für die Ansichten auf den Datensatztypseiten. Sie müssen einzelnen Ansichten auf einer Datensatztypseite Berechtigungen erteilen, um sie für andere Benutzer freigeben zu können. Weitere Informationen finden Sie unter [Freigeben einer Ansicht](/help/quicksilver/planning/access/share-views.md).


## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für Workfront Planning anzuzeigen.

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
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p>
<p>Das Unternehmen muss in das einheitliche Adobe-Erlebnis integriert sein, damit Benutzer über eine Berechtigungsanfrage Berechtigungen für einen Arbeitsbereich anfordern und erteilen können. </p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
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
   <td>  <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--

OLD: 
 
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan </p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p> 
</td>
  </tr>
 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).-->



## Freigeben von Berechtigungen für einen Arbeitsbereich

Die folgenden Benutzer können einen Arbeitsbereich für andere Benutzer freigeben:

* Systemadministratoren können alle Arbeitsbereiche freigeben, auch die, die sie nicht erstellt haben.
* Alle anderen Benutzer können nur Arbeitsbereiche freigeben, für die sie über Verwaltungsberechtigungen verfügen.

So geben Sie einen Arbeitsbereich für andere frei:

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, den Sie freigeben möchten, und klicken **oben rechts** Bildschirm auf „Freigeben“.

   ![Freigabe-Schaltfläche oben rechts in Workspace](assets/share-button-on-workspace-top-right.png)

1. Beginnen Sie im Feld **Zugriff auf diesen Arbeitsbereich gewähren** mit der Eingabe des Namens eines Benutzers, einer Gruppe, eines <span class="preview">Teams, eines Unternehmens oder eines </span> und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   ![Freigabe der Benutzeroberfläche für Gruppen](assets/sharing-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Anzeigen
   * Mitwirken
   * Verwalten

     Informationen zu Berechtigungsebenen und den Aktionen, die Benutzende für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
1. Klicken Sie **Link kopieren**, um einen Link in den Arbeitsbereich in die Zwischenablage zu kopieren.
1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf den Arbeitsbereich zugreifen zu können.
1. Klicken Sie auf **Speichern**.

## Erteilen von Berechtigungen für einen Arbeitsbereich über eine Berechtigungsanfrage

Benutzende, die auf einen Link zu einem Arbeitsbereich zugreifen, für den sie keine Berechtigungen haben, können Berechtigungen für den Arbeitsbereich anfordern. Alle Benutzenden mit der Berechtigung Verwalten für den Arbeitsbereich erhalten die Berechtigungsanfrage und können die Berechtigungen erteilen oder verweigern.

1. (Bedingt) Wenn Sie der Manager eines Arbeitsbereichs sind, erhalten Sie möglicherweise eine Anfrage eines anderen Benutzers, in den folgenden Bereichen auf die Ansicht zuzugreifen:

   * In-App-Benachrichtigung
     ![In-App-Benachrichtigung bei Zugriffsanfrage](assets/in-app-notification-for-access-request.png)
   * Eine E-Mail-Benachrichtigung
     ![E-Mail-Benachrichtigung für Zugriffsanfrage](assets/email-notification-for-access-request.png)
1. (Bedingt) Klicken Sie im Benachrichtigungsbereich in Workfront auf die In-App-Benachrichtigung
oder
Klicken Sie in der E-Mail-Benachrichtigung **Alle Benachrichtigungen anzeigen** und klicken Sie dann auf die Benachrichtigung in der Liste.

   Das **Ausstehende**&quot; wird angezeigt.

   ![Benachrichtigungslisten-Genehmigungsfeld](assets/notifications-list-approval-box.png)

1. (Optional) Wählen Sie für den Benutzer, dessen Berechtigungen Sie genehmigen möchten, eine der folgenden Optionen aus dem Dropdown-Menü rechts neben dem Namen des Benutzers aus:
   * **Anzeigen**
   * **Beitragen**
   * **Verwalten**
1. Wählen Sie den Benutzer aus, für den Sie die Berechtigung genehmigen oder ablehnen möchten, und klicken Sie dann auf **Alle genehmigen** oder **Alle ablehnen**.
1. Klicken Sie auf den nach links zeigenden Pfeil links neben **Ausstehende**) und dann auf **Speichern**.

   Wenn Sie die Anfrage genehmigt haben, werden die Benutzer zum Feld Freigabe des Arbeitsbereichs hinzugefügt. Der Benutzer, der die Berechtigung anfordert, erhält eine E-Mail-Bestätigung, dass seine Anforderung genehmigt wurde. <!--will they also get an in-app notification??-->


## Entfernen von Berechtigungen für einen Arbeitsbereich


{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dem Berechtigungen entfernt werden sollen, und klicken Sie **oben rechts** Bildschirm auf „Freigeben“.
1. Klicken Sie auf das Dropdown-Menü rechts neben dem Namen einer Entität, für die Sie den Arbeitsbereich freigeben, und klicken Sie dann auf **Entfernen**.
1. Klicken Sie auf **Speichern**.

   Die entfernten Benutzer haben keinen Zugriff mehr auf den Arbeitsbereich oder dessen Objekte.
