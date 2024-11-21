---
title: Verwalten von Datensätzen im Planungsabschnitt von Adobe Workfront-Objekten
description: Sie können die mit Adobe Workfront-Objekten verknüpften Workfront-Planungsdatensätze im Planungsabschnitt eines Workfront-Objekts im linken Bereich anzeigen.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: 9629558bfc2c4fa7fb040bcc45534164e0d8b3b4
workflow-type: tm+mt
source-wordcount: '1493'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Datensatzverbindungen über Workfront-Objekte verwalten

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>.

{{planning-important-intro}}

Sie können Workfront-Planungsdatensätze und die mit Adobe Workfront-Objekten verbundenen Datensätze in den folgenden Bereichen in Workfront anzeigen:

* Planungsabschnitt eines Workfront-Objekts: Zeigt alle Datensatztypen an, die mit einem Objekt und den zugehörigen Datensätzen verbunden sind.
* <span class="preview">Ein benutzerdefiniertes Feld für die Planung einer Verbindung: Zeigt einen Datensatztyp und die entsprechenden verbundenen Datensätze an. </span>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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
<p>Alle</p>
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p>
   </td>

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
   <td> <p>Anzeigen oder Aufrufen von Projekten, Programmen und Portfolios</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <p>Zeigen Sie in Workfront die Berechtigungen für ein Projekt, Portfolio oder Programm an oder höher</a> </p> 
   <p>Zeigen Sie in der Workfront-Planung die Berechtigungen für einen Arbeitsbereich an, um verbundene Datensätze oder Contribute oder höhere Berechtigungen für einen Arbeitsbereich zum Verbinden oder Trennen von Datensätzen anzuzeigen</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche der Workfront-Planung, einschließlich derjenigen, die sie nicht erstellt haben</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Um den Planungsbereich oder den Planungsabschnitt für ein Workfront-Objekt anzuzeigen, müssen allen Benutzern, einschließlich Workfront-Administratoren, eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü und den Planungsbereich für Projekte, Portfolios und Programme enthält. </p> Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Übersicht über den Zugriff auf die Adobe-Planung</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verwalten von Datensätzen im Abschnitt &quot;Planung&quot;

Sie können den Abschnitt Planung eines Workfront-Objekts verwenden, um alle mit dem Workfront-Objekt verbundenen Datensatztypen und die entsprechenden Datensätze anzuzeigen.
Der Abschnitt Planung ist für die folgenden Workfront-Objekte verfügbar:

* Projekt
* Portfolio
* Programm
<!--* Group
* Company-->

### Überlegungen zum Abschnitt &quot;Planung&quot;von Workfront-Objekten

Beachten Sie Folgendes, wenn Sie Workfront Planning-Datensätze im Planungsabschnitt eines Workfront-Objekts anzeigen:

* Die Datensatztypen für die Workfront-Planung müssen zunächst mit den Workfront-Objekttypen verbunden werden.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Datensatztypen verbinden](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md)
* Sie können den Planungsabschnitt von einem Workfront-Objekt aus anzeigen, selbst wenn dem Workfront-Objekt keine Datensätze zugeordnet sind.

### Datensatzverbindungen im Abschnitt Planung verwalten

{{step1-to-planning}}

1. Klicken Sie auf die Karte eines Arbeitsbereichs.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf die Karte eines Datensatztyps, der mit einem Workfront-Projekt, -Portfolio oder -Programm verbunden ist.
1. Wechseln Sie zu einem verbundenen Datensatzfeld, das über eine Verbindung mit einem Workfront-Objekt verfügt, entweder in der Tabellenansicht oder auf der Detailseite eines Datensatzes. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).
1. Klicken Sie im Feld &quot;Verbundener Datensatz&quot;auf den Namen eines Workfront-Objekts.
Die Seite des Objekts wird in Workfront geöffnet.

   >[!NOTE]
   >
   >  Wenn Sie ein Workfront-Objekt kennen, das bereits mit einem Planungsdatensatz verbunden ist, können Sie vom Workfront-Objekt aus zum Abschnitt Planung navigieren.

