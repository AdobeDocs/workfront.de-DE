---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Erstellen und Verwalten benutzerdefinierter Ansichten in [!DNL Workfront Proof]
description: Sie können benutzerdefinierte Ansichten Ihrer Dateien und Testsendungen erstellen, um die gewünschten Elemente so aufzulisten, wie sie angezeigt werden sollen. Sie können die Informationen auch in Ihrer benutzerdefinierten Ansicht als Bericht exportieren (in CSV, durch Kommas getrennten Wert, Dateiformat).
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 7c6f3fdd-f767-4e8d-937a-1c7645aba55b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2458'
ht-degree: 0%

---

# Erstellen und Verwalten benutzerdefinierter Ansichten in [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Dieser Artikel bezieht sich auf die Funktionalität im eigenständigen Produkt [!DNL Workfront Proof]. Informationen zum Testen innerhalb von [!DNL Adobe Workfront] finden Sie unter [Testversand](../../../review-and-approve-work/proofing/proofing.md).

Sie können benutzerdefinierte Ansichten Ihrer Dateien und Testsendungen erstellen, um die gewünschten Elemente so aufzulisten, wie sie angezeigt werden sollen. Sie können die Informationen auch in Ihrer benutzerdefinierten Ansicht als Bericht exportieren (in CSV, durch Kommas getrennten Wert, Dateiformat).

>[!NOTE]
>
>Benutzerdefinierte Ansichten sind nur bei Auswahl- und Premium-Plänen verfügbar. Wenden Sie sich an unser Verkaufsteam, um ein Angebot zu erhalten.

## Erstellen einer benutzerdefinierten Ansicht

Wenn Sie eine benutzerdefinierte Ansicht erstellen, können Sie Folgendes auswählen:

* Ob Testsendungen, Dateien oder beides enthalten sein sollen
* Welche Spalten werden angezeigt?
* Nach welcher Spalte sortiert werden soll
* Die Sortierreihenfolge für die Spalte (aufsteigend oder absteigend)
* Welche Filtertypen werden verwendet, um zu bestimmen, welche Informationen in der Ansicht enthalten sind

Nachdem die benutzerdefinierte Ansicht erstellt wurde, kann sie sofort verwendet werden. Der Name der neuen Ansicht ist auch im Dropdown-Menü unter der Überschrift Meine benutzerdefinierten Ansichten (unter den Standardansichten) enthalten.

So erstellen Sie eine benutzerdefinierte Ansicht:

1. Rufen Sie die Seite **[!UICONTROL Ansichten]** auf.
1. Weitere Informationen zu Ansichten finden Sie unter [Elemente auf der Ansichtsseite verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).
1. Führen Sie je nachdem, ob Sie eine neue benutzerdefinierte Ansicht von Grund auf neu erstellen möchten, einen der folgenden Schritte aus oder erstellen Sie eine neue benutzerdefinierte Ansicht basierend auf einer vorhandenen Standardansicht:

   * Um eine neue benutzerdefinierte Ansicht basierend auf einer vorhandenen Standardansicht zu erstellen: Wählen Sie aus dem Dropdown-Menü die vorhandene Standardansicht aus, die Sie als Grundlage für Ihre neue benutzerdefinierte Ansicht verwenden möchten. Klicken Sie auf das Symbol **[!UICONTROL Anzeigeeinstellungen]** und dann auf **[!UICONTROL Kopieren]** , um eine neue benutzerdefinierte Ansicht anzuzeigen.

   * ![](assets/proof-custom-view-icon.png)

   * So erstellen Sie eine neue benutzerdefinierte Ansicht von Grund auf: Klicken Sie auf das Symbol **[!UICONTROL Neue Ansicht]** .
   * ![](assets/proof-newview.png)

1. Geben Sie im Abschnitt **[!UICONTROL Details]** die folgenden Informationen an:

   * **[!UICONTROL Name]** (erforderlich): Der Name für die neue Ansicht. Verwenden Sie einen eindeutigen Namen, damit Benutzer die benutzerdefinierte Ansicht im Dropdown-Menü in den Ansichten leicht finden können.
   * **[!UICONTROL Elemente]**: Wählen Sie aus, ob sowohl Testsendungen als auch Dateien, nur Testsendungen oder nur Dateien in der Ansicht enthalten sein sollen. Standardmäßig sind sowohl Testsendungen als auch Dateien enthalten.

