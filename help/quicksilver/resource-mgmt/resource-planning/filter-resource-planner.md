---
product-area: resource-management
navigation-topic: resource-planning
title: Filtern von Informationen im Ressourcenplaner
description: '''(AL:*Iterate on this article: filtering by custom data. Weitere Verbesserungen? Sonderzeichen können sich ändern - folgen Sie der Geschichte, um zu erfahren, wann. Ursprünglich kam es in Beta 3 17.3.)"'
author: Alina
feature: Resource Management
exl-id: 7186cae5-1e16-421e-b26d-afb50aa7f6eb
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '2415'
ht-degree: 0%

---

# Filtern von Informationen im Ressourcenplaner

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(AL:*Iterate on this article: filtering by custom data. Other enhancements? Special characters caveat might change - follow the story to know when. It originally came in Beta 3 17.3.)</p>
-->

Mithilfe von Filtern können Sie ändern, welche Informationen im Ressourcenplaner aus allen im System gespeicherten Informationen angezeigt werden.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte, Benutzer und Ressourcenverwaltung anzeigen oder höher </p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Projekte anzeigen</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Übersicht über die Filter für Ressourcenplaner

Um die im Ressourcenplaner angezeigte Datenmenge zu minimieren, stellt Adobe Workfront einen Standardfilter mit vorkonfigurierten Kriterien bereit. Weitere Informationen zum Standardfilter finden Sie im Abschnitt [Überblick über den Standardfilter im Ressourcenplaner](#overview-of-the-default-filter-in-the-resource-planner) in diesem Artikel.

Sie können auch benutzerdefinierte Filter erstellen. Informationen zum Anpassen von Filtern im Ressourcenplaner finden Sie im Abschnitt [Erstellen von Ressourcenplanern-Filtern](#create-resource-planner-filters) in diesem Artikel.

Beachten Sie bei der Verwendung von Filtern im Ressourcenplaner Folgendes:

* Die von Ihnen erstellten Filter sind nur für Sie sichtbar. Sie können Filter freigeben, um sie für andere Benutzer verfügbar zu machen.
* Als Workfront-Administrator können Sie nur Filter sehen, die Sie erstellen oder die für Sie freigegeben sind.
* Die gefilterten Ergebnisse ändern sich nicht, wenn Sie eine andere Ansicht für den Ressourcenplaner auswählen.\
  Weitere Informationen zum Ändern der Ansicht im Ressourcenplaner finden Sie im Auswahlabschnitt &quot;Projekt-/Rolle-/Benutzeransicht&quot;in der [Navigationsübersicht für Ressourcenplaner](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

* Beim Anwenden eines Filters werden die Zuordnungs- und Verfügbarkeitsdaten im Ressourcenplaner für Projekte, Rollen oder Benutzer nicht geändert. Ein Filter ändert nur die Anzahl der Objekte, die im Ressourcenplaner angezeigt werden.
* Die Filterung gilt für alle Objekte, die gleichzeitig im Ressourcenplaner angezeigt werden. Wenn Sie beispielsweise nach einem bestimmten Benutzer filtern, zeigt der Ressourcenplaner nur die folgenden Ergebnisse an:

   * Projekte, bei denen dieser Benutzer Teil des Ressourcen-Pools ist (für die Projekt- und Rollenansicht) oder eine Zuweisung für das Projekt hat (für die Benutzeransicht)
   * Mit dem Benutzer verknüpfte Rollen für diese Projekte\
     Andere Rollen oder Benutzer in den Projekten, mit denen der Benutzer verknüpft ist, werden nicht angezeigt.

## Übersicht über den Standardfilter im Ressourcenplaner {#overview-of-the-default-filter-in-the-resource-planner}

Wenn Sie den Ressourcenplaner zum ersten Mal öffnen, wendet Workfront den Standardfilter an. Sie können den Standardfilter bearbeiten, um nur nach den Elementen zu filtern, die angezeigt werden sollen. Informationen zum Ändern von Filtern finden Sie im Abschnitt [Filter im Ressourcenplaner bearbeiten](#edit-a-filter-in-the-resource-planner) in diesem Artikel.

Beachten Sie bei Verwendung des Standardfilters Folgendes:

* Der Standardfilter ruft Informationen nur aus Projekten mit folgenden Eigenschaften ab:

   * Ein geplantes Abschlussdatum, das nach dem ersten Datum des aktuellen Monats eintritt
   * Ein geplantes Startdatum, das vor dem letzten Tag des vierten Monats ab dem aktuellen Datum eintritt
   * Status &quot;Aktuell&quot;oder &quot;Planung&quot;

  >[!IMPORTANT]
  >
  >Der Filter Standard ruft Informationen aus den Projekten ab, die immer innerhalb von vier Monaten ab dem ersten Tag des aktuellen Monats auftreten, unabhängig vom Zeitrahmen, den Sie für die Anzeige im Ressourcenplaner auswählen.

* In der Benutzeransicht werden alle Benutzer im System angezeigt, aber nur die mit den gefilterten Projekten verknüpften Benutzer zeigen Stundeninformationen an.
* Sie können die Informationen im Standardfilter bearbeiten, ohne den Filter zu speichern.
* Sie können eine Kopie des Standardfilters duplizieren und bearbeiten, die gewünschten Kriterien darin ändern und sie dann als neuen Filter speichern.
* Der Standardfilter kann nicht gelöscht oder freigegeben werden.

  ![RP_new_default_fitler_kriterien__1_.PNG](assets/rp-new-default-fitler-criteria--1--301x547.png)

## Filter für Ressourcenplaner erstellen {#create-resource-planner-filters}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(Alina: **^ This section is somewhat duplicated (format more than content) from the "Filtering Utilization Information" section in "Viewing Utilization Information for Projects, Programs, and Portfolios.")</p>
-->

Das Erstellen eines Filters im Ressourcenplaner ist für alle Ansichten identisch.

Stellen Sie sicher, dass die Voraussetzungen für die Anzeige der richtigen Informationen im Ressourcenplaner vorhanden sind, bevor Sie einen Filter erstellen.\
Informationen dazu, wie Sie die erforderlichen Voraussetzungen für die Arbeit mit dem Ressourcenplaner erfüllen, finden Sie im Artikel &quot;Voraussetzungen für die Arbeit mit dem Ressourcenplaner&quot;im Abschnitt [Ressourcenplanerübersicht](../../resource-mgmt/resource-planning/get-started-resource-planner.md) .

Beachten Sie beim Erstellen eines Filters Folgendes:

* Die Anzahl der Objekte, nach denen Sie filtern können, ist nicht begrenzt.
* Die verfügbaren Felder, die Sie zu einem Filter hinzufügen können, ändern sich entsprechend dem Objekt der Ansicht, die Sie auf den Ressourcenplaner anwenden. Beispielsweise können Sie nur in der Benutzeransicht nach den Feldern &quot;Problem&quot;oder &quot;Aufgabe&quot;filtern, da diese Objekte nur in der Benutzeransicht angezeigt werden. Wenn Sie einen Filter für Probleme oder Aufgaben in der Ansicht &quot;Benutzer&quot;erstellen und ihn dann auf die Projekt- oder Rollenansichten anwenden, wird er ignoriert, da die Felder nicht in den Projekt- oder Rollenansichten vorhanden sind. In diesem Fall ist der Filter nicht verfügbar.

So erstellen Sie einen Filter im Ressourcenplaner:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Ressourcen**.

   Der **Planer** wird standardmäßig angezeigt.

   Standardmäßig wird beim ersten Zugriff auf den Ressourcenplaner der <strong>Standardfilter</strong> angewendet.<br>Weitere Informationen zum Standardfilter finden Sie im Abschnitt <a href="#overview-of-the-default-filter-in-the-resource-planner" class="MCXref xref">Überblick über den Standardfilter im Ressourcenplaner</a> in diesem Artikel.

1. Klicken Sie in der linken oberen Ecke der auf das Symbol **Filter** .\
   ![filter_icon.png](assets/filter-icon.png)\
   Oder\
   Erweitern Sie das Dropdown-Menü **Filter** und klicken Sie auf **Neuen Filter hinzufügen**.\
   ![](assets/rp-filter-dropdown-expanded-with-default-filter-selected-350x283.png)

1. Um einen Filter mithilfe der integrierten Kriterien zu erstellen, geben Sie eines der folgenden Felder an:

   * **Portfolio**: Geben Sie den Namen des Portfolios ein, das die Informationen enthält, die Sie in den Ressourcenplaner aufnehmen möchten, und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.\
     Wiederholen Sie diesen Vorgang, um Informationen aus mehreren Portfolios einzuschließen.

   * **Projektstatus**: Erweitern Sie das Dropdown-Menü Projektstatus und wählen Sie einen oder mehrere Projektstatus aus, die in der Liste verfügbar sind.
   * **Team**: Beginnen Sie mit der Eingabe des Namens eines oder mehrerer Teams, die mit den Benutzern verknüpft sind, die Aufgaben in den Projekten zugewiesen sind, die Sie anzeigen möchten.
   * **Auftragsrolle**: Beginnen Sie mit der Eingabe des Namens einer oder mehrerer Vorgangsrollen, die mit den Benutzern verknüpft sind, die Aufgaben in den Projekten zugewiesen sind, die Sie anzeigen möchten.
   * **Pools**: Beginnen Sie mit der Eingabe des Namens eines oder mehrerer Ressourcen-Pools, die mit den Projekten (für die Projektansicht) verknüpft sind, der Benutzer (für die Benutzeransicht) oder der sowohl den Projekten als auch den Benutzern (für die Rollenansicht) zugeordnet sind, die Sie anzeigen möchten.
   * **Gruppe**: Beginnen Sie mit der Eingabe des Namens einer oder mehrerer Gruppen, die mit den Benutzern (in der Benutzeransicht) oder Projekten (in den Projekt- und Rollenansichten) verknüpft sind, die Sie anzeigen möchten.

1. Klicken Sie auf **Filterregel hinzufügen** und beginnen Sie dann mit der Eingabe des Feldnamens, nach dem Sie filtern möchten, im Feld **Typ , um Elemente zu filtern** . Wenn das Feld verfügbar ist, wird es für jedes Objekt gefüllt, mit dem es verknüpft werden kann.

   >[!IMPORTANT]
   >
   >Beim Referenzieren von benutzerdefinierten Feldern müssen Sie den Feldnamen und nicht die Feldbezeichnung eingeben. Die Feldbeschriftung wird in einem benutzerdefinierten Formular angezeigt, das an ein Objekt angehängt ist. Informationen zum Unterschied zwischen der Beschriftung und dem Namen eines benutzerdefinierten Felds finden Sie unter [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

1. Klicken Sie auf den Namen des Felds, um es dem Filter hinzuzufügen, wenn es in der Liste angezeigt wird.\
   Weitere Informationen zu den in der Liste angezeigten Feldern finden Sie unter [Glossar der Adobe Workfront-Terminologie](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

1. (Optional) Wählen Sie den Filter und die Bedingungsmodifikatoren für den Filter aus. Die verfügbaren Modifikatoren werden unter [Filter und Bedingungsmodifikatoren](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md) beschrieben.

   Sie können benutzerbasierte oder datumsbasierte Platzhalter verwenden, um nach Informationen zu filtern, die dem angemeldeten Benutzer zugeordnet sind.\
   Informationen zu unterstützten Platzhaltern in Filtern finden Sie unter [Übersicht über Wildcard-Filtervariablen](../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

1. Klicken Sie auf **Speichern** , um die Filterregel zu speichern.
1. (Optional) Klicken Sie auf **Filterregel hinzufügen** , um eine neue Regel für ein anderes Objekt oder Feld hinzuzufügen.
1. Klicken Sie auf **Anwenden** , um den Filter anzuwenden, ohne ihn zu speichern.

   Oder

   Klicken Sie auf **Filter speichern** , um den Filter zu speichern.\
   ![RP_Apply_or_Save_button_on_filters.png](assets/rp-apply-or-save-buttons-on-filters-320x79.png)

1. (Bedingt) Nachdem Sie auf **Speichern** geklickt haben, geben Sie im Dialogfeld **Filter speichern** im Feld **Filtername** einen Namen für den Filter an. Dies ist ein Pflichtfeld.\
   ![RP_new_save_filter_box__with_Save_button__without_apply.png](assets/rp-new-save-filter-box--with-save-button--without-apply-350x175.png)

   >[!NOTE]
   >
   >Wenn Ihr Filtername Sonderzeichen enthält, verwenden Sie nur die folgenden Zeichen:
   >
   >* Komma
   >* Schrägstrich
   >* Bindestrich
   >* Unterstrich

1. Klicken Sie auf **Speichern**.

   Die Ergebnisse im Ressourcenplaner werden nun nach den Informationen gefiltert, die Sie in die Filterregeln aufgenommen haben.

## Vorhandenen Filter anwenden

Wenn Sie oder ein Benutzer mit Zugriff auf den Ressourcen-Planer einen Filter speichern, wird dieser für alle Benutzer verfügbar, die den Ressourcen-Planer verwenden.

So wenden Sie einen vorhandenen Filter an:

1. Wechseln Sie zum Ressourcen-Planer.
1. Erweitern Sie links oben das Dropdown-Menü **Filter** .

   In diesem Menü können Sie von Ihnen erstellte oder für Sie freigegebene Filter anzeigen.\
   ![RP_filter_drop_down.png](assets/rp-filter-drop-down-350x152.png)

1. Wählen Sie im Dropdown-Menü einen Filter aus. In diesem Menü werden Filter angezeigt, die Sie oder andere Benutzer erstellt haben.\
   Wenn Sie einen Filter auswählen, wird dadurch automatisch die Anzahl der im Ressourcenplaner angezeigten Informationen verringert.

## Filter im Ressourcenplaner bearbeiten {#edit-a-filter-in-the-resource-planner}

Sie können einen Filter im Ressourcenplaner bearbeiten, indem Sie einen der folgenden Schritte ausführen:

* [Umbenennen eines Filters](#rename-a-filter)
* [Bearbeiten der Informationen in einem Filter](#edit-the-information-in-a-filter)
* [Filter duplizieren](#duplicate-a-filter)

Wenn Sie einen Filter bearbeiten, wird er für alle Benutzer im System aktualisiert, die Zugriff auf den Ressourcenplaner haben.

### Filter umbenennen {#rename-a-filter}

Sie können den Namen eines Filters ändern, ohne dessen Kriterien zu ändern. Es wird empfohlen, andere Benutzer im System über diese Änderung zu informieren, da Filter für andere Benutzer sichtbar sind. Diese Änderung betrifft die Filterlisten für alle, die den Ressourcenplaner sehen können.

1. Wechseln Sie zum Ressourcenplaner und erweitern Sie das Dropdown-Menü **Filter** , um einen gespeicherten Filter auszuwählen.
1. Erweitern Sie das Dropdown-Menü **Filter** . Suchen Sie den Filter, den Sie umbenennen möchten, und bewegen Sie den Mauszeiger über den Namen.
1. Wählen Sie das Symbol **Filter umbenennen** neben dem Namen des Filters aus.

   ![](assets/rp-filter-options-edit-350x154.png)

1. Geben Sie im Feld **Filtername** einen neuen Namen für den Filter an.
1. Klicken Sie auf **Speichern**.\
   Die im Filter enthaltenen Informationen sind identisch und der Name wird aktualisiert.

### Informationen in einem Filter bearbeiten {#edit-the-information-in-a-filter}

Sie können die Informationen, die Sie in einen Filter einschließen, ändern, ohne dessen Namen zu ändern. Es wird empfohlen, andere Benutzer im System über diese Änderung zu informieren, da Filter für sie sichtbar sind. Diese Änderung betrifft die Filterlisten für alle, die den Ressourcenplaner sehen können.

1. Wechseln Sie zum Ressourcen-Planer und erweitern Sie das Dropdown-Menü **Filter** in der linken oberen Ecke.
1. Wählen Sie einen vorhandenen Filter aus, den Sie bearbeiten möchten.
1. Klicken Sie auf das Symbol **Filter** .\
   ![filter_icon.png](assets/filter-icon.png)

1. Fügen Sie dem Filter neue Felder hinzu.\
   Weitere Informationen zum Erstellen von Filtern finden Sie unter [Erstellen von Ressourcen-Planerfiltern](#create-resource-planner-filters).

1. Bewegen Sie den Mauszeiger über die für den Filter ausgewählten Felder und klicken Sie auf das Symbol **Bearbeiten** , um ein anderes Feld auszuwählen, oder auf das Symbol **Löschen** , um das Feld zu löschen.\
   ![RP_custom_filter_delete_and_edit_icons.png](assets/rp-custom-filter-delete-and-edit-icons-350x169.png)

1. (Optional) Klicken Sie auf **Filterregel hinzufügen** , um dem Filter neue Felder hinzuzufügen.\
   Weitere Informationen zum Definieren von Filterkriterien finden Sie unter [Erstellen von Ressourcen-Planerfiltern](#create-resource-planner-filters).

1. Klicken Sie auf **Anwenden** , um den Filter anzuwenden, ohne ihn zu speichern.

   Oder

   Klicken Sie auf **Speichern** , um den Filter zu speichern.\
   Der Filter wird mit demselben Namen, aber mit neuen Filterkriterien gespeichert.

### Filter duplizieren {#duplicate-a-filter}

Sie können einen vorhandenen Filter duplizieren. Die ursprünglichen Filterkriterien bleiben im duplizierten Filter gleich und Sie können den neuen Filter unter einem neuen Namen speichern.

1. Wechseln Sie zum Ressourcen-Planer und erweitern Sie das Dropdown-Menü **Filter** in der linken oberen Ecke.
1. Bewegen Sie den Mauszeiger über den Namen eines gespeicherten Filters, den Sie duplizieren möchten.
1. Klicken Sie auf das Symbol **Duplizieren** .

   ![](assets/rp-filter-options---duplicate-350x154.png)\
   Das Feld Filter duplizieren wird angezeigt.

1. Geben Sie im Feld **Filtername** einen neuen Namen für den duplizierten Filter an.\
   Der Standardname für den neuen Filter ist *`<Original Filter Name>`(copy)*.

1. Klicken Sie auf **Speichern**. Ein neuer Filter wird mit denselben Kriterien wie der ursprüngliche Filter und einem neuen Namen erstellt.

   >[!NOTE]
   >
   >Obwohl Sie zwei Filter mit demselben Namen und identischen Kriterien haben können, empfehlen wir, Filter mit eindeutigen Filterkriterien und Namen in Ihrem Ressourcenplaner zu speichern, um Verwirrung zu vermeiden.

## Filter löschen

Sie können Filter löschen, wenn sie nicht mehr benötigt werden. Der Standardfilter kann nicht gelöscht werden.

Weitere Informationen zum Standardfilter finden Sie im Abschnitt [Überblick über den Standardfilter im Ressourcenplaner](#overview-of-the-default-filter-in-the-resource-planner) in diesem Artikel.

Wenn Sie einen Filter löschen, wird der Filter für alle Workfront-Benutzer gelöscht, die Zugriff auf den Ressourcenplaner haben. Stellen Sie vor dem Entfernen sicher, dass der Filter, den Sie entfernen möchten, von niemandem mehr verwendet wird, der im Ressourcenplaner arbeitet. Ein gelöschter Filter kann nicht wiederhergestellt werden.

So entfernen Sie einen Filter:

1. Wechseln Sie zum Ressourcen-Planer.
1. Erweitern Sie das Dropdown-Menü **Filter** .
1. Suchen Sie den Filter, den Sie entfernen möchten, und bewegen Sie den Mauszeiger über den Namen.
1. Wählen Sie das Symbol **Filter löschen** neben dem Namen des Filters aus.

   ![](assets/rp-filter-options---delete-350x154.png)

1. Klicken Sie im Dialogfeld **Filter löschen** auf **Löschen** .

1. Der Filter wird gelöscht und aus dem Ressourcenplaner entfernt.

## Filter freigeben

Sie können einen von Ihnen erstellten Filter oder einen Filter freigeben, den Sie für andere Benutzer freigeben können. Sie können den Standardfilter nicht freigeben, aber Sie können ihn duplizieren und die Kopie freigeben.

>[!NOTE]
>
>Alle Benutzer, einschließlich Workfront-Administratoren, können nur auf Filter zugreifen, die sie erstellt haben oder die für sie freigegeben wurden. Sie können einen Filter für bestimmte Benutzer freigeben, um einen Filter für alle Ressourcen-Planer-Benutzer verfügbar zu machen.

Weitere Informationen zum Standardfilter finden Sie im Abschnitt [Überblick über den Standardfilter im Ressourcenplaner](#overview-of-the-default-filter-in-the-resource-planner) in diesem Artikel.

Informationen zum Duplizieren von Filtern finden Sie im Abschnitt [Filter duplizieren](#duplicate-a-filter) in diesem Artikel.

1. Wechseln Sie zum Ressourcen-Planer.
1. Erweitern Sie das Dropdown-Menü **Filter** .
1. Suchen Sie den Filter, den Sie freigeben möchten, und bewegen Sie den Mauszeiger über den Namen.
1. Wählen Sie das Symbol **Filter freigeben** neben dem Namen des Filters aus.

   ![](assets/rp-filter-options---share-350x154.png)

   Das Dialogfeld Filterzugriff wird angezeigt.

1. (Optional) Um den Filter für alle Benutzer des Ressourcenplaners verfügbar zu machen, klicken Sie auf das Symbol **Einstellungen** und wählen Sie dann **Diese Funktion systemweit anzeigen** aus.

   ![](assets/make-this-visible-system-wide-350x119.png)

1. Geben Sie im Feld &quot;**Ressourcentyp-Filterzugriff auf:**&quot;die Namen der Benutzer, Teams, Rollen, Gruppen oder Unternehmen ein, für die Sie den Filter freigeben möchten.
1. Wählen Sie aus den folgenden Berechtigungsebenen aus:

   * Anzeigen
   * Verwalten

     Informationen zu Berechtigungen in Workfront finden Sie unter [Überblick über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)

1. (Optional) Klicken Sie auf **Erweiterte Einstellungen** s , um Berechtigungen für jede Ebene hinzuzufügen, indem Sie sie auswählen oder Berechtigungen für jede Ebene entfernen, indem Sie deren Auswahl aufheben.

   ![](assets/rp-share-filter-manage-advanced-settings-350x271.png)

1. Klicken Sie auf **Speichern**.

   Der Filter wird für die von Ihnen ausgewählten Entitäten freigegeben und im Bereich **Für mich freigegeben** angezeigt.

   ![](assets/rp-shared-with-me-area.png)