1. Klicken Sie im linken Bereich auf **Planung** .

   >[!NOTE]
   >
   >   Ihr Workfront- oder Gruppenadministrator muss den Bereich Planung zu Ihrer Layoutvorlage hinzufügen, bevor er für ein Workfront-Projekt, -Portfolio oder -Programm angezeigt wird.

   Der Abschnitt Planung wird mit den folgenden Informationen angezeigt:

   * Die verbundenen Datensätze werden auf einzelnen Karten angezeigt, die die folgenden Informationen enthalten:
      * Name des Datensatzes
      * Die Miniaturansicht des Datensatzes
      * Der Name des verbundenen Datensatzfelds, wie er in der Workfront-Planung angezeigt wird.
   * Datensätze werden unter ihrem jeweiligen Arbeitsbereich und Datensatztyp angezeigt.

   ![](assets/planning-section-on-project.png)

1. (Optional) Klicken Sie auf **Alle Verbindungen anzeigen** , um alle verbundenen Datensatztypen anzuzeigen, einschließlich der Typen ohne verbundene Datensätze. Standardmäßig werden Datensatztypen ohne verbundene Datensätze nicht angezeigt.
1. Klicken Sie auf eine Datensatzkarte, um weitere Informationen zum Datensatz anzuzeigen. Das Vorschaufeld für Datensätze wird angezeigt.
1. (Optional) Beginnen Sie mit der Änderung der Felder im Vorschaufeld des Datensatzes. Ihre Änderungen werden automatisch gespeichert.
1. (Optional) Klicken Sie oben rechts im Vorschaufenster auf das Symbol **In einer neuen Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) , um die Detailseite des Datensatzes zu öffnen. Die Detailseite des Datensatzes wird in der Workfront-Planung geöffnet.
1. (Optional) Bewegen Sie den Mauszeiger über eine Datensatzkarte, klicken Sie auf das Symbol zum Trennen des Datensatzes **-** und klicken Sie dann auf **Trennen**.
Folgendes geschieht:
   * Der Datensatz ist nicht mehr mit dem Workfront-Objekt verbunden.
   * Das Workfront-Objekt wird auch aus dem verbundenen Feld des Datensatzes aus der Workfront-Planung entfernt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden ebenfalls gelöscht.
1. Klicken Sie auf **Verbinden** , um weitere Datensätze für die verbundenen Datensatztypen zu verbinden. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).

   Folgendes geschieht:

   * Die Datensätze sind sofort mit dem Workfront-Objekt verbunden und werden im Abschnitt Planung angezeigt.
   * Das Workfront-Objekt wird dem Verbindungsfeld des Workfront-Planungsdatensatzes hinzugefügt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden in der Workfront-Planung ausgefüllt.

<div class="preview">

## Verwalten von Datensätzen im Feldtyp Planen der Verbindung

Sie können ein benutzerdefiniertes Verbindungsfeld für ein Workfront-Objekt verwenden, um einen Datensatztyp und die entsprechenden mit dem Workfront-Objekt verbundenen Datensätze anzuzeigen.

Sie können steuern, welche Datensatztypen für das Workfront-Objekt geplant werden, wenn Sie benutzerdefinierte Felder für die Planungsverbindung erstellen.

* Im Feld Verbindungsplanung werden die Planungsdatensätze angezeigt, nachdem eine Verbindung hergestellt wurde und das Feld an Formulare für die folgenden Workfront-Objekte angehängt ist:

   * Projekt
   * Portfolio
   * Programm
   * Gruppe
   * Firma