1. Legen Sie im Abschnitt **[!UICONTROL Spalten]** fest, welche Spalten Sie in die benutzerdefinierte Ansicht aufnehmen möchten.

   1. Klicken Sie auf das Symbol mit dem Pfeil nach rechts.
   1. ![](assets/proof-view-rightarrow.png)

   1. Doppelklicken Sie auf den Namen der ausgewählten Spalte.
   1. Sie müssen mindestens eine Spalte auswählen. Eine Spalte kann nur einmal hinzugefügt werden.
   1. Wählen Sie eine Spalte aus dem Bereich **[!UICONTROL Verfügbare Spalten]** aus, den Sie in die neue Ansicht aufnehmen möchten.
   1. Die Spalten werden aus der Liste **[!UICONTROL Verfügbare Spalten]** in die Liste **[!UICONTROL Ausgewählte Spalten]** verschoben.

   1. Sie können aus den Standardspalten auswählen oder benutzerdefinierte Felder und Entscheidungsgründe als Spalten in Ihrer benutzerdefinierten Ansicht auswählen. (Wenn Sie diese in Ihrem Konto konfiguriert haben, werden sie unter der Standardliste des Bereichs Verfügbare Spalten angezeigt.)
   1. Standardspalten, die eingeschlossen werden können

      <table style="table-layout:auto">
      <thead>

      </thead>
      <tbody>  
      <tr>   
      <td><strong>Name der aktiven Bühne</strong></td>   
      <td>Name der aktiven Phase im automatisierten Workflow.</td>  
      </tr>  
      <tr>   
      <td><strong>Kommentare</strong></td>   
      <td>Anzahl der eingegangenen Stellungnahmen.</td>
      </tr>  
      <tr>   
      <td><strong>Zähler</strong></td>
      <td>Zeigt eine Nummer des Testversands an, der in Ihr Konto hochgeladen wurde (Sie müssen in den Kontoeinstellungen eine Option für den Testversand-Zähler aktivieren).</td>
      </tr>
      <tr>
      <td><strong>Erstellt</strong></td>
      <td>Datum und Uhrzeit der Erstellung des Elements.</td>
      </tr>
      <tr>
      <td><strong>Erstellerin oder Ersteller</strong></td>
      <td>Der Benutzer, der das Element erstellt hat.</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Datum zum Testversand hinzugefügt]</strong></td>
      <td>Das Datum, an dem Sie zum Testversand hinzugefügt wurden. </td>
      </tr>
      <tr>
      <td><strong>Frist</strong></td>
      <td>Die Frist für den gesamten Nachweis.</td>
      </tr>
      <tr>
      <td><strong>Entscheidungen</strong></td>
      <td>Die Anzahl der von der erwarteten Anzahl gegebenen Entscheidungen (z. B. 0 von 1, 1 von 1 usw.)</td>
      </tr>
      <tr>
      <td><strong>[!UICONTROL Downloads]</strong></td>
      <td>Die Häufigkeit, mit der die Originaldatei heruntergeladen wurde.</td>
      </tr>
      <tr>
      <td><strong>Dateiname</strong></td>
      <td>Der Name der Datei oder des Testversands.</td>
      </tr>
      <tr>
      <td><strong>Ordner</strong></td>
      <td>Der Ordner mit dem Element.</td>
      </tr>
      <tr>
      <td><strong>Letzte Aktivität</strong></td>
      <td>Datum und Uhrzeit der letzten Aktivität des Elements.</td>
      </tr>
      <tr>
      <td><strong>Neueste Entscheidung über</strong></td>
      <td>Datum und Uhrzeit der letzten Entscheidung.</td>
      </tr>
      <tr>
      <td><strong>Meine Deadline</strong></td>
      <td>Ihre eigene Frist für die Testsendungen, in der Sie explizit als Validierer/Genehmiger hinzugefügt werden (falls zutreffend).</td>
      </tr>
      <tr>
      <td><strong>Besitzerin bzw. Besitzer</strong></td>
      <td>Der Eigentümer des Artikels.</td>
      </tr>
      <tr>
      <td><strong>Land des Eigentümers</strong></td>
      <td>Das im System für den Eigentümer des Testversands eingetragene Land. </td>
      </tr>
      <tr>
      <td><strong>Übergeordneter Testversand</strong></td>
      <td>Der Name des übergeordneten Testversands.</td>
      </tr>
      <tr>
      <td><strong>Fortschritt</strong></td>
      <td><p>Fortschrittsleiste. Zeigt Testsendungen an, die noch nicht gestartet, geöffnet, kommentiert oder entschieden wurden.</p><p>Diese Informationen werden nicht sortiert.</p></td>
      </tr>
      <tr>
      <td><strong>Name des Korrekturabzugs</strong></td>
      <td>Der Name des Testversands.</td>
      </tr>
      <tr>
      <td><strong>Testversandtyp</strong></td>
      <td><p>Der Typ des Testversands: Statische Datei, statische Webseite, interaktives Web (.zip-Upload), interaktive Webseite (https), Video, Audio und Sonstige. </p><p>Kombinierte Testsendungen werden als "kombinierter Testversand-Typ"identifiziert. Dateityp des Testversands.</p></td>
      </tr>
      <tr>
      <td><strong>Dateigröße (MB)</strong></td>
      <td><p>Dateigröße des Testversands in Bezug auf das Speicherplatzkontingent.</p><p>Diese Informationen enthalten die aktuelle Version des Testversands. Wenn es keine aktuelle Version gibt, gilt dies für die neueste Version.</p></td>
      </tr>
      <tr>
      <td><p> </p><p><strong>Bearbeitungsetappe</strong></p></td>
      <td>Deadline der Phasen im automatisierten Workflow.</td>
      </tr>
      <tr>
      <td><strong>Staging-Name</strong></td>
      <td>Name der einzelnen Phasen des automatisierten Workflows. Dies umfasst vergangene Phasen, aktive Phasen und zukünftige Phasen.</td>
      </tr>
      <tr>
      <td><strong>Status</strong></td>
      <td>Aktiv, gesperrt, Entwurf oder Gesendet.</td>
      </tr>
      <tr>
      <td><strong>Status</strong></td>
      <td>Ausstehend, erforderliche Änderungen, Mit Änderungen genehmigt, Genehmigt oder Nicht relevant.</td>
      </tr>
      <tr>
      <td><strong>Tags</strong></td>
      <td>Alle Tags, die an das Element angehängt sind.</td>
      </tr>
      <tr>
      <td><strong>Bevorstehende Staging-Namen</strong></td>
      <td> Name der einzelnen Phasen, die noch nicht im automatisierten Workflow gestartet wurden. </td>
      </tr>
      <tr>
      <td><strong>Versionszähler</strong></td>
      <td> Die Anzahl der Versionen des Elements. </td>
      </tr>
      <tr>
      <td><strong>Versionsnummer des Testversands</strong></td>
      <td><i>Die Versionsnummer des Testversands.</i></td>
      </tr> 
      </tbody>
      </table>

   1. (Optional) Führen Sie einen der folgenden Schritte aus, um die Spalte in den Bereich **[!UICONTROL Ausgewählte Spalten]** zu verschieben, damit sie in die neue Ansicht aufgenommen wird:

      * Ordnen Sie alle Spalten in der Liste **[!UICONTROL Ausgewählte Spalten]** neu an.
      * Die Reihenfolge, in der Spalten in der Liste **[!UICONTROL Ausgewählte Spalten]** angezeigt werden, bestimmt die Reihenfolge, in der die Spalten in der benutzerdefinierten Ansicht angezeigt werden.
      * Die Spalten werden in der Liste **[!UICONTROL Ausgewählte Spalten]** in der Reihenfolge angezeigt, in der Sie sie aus der Liste **[!UICONTROL Verfügbare Spalten]** hinzugefügt haben.

      * Um eine Spalte in der Liste **[!UICONTROL Ausgewählte Spalten]** neu anzuordnen, wählen Sie den Namen der Spalte aus und ziehen Sie sie in der Liste nach oben oder unten.

      * Entfernen Sie eine Spalte aus der Liste **[!UICONTROL Ausgewählte Spalten]**, indem Sie auf den Namen der ausgewählten Spalte klicken und dann auf den Pfeil **[!UICONTROL Links]** klicken. Alternativ können Sie auf den Namen der ausgewählten Spalte doppelklicken (die Spalte wird zurück in die Liste **[!UICONTROL Verfügbare Spalten]** verschoben).

      * Eine Spalte kann nur einmal hinzugefügt werden. Wenn Sie beispielsweise die Spalte &quot;Kommentare&quot;aus der Liste [!UICONTROL Verfügbar] in die Liste [!UICONTROL Ausgewählte Spalten] verschieben, wird der Name dieser Spalte aus der Liste [!UICONTROL Verfügbare Spalten] entfernt.

