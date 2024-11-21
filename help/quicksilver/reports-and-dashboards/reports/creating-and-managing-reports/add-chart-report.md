---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Diagramm zu einem Bericht hinzufügen
description: Sie können Ihre Berichte durch Hinzufügen eines Diagramms erweitern. Sie können Diagramme zu vorhandenen Berichten oder zu Berichten hinzufügen, die Sie erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 9b58d68c-4b7b-4344-bde3-7c65e2e1aac8
source-git-commit: 9396cd2ac073a57b7d99618cdf09e54ddcf95130
workflow-type: tm+mt
source-wordcount: '2734'
ht-degree: 0%

---

# Diagramm zu einem Bericht hinzufügen

<!--Audited: 11/2024-->

Sie können Ihre Berichte durch Hinzufügen eines Diagramms erweitern. Sie können Diagramme zu vorhandenen Berichten oder zu Berichten hinzufügen, die Sie erstellen.

Bevor Sie einem Bericht ein Diagramm hinzufügen, sollten Sie eine Ansicht und eine Gruppierung für den Bericht erstellen.

Sie können den meisten Berichten nur dann Grafiken hinzufügen, wenn Sie die Informationen im Bericht zuerst gruppieren. Das einzige Diagramm, das ohne Gruppierung hinzugefügt werden kann, ist ein Lichtraumdiagramm.