Weitere Informationen finden Sie unter [Erstellen eines Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Überlegungen zum Planungs-Verbindungs-Feldtyp

Beachten Sie Folgendes, wenn Sie Workfront Planning-Datensätze aus einem Verbindungsfeld für ein Workfront-Objekt anzeigen:

* Sie können nur einen Datensatztyp mit einem Verbindungsfeld Planung verknüpfen.
* Sie müssen ein benutzerdefiniertes Formular mit einem benutzerdefinierten Feld für die Planungsverbindung an ein Workfront-Objekt anhängen, das über die Workfront-Planung verbunden werden kann, wenn Sie über den richtigen Zugriff verfügen.
* Die Datensatztypen für die Workfront-Planung müssen zunächst mit den Workfront-Objekttypen verbunden werden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
* Sie können Datensätze nur für Objekte mit Workfront-Planungs-Verbindungen über das Verbindungsfeld Planen eines Workfront-Objekts verbinden oder trennen.
* Sie müssen über Contribute-Berechtigungen für einen Arbeitsbereich in der Workfront-Planung verfügen, um Datensätze über das Verbindungsfeld Planung eines Workfront-Objekts verbinden oder trennen zu können.
* Sie können ein Verbindungsfeld für die Planung nicht bearbeiten, wenn Sie Workfront-Objekte stapelweise bearbeiten.

### Verwalten von Datensatzverbindungen über den Feldtyp Planungsverbindung

1. Wechseln Sie zu einem der folgenden Objektarten, die mit einem Workfront Planning-Record-Typ verbunden sind:

   * Projekt
   * Portfolio
   * Programm
   * Firma
   * Gruppe

1. Klicken Sie im linken Bereich auf **&lt; Objekt > Details** .
1. (Bedingt) Fügen Sie ein benutzerdefiniertes Formular mit mindestens einem Verbindungsfeld Planen für das ausgewählte Objekt hinzu, falls eines nicht vorhanden ist.

   >[!NOTE]
   >
   >Ihr Workfront- oder Gruppenadministrator muss zunächst das Formular erstellen und ein Verbindungsfeld für die Planung hinzufügen, bevor Sie es zu einem Objekt hinzufügen können.


1. Klicken Sie in das Feld, um verbundene Datensätze hinzuzufügen, und klicken Sie dann auf den Pfeil nach unten innerhalb des Felds, um Datensätze aus der Liste auszuwählen.

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Es ist nicht möglich, Datensätze zu Verbindungsfeldern der Planung hinzuzufügen, die mit anderen Workfront-Objekten als dem bei der Feldkonfiguration ausgewählten Objekt verknüpft sind.
   >
   >Beispielsweise können Sie keinem Verbindungsfeld Planung Datensätze hinzufügen, das für eine Projektverbindung über das benutzerdefinierte Formular eines Portfolios erstellt wurde.
   >
   >Es gibt einen Hinweis darauf, dass das Objekt des Felds und das von Ihnen ausgewählte Objekt nicht übereinstimmen.
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Klicken Sie außerhalb der Liste, um sie zu schließen.

   Folgendes geschieht:

   * Die Datensätze sind sofort mit dem Workfront-Objekt verbunden und werden im Feld Planen der Verbindung sowie im Abschnitt Planung des Workfront-Objekts angezeigt.
   * Das Workfront-Objekt wird dem Verbindungsfeld des Workfront-Planungsdatensatzes hinzugefügt.
   * Die Werte für die Workfront-Suchfelder, die mit dem Planungsdatensatz verbunden sind, werden in der Workfront-Planung ausgefüllt.
1. (Optional) Klicken Sie im Feld Verbindung planen auf den Namen eines Datensatzes, um ihn in der Workfront-Planung zu öffnen.
Die Registerkarte Datensatzdetails wird in der Workfront-Planung geöffnet.
Sie können Informationen zum Datensatz überprüfen oder zur Seite mit dem Datensatztyp navigieren.

1. (Optional) Klicken Sie im benutzerdefinierten Formular in Workfront auf das Symbol **Entfernen** ![](assets/remove-icon.png) für einen Datensatz, um ihn aus dem Feld Planungs-Verbindung zu entfernen und vom Workfront-Objekt zu trennen.
Das Workfront-Objekt wird vom Planungsdatensatz getrennt und alle Lookup-Informationen aus Workfront werden aus dem Datensatz entfernt.

</div>