1. Geben Sie im Abschnitt **[!UICONTROL Sortierung]** die folgenden Informationen an:

   * **Sortieren nach:** Verwenden Sie die Registerkarte [!UICONTROL Sortierung] , wenn Sie eine bestimmte Reihenfolge festlegen möchten, in der Elemente in Ihrer benutzerdefinierten Ansicht aufgeführt werden. Wenn Sie keine Spalte zum Sortieren auswählen, ist die Standardeinstellung Keine Spalte - d. h. keine spezielle Sortierungsspalte oder -reihenfolge.
   * Nur die Spalten, die Sie auf der Registerkarte [!UICONTROL Spalten] ausgewählt haben, sind in der Dropdownliste [!UICONTROL Nach Spalte sortieren] enthalten.
   * **Aufsteigend oder Absteigend:** Wählen Sie aus, ob die Spalte standardmäßig auf- oder absteigend sortiert werden soll.

1. Verwenden Sie den Abschnitt **[!UICONTROL Filter]** , um ein oder mehrere Kriterien für die Auswahl von Elementen zu definieren, die in Ihre benutzerdefinierte Ansicht aufgenommen werden sollen. Filter sind besonders hilfreich, wenn Sie Ihre benutzerdefinierte Ansicht als Bericht verwenden möchten.
1. Um alle Elemente in Ihre benutzerdefinierte Ansicht einzuschließen, überspringen Sie den Abschnitt **[!UICONTROL Filter]** .
1. Verfügbare Filter:

   * **Feld:** Wählen Sie das Feld für diesen Filter aus (Kommentare ist das Standardfeld.) Die Liste Feld enthält alle Standardfelder (wie auf der Registerkarte [!UICONTROL Spalten] ). Die Liste ist nicht auf die Spalten beschränkt, die Sie für die Anzeige ausgewählt haben.
   * **Operator:** Die für den Filter verfügbaren Operatoren hängen vom ausgewählten Feldtyp ab. Wählen Sie einen Operator aus, der die Beziehung zwischen Feld und Wert anzeigt. Sie werden diese Informationen später ausfüllen.
   * **Wert:** Wählen Sie Ihren ausgewählten Wert in dieses Feld aus oder geben Sie ihn entsprechend dem ausgewählten Feld und dem ausgewählten Operator ein. Je nach gewähltem Operator kann es ein Wert -Feld oder zwei oder keine geben. Siehe die Beispiele unten.
   * **Filter werden mit der folgenden Logik angewendet:** Filterkriterien zwischen verschiedenen Feldern verwenden den Operator UND . Für mehrere Filterkriterien, die dasselbe Feld verwenden, wird der ODER-Operator für dasselbe Feld verwendet.

     Wenn Sie nur Testsendungen ohne Kommentare anzeigen möchten, wählen Sie die folgenden Werte aus:

      * Feld: Kommentare
      * Operator: Gleich
      * Wertfeld: 0

     Wenn Sie nur Testsendungen mit zwei oder mehr Kommentaren anzeigen möchten, wählen Sie die folgenden Werte aus:

      * Feld: Kommentare
      * Operator: Größer oder gleich
      * Wertfeld: 2

     Wenn Sie nur Testsendungen mit 1 bis 4 Kommentaren anzeigen möchten, wählen Sie die folgenden Werte aus:

      * Feld: Kommentare
      * Operator: Between
      * Wertfeld (erstes Feld): 1
      * Wertfeld (zweites Feld): 4

        Sie können einen Filter, den Sie ohne Probleme zur benutzerdefinierten Ansicht hinzugefügt haben, ändern oder entfernen, indem Sie bei Bedarf auf das Kreuzsymbol neben dem Filter [!UICONTROL setup] klicken.

        Da die Liste &quot;Feld&quot;nicht auf die Spalten beschränkt ist, die Sie auf der Registerkarte [!UICONTROL Spalten] ausgewählt haben, sollten Sie beim Erstellen eines Filters mit einer Spalte, die Sie nicht für die Anzeige in Ihrer benutzerdefinierten Ansicht ausgewählt haben, vorsichtig sein. Beispielsweise werden mit dem folgenden Filter für die Ansicht alle Testsendungen mit einem Versionszählerwert von 2 oder mehr ausgewählt:

         * Feld = Versionszähler
         * Operator = Größer oder gleich
         * Wertfeld = 2

           >[!NOTE]
           >
           >Sie können einen Filter, den Sie ohne Probleme zur benutzerdefinierten Ansicht hinzugefügt haben, ändern oder entfernen, indem Sie bei Bedarf auf das Kreuzsymbol neben dem Filter [!UICONTROL setup] klicken.



