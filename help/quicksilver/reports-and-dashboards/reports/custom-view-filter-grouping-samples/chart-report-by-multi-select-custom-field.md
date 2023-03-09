---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Bericht anhand eines benutzerdefinierten Mehrfachauswahlfelds grafisch darstellen
description: Sie können einen Bericht nicht nach einem benutzerdefinierten Mehrfachfeld ordnen. Sie müssen ein zusätzliches berechnetes Feld erstellen, das auf das benutzerdefinierte Mehrfachauswahlfeld verweist, um den Bericht auch nach dem Wert des benutzerdefinierten Mehrfachfelds zu kartieren.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: 23257f11b0795aa1f1e422923f6d596017c58126
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Bericht anhand eines benutzerdefinierten Mehrfachauswahlfelds grafisch darstellen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung verfügbar.</span>

Sie können einen Bericht nicht nach einem benutzerdefinierten Mehrfachfeld ordnen. Sie müssen ein zusätzliches berechnetes Feld erstellen, das auf das benutzerdefinierte Mehrfachauswahlfeld verweist, um den Bericht auch nach dem Wert des benutzerdefinierten Mehrfachfelds zu kartieren.

## Zugriffsanforderungen

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie ein berechnetes benutzerdefiniertes Feld erstellen, das die aus dem benutzerdefinierten Mehrfachfeld ausgewählten Werte anzeigt. Weitere Informationen finden Sie unter [Erstellen Sie ein berechnetes benutzerdefiniertes Feld, das auf ein benutzerdefiniertes Mehrfachauswahlfeld verweist.](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) in diesem Artikel.

## Bericht mit Mehrfachauswahl benutzerdefinierter Felder im Diagramm darstellen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

Sie können kein Diagramm in einem Bericht erstellen, indem Sie auf ein benutzerdefiniertes Feld mit Mehrfachauswahl verweisen. Stattdessen können Sie ein berechnetes Feld erstellen, das die Werte des benutzerdefinierten Mehrfachfelds für ein bestimmtes Objekt und eine bestimmte Gruppe anhand des berechneten Felds aufzeichnet. 

* [Erstellen Sie ein berechnetes benutzerdefiniertes Feld, das auf ein benutzerdefiniertes Mehrfachauswahlfeld verweist.](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Erstellen Sie ein Diagramm, das auf ein berechnetes benutzerdefiniertes Feld verweist.](#build-a-chart-that-references-a-calculated-custom-field)

### Erstellen Sie ein berechnetes benutzerdefiniertes Feld, das auf ein benutzerdefiniertes Mehrfachauswahlfeld verweist. {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Um ein berechnetes Feld erstellen zu können, das auf ein benutzerdefiniertes Mehrfachauswahlfeld verweist, müssen folgende Voraussetzungen erfüllt sein:

* Erstellen Sie das benutzerdefinierte Mehrfachauswahlfeld in einem benutzerdefinierten Formular.\
   Informationen zum Erstellen benutzerdefinierter Formulare und zum Hinzufügen benutzerdefinierter Felder finden Sie im Artikel [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Hängen Sie das benutzerdefinierte Formular an Objekte an.
* Füllen Sie das benutzerdefinierte Feld mit Mehrfachauswahl mit einem Wert für jedes Objekt.

So erstellen Sie das berechnete benutzerdefinierte Feld, das auf das benutzerdefinierte Mehrfachauswahlfeld verweist:

1. Erstellen Sie ein benutzerdefiniertes Formular oder bearbeiten Sie ein vorhandenes.\
   Informationen zum Erstellen benutzerdefinierter Formulare finden Sie im Artikel [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Wählen Sie das Objekt oder die Objekte aus, die Sie für das benutzerdefinierte Formular verwenden möchten.
1. Klicken **Feld hinzufügen**, dann **Berechnet** , um das benutzerdefinierte Feld mit mehreren Auswahlen zum Formular hinzuzufügen.

1. Im **Titel** geben Sie dem neuen berechneten Feld einen Namen, um anzugeben, dass es auf das benutzerdefinierte Feld mit mehreren Auswahlen verweist.\
   Beispiel: &quot;Berechnetes Mehrfachauswahlfeld-Feld&quot;.

1. Im **Berechnung** geben Sie folgenden Code ein:

   ```
   {DE:Multi-select Custom Field}
   ```

1. Ersetzen Sie &quot;Benutzerdefiniertes Feld mit Mehrfachauswahl&quot;durch den tatsächlichen Namen Ihres benutzerdefinierten Mehrfachauswahlfelds, wie er in Workfront angezeigt wird.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Optional) Wenn sich das benutzerdefinierte Feld mit mehreren Auswahlen bereits in diesem Formular befindet und dieses Formular bereits an Objekte angehängt ist, aktivieren Sie die **Vorherige Berechnungen aktualisieren** -Option.\
   Dadurch wird sichergestellt, dass das neue Feld automatisch mit dem Wert aus dem benutzerdefinierten Mehrfachfeld ausgefüllt wird, da es zu den Formularen hinzugefügt wird, die bereits an die Objekte angehängt sind.

1. Klicken **Fertig**.
1. Klicken **Speichern +Schließen**.

### Erstellen Sie ein Diagramm, das auf ein berechnetes benutzerdefiniertes Feld verweist. {#build-a-chart-that-references-a-calculated-custom-field}

1. (Optional) Um sicherzustellen, dass alle berechneten Felder, nach denen Sie ein Diagramm erstellen möchten, mit Werten gefüllt sind, wählen Sie alle Objekte in Ihrem Bericht aus, die das benutzerdefinierte Formular mit dem benutzerdefinierten Mehrfachfeld und dem berechneten Feld enthalten, und klicken Sie dann auf **Bearbeiten**.
1. (Optional und bedingt) Aktivieren Sie die **Benutzerdefinierte Ausdrücke neu berechnen** und klicken Sie auf **Änderungen speichern**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   ><span class="preview">Diese Option wurde aus der Massenbearbeitung von Projekten in der Vorschau-Umgebung entfernt.  Sie können Ausdrücke für Projekte weiterhin stapelweise neu berechnen, indem Sie auf **Mehr** ![](assets/more-icon-45x33.png) am Anfang einer Projektliste und **Ausdrücke neu berechnen**. </span>


1. Rufen Sie den Bericht auf, in dem Sie die Grafik für das berechnete Feld hinzufügen möchten, das auf das benutzerdefinierte Feld mit Mehrfachauswahl verweist.
1. Klicken **Berichtaktionen**, dann **Bearbeiten**.

1. Wählen Sie die <strong>Gruppierungen</strong> Registerkarte und klicken Sie dann auf <strong>Gruppierung hinzufügen</strong>.
1. Fügen Sie die<strong>Berechnetes Mehrfachauswahlfeld</strong> die Sie als Gruppierung erstellt haben.
1. Wählen Sie die <strong>Diagramm</strong> und fügen Sie dem Bericht ein Diagramm hinzu.<br>Informationen zum Hinzufügen eines Diagramms zu einem Bericht finden Sie im Abschnitt <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Diagramm zu einem Bericht hinzufügen</a> im Artikel <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Benutzerdefinierten Bericht erstellen</a>.
1. Wählen Sie die <strong>Berechnetes Mehrfachauswahlfeld</strong> als eines der im Diagramm anzuzeigenden Felder.
1. Klicken <strong>Speichern und schließen</strong>.<br>Der Bericht zeigt die Ergebnisse, die nach dem Feld für die Mehrfachauswahl mit berechneten Werten gruppiert wurden, in einer Grafik an.
