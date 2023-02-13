---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Filtern von Informationen im Arbeitslastausgleich
description: Um Arbeitselemente effizient zu finden und uns auf die von Ihnen verwalteten Benutzer oder Elemente zu konzentrieren, empfehlen wir dringend, Filter im Arbeitsladeregel zu verwenden.
author: Alina
feature: Resource Management
exl-id: f8ffb40e-4e71-45fe-bcae-801d45d75a21
source-git-commit: 10b905c8a66f2507cbfac7c15a01f38d40ab3e00
workflow-type: tm+mt
source-wordcount: '2466'
ht-degree: 0%

---

# Filtern von Informationen im Arbeitslastausgleich

<!--
(when they add custom fields to fitlering, add the caveat you added for the Resource Planner : only field NAMES and not LABELS are to be found in the drop-down >> ADD THIS IN THE STEP BELOW WHEN ADDING A FILTER)
-->

Als Ressourcen-Manager können Sie den Lastenausgleich verwenden, um die Arbeitslast Ihrer Benutzer anzuzeigen und zu verwalten. Weitere allgemeine Informationen zum Arbeitslastausgleich finden Sie in den folgenden Artikeln:

* [Übersicht über den Lastenausgleich](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
* [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Um Arbeitselemente effizient zu finden und uns auf die von Ihnen verwalteten Benutzer oder Elemente zu konzentrieren, empfehlen wir dringend, Filter im Arbeitsladeregel zu verwenden. Auf diese Weise können Sie die richtigen Informationen anzeigen, bevor Sie mit der Verwaltung der Ressourcenzuweisungen beginnen.
>
>Wenn Sie einen neuen Filter speichern und anwenden und dann vom Arbeitslastausgleich weg navigieren, bleibt der Filter auch nach dem Abmelden und erneuten Anmelden erhalten.


Dieser Artikel enthält Informationen zu Filtern im Arbeitslastausgleich. Informationen zu Filtern in Workfront finden Sie unter [Filterübersicht in Adobe Workfront](../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle Pläne</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Planen Sie bei Verwendung des Lastenausgleichs für ein Team oder im Ressourcenbereich </p>
   <p>Arbeiten, wenn Sie den Lastenausgleich eines Projekts verwenden </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zeigen Sie den Zugriff auf Folgendes an oder höher:</p> 
    <ul> 
     <li> <p>Ressourcenverwaltung</p> </li> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Aufgaben</p> </li> 
     <li> <p>Probleme</p> </li> 
     <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Filter, Ansichten und Gruppierungen</p> </li> 
    </ul> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"><span>Zugriff auf Filter, Ansichten und Gruppierungen beim Erstellen oder Bearbeiten von Filtern bearbeiten</span> </p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Höhere Berechtigungen für Projekte, Aufgaben, Probleme</p>
   <p>Berechtigungen für Filter verwalten, die Sie bearbeiten oder löschen möchten</p>
     </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Übersicht über Filter im Arbeitslastausgleich

Beachten Sie Folgendes beim Arbeiten mit Filtern im Arbeitslastausgleich:

* Je nachdem, von wo aus Sie auf den Lastenausgleich zugreifen, filtert Workfront die Informationen möglicherweise bereits für Sie. Informationen zu vorab angewendeten Filtern finden Sie im Abschnitt [Vorab angewendete Filter im Lastenausgleich](#pre-applied-filters-in-the-workload-balancer) in diesem Artikel.
* Sie können einen Filter erstellen und anwenden, ohne ihn zu speichern, oder Sie können einen Filter speichern, um ihn später wiederzuverwenden.
* Wenn Sie einen Filter anwenden, ohne ihn zu speichern, können Sie zu den ursprünglichen Listen zurückkehren, indem Sie Ihre Seite aktualisieren.
* Sie können von Ihnen erstellte Filter oder Filter anzeigen, die von anderen Benutzern erstellt und für Sie freigegeben wurden.
* Wenn Sie einen freigegebenen Filter löschen oder bearbeiten, wird er auch für alle Personen gelöscht oder bearbeitet, für die er freigegeben ist.
* Wenn Sie in einem Bereich Filter im Arbeitslastausgleich erstellen, sind diese in anderen Bereichen nicht verfügbar.

   Beispielsweise sind Filter, die im Bereich &quot;Ressourcen&quot;erstellt wurden, nicht im Arbeitslastausgleich eines Projekts oder eines Teams verfügbar.

   Informationen darüber, wo Sie den Lastenausgleich finden können, finden Sie unter [Suchen Sie den Lastenausgleich .](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

* Sie können nur die Elemente anzeigen, die mit den ausgewählten Filtern übereinstimmen, die auch mit den Daten in der Timeline übereinstimmen, die auf dem Bildschirm des Workload Balancer angezeigt wird.

## Vorab angewendete Filter im Lastenausgleich {#pre-applied-filters-in-the-workload-balancer}

Der Lastenausgleich zeigt Informationen in zwei separaten Bereichen an:

* **Der nicht zugewiesene Arbeitsbereich**: Arbeitselemente, die noch nicht Benutzern zugewiesen sind.
* **Der zugewiesene Arbeitsbereich**: Arbeitselemente, die Benutzern zugewiesen sind.

   Informationen dazu, was in den einzelnen Bereichen angezeigt wird, finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

>[!IMPORTANT]
>
>Jeder Bereich des Workload Balancers verfügt über einen eigenen Satz von Filtern, die unabhängig voneinander funktionieren. Sie müssen beide Filter konfigurieren, um anzugeben, welche Informationen in den einzelnen Bereichen angezeigt werden sollen.

Der Lastenausgleich zeigt Benutzer und deren Arbeitselemente an.
Die den Benutzern zugewiesenen Arbeitselemente werden nur angezeigt, wenn das Datum der Elemente mit dem auf dem Bildschirm angezeigten Zeitrahmen übereinstimmt.

Je nachdem, von wo aus Sie auf den Lastenausgleich zugreifen, werden die nicht zugewiesenen und zugewiesenen Bereiche bereits nach bestimmten Kriterien gefiltert, wie in der folgenden Tabelle beschrieben:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Workfront-Bereich, in dem Sie auf den Lastenausgleich zugreifen</strong></td> 
   <td><b>Elemente, die standardmäßig im nicht zugewiesenen Arbeitsbereich angezeigt werden</b> </td> 
   <td><b>Elemente, die standardmäßig im Bereich "Zugewiesene Arbeit"angezeigt werden</b> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ressourcenbereich</td> 
   <td>Standardmäßig werden hier keine Elemente angezeigt. Sie müssen Filter anpassen, um Arbeitselemente in diesem Bereich anzuzeigen.</td> 
   <td>Benutzer, die Mitglieder eines Ihrer Teams sind, und deren Arbeitselemente. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Team</td> 
   <td>Arbeitselemente, die dem Team oder dem Team zugewiesen sind, und eine Job-Rolle. </td> 
   <td> <p>Benutzer, die Mitglieder des ausgewählten Teams sind, und deren Arbeitselemente.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ein Projekt</td> 
   <td> <p>Nicht zugewiesene Arbeitselemente oder Elemente, die Teams oder Auftragsrollen im ausgewählten Projekt zugewiesen sind, werden in diesem Bereich angezeigt.</p> </td> 
   <td> <p>Benutzer, die mindestens einem Arbeitselement im ausgewählten Projekt zugewiesen sind, und deren Arbeitselemente im Projekt, wenn der Systemstandardfilter <b>Die Arbeitselemente dieses Projekts</b> ausgewählt ist. </p>

<p>Wenn der Systemstandardfilter <b>Die Arbeitselemente dieses Projekts</b> deaktiviert ist, zeigt der Bereich "Zugewiesene Arbeit"alle Arbeitselemente der Benutzer an, die mindestens einem Element des ausgewählten Projekts zugewiesen sind.  </p> Dieser Filter ist standardmäßig deaktiviert.

<b>NOTIZ</b>
<p>Sie können die Option Alle Benutzer anzeigen im Lastenausgleich eines Projekts aktivieren, um alle Benutzer im System anzuzeigen. Weitere Informationen finden Sie unter <a href="../workload-balancer/navigate-the-workload-balancer.md" class="MCXref xref">Navigieren Sie zum Lastenausgleich .</a></p>

</td> 
  </tr> 
 </tbody> 
</table>

## Filter für den Lastenausgleich erstellen

Der Prozess zum Erstellen von Filtern für die Bereiche &quot;Nicht zugewiesene Arbeit&quot;und &quot;Zugewiesene Arbeit&quot;im Arbeitslastausgleich ist identisch, unabhängig davon, von wo aus Sie auf den Arbeitslastausgleich zugreifen. Informationen zum Auffinden des Lastenausgleichs finden Sie unter [Suchen Sie den Lastenausgleich .](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

Sie können einen Filter von Grund auf neu erstellen oder einen der vordefinierten Filter bearbeiten. Informationen zu vorhandenen Filtern, die Sie bearbeiten können, finden Sie unter [Vorhandenen Filter im Arbeitslastausgleich bearbeiten](#edit-an-existing-filter-in-the-workload-balancer) in diesem Artikel.

1. Wechseln Sie zum Lastenausgleich.

   Informationen zum Zugriff auf den Lastenausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Klicken Sie auf **Filter** icon ![](assets/filter-icon.png) in der oberen rechten Ecke des **Nicht zugewiesene Arbeit** oder **Zugewiesene Arbeit** Gebiete.

   Das Feld &quot;Filter-Builder&quot;wird rechts angezeigt. Der Name des Bereichs, für den Sie den Filter erstellen, wird in der Kopfzeile des Felds angezeigt.

   ![](assets/filters-list-wb-assigned-work-with-filters-listed-nwe-350x377.png)

1. (Optional und bedingt) Wenn Sie im Bereich &quot;Ressourcen&quot;auf den Arbeitslastausgleich zugreifen, wird der vordefinierte Standardfilter möglicherweise bereits auf den Bereich &quot;Zugewiesene Arbeit&quot;angewendet. Sie können eine Kopie des Standardfilters bearbeiten und speichern.

   >[!TIP]
   >
   >Der Filter Standard zeigt Benutzer an, die zu einem Ihrer Teams gehören, sowie deren Arbeitselemente. Sie können eine Kopie dieses Filters bearbeiten.

   Wenn Sie auf [!UICONTROL Lastenausgleich] aus einem Projekt: &quot;[!UICONTROL Die Arbeitselemente dieses Projekts]Der Filter wurde möglicherweise bereits angewendet. Dadurch werden nur Arbeitselemente angezeigt, die Benutzern in diesem Projekt zugewiesen sind. Sie können eine Kopie dieses Filters duplizieren und speichern.

   Standardmäßig wird die [!UICONTROL Lastenausgleich] eines Projekts zeigt alle Arbeitselemente an, die allen Benutzern des Projekts zugewiesen sind.


1. Klicken **Neuer Filter.**

   ![](assets/new-filters-empty-panel-workload-balancer-350x460.png)

1. Gehen Sie wie folgt vor, um einen Filter zu erstellen:

   1. Wählen Sie im ersten Dropdown-Menü einen Feldnamen aus oder klicken Sie auf **Felder durchsuchen** um den Namen eines Felds einzugeben, das nicht standardmäßig angezeigt wird.

      >[!IMPORTANT]
      >
      >Beim Referenzieren von benutzerdefinierten Feldern müssen Sie den Feldnamen und nicht die Feldbezeichnung eingeben. Die Feldbezeichnung wird in einem benutzerdefinierten Formular angezeigt, das an ein Objekt angehängt ist. Informationen zum Unterschied zwischen der Beschriftung und dem Namen eines benutzerdefinierten Felds finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. (Bedingt) Wenn Sie auf **Felder durchsuchen**, geben Sie den Namen eines Felds im **Suche** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

      ![](assets/new-filters-search-for-a-field-highlighted-wb-nwe-350x386.png)

      >[!TIP]
      >
      >Sie können ein Feld aus den folgenden Abschnitten auswählen:
      >
      >* **Letzte Auswahlen**: die Felder, nach denen Sie kürzlich gefiltert haben.
      >* **Vorgeschlagene Felder**: die am häufigsten verwendeten Felder.



   1. Wählen Sie einen Modifikator aus dem zweiten Dropdown-Menü aus. Weitere Informationen zu Workfront-Filtermodifikatoren finden Sie unter [Filter und Bedingungs-Modifikatoren](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).
   1. Wählen Sie einen Wert für das Feld aus, nach dem Sie filtern möchten, oder geben Sie einen Wert ein.

      >[!NOTE]
      >
      > Wenn Sie Arbeitsobjekte aus einem bestimmten Portfolio anzeigen möchten, können Sie den folgenden Filter anwenden: &quot;Portfolio name contains marketing.&quot; Dadurch werden Arbeitselemente angezeigt, die zu einem Portfolio gehören, das &quot;Marketing&quot;im Namen enthält.
      >
      >![](assets/portfolio-name-filter-statement-wb-350x262.png)

   1. (Optional) Klicken Sie auf die **Löschen** icon ![](assets/delete.png) , um ein Filterkriterium zu entfernen.

1. (Optional) Klicken Sie auf **Filter hinzufügen** um ein weiteres Filterkriterium hinzuzufügen, wiederholen Sie dann die Aktionen aus Schritt 4.

   <!--(NOTE: ensure this stays correct)-->

1. Klicken **Anwenden** , um die Ergebnisse des Filters auf den ausgewählten Arbeitslastausgleichsbereich anzuwenden, ohne ihn zu speichern.

   Die Liste der Arbeitselemente wird auf der linken Seite aktualisiert.

   >[!IMPORTANT]
   >
   >Die Ergebnisse werden im Arbeitslast-Balancer angezeigt, wenn alle von Ihnen hinzugefügten Filteranweisungen gleichzeitig &quot;true&quot;sind.

   Der Filter bleibt erhalten, bis Sie die Seite aktualisieren.

   Die **Anwenden** Schaltfläche durch eine **Als neu speichern** Schaltfläche.

1. Klicken **Als neu speichern** , um den Filter für die zukünftige Verwendung zu speichern.

   ![](assets/new-filters-save-as-box-unassigned-area-wb-350x467.png)

   >[!TIP]
   >
   >Klicken **Abbrechen** Sie können jederzeit zum Filterbaubereich zurückkehren.

1. Auswählen **Unbenannter Filter** und geben Sie stattdessen den Namen des neuen Filters ein.
1. Wählen Sie ein Symbol für den neuen Filter aus der **Symbol** Dropdown-Menü.

   ![](assets/new-filters-select-icon-expanded-drop-down-wb.png)

1. (Optional) Fügen Sie eine Beschreibung für den Filter hinzu, um anzugeben, was eindeutig ist. Die Beschreibung wird unter dem Filternamen in der Filterliste angezeigt.
1. Klicken Sie auf **Speichern**.

   Gespeicherte Filter werden im Bereich Eigene Filter des Filterfelds angezeigt.

   Informationen zum Anwenden gespeicherter Filter finden Sie im Abschnitt . [Löschen eines gespeicherten Filters im Lastenausgleich](#delete-a-saved-filter-in-the-workload-balancer) in diesem Artikel.

1. (Bedingt) Bewegen Sie den Mauszeiger über den **Filtersymbol** ![](assets/filter-icon.png) in der oberen rechten Ecke des **Nicht zugewiesene Arbeit** oder **Zugewiesene Arbeit** Bereiche, um eine QuickInfo mit dem Namen oder der Anzahl der aktuell angewendeten Filter anzuzeigen.

   ![](assets/filter-icon-with-number-and-tooltip-with-name-of-filter-wb-nwe-350x98.png)

## Filter duplizieren

Sie können einen Filter duplizieren und bearbeiten, um einen neuen zu erstellen.

1. Wechseln Sie zum Lastenausgleich.

   Informationen zum Zugriff auf den Lastenausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Klicken Sie auf **Filter** icon ![](assets/filter-icon.png) in der oberen rechten Ecke des **Nicht zugewiesene Arbeit** oder **Zugewiesene Arbeit** Gebiete.

   Das Feld &quot;Filter-Builder&quot;wird rechts angezeigt. Der Name des Bereichs, für den Sie den Filter erstellen, wird in der Kopfzeile des Felds angezeigt.

1. Bewegen Sie den Mauszeiger über einen vorhandenen Filter und klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Duplizieren**.

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Bei der Bearbeitung eines Filters können Sie auf die **Mehr** Menü in der linken unteren Ecke des Felds Filter bearbeiten und klicken Sie auf **Duplizieren**.

1. Bearbeiten Sie die folgenden Informationen für den duplizierten Filter:

   * Name

      Standardmäßig lautet der neue Filtername &quot;(Ursprünglicher Filtername) Kopieren&quot;.

   * Symbol
   * Beschreibung
   * Alle Felder, Modifikatoren oder Werte.

1. (Optional) Klicken Sie auf **Filter hinzufügen** , um dem duplizierten Filter weitere Anweisungen hinzuzufügen.
1. Klicken **Speichern** , um den duplizierten Filter im **Meine Filter** Bereich.

   Der ursprüngliche Filter bleibt unverändert und der duplizierte Filter wird als neuer Filter gespeichert.

## Vorhandenen Filter im Arbeitslastausgleich bearbeiten {#edit-an-existing-filter-in-the-workload-balancer}

Sie können einen gespeicherten Filter im Lastenausgleich bearbeiten.

>[!TIP]
>
>Wenn Sie einen für andere freigegebenen Filter bearbeiten, sehen diese auch die Änderungen, die Sie vornehmen.

1. Wechseln Sie zum Lastenausgleich.

   Informationen zum Zugriff auf den Lastenausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. Klicken Sie auf **Filtersymbol** ![](assets/filter-icon.png) in der oberen rechten Ecke des **Nicht zugewiesen** oder **Zugewiesene Arbeit** Gebiete.\
   Der Filter-Builder wird rechts angezeigt.

1. Bewegen Sie den Mauszeiger über den Filter, den Sie bearbeiten möchten, und klicken Sie auf **Bearbeiten** ![](assets/wb-edit-filter-icon.png).

   ![](assets/filter-more-menu-options-wb.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Ändern von Filteranweisungen
   * Klicken **Filter hinzufügen** Hinzufügen neuer Filteranweisungen
   * Klicken Sie auf **Löschen** icon ![](assets/delete.png) um vorhandene Filteranweisungen zu entfernen.

1. (Optional) Klicken Sie auf **Anwenden**.

   Die Ergebnisse werden im Arbeitslast-Balancer auf der linken Seite aktualisiert, um die Änderungen zu veranschaulichen, die Sie am Filter vorgenommen haben.

1. Klicken Sie auf **Speichern.**

   Die Ergebnisse werden im Arbeitslastausgleich auf der linken Seite aktualisiert und der Filter wird mit den von Ihnen ausgewählten neuen Informationen aktualisiert.

## Löschen eines gespeicherten Filters im Lastenausgleich {#delete-a-saved-filter-in-the-workload-balancer}

Beachten Sie Folgendes, bevor Sie einen Filter löschen:

* Gelöschte Filter können nicht wiederhergestellt werden.
* Vordefinierte Filter können nicht gelöscht werden.
* Ein nicht gespeicherter Filter kann nicht gelöscht werden. Sie werden nach dem Abmelden und der erneuten Anmeldung bei Workfront automatisch entfernt.
* Wenn Sie einen freigegebenen Filter löschen, wird er auch für alle Benutzer gelöscht, für die er freigegeben ist.
* Nachdem Sie alle gespeicherten Filter gelöscht haben, wird der Lastenausgleich entsprechend den ursprünglichen Standardeinstellungen angezeigt.

>[!NOTE]
>
>Wenn Sie einen Filter löschen, der für andere freigegeben wurde, wird er auch für diese gelöscht.

1. Wechseln Sie zum Lastenausgleich .
1. Klicken Sie auf **Filtersymbol** ![](assets/filter-icon.png) in der oberen rechten Ecke des **Nicht zugewiesene Arbeit** oder **Zugewiesene Arbeit** Gebiete.\
   Das Feld &quot;Filter-Builder&quot;wird rechts angezeigt.

1. Bewegen Sie den Mauszeiger über einen Filter und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Löschen**.
   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   >Bei der Bearbeitung eines Filters können Sie auf die **Mehr** Menü in der linken unteren Ecke des Felds Filter bearbeiten und klicken Sie auf **Löschen**.

1. (Optional) Klicken Sie auf **Abbrechen** um das Löschen zu vermeiden und zur Filterliste zurückzukehren.
1. Klicken **Löschen** , um den Löschvorgang zu bestätigen.

   Der Filter wird für Sie und alle Benutzer gelöscht, die über entsprechende Berechtigungen verfügen.

## Filter im Arbeitslastausgleich freigeben

Sie können einen von Ihnen erstellten oder von anderen Benutzern für Sie freigegebenen Filter freigeben.

Beachten Sie beim Freigeben von Filtern im Arbeitslade-Balancer Folgendes:

* Sie können Filter für aktive Benutzer, Teams, Rollen und Unternehmen freigeben oder sie für alle Benutzer in Ihrer Workfront-Instanz sichtbar machen.
* Filter, die Sie im Bereich &quot;Ressourcen&quot;freigeben, sind nicht im Arbeitslastausgleich eines Projekts oder eines Teams sichtbar.
* Arbeitslastausgleichsfilter, die Sie für andere freigeben, sind in anderen Bereichen von Workfront nicht sichtbar.

So geben Sie einen Filter frei:

1. Wechseln Sie zum Lastenausgleich .
1. Klicken Sie auf **Filtersymbol** ![](assets/filter-icon.png) in der oberen rechten Ecke des **Nicht zugewiesene Arbeit** oder **Zugewiesene Arbeit** Gebiete.\
   Das Feld &quot;Filter-Builder&quot;wird rechts angezeigt.

1. Bewegen Sie den Mauszeiger über einen Filter und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Freigeben.**

   ![](assets/filter-more-menu-options-wb.png)

   >[!TIP]
   >
   > Bei der Bearbeitung eines Filters können Sie auf die **Mehr** Menü in der linken unteren Ecke des Felds Filter bearbeiten und klicken Sie auf **Freigeben**.

   Das Freigabefeld Filter wird angezeigt.

1. Aktivieren Sie die **Systemweit anzeigen** -Einstellung. Dadurch kann jeder in Workfront den Filter anzeigen.

   Oder

   Beginnen Sie mit der Eingabe der Namen von Benutzern, Teams, Rollen, Gruppen oder Unternehmen, für die Sie den Filter in die **Zugriff auf gewähren** -Feld.

   ![](assets/new-filters-sharing-ui-wb-350x422.png)

1. (Optional) Klicken Sie auf den Rechtspfeil neben dem Namen einer Entität, um ihre Berechtigungen für den Filter zu bearbeiten, und aktivieren Sie dann entweder das **Ansicht** oder **Verwalten** -Option.

   ![](assets/new-filters-granular-permissions-for-manage-wb-350x107.png)

1. (Optional) Aktivieren oder deaktivieren Sie die zusätzlichen Berechtigungen für eine Entität, indem Sie eine der folgenden Aktionen ausführen:

   1. Klicken **Ansicht** und deaktivieren Sie die **Freigeben** -Option. Sie ist standardmäßig aktiviert.

   1. Klicken **Verwalten** und deaktivieren Sie entweder die **Freigeben** oder **Löschen** -Option. Sie sind standardmäßig aktiviert.
   >[!TIP]
   >
   >Benutzer können keine höhere Berechtigung als ihre Zugriffsstufe erhalten. Wenn sie keinen Zugriff auf Filter bearbeiten in ihrer Zugriffsebene haben, können sie keine Berechtigungen zum Verwalten eines Filters erhalten. Workfront deaktiviert die Option Verwalten für diese Benutzer und die Option ist abgeblendet.

1. Klicken **Freigeben**. Der Filter wird für die angegebenen Entitäten freigegeben.

   Die von Ihnen freigegebenen Filter werden im **Freigegeben für mich** Bereich des Filterfelds.

   ![](assets/new-filters-shared-with-me-area-wb-350x236.png)

<!--   

## Add a filter to your favorites list

You can mark a filter as a favorite for quicker access to it. 

The filters that you mark as a favorite do not count towards your system Favorites list. There is no limit for how many filters you can favorite. 

1. Go to the Workload Balancer
1. Click the **Filter** icon ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or **Assigned Work** areas. The filter builder box displays on the right. 
1. Mouse over a filter, then click the **Favorite** ![](assets/favorites-icon-small.png). 
(NOTE: insert screen shot here with Favorite as part of this menu - same as above ones but with Favorite)
1. The filter is listed in the **Favorited** section inside the filter panel. 
1. (Optional) Click the **Favorite** icon again to remove the filter from the list of favorite filters
(I logged bugs for "Favorited" and "Unfavorite" wordings - make sure these have not updated)
-->