1. Wählen Sie im Abschnitt **[!UICONTROL Freigabe]** aus, welche Benutzer in Ihrem Konto Ihre benutzerspezifische Ansicht anzeigen können.
1. Benutzerdefinierte Ansichten sind spezifisch für den Benutzer, der sie erstellt. Standardmäßig ist die neue benutzerdefinierte Ansicht nur für den Ersteller sichtbar. Sie können jedoch Ihre benutzerdefinierte Ansicht freigeben, indem Sie eine der folgenden Optionen auswählen:

   * **Nur Sie können diese benutzerdefinierte Ansicht anzeigen** (Standard): Wählen Sie diese Option aus, wenn die benutzerdefinierte Ansicht nur Ihnen zur Verfügung stehen soll.
   * **Alle Benutzer können diese benutzerdefinierte Ansicht sehen**: Wählen Sie diese Option, um die benutzerdefinierte Ansicht für alle Benutzer in Ihrem Konto verfügbar zu machen.
   * **Wählen Sie Benutzer aus, die diese benutzerdefinierte Ansicht anzeigen können**: Wählen Sie diese Option, um die benutzerdefinierte Ansicht nur bestimmten Benutzern zur Verfügung zu stellen.
   * Geben Sie den Namen oder die E-Mail-Adresse des Benutzers ein, der Zugriff auf die benutzerdefinierte Ansicht erhalten soll, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.
   * Wenn Sie Ihre Ansicht zu diesem Zeitpunkt nicht für andere Benutzer freigeben möchten, können Sie dies später tun, indem Sie die benutzerdefinierte Ansicht bearbeiten.

