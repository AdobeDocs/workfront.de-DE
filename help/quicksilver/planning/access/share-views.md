---
title: Ansichten freigeben
description: Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Verwendung der Adobe Workfront-Planung sicherzustellen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '1433'
ht-degree: 1%

---


# Ansichten freigeben

{{planning-important-intro}}

Sie können eine Ansicht für andere freigeben, um die Zusammenarbeit bei der Arbeit mit Datensätzen in der Adobe Workfront-Planung sicherzustellen.

>[!IMPORTANT]
>
>* Wenn Sie Berechtigungen für einen Arbeitsbereich erteilen, erhalten andere Benutzer keine Berechtigungen für die Ansichten auf den Seiten vom Typ Datensatz. Sie müssen einzelnen Ansichten auf einer Seite vom Typ Datensatz Berechtigungen erteilen, um sie für andere Benutzer freizugeben.
>
>* Wenn Sie einer Ansicht Berechtigungen erteilen, werden die Berechtigungen zum Anzeigen der Datensätze nicht geändert. Berechtigungen für Datensätze werden durch Freigeben von Arbeitsbereichen gewährt.
>
>* Wenn Sie eine Ansicht freigeben, gewähren Sie anderen Berechtigungen für den Zugriff auf alle Elemente der Ansicht. Wenn Sie ihnen beispielsweise Berechtigungen zum Verwalten für eine Ansicht erteilen, können sie die Gruppierung, den Filter, die Sortierung oder das Erscheinungsbild der Leiste ändern.


Sie können eine Ansicht für die folgenden Entitäten freigeben:

* Intern mit Workfront-Benutzern und -Gruppen
* Öffentlich für Benutzer außerhalb von Workfront

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
<p>Ihr Unternehmen muss in das Adobe Unified Experience integriert sein, damit Benutzer über eine Berechtigungsanfrage Berechtigungen für eine Ansicht anfordern und gewähren können. </p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard</p>
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
   <td>  <p>Berechtigungen für eine Ansicht verwalten</p>  
   <p>Nur Benutzer mit Verwaltungsberechtigungen für einen Arbeitsbereich können eine Ansicht öffentlich freigeben.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--OLD: 

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
   <td> <p>Manage permissions to a view</p>  
   <p>Only users with Manage permissions to a workspace can share a view publicly.</p>
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

+++

## Überlegungen beim Freigeben von Ansichten

* Sie können internen Workfront-Benutzern Ansichts- oder Verwaltungsberechtigungen für eine Ansicht erteilen.

* Benutzer mit Verwaltungsberechtigungen können die Ansichtseinstellungen ändern, freigeben, duplizieren oder löschen.

* Sie können Ansichten für Personen außerhalb Ihres Unternehmens über einen öffentlichen Link freigeben.

* Wenn Sie eine Ansicht öffentlich freigeben, steht der Link für eine begrenzte Zeit für jedermann außerhalb Ihres Unternehmens zur Verfügung, angegeben durch das Ablaufdatum. Zum Anzeigen der freigegebenen Ansicht ist keine Anmeldung erforderlich.

* Personen außerhalb Ihrer Organisation, die Zugriff auf eine Ansicht haben, können keine anderen Ansichten erstellen, die freigegebene Ansicht bearbeiten oder Datensatzinformationen in der Ansicht hinzufügen, löschen oder bearbeiten.

## Berechtigungen intern für eine Ansicht freigeben

Sie können von Ihnen erstellte Ansichten oder Ansichten, für die Sie über Verwaltungsberechtigungen verfügen, in Workfront für Benutzer oder Gruppen freigeben.

>[!NOTE]
>
>Systemadministratoren können keine Ansichten anzeigen oder freigeben, die sie selbst nicht erstellt haben. Sie können nur auf Ansichten zugreifen oder diese freigeben, die für sie freigegeben sind.
>
>Systemadministratoren können nur über Verwaltungsberechtigungen für eine Ansicht verfügen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz.

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.

1. Bewegen Sie auf der Registerkarte &quot;Ansicht&quot;den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Ansichtsnamen und klicken Sie dann auf **Freigeben** .

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

   Die Registerkarte **Interne Freigabe** sollte standardmäßig ausgewählt sein.

