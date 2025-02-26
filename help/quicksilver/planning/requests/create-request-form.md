---
title: Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning
description: Nachdem Sie im Bereich Adobe Workfront-Planung einen Datensatztyp ausgewählt haben, können Sie ein Anforderungsformular erstellen und es mit diesem Datensatztyp verknüpfen. Sie können dann einen Link dazu für andere interne oder externe Benutzer freigeben. Benutzer mit einem Link zum Formular können die Feldwerte darin ausfüllen und durch Senden einen neuen Datensatz für den damit verknüpften Datensatztyp hinzufügen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: 5510f99e9e5c8c4c5f85953e19563f9ab18b0fae
workflow-type: tm+mt
source-wordcount: '1538'
ht-degree: 2%

---

# Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Sie können ein Anfrageformular erstellen und es mit einem Datensatztyp in Adobe Workfront Planning verknüpfen. Sie können dann einen Link dazu für andere interne oder externe Benutzer freigeben.

Benutzer mit einem Link zum Formular können die darin enthaltenen Feldwerte aktualisieren und neue Datensätze hinzufügen, indem sie sie übermitteln.

In diesem Artikel wird beschrieben, wie ein Workspace-Manager ein Anfrageformular erstellen kann, das mit einem Datensatztyp verknüpft ist.