1. Klicken Sie auf **[!UICONTROL Erstellen]**.
1. Die Ansicht &quot;Benutzerdefiniert&quot;wird angezeigt und ist auf der Seite &quot;[!DNL Views]&quot;verfügbar. Weitere Informationen zu Ansichten finden Sie unter [Elemente auf der [!DNL Views] Seite in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md) verwalten.

## Bearbeiten benutzerdefinierter Ansichten

Sie können eine benutzerdefinierte Ansicht einfach bearbeiten. So bearbeiten Sie eine benutzerdefinierte Ansicht:

1. Rufen Sie die Seite **[!UICONTROL Ansichten]** auf.\
   Weitere Informationen zu Ansichten finden Sie unter [Elemente auf der Ansichtsseite verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicken Sie auf die Schaltfläche [!UICONTROL Ansichten] (1).
1. Wählen Sie die zu bearbeitende Ansicht aus dem Dropdownmenü aus.\
   ![](assets/proof-view-edit.png)

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Anzeigeoptionen]** und dann auf **[!UICONTROL Ansicht bearbeiten]**.\
   ![](assets/proof-view-options.png)\
   Die Seite Benutzerdefinierte Ansicht bearbeiten wird angezeigt.

1. Klicken Sie auf das Menü [!UICONTROL Aktionen] . Absatz 3\
   Diese Schaltfläche ist nur verfügbar, wenn Sie die Spalte Testversand-Name in Ihre Ansicht aufnehmen.
