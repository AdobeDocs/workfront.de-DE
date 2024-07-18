---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Referenzieren eines benutzerdefinierten Formulars in einem Bericht
description: Sie können die benutzerdefinierten Formulare eines Objekts in den Ansichten, Filtern und Gruppierungen eines Berichts für dieses Objekt referenzieren.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '1000'
ht-degree: 2%

---

# Referenzieren eines benutzerdefinierten Formulars in einem Bericht

Sie können die benutzerdefinierten Formulare eines Objekts in den Ansichten, Filtern und Gruppierungen eines Berichts für dieses Objekt referenzieren.

Sie können auf den Inhalt von benutzerdefinierten Formularen verweisen, die in einen Bericht aufgenommen werden sollen, oder Sie können Informationen über die benutzerdefinierten Formulare selbst referenzieren, um sie in einen Bericht aufzunehmen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
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
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Das benutzerdefinierte Formular muss vorhanden sein, bevor Sie es in einem Bericht referenzieren können.

Weitere Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter [Entwerfen eines Formulars mit dem Formularentwickler](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Referenzieren des Inhalts benutzerdefinierter Formulare

Sie können Felder in benutzerdefinierten Formularen referenzieren. Nachdem ein benutzerdefiniertes Formular auf ein Objekt angewendet wurde, können alle mit diesem benutzerdefinierten Formular verknüpften Felder wie jedes andere Feld im Objekt in einem Bericht referenziert werden.

>[!NOTE]
>
>Für Felder mit mehreren Optionen sind alle Optionen in den Filtern und Eingabeaufforderungen des Berichts verfügbar, einschließlich der ausgeblendeten Optionen.\
>Weitere Informationen zum Ausblenden von Optionen in einem benutzerdefinierten Feld mit mehreren Optionen finden Sie im Artikel [Formular mit dem Formularentwickler entwerfen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Verwenden Sie beim Erstellen des Berichts einfach den Objekttyp des Formulars als Feldquelle und verwenden Sie den Namen des benutzerdefinierten Felds als Feldnamen.

Sie können beispielsweise ein benutzerdefiniertes Formular auf alle Projekte anwenden, die das benutzerdefinierte Feld **Berater** enthalten. Um einen Bericht zu erstellen, in dem alle Projekte aufgelistet sind, bei denen Olivia Kim als Berater tätig ist, verwenden Sie den Objekttyp **Projekt** als Feldquelle und verwenden Sie **Berater** als Feldnamen. Setzen Sie den Filterqualifizierer auf **Equal** und geben Sie dann Olivia Kim ein.

![](assets/qs-consultant-filter-example-350x126.png)

Weitere Informationen zum Erstellen eines Berichts finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Referenzinformationen zu benutzerdefinierten Formularen

Sie können Informationen zu benutzerdefinierten Formularen referenzieren, z. B. den Namen von benutzerdefinierten Formularen, die mit einem Objekt verknüpft sind.

&#x200B; Je nach Element (Ansicht, Filter oder Gruppierung) können Sie auf eine der folgenden Arten verweisen:

* Das primäre benutzerdefinierte Formular, das auf ein Objekt angewendet wird:

  Dies ist das Formular, das zuerst auf der Detailseite des Objekts angezeigt wird.

* Alle benutzerdefinierten Formulare (wenn mehr als ein benutzerdefiniertes Formular auf ein Objekt angewendet wird)

Sie können benutzerdefinierte Formulare in Ansichten, Filtern und Gruppierungen referenzieren:

* [Verweisen auf benutzerdefinierte Formulare in einer Berichtsansicht (Spalte)](#reference-custom-forms-in-a-report-view-column)
* [Verweisen auf benutzerdefinierte Formulare in einem Berichtsfilter](#reference-custom-forms-in-a-report-filter)
* [Referenzieren benutzerdefinierter Formulare in einer Berichtsgruppierung](#reference-custom-forms-in-a-report-grouping)

### Referenzieren benutzerdefinierter Formulare in einer Berichtsansicht (Spalte) {#reference-custom-forms-in-a-report-view-column}

So zeigen Sie alle mit einem Objekt verknüpften benutzerdefinierten Formulare an:

1. Beginnen Sie mit der Erstellung eines Berichts, wie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.
1. Erweitern Sie auf der Registerkarte **Spalten** den Objekttyp, auf den das benutzerdefinierte Formular, auf das Sie verweisen möchten, angewendet wird, und klicken Sie dann auf **Kategoriename**.\
   Um beispielsweise alle benutzerdefinierten Formulare anzuzeigen, die mit einer Aufgabe verknüpft sind, erweitern Sie die Feldquelle **Aufgabe** und klicken Sie dann auf den Feldnamen **Kategoriename** .\
   ![](assets/qs-category-name-column-350x267.png)

So zeigen Sie nur das primäre benutzerdefinierte Formular an, das mit dem Objekt verknüpft ist:

1. Beginnen Sie mit der Erstellung eines Berichts, wie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.
1. Erweitern Sie auf der Registerkarte **Spalten** die Feldquelle **Kategorie** und klicken Sie dann auf den Feldnamen **Name** .\
   ![](assets/qs-category-name-column-2-350x248.png)

### Referenzieren benutzerdefinierter Formulare in einem Berichtsfilter {#reference-custom-forms-in-a-report-filter}

So filtern Sie nach allen benutzerdefinierten Formularen, die mit dem Objekttyp verknüpft sind:

1. Beginnen Sie mit der Erstellung eines Berichts, wie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.
1. Erweitern Sie auf der Registerkarte **Filter** den Eintrag **Kategorien** und klicken Sie dann auf **Name**.\
   ![](assets/qs-categories-name-filter-350x311.png)

1. Wählen Sie den Bedingungsbezeichner aus, den Sie verwenden möchten:

   * Leer
   * Nicht leer
   * Enthält
   * Enthält nicht
   * Gleich (ignoriert Groß- und Kleinschreibung)
   * Ungleich

   Weitere Informationen zu den einzelnen Qualifikatoren finden Sie im Artikel [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Wenn das Feld, für das Sie filtern, mehrere Optionen hat und Sie die Qualifikatoren **Nicht gleich** oder **Enthält nicht** verwenden, werden die Ergebnisse herausgefiltert, die nur die von Ihnen angegebene Auswahl enthalten. Wenn das Feld zusätzliche Optionen einschließlich der angegebenen enthält, werden diese Ergebnisse nicht aus dem Bericht gefiltert. Dazu gehört das Filtern nach mehreren benutzerdefinierten Forms, wenn diese an dasselbe Objekt angehängt sind.

1. Geben Sie den Namen des benutzerdefinierten Formulars ein, nach dem Sie filtern möchten, und klicken Sie dann auf den Namen, wenn es in der Dropdown-Liste angezeigt wird.
1. (Optional) Klicken Sie auf **Andere Filterregel hinzufügen** und wiederholen Sie dann die Schritte 2 bis 4, um weitere Filterregeln zu erstellen.
1. Klicken Sie auf **Speichern+Schließen**.

So filtern Sie nur nach dem primären benutzerdefinierten Formular, das mit dem Objekttyp verknüpft ist:

1. Beginnen Sie mit der Erstellung eines Berichts, wie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.
1. Erweitern Sie auf der Registerkarte **Filter** die Feldquelle **Kategorie** und klicken Sie dann auf den Feldnamen **Name** .\
   ![](assets/qs-category-name-filter-350x437.png)

1. Wählen Sie den Bedingungsbezeichner aus, den Sie verwenden möchten:

   * Leer
   * Nicht leer
   * Enthält
   * Enthält nicht
   * Gleich (ignoriert Groß- und Kleinschreibung)
   * Ungleich

   Weitere Informationen zu den einzelnen Qualifikatoren finden Sie im Artikel [Filter und Bedingungsmodifikatoren](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Geben Sie den Namen des benutzerdefinierten Formulars ein, nach dem Sie filtern möchten, und klicken Sie dann auf den Namen, wenn es in der Dropdown-Liste angezeigt wird.
1. (Optional) Klicken Sie auf **Andere Filterregel hinzufügen** und wiederholen Sie dann die Schritte 2 bis 4, um weitere Filterregeln zu erstellen.
1. Klicken Sie auf **Speichern+Schließen**.

### Referenzieren benutzerdefinierter Formulare in einer Berichtsgruppierung {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>Sie können Elemente nur nach dem primären benutzerdefinierten Formular gruppieren, das mit dem Objekt verknüpft ist. Sie können Elemente nicht nach allen Formularen gruppieren, die mit dem Objekt verknüpft sind.

1. Beginnen Sie mit der Erstellung eines Berichts, wie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.
1. Erweitern Sie auf der Registerkarte **Gruppierungen** den Eintrag **Kategorie** und klicken Sie dann auf **Name**.\
   ![](assets/qs-category-name-grouping-350x373.png)