Weitere Informationen zu Ansichten finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Weitere Informationen zu Gruppierungen finden Sie unter [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Wenn Ihr Bericht zu viele Elemente anzeigt, wird kein Diagramm erstellt. In diesem Fall müssen Sie dem Bericht auch einen Filter hinzufügen, um die Anzahl der Ergebnisse in Ihrem Bericht zu reduzieren.

Weitere Informationen zu Filtern finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Diagramm zu einem Bericht hinzufügen

1. Öffnen Sie einen vorhandenen Bericht oder erstellen Sie einen neuen. Weitere Informationen zum Erstellen eines neuen Berichts finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. (Bedingt) Wenn Sie zu einem vorhandenen Bericht gewechselt sind, klicken Sie auf **Berichtaktionen** > **Bearbeiten**.

1. Stellen Sie sicher, dass die Registerkarte **Spalten (Ansicht)** aktualisiert wurde, um die Informationen anzuzeigen, die Sie im Bericht grafisch darstellen möchten.

   Informationen zum Erstellen oder Ändern der Berichtsansicht finden Sie unter [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

1. Klicken Sie auf die Registerkarte **Gruppierungen** und fügen Sie eine Gruppierung hinzu.

   >[!TIP]
   >
   >* Sie können einem Bericht nur dann eine Grafik hinzufügen, wenn die Berichtsergebnisse gruppiert sind.
   >* Gruppierungen im Textmodus werden in Diagrammen nicht unterstützt. Weitere Informationen zu Textmodusgruppierungen finden Sie unter [Textmodus in einer Gruppierung bearbeiten](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-grouping.md).
   >* Wenn Sie eine einzelne Gruppierung hinzufügen, die eine Metrik darstellt, werden in allen Diagrammen mit Ausnahme eines Tortendiagramms alle Ergebnisse in der Gruppierung in derselben Farbe angezeigt.

   Weitere Informationen zum Erstellen von Gruppierungen finden Sie unter [Erstellen von Gruppierungen in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-groupings.md).

1. Wählen Sie die Registerkarte **Diagramm** aus.

1. Klicken Sie auf einen Diagrammtyp, um ihn auszuwählen.\
   ![Grafiktyp auswählen](assets/unshimmed-report-builder-chart.png)

1. Wählen Sie aus den folgenden Grafiktypen aus:

   * [Spaltendiagramm](#column-chart)
   * [Balkendiagramm](#bar-chart)
   * [Tortendiagramm](#pie-chart)
   * [Liniendiagramm](#line-chart)
   * [Diagrammdiagramm](#gauge-chart)
   * [Punktdiagramm](#bubble-chart)

1. Klicken Sie auf **Speichern + Schließen** , um das Diagramm und den Bericht zu speichern.

### Spaltendiagramm {#column-chart}

So fügen Sie Ihrem Bericht ein **Spalte** -Diagramm hinzu:

1. Beginnen Sie mit dem Hinzufügen eines Diagramms zu Ihrem Bericht, wie unter [Hinzufügen eines Diagramms zu einem Bericht](#add-a-chart-to-a-report) beschrieben.

1. Wählen Sie im Feld **Linke (Y) Achse** die Werte aus, die Sie auf der Y-Achse des Diagramms einbeziehen möchten, und wählen Sie dann aus, wie die Informationen im Feld **Zusammengefasst von** dargestellt werden sollen.

1. (Optional) Klicken Sie auf **Benutzerdefinierte Farben** , um jeder Spalte die gewünschten Farben zuzuweisen.\
   Weitere Informationen zum Anpassen der Diagrammfarben finden Sie unter [Anpassen der Diagrammfarben](#customize-chart-colors).

1. Wählen Sie im Feld **Untere (X) Achse** die Gruppierung aus, die Sie in das Diagramm aufnehmen möchten.

1. (Optional) Klicken Sie auf **In 3D anzeigen** , um das Diagramm in einer dreidimensionalen Ansicht anzuzeigen.

1. (Optional) **Gruppenspalten**: Wählen Sie diese Option, um festzulegen, wie die Spalten gruppiert werden sollen.\
   Wählen Sie aus den folgenden Optionen aus:

   * Klicken Sie auf eine der folgenden Optionen, um festzulegen, wie die gruppierten Spalten angezeigt werden sollen:

      * **Seite um Seite**
      * **gestapelt**
      * **Gestapelt zu 100 %**

   * Wählen Sie die Gruppierung, die Sie in die Grafik aufnehmen möchten, aus dem Dropdown-Menü **Gruppendaten nach** aus.
   * (Optional) Klicken Sie auf **Benutzerdefinierte Farben** , um die Farben der Spalten anzupassen.\
     Weitere Informationen zum Anpassen der Diagrammfarben finden Sie unter [Anpassen der Diagrammfarben](#customize-chart-colors).

1. (Optional) Klicken Sie auf **Kombinationsdiagramm** , um einen zusätzlichen Wert in das Diagramm aufzunehmen und festzulegen, wie die Informationen zusammengefasst werden sollen.\
   Beachten Sie die folgenden Optionen:

   * **Auf Sekundäre Achse zeichnen**: Wählen Sie diese Option, um die Daten auf der rechten Seite des Diagramms darzustellen.
   * **Diagrammtyp**: Wählen Sie aus, ob dieser zusätzliche Wert als Zeile oder dritte Spalte angezeigt werden soll.

1. Klicken Sie auf **Speichern + Schließen** , um das Diagramm und den Bericht zu speichern.

### Balkendiagramm {#bar-chart}

So fügen Sie Ihrem Bericht ein **Balkendiagramm** hinzu:

1. Beginnen Sie mit dem Hinzufügen eines Diagramms zu Ihrem Bericht, wie unter [Hinzufügen eines Diagramms zu einem Bericht](#add-a-chart-to-a-report) beschrieben.

1. Wählen Sie im Feld **Untere (X) Achse** die Werte aus, die Sie auf der X-Achse des Diagramms einbeziehen möchten, und wählen Sie dann aus, wie die Informationen im Feld **Zusammengefasst durch** zusammengefasst werden sollen.

1. (Optional) Klicken Sie auf **Benutzerdefinierte Farben** , um die Farben der Balken anzupassen.\
   Weitere Informationen zum Anpassen der Diagrammfarben finden Sie unter [Anpassen der Diagrammfarben](#customize-chart-colors).

1. Wählen Sie im Feld **Linke (Y) Achse** die Gruppierung aus, die Sie in das Diagramm aufnehmen möchten.

1. (Optional) Klicken Sie auf **In 3D anzeigen** , um das Diagramm in einer dreidimensionalen Ansicht anzuzeigen.

1. (Optional) Klicken Sie auf **Gruppenbalken** , um festzulegen, wie die Balken gruppiert werden sollen.\
   Wählen Sie aus den folgenden Optionen aus:

   * Klicken Sie auf eine der folgenden Optionen, um festzulegen, wie die gruppierten Balken angezeigt werden sollen:

      * **Seite um Seite**
      * **gestapelt**
      * **Gestapelt zu 100 %**

   * Wählen Sie aus dem Dropdownmenü **Gruppendaten nach** aus, wie Sie die Informationen im Diagramm gruppieren möchten.
   * (Optional) Klicken Sie auf **Benutzerdefinierte Farben** , um die Farben Ihrer Spalten anzupassen.\
     Weitere Informationen zum Anpassen der Diagrammfarben finden Sie unter [Anpassen der Diagrammfarben](#customize-chart-colors).

1. (Optional) Klicken Sie auf **Kombinationsdiagramm** , um einen zusätzlichen Wert in das Diagramm aufzunehmen und festzulegen, wie die Informationen zusammengefasst werden sollen.

1. Klicken Sie auf **Speichern + Schließen** , um das Diagramm und den Bericht zu speichern.

>[!IMPORTANT]
>
>Begrenzen Sie Balkendiagramme auf 23 oder weniger Balken, da Balkendiagramme mit mehr als 23 Balken nicht alle Balkendiagramme korrekt anzeigen.

### Tortendiagramm {#pie-chart}

So fügen Sie Ihrem Bericht ein **Tortendiagramm** hinzu:

1. Beginnen Sie mit dem Hinzufügen eines Diagramms zu Ihrem Bericht, wie unter [Hinzufügen eines Diagramms zu einem Bericht](#add-a-chart-to-a-report) beschrieben.

1. Wählen Sie im Feld **Werte** die Werte aus, die im Bericht angezeigt werden sollen, und wählen Sie dann aus, wie die Informationen im Feld **Zusammengefasst durch** zusammengefasst werden sollen.\
   Wählen Sie im Feld **Kanten** die Gruppierung aus, die Sie in das Diagramm aufnehmen möchten. Die Gruppierung wird durch die Kanten der Grafik dargestellt.

1. (Optional) Klicken Sie auf **Benutzerdefinierte Farben** , um die Farben der Kanten im Diagramm anzupassen.\
   Weitere Informationen zum Anpassen der Diagrammfarben finden Sie unter [Anpassen der Diagrammfarben](#customize-chart-colors).

1. (Optional) Klicken Sie auf **In 3D anzeigen** , um das Diagramm in einer dreidimensionalen Ansicht anzuzeigen.

1. Wählen Sie im Feld **Ergebnisse anzeigen als** aus, wie die Ergebnisse im Diagramm dargestellt werden sollen. Beachten Sie die folgenden Optionen:

   * **Prozentsatz**: Die Diagrammergebnisse werden als Prozentsatz angezeigt.
   * **Zahlen**: Die Diagrammergebnisse werden als Zahl angezeigt.

1. Klicken Sie auf **Speichern + Schließen** , um das Diagramm und den Bericht zu speichern.

### Liniendiagramm {#line-chart}

So fügen Sie Ihrem Bericht ein **Liniendiagramm** hinzu:

1. Beginnen Sie mit dem Hinzufügen eines Diagramms zu Ihrem Bericht, wie unter [Hinzufügen eines Diagramms zu einem Bericht](#add-a-chart-to-a-report) beschrieben.

1. Wählen Sie im Feld **Linke (Y) Achse** die Werte aus, die Sie auf der Y-Achse des Diagramms einbeziehen möchten, und wählen Sie dann aus, wie die Informationen im Feld **Zusammengefasst von** dargestellt werden sollen.

1. Wählen Sie im Feld **Untere (X) Achse** die Gruppierung aus, die Sie in das Diagramm aufnehmen möchten.

1. (Optional) Klicken Sie auf **Gruppenzeilen** , um eine zusätzliche Gruppierung für das Diagramm auszuwählen.\
   (Optional) Klicken Sie auf **Benutzerdefinierte Farben** , um die Farben für die neue Gruppierung anzupassen.\
   Weitere Informationen zum Anpassen der Diagrammfarben finden Sie unter [Anpassen der Diagrammfarben](#customize-chart-colors).

1. (Optional) Klicken Sie auf **Kombinationsdiagramm** , um Ihre Zeilen mit einem zusätzlichen Wert zu kombinieren.\
   Beachten Sie die folgenden Optionen:

   * Wählen Sie den Wert aus, den Sie in die Grafik aufnehmen möchten, sowie die Art und Weise, wie die Informationen zusammengefasst werden sollen.
   * Klicken Sie auf das Feld **Auf Sekundäre Achse positionieren** , um die Daten auf der rechten Seite des Diagramms darzustellen.

1. Klicken Sie auf **Speichern + Schließen** , um das Diagramm und den Bericht zu speichern.

### Diagrammdiagramm {#gauge-chart}

Ein Diagramm **Messung** zeigt die Anzahl der Datensätze an, die bestimmte Kriterien im Spurformat erfüllen. Der Indikator der Messung zeigt die Anzahl der Datensätze an, die den in der Ansicht und Gruppierung des Berichts ausgewählten Kriterien entsprechen. Zum Konfigurieren eines Diagramms ist keine Berichtsgruppierung erforderlich.

So fügen Sie Ihrem Bericht ein **Seiten**-Diagramm hinzu:

1. Beginnen Sie mit dem Hinzufügen eines Diagramms zu Ihrem Bericht, wie unter [Hinzufügen eines Diagramms zu einem Bericht](#add-a-chart-to-a-report) beschrieben.

1. Wählen Sie im Feld **Werte** die Werte aus, die im Bericht angezeigt werden sollen, und wählen Sie dann aus, wie die Informationen im Feld **Zusammengefasst durch** zusammengefasst werden sollen. Wenn Sie **Anzahl der Datensätze** auswählen, sind die angezeigten Werte das Objekt des Berichts.

1. Wählen Sie im Feld **Indikatoren** die Gruppierung aus, die Sie in das Diagramm aufnehmen möchten. Die Gruppierung wird durch die Indikatorlinie im Diagramm dargestellt.\
   Wenn die Gruppierung zwei Elemente enthält, werden zwei Indikatoren im Diagramm angezeigt.\
   Wenn Sie z. B. eine Gruppierung des Projektstatus haben und zwei Projektstatus vorliegen (Aktuell und Bei Halten), enthält Ihr Bilddiagramm zwei Kennzahlindikatoren. Sie werden auf die Anzahl der Projekte verweisen, die sich in diesem Status befinden.\
   (Optional) Wählen Sie **Total** im Feld **Indicators** aus, um die Gesamtzahl der im Feld **Werte** ausgewählten Objekte anzuzeigen.

1. (Optional) Klicken Sie auf **Neuen Wertebereich hinzufügen** , um dem Diagramm einen Wertebereich hinzuzufügen.

1. (Optional) Geben Sie im Feld **Wertebereich** den Wertebereich und die Farbe an, die für die Werte gelten sollen, die im Diagrammdiagramm angezeigt werden sollen.

1. Klicken Sie auf **Speichern + Schließen** , um das Diagramm und den Bericht zu speichern.

### Punktdiagramm {#bubble-chart}

Sie können bis zu drei Felder eines Objekts in einem **Punktdiagramm** anzeigen. Das bedeutet, dass Sie bis zu vier Datenpunkte in einem Punktdiagramm anzeigen können. Jede Entität mit drei verbundenen Feldern wird als Kreis angezeigt, der zwei der Felder innerhalb ihrer Position innerhalb der X- und Y-Achsen ausdrückt. Das dritte Feld wird durch die Größe des Kreises dargestellt.

So fügen Sie Ihrem Bericht ein **Punktdiagramm** hinzu:

1. Beginnen Sie mit dem Hinzufügen eines Diagramms zu Ihrem Bericht, wie unter [Hinzufügen eines Diagramms zu einem Bericht](#add-a-chart-to-a-report) beschrieben.

1. Wählen Sie im Feld **Linke (Y) Achse** die Werte aus, die Sie auf der Y-Achse des Diagramms einbeziehen möchten. Die Werte stammen aus der Sicht des Berichts. Geben Sie an, wie die Informationen im Feld **Zusammengefasst von** zusammengefasst werden sollen.

1. Wählen Sie im Feld **Untere (X) Achse** die Werte aus, die Sie auf der X-Achse des Diagramms einbeziehen möchten. Die Werte stammen aus der Sicht des Berichts. Geben Sie an, wie die Informationen zusammengefasst werden sollen.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie mindestens eine Spalte haben, die zusammengefasst ist, damit dieses Feld aktiv ist.\
   >Weitere Informationen zur Zusammenfassung der Informationen in einer Berichtsspalte finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Wählen Sie im Feld **Blasengröße** die Werte aus, die Sie durch die Größe der Blasen im Diagramm darstellen möchten. Die Werte stammen aus der Sicht des Berichts. Geben Sie an, wie die Informationen zusammengefasst werden sollen.

   >[!NOTE]
   >
   >Stellen Sie sicher, dass Sie mindestens eine Spalte haben, die zusammengefasst ist, damit dieses Feld aktiv ist.\
   >Weitere Informationen zur Zusammenfassung der Informationen in einer Berichtsspalte finden Sie unter [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Wählen Sie im Feld **Blasen** die Gruppierung aus, die Sie in das Diagramm aufnehmen möchten. Die Gruppierung wird durch die Platzierung der Punkte im Diagramm dargestellt.

1. Wählen Sie im Feld **Blasenfarbe** das Feld aus, das durch die Farben der Blasen dargestellt werden soll.

   Die **Blasenfarbe** kann eine Gruppierung sein, die Sie im Bericht definieren. Die Option ist jedoch nur verfügbar, wenn Sie eine Gruppierung im Feld **Blasen** auswählen, die den **Namen** eines übergeordneten Objekts relativ zum Objekt des Berichts enthält, z. B. **Projektname** für einen Aufgabenbericht oder **Programmname** für einen Projektbericht.

   Wenn Sie beispielsweise **Projektname** in einem Aufgabenbericht ausgewählt haben, können Sie **Aufgabenstatus** als Feld **Blasenfarbe** hinzufügen.

   ![](assets/bubbles-field-correct-can-select-bubbles-color-example.png)

   Wenn Sie jedoch **Aufgabenstatus** für das Feld **Blasen** ausgewählt haben, können Sie kein Feld **Blasenfarbe** auswählen. Sie können auch nicht &quot;**Projektname**&quot;für das Feld **Blasenfarbe**&quot;auswählen, selbst wenn Sie &quot;**Projektname**&quot;für das Feld **Blasen**&quot;auswählen.

   ![](assets/bubbles-field-wrong-cannot-select-bubbles-color-example.png)

1. Klicken Sie auf **Speichern + Schließen** , um die Änderungen am Oberflächenaufbau zu speichern.

## Grafikfarben anpassen {#customize-chart-colors}

Sie können Workfront die Farben der Elemente in Ihrem Diagramm auswählen lassen oder diese anpassen, während Sie Ihren Berichten ein Diagramm hinzufügen. Wenn Ihr Diagramm eine Gruppierung enthält, die eine Metrik darstellt, z. B. einen Aufgabenbericht, der die Anzahl der nach dem tatsächlichen Abschlussdatum gruppierten Aufgaben anzeigt, wird jedes Ergebnis in der Gruppierung in derselben Farbe angezeigt.

Sie können nur eine Farbe für die Felder auswählen, die in der Berichtansicht angezeigt werden. Für die in der Berichtsgruppierung angezeigten Felder können Sie mehrere Farben auswählen - eine für jede Option.

>[!IMPORTANT]
>
>Bei Datumsfeldern können Sie nur eine Farbe für Ihre Diagrammelemente auswählen.

So passen Sie Diagrammfarben an:

1. Gehen Sie beim Erstellen eines Berichts zur Registerkarte **Diagramm** in ReportBuilder.

1. Wählen Sie einen Diagrammtyp aus, den Sie Ihrem Bericht hinzufügen möchten.\
   Weitere Informationen zum Hinzufügen eines Diagramms zum Bericht finden Sie unter [Hinzufügen eines Diagramms zu einem Bericht](#add-a-chart-to-a-report).

1. Klicken Sie auf **Benutzerdefinierte Farben** , wenn dieses Feld verfügbar ist.\
   Das Dialogfeld Benutzerdefinierte Farben wird angezeigt.\
   ![](assets/unshimmed-custom-colors-in-charts.png)

   >[!NOTE]
   >
   >Sie können benutzerdefinierte Farben mit jedem Feld verknüpfen, das Sie gruppieren können, und mit einigen Feldern, die in einer Ansicht angezeigt werden können, einschließlich benutzerdefinierten Feldern. Bei den benutzerdefinierten Feldern oder benutzerdefinierten Optionen der Felder, die Sie im Dialogfeld &quot;Benutzerdefinierte Farbe&quot;auswählen, wird zwischen Groß- und Kleinschreibung unterschieden.

1. Wählen Sie eine der folgenden Optionen aus:

   * **Use one color**: Alle Elemente des Diagramms werden in der ausgewählten Farbe angezeigt.
   * **Farbe hinzufügen**: Fügen Sie eine benutzerdefinierte Farbe für einen möglichen Wert des ausgewählten Felds hinzu.
   * **Alle entfernen**: Wählen Sie diese Option, um alle oben angegebenen Feldwerte und Farben zu entfernen.
   * **Kein Wert**: Wählen Sie dieses Feld und eine benutzerdefinierte Farbe aus, um die Diagrammspalte anzuzeigen, in der &quot;kein Wert&quot;gruppiert ist. Dies sind Elemente, die nicht nach einer der Optionen des in Ihrer Gruppierung ausgewählten Felds gruppiert werden können.
   * **Alle anderen Werte**: Wählen Sie dieses Feld und eine benutzerdefinierte Farbe aus, um alle anderen Diagrammelemente anzuzeigen, deren Optionen oben nicht definiert sind.

     >[!NOTE]
     >
     >Die zuletzt bearbeiteten Farben werden rechts neben der Schaltfläche **Benutzerdefinierte Farben** angezeigt. Wenn Sie den Mauszeiger über eine Farbe bewegen, wird der Name des mit ihr verknüpften Felds angezeigt. Sie können auch auf eine Farbe klicken, um sie zu bearbeiten, ohne erneut **Benutzerdefinierte Farben** zu öffnen.

1. So wählen Sie eine Farbe:
Klicken Sie in die Farbauswahl, um eine Farbe auszuwählen.
ODER
Geben Sie einen hexadezimalen Farbwert für Ihre Farbe an.

1. Klicken Sie auf eine beliebige Stelle außerhalb des Dialogfelds &quot;Benutzerdefinierte Farben&quot;, um es zu schließen. Die ausgewählten Farben werden automatisch gespeichert.

1. Klicken Sie auf **Speichern + Schließen** , um das Diagramm zu speichern und den Bericht auszuführen.

## Grafik exportieren

Sie können ein Diagramm in eine PDF-Datei exportieren.

So exportieren Sie eine Grafik:

1. Klicken Sie auf der Registerkarte &quot;Diagramm&quot;eines Berichts auf **Exportieren** , um das Diagramm in das PDF-Format zu exportieren.\
   Eine PDF-Datei wird auf Ihren Computer heruntergeladen.

1. Öffnen Sie die PDF-Datei.\
   Die exportierte Datei enthält die folgenden Informationen:

   * Ein Bild des Diagramms.
   * Ein Titel, der den Namen des Berichts angibt.
   * Ein eindeutiger Dateiname, der auf dem Namen des Berichts basiert.
   * Fußzeile mit Datum und Uhrzeit des Exports des Berichts und der Seitenzahl.

## Grafiken aus Berichten entfernen

So entfernen Sie ein Diagramm aus einem Bericht:

1. Öffnen Sie die Registerkarte **Diagramm** des ReportBuilder.

1. Klicken Sie auf die Schaltfläche &quot;x&quot;rechts neben den Grafiktypen, um die Grafik zu entfernen.

1. Klicken Sie auf **Speichern + schließen**.

## Einschränkungen beim Arbeiten mit Diagrammen

Beachten Sie beim Arbeiten mit Diagrammen die folgenden Einschränkungen:

* Der Abschnitt **Diagrammvorschau** rechts neben ReportBuilder enthält keine tatsächlichen Daten aus Ihrem Bericht. Sie müssen das Diagramm speichern und es auf der Registerkarte **Diagramm** anzeigen, um das Diagramm mit Ihren Daten anzuzeigen.

* Einige Diagrammelemente können nicht bearbeitet werden:

   * Sie können den Schrifttyp und die Größe der Werte der einzelnen Elemente nicht ändern.
   * Die Namen der Achsen im Diagramm können nicht geändert werden.

* Die Legende des Diagramms kann nicht bearbeitet werden.
* Bei der Verwendung berechneter Felder für Gruppierungen ist ein Klick auf die Diagrammelemente nicht möglich.
* Die größte Anzahl von Datenpunkten, die Sie in einem Diagramm anzeigen können, beträgt vier in einem Punktdiagramm. Alle anderen Diagrammtypen zeigen zwei oder maximal drei Datenpunkte an.