1. Wählen Sie [!UICONTROL Ansicht bearbeiten] aus dem Menü aus. Absatz 4 \
   ![editing_custom_view_2.png](assets/editing-custom-view-2-350x258.png)

1. Die Seite &quot;Benutzerdefinierte Ansicht bearbeiten&quot;wird angezeigt.

![Edit_custom_view_page.png](assets/edit-custom-view-page-350x543.png)

>[!NOTE]
>
>Wenn Sie Ihre benutzerdefinierte Ansicht bearbeiten, werden die Spalten in der Liste Ausgewählte Spalten automatisch in alphabetischer Reihenfolge angeordnet. Sie müssen sie bei Bedarf neu anordnen, bevor Sie die Ansicht aktualisieren.


## Kopieren benutzerdefinierter Ansichten

Mit der Funktion Ansicht kopieren können Sie einfach eine Kopie einer vorhandenen benutzerdefinierten Ansicht erstellen. Dies ist beispielsweise wirklich nützlich, wenn Sie separate Ansichten für alle Ihre Designer einrichten möchten, wobei jede Ansicht mit Ausnahme des Testversand-Eigentümers (Designer) identisch ist.

So kopieren Sie eine benutzerdefinierte Ansicht:

1. Rufen Sie die Seite **[!UICONTROL Ansichten]** auf.\
   Weitere Informationen zu Ansichten finden Sie unter [Elemente auf der Ansichtsseite verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Ansichten]**. Absatz 1
1. Wählen Sie Ihre benutzerdefinierte Ansicht aus der Liste aus. Absatz 2
1. Klicken Sie auf das Menü **[!UICONTROL Aktionen]** . Absatz 3\
   Diese Schaltfläche ist nur verfügbar, wenn Sie die Spalte Testversand-Name in Ihre Ansicht aufnehmen.

1. Wählen Sie [!UICONTROL Kopieren] aus dem Menü aus. Absatz 4\
   ![copy_custom_view.png](assets/copying-custom-view-350x258.png)

1. Auf der Seite Benutzerdefinierte Ansicht kopieren werden alle ursprünglichen Einstellungen ausgefüllt. Ändern Sie die benutzerdefinierte Ansicht nach Ihrer Wahl und klicken Sie auf die Schaltfläche **[!UICONTROL Ansicht kopieren]** . Sie werden sofort zu Ihrer neuen Ansicht geführt.\
   ![](assets/copy-custom-view-page-350x542.png)

## Freigeben benutzerdefinierter Ansichten

Mit der Funktion Ansicht freigeben können Sie eine Ansicht für andere Benutzer in Ihrem Konto freigeben, wenn Sie sie nicht bereits im Bereich Freigabe für die Ansicht ausgewählt haben. Wenn Sie eine benutzerdefinierte Ansicht für andere Benutzer freigeben, wird die Ansicht im Abschnitt [!UICONTROL Meine benutzerdefinierten Ansichten] des Dropdownmenüs &quot;Ansichten&quot;angezeigt.

So geben Sie eine benutzerdefinierte Ansicht für andere Benutzer frei:

1. Rufen Sie die Seite **[!UICONTROL Ansichten]** auf.\
   Weitere Informationen zu Ansichten finden Sie unter [Elemente auf der Ansichtsseite verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Ansichten]** (1).