Weitere Informationen zum Senden einer Anfrage an einen Datensatztyp zum Erstellen eines Datensatzes finden Sie unter [Senden von Adobe Workfront Planning-Anfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td>
   <td>
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Standard</p>
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
   <td>
   <ul>
   <li><p>Verwalten von Berechtigungen für einen Arbeitsbereich</p></li>
    <li><p>Systemadministratoren können Arbeitsbereiche verwalten, die sie nicht erstellt haben. </p></li>
    </ul>
   <p>Informationen zu Freigabeberechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Übersicht über Freigabeberechtigungen in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutvorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Einschränkungen bei der Anzeige von Feldern und Werten in Anfrageformularen

<!--

There are limitations in how certain fields display on the request form and how their values later display on the records or the request details page, after you submit a request. 

For information about submitting requests to create records, see [Submit Adobe Workfront Planning requests to create records](/help/quicksilver/planning/requests/submit-requests.md). 

The following are limitations for how certain fields display in request forms, records created by a request form, or on the request details page: -->

* Sie können keine Felder der folgenden Typen zu einem Anfrageformular hinzufügen:

   * Erstellt von und Zuletzt geändert von
   * Erstellungsdatum und Datum der letzten Änderung
   * Formel. Formelfelder werden in der Vorschau-Umgebung unterstützt.
   * Suchfelder der Workfront-Objekte
   * Suchfelder für verknüpfte Datensätze in Workfront

<!--at release to Preview, replace the above with this:  
>
>Fields of the following types do not display in the request form:
>* Created by and Last modified by
>* Created date and Last modified date
>* Formula. <span class="preview">Formula fields display in request forms in the Preview environment.</span>
>* Workfront objects' lookup fields
>* Workfront Planning connected records' lookup fields-->

* Unterschied zwischen der Anzeige von Feldformaten im Formular-Builder für Anfragen und der Formatierung der Werte im Datensatz oder auf der Seite mit den Anfragedetails:

   * Die Felder Währung, Zahl und Prozentsatz werden im Formular-Builder als einzeiliges Textfeld angezeigt.

     Das Feldformat wird jedoch beibehalten und die Werte der Zahlen in diesen Feldern werden als Währungs-, Zahl- und Prozentwerte auf dem Datensatztyp und auf der Seite mit den Anfragedetails angezeigt.

<!--
* The following describes how some field values display on request forms and the request details pages: 

   * Special formatting for Currency, Number, and Percentage fields is not preserved. For example, the decimal precision is not preserved for these fields' values in these areas.
   * People field values display as IDs.
   * Formula fields that don't refer to other fields or calculations don't display any values. For example, a field with a `STRING` formula displays a "N/A" value.
   * Formula fields that refer to Currency fields display the values without accounting for exchange rates.
   * The values of Paragraph fields that contain special formatting display a "N/A" value on the request form and they display html tags instead of the formatted text in the request details page.
-->

## Erstellen eines Anfrageformulars für einen Datensatztyp

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Weitere Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite mit dem Datensatztyp in der Tabellenansicht geöffnet.

1. Klicken Sie auf das **Mehr**-Menü ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps in der Seitenkopfzeile und dann auf **Anforderungsformular erstellen**.
1. Aktualisieren Sie den Namen des Anfrageformulars. Standardmäßig lautet der Name des Formulars &quot;**Formular**. <!--check this; you logged a bug to rename it to 'Untitled request form' but was it fixed?-->
1. (Optional) Fügen Sie **Anfrageformular eine** Beschreibung“ hinzu.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Klicken Sie auf **Erstellen**. Das Anfrageformular für den ausgewählten Datensatztyp wird auf der Registerkarte Formular geöffnet.

   ![](assets/campaigns-request-form-edit-mode.png)

   Das Anfrageformular enthält standardmäßig die folgenden Informationen:

   * Verfügbare Datensatzfelder in der Tabellenansicht des ausgewählten Datensatztyps. <!--they are working on removing the limitation below-->

   * **Standardabschnitt**: Dies ist der standardmäßige Abschnittsumbruch, den Workfront auf das Anfrageformular anwendet. Alle Datensatzfelder werden im Bereich **Standard** angezeigt.
   * **Betreff** Feld: Das Feld, das die Anfrage in Workfront identifiziert. Die Konfiguration und der Wert des Felds Betreff können nicht bearbeitet werden.

     >[!TIP]
     >
     >Das **Betreff** Feld erfordert einen Wert, wenn er im Anfrageformular sichtbar ist. Sie können jedoch bei Bedarf das Feld **Betreff** entfernen. Anfordernde sehen es nicht im Formular, wenn sie die Anfrage senden.

   * Alle mit dem Datensatztyp verknüpften Felder.

     Die im Anfrageformular enthaltenen Felder sind für alle sichtbar, die eine Anfrage an diesen Datensatztyp senden.

1. (Optional) Bewegen Sie den Mauszeiger über die Felder im Formular, die Sie entfernen möchten, und klicken Sie dann auf das Symbol **x**, um sie zu entfernen. Sie werden der Registerkarte **Felder** links neben dem Formular hinzugefügt.

   Entfernen Sie beispielsweise das Feld **Betreff**, da dies in Workfront Planning nicht angezeigt wird. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. (Optional) Gehen Sie wie **vor, um den Abschnitt** Standard“ aus dem Formular zu entfernen:

   1. Entfernen Sie alle Felder aus dem Standardabschnitt.
   1. Klicken Sie **Inhaltselemente** und fügen Sie einen neuen Abschnitt und dann einen Namen für den Abschnitt hinzu.
   1. Fügen Sie Felder zum neuen Abschnitt hinzu.
   1. Klicken Sie auf das **x**-Symbol, um den **Standardabschnitt“** entfernen.
1. Klicken Sie auf ein beliebiges Feld und verwenden Sie dann die Steuerelemente im rechten Bereich im Formular, um ihre Größe oder eine der folgenden Informationen zu definieren:

   * **label**: Dies ist der Name des Felds, wie er im Anfrageformular angezeigt wird. Der Name des Datensatzfelds wird dadurch nicht geändert.
   * **Anweisungen**: Fügen Sie weitere Informationen über das Feld hinzu.
   * **Erforderliches Feld festlegen**: Wenn diese Option aktiviert ist, muss das Feld einen Wert enthalten. Andernfalls kann das Formular nicht gesendet werden.
   * **Logik hinzufügen**: Definieren Sie, welche Bedingungen erfüllt sein müssen, damit das Feld angezeigt oder ausgeblendet wird.

   >[!TIP]
   >
   >   Der Feldtyp der einzelnen Felder wird oben im rechten Bereich angezeigt, nachdem Sie das Feld im Formular ausgewählt haben.
   >     

1. (Optional) Klicken Sie auf **Registerkarte** Inhaltselemente“ auf der linken Seite des Formulars und fügen Sie eines der folgenden Elemente hinzu:

   * **Beschreibender Text**
   * **Abschnittsumbruch**

   Weitere Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Optional) Klicken Sie auf **Vorschau**, um anzuzeigen, wie das Formular für andere Benutzer angezeigt wird, wenn diese es zum Senden eines neuen Datensatzes verwenden werden.