1. (Optional) Wählen Sie im Bereich **Wer Zugriff hat** aus den folgenden Optionen aus:

   * **Nur eingeladene Personen können auf** zugreifen: Sie müssen Benutzer oder Gruppen angeben, für die Sie die Ansicht freigeben möchten. Dies ist die Standardoption.
   * **Alle Benutzer im Arbeitsbereich können anzeigen**: Alle Benutzer mit der Berechtigung &quot;Ansicht&quot;oder höher für Arbeitsbereiche können auf die Ansicht zugreifen.

1. Geben Sie im Feld **Gewähren des Ansichtszugriffs auf** den Namen eines Benutzers oder einer Gruppe ein und klicken Sie dann auf diesen, wenn er in der Liste angezeigt wird.

   ![](assets/sharing-a-view-ui-with-groups.png)

1. Wählen Sie eine der folgenden Berechtigungsebenen aus dem Dropdown-Menü aus:
   * Anzeigen
   * Verwalten

     Informationen zu Berechtigungsebenen und zu den Aktionen, die Benutzer für die einzelnen Ebenen ausführen können, finden Sie unter [Übersicht über die Berechtigungen für die Freigabe in der Adobe Workfront-Planung](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Systemadministratoren erhalten immer Berechtigungen zum Verwalten von Ansichten, die für sie freigegeben sind.

1. Klicken Sie auf **Link kopieren** , um einen Link in die Ansicht in die Zwischenablage zu kopieren.
1. Klicken Sie auf **Speichern**.

   Die Ansicht wird mit dem Personensymbol ![](assets/view-shared-with-others-people-icon.png) aktualisiert, um anzugeben, dass die Ansicht jetzt für andere Benutzer freigegeben ist.

   >[!TIP]
   >
   >Ansichten ohne Personen oder ein globales Symbol sind Ansichten, die Sie erstellt haben und die nicht für andere freigegeben sind. Nicht freigegebene Ansichten sind nur für Sie sichtbar.

1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite vom Typ Datensatz zugreifen und sie in der ausgewählten Ansicht anzeigen zu können.

## Berechtigungen öffentlich für eine Ansicht freigeben

Sie können von Ihnen erstellte Ansichten oder Ansichten, für die Sie über Verwaltungsberechtigungen verfügen, für Personen freigeben, die keine Workfront-Lizenz besitzen und die möglicherweise nicht zu Ihrem Unternehmen gehören.

>[!IMPORTANT]
>
>Nur Benutzer mit Verwaltungsberechtigungen für einen Arbeitsbereich können die Ansichten des Arbeitsbereichs öffentlich freigeben.


So geben Sie eine Ansicht in der Workfront-Planung öffentlich frei:

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz.

   Dadurch wird die Seite mit dem Datensatztyp geöffnet.

1. Bewegen Sie auf der Registerkarte &quot;Ansicht&quot;den Mauszeiger über die Ansicht, die Sie freigeben möchten, und klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Ansichtsnamen und klicken Sie dann auf **Freigeben** .

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. Klicken Sie auf **Öffentliche Freigabe**.

   ![](assets/public-sharing-tab-for-views.png)

1. Aktivieren Sie die Einstellung **Öffentlichen Link erstellen** .

   Ein Link wird verfügbar. Dies ist ein öffentlicher Link. Bei der Freigabe kann jeder, der über den Link verfügt, einschließlich Personen außerhalb Ihrer Organisation, auf die Seite mit dem Datensatztyp zugreifen und Datensätze und Felder auf der Seite anzeigen.

1. Klicken Sie auf das Symbol **Link kopieren** ![](assets/copy-link-view.png) , um den Link in die Zwischenablage zu kopieren.

1. Geben Sie manuell ein Datum ein oder verwenden Sie den Kalender im Feld **Ablaufdatum des Links** , um ein Ablaufdatum für den öffentlichen Link auszuwählen. Nach dem ausgewählten Datum ist die Ansicht der Datensatzseite nicht mehr verfügbar.

1. Klicken Sie auf **Speichern**.

   Die Ansicht wird mit dem globalen Symbol ![](assets/public-shared-view-icon-highlighted.png) aktualisiert, um anzugeben, dass die Ansicht öffentlich freigegeben ist.

   >[!TIP]
   >
   >Ansichten ohne Personen oder ein globales Symbol sind Ansichten, die Sie erstellt haben und die nicht für andere freigegeben sind. Nicht freigegebene Ansichten sind nur für Sie sichtbar.


1. (Optional) Fügen Sie den kopierten Link in eine E-Mail, eine Chat-Nachricht, ein Dokument oder einen Workfront-Kommentar ein, um ihn für andere freizugeben.

## Berechtigungen für eine Ansicht über eine Berechtigungsanforderung gewähren

Benutzer, die auf einen Link zu einer Ansicht zugreifen, für die sie keine Berechtigungen haben, können Berechtigungen für die Ansicht anfordern. Alle Benutzer mit Verwaltungsberechtigungen für die Ansicht erhalten die Berechtigungsanforderung und können die Berechtigungen gewähren oder verweigern.

1. (Bedingt) Wenn Sie der Manager einer Ansicht sind, erhalten Sie möglicherweise eine Anfrage eines anderen Benutzers zum Zugriff auf die Ansicht in den folgenden Bereichen:

   * In-App-Benachrichtigung
     ![](assets/in-app-notification-for-access-request-for-view.png)
   * Eine E-Mail-Benachrichtigung
     ![](assets/in-app-notification-for-access-request-for-view.png)
1. (Bedingt) Klicken Sie im Benachrichtigungsbereich in Workfront auf die In-App-Benachrichtigung
Oder
Klicken Sie in der E-Mail-Benachrichtigung auf **Alle Benachrichtigungen anzeigen** und klicken Sie dann auf die Benachrichtigung in der Liste.

   Das Feld **Ausstehende Zugriffsanforderungen** wird angezeigt.

   ![](assets/notifications-list-approval-box.png)
1. (Optional) Wählen Sie für den Benutzer, dessen Berechtigungen Sie genehmigen möchten, eine der folgenden Optionen aus dem Dropdown-Menü rechts neben dem Benutzernamen aus:
   * **Anzeigen**
   * **Verwalten**
1. Wählen Sie den Benutzer aus, für den Sie die Berechtigung genehmigen oder verweigern möchten, und klicken Sie dann auf **Alle genehmigen** oder **Alle verweigern**.
1. Klicken Sie auf den nach links zeigenden Pfeil neben **Ausstehende Zugriffsanforderungen** und dann auf **Speichern**.

   Wenn Sie die Anfrage genehmigt haben, werden die Benutzer zum Freigabefeld der Ansicht hinzugefügt. Der Benutzer, der die Berechtigung anfordert, erhält eine E-Mail-Bestätigung, dass seine Anfrage genehmigt wurde. <!--will they also get an in-app notification??-->

## Berechtigungen für eine Ansicht entfernen

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Ansicht Sie die Freigabe stoppen möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz. Dadurch wird die Seite mit dem Datensatztyp geöffnet.
1. Bewegen Sie den Mauszeiger über den Registerkartennamen der Ansicht, von der Sie die Freigabe entfernen möchten, und klicken Sie auf das Menü **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Freigeben**.
1. Gehen Sie wie folgt vor, um die interne Freigabe einer Ansicht zu entfernen:

   1. Stellen Sie sicher, dass die Registerkarte **Interne Freigabe** ausgewählt ist.
   1. Suchen Sie den Benutzer oder die Gruppe, was Sie entfernen möchten, erweitern Sie das Dropdown-Menü für Berechtigungen rechts neben dem Namen des Benutzers oder der Gruppe und klicken Sie dann auf **Entfernen**.

1. Gehen Sie wie folgt vor, um die öffentliche Freigabe einer Ansicht zu entfernen:

   1. Klicken Sie auf die Registerkarte **Öffentliche Freigabe**.
   1. Deaktivieren Sie die Option **Öffentlichen Link erstellen** .

1. Klicken Sie auf **Speichern**.

   Benutzer haben keinen Zugriff mehr auf die Ansicht. Es gibt keine Benachrichtigung für Benutzer, die nicht mehr auf die Ansicht zugreifen können, dass sie diesen Zugriff nicht mehr haben.