1. Wählen Sie Ihre benutzerdefinierte Ansicht aus der Liste aus (2)
1. Klicken Sie auf das Menü **[!UICONTROL Aktionen]** . Absatz 3\
   Diese Schaltfläche ist nur verfügbar, wenn Sie die Spalte Testversand-Name in Ihre Ansicht aufnehmen.

1. Wählen Sie [!UICONTROL Freigabeansicht] aus dem Menü (4)
1. Die Seite &quot;Benutzerdefinierte Ansicht bearbeiten&quot;wird angezeigt.
1. Wählen Sie im Abschnitt [!UICONTROL Freigabe] die Benutzer aus, für die Sie die Ansicht freigeben möchten, und klicken Sie auf **[!UICONTROL Ansicht aktualisieren]**.

   ![Edit_custom_view_page__1_.png](assets/edit-custom-view-page--1--350x543.png)

## Exportieren benutzerdefinierter Ansichten in CSV-Dateien

So exportieren Sie die Daten aus einer benutzerdefinierten Ansicht in eine CSV-Datei:

1. Rufen Sie die Seite **[!UICONTROL Ansichten]** auf.\
   Weitere Informationen zu Ansichten finden Sie unter [Elemente auf der Ansichtsseite verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Ansichten]**. Absatz 1
1. Wählen Sie Ihre benutzerdefinierte Ansicht aus der Liste aus. Absatz 2
1. Klicken Sie auf das Menü **[!UICONTROL Aktionen]** . Absatz 3\
   Diese Schaltfläche ist nur verfügbar, wenn Sie die Spalte Testversand-Name in Ihre Ansicht aufnehmen.

1. Wählen Sie im Menü [!UICONTROL In CSV exportieren] aus. Absatz 4\
   ![ export_custom_view.png](assets/exporting-custom-view-350x258.png)\
   In einem separaten Browser-Fenster wird die Meldung &quot;Bericht erzeugen: 100 %&quot;angezeigt sowie die Anzahl der Datensätze (die Anzahl der im Bericht enthaltenen Elemente aus Ihrer benutzerdefinierten Ansicht).

1. (Bedingt) Wenn eine Sicherheitsmeldung angezeigt wird, die angibt, dass der Bericht-Download derzeit blockiert ist, klicken Sie auf , um den Download zuzulassen.
1. Klicken Sie auf **[!UICONTROL Speichern]** , wenn das Fenster Dateidownload mit der Frage angezeigt wird, ob Sie die Datei öffnen oder speichern möchten.
1. Wählen Sie einen Speicherort auf Ihrem Computer aus und speichern Sie die Datei.

## Löschen benutzerdefinierter Ansichten

Sie können eine benutzerdefinierte Ansicht einfach löschen. Gehen Sie dazu folgendermaßen vor:

1. Rufen Sie die Seite **[!UICONTROL Ansichten]** auf.\
   Weitere Informationen zu Ansichten finden Sie unter [Elemente auf der Ansichtsseite verwalten in [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

1. Klicken Sie auf die Schaltfläche **[!UICONTROL Ansichten]**.
1. Wählen Sie Ihre benutzerdefinierte Ansicht aus der Liste aus.
1. Klicken Sie auf das Menü **[!UICONTROL Aktionen]** . Absatz 3\
   Diese Schaltfläche ist nur verfügbar, wenn Sie die Spalte Testversand-Name in Ihre Ansicht aufnehmen.

1. Wählen Sie [!UICONTROL Löschen] aus dem Menü aus. Absatz 4\
   ![Löschen_benutzerdefinierter_Ansicht.png](assets/deleting-custom-view-350x258.png)

1. Klicken Sie auf **[!UICONTROL Löschen]** (5), um zu bestätigen, dass Sie die aktuelle benutzerdefinierte Ansicht löschen möchten\
   ![delete__1_.png](assets/delete--1--350x187.png)

1. Die standardmäßige Ansicht Alle Elemente wird angezeigt und Ihre gelöschte benutzerdefinierte Ansicht wird nicht mehr im Dropdownmenü **[!UICONTROL Ansichten]** angezeigt.