1. (Optional) Klicken Sie auf die **Konfiguration** und fügen Sie dann mindestens einen Benutzer zum Feld **Genehmiger** hinzu, um neue Anfragen für dieses Datensatzformular zu genehmigen.

   ![](assets/configuration-tab.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

   * Wenn Sie ein Anfrageformular mit genehmigenden Personen verknüpfen, muss jede neue Anfrage zunächst von allen genehmigenden Personen genehmigt werden, bevor ein neuer Datensatz generiert wird.
   * Sie können einem Anfrageformular eine oder mehrere genehmigende Personen hinzufügen.
   * Wenn mindestens eine genehmigende Person die Anforderung ablehnt, wird die Anforderung abgelehnt und der Datensatz nicht erstellt.
   * Alle genehmigenden Personen müssen eine Entscheidung treffen, bevor eine Anfrage genehmigt oder abgelehnt wird.

     Weitere Informationen zum Hinzufügen von Genehmigungen zu Anfrageformularen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

1. (Optional) Klicken Sie auf das **Mehr**-Menü ![](assets/more-menu.png) rechts neben dem Namen des Formulars in der Kopfzeile und klicken Sie dann auf **Bearbeiten**, um den Namen des Formulars zu aktualisieren.
1. Klicken Sie auf **Veröffentlichen**, um das Formular zu veröffentlichen und einen eindeutigen Link für es zu erhalten.

   Folgendes geschieht:

   * Die Schaltfläche **Veröffentlichen** wird entfernt.
   * Die **Veröffentlichung aufheben** wird dem Formular hinzugefügt. Wenn Sie darauf klicken, ist der Zugriff auf das Formular nicht möglich.
   * Eine **Freigeben**-Schaltfläche wird dem Formular hinzugefügt.

1. Klicken Sie **Freigeben**, um das Formular für andere freizugeben.

   ![](assets/share-box-for-request-form.png)

1. Wählen Sie aus den folgenden Optionen aus, um anzugeben, welche Benutzertypen auf dieses Formular zugreifen können:

   * Jede Person mit Zugriff auf den Arbeitsbereich (Ansicht oder höher)
   * Jede Person mit Zugriff auf den Arbeitsbereich (Beitrag oder höher)
   * Jede Person mit dem Link

   >[!WARNING]
   >
   >* Wenn Sie **Alle mit dem Link** auswählen, kann jeder auf das Formular zugreifen und einen neuen Datensatz senden, auch Personen außerhalb Ihres Unternehmens, die kein Workfront-Konto haben.
   >
   > * Ein Formular, das die folgenden Feldtypen enthält, kann nicht öffentlich freigegeben werden:
   >
   >     * Workfront- oder AEM Assets-Verbindungen
   >     * Personen
   >

1. (Bedingt) Wenn Sie im vorherigen Schritt **Alle mit dem Link** ausgewählt haben, wählen Sie das **Link-Ablaufdatum** aus dem verfügbaren Kalender aus. Personen erhalten nach Ablauf des Links einen Fehler, und Sie müssen das Link-Datum aktualisieren und einen neuen Link zur Freigabe generieren, bevor Personen erneut auf das Formular zugreifen können.

   Sie können zukünftige Termine innerhalb von 180 Tagen ab dem aktuellen Datum auswählen.

1. Klicken Sie **Speichern und Link kopieren**, um die Freigabedetails für das Formular zu speichern. Wenn das Formular zuvor gespeichert wurde, klicken Sie auf **Link kopieren**.

   Die Formularfreigabeoptionen werden gespeichert und der Link wird in die Zwischenablage kopiert. Sie können sie jetzt für andere freigeben.

   Weitere Informationen zum Erstellen von Datensätzen über einen Link zu einem Anfrageformular finden Sie unter [Senden von Adobe Workfront Planning-Anfragen](/help/quicksilver/planning/requests/submit-requests.md).

1. Klicken Sie **Speichern** in der rechten unteren Ecke der Registerkarte **Formular**, um das Formular zu speichern.
1. Klicken Sie auf den nach links zeigenden Pfeil links neben dem Namen des Formulars in der Kopfzeile, um das Formular zu schließen.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Optional) Klicken Sie auf das **Mehr**-Menü ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps in der Kopfzeile und führen Sie dann einen der folgenden Schritte aus:
   * Klicken Sie **Anfrageformular aktualisieren**, um Änderungen am Anfrageformular vorzunehmen.
   * Klicken Sie auf **Link zum Anfrageformular kopieren**, um den Link zum Formular für andere freizugeben.

   >[!TIP]
   >
   >Es gibt einen Hinweis darauf, dass der Link öffentlich freigegeben wird, wenn dies der Fall ist.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
