---
title: Anforderungsformular in der Adobe Workfront-Planung erstellen und verwalten
description: Nachdem Sie im Adobe Workfront-Planungsbereich einen Datensatztyp ausgewählt haben, können Sie ein Anforderungsformular erstellen und dieses mit diesem Datensatztyp verknüpfen. Sie können dann einen Link mit anderen internen oder externen Benutzern teilen. Benutzer mit einem Link zum Formular können die Feldwerte ausfüllen und durch Senden einen neuen Datensatz für den damit verknüpften Datensatztyp hinzufügen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 49f25b03-90bb-4317-9e48-289fd61df791
source-git-commit: b89f4aa6f779e09d6749e59bdf3d54f0dd9bbf03
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 2%

---

# Anforderungsformular in der Adobe Workfront-Planung erstellen und verwalten

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

Sie können ein Anfrageformular erstellen und es in der Adobe Workfront-Planung einem Datensatztyp zuordnen. Sie können dann einen Link mit anderen internen oder externen Benutzern teilen.

Benutzer mit einem Link zum Formular können die Feldwerte darin aktualisieren und neue Datensätze durch Senden hinzufügen.

In diesem Artikel wird beschrieben, wie ein Workspace-Manager ein Anforderungsformular erstellen kann, das mit einem Datensatztyp verknüpft ist.

Weitere Informationen zum Senden einer Anfrage an einen Datensatztyp zum Erstellen eines Datensatzes finden Sie unter [Planungsanfragen zum Erstellen von Datensätzen durch Adobe Workfront übermitteln](/help/quicksilver/planning/requests/submit-requests.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </td>

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
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <ul>
   <li><p>Berechtigungen für einen Arbeitsbereich verwalten</p></li>
    <li><p>Systemadministratoren können nicht erstellte Arbeitsbereiche verwalten. </p></li>
    </ul>
   <p>Informationen zum Freigeben von Berechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Überblick über die Freigabe von Berechtigungen in der Adobe Workfront-Planung</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anforderungsformular für einen Datensatztyp erstellen

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in den Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite mit dem Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite vom Typ Datensatz in der Tabellenansicht geöffnet.

1. Klicken Sie auf das Menü **Mehr** rechts neben dem Namen des Datensatztyps in der Kopfzeile der Seite und klicken Sie dann auf **Anforderungsformular erstellen**.![](assets/more-menu.png)
1. Aktualisieren Sie den Namen des Anfrageformulars. Standardmäßig lautet der Name des Formulars **Unbenanntes Anforderungsformular**. <!--check this; you logged a bug to rename it to this but was it fixed?-->
1. (Optional) Fügen Sie eine **Beschreibung** für das Anfrageformular hinzu.

   <!--Not possible yet: The Description is visible when you access the request form from the Requests area of Workfront.-->

1. Klicken Sie auf **Erstellen**. Das Anfrageformular für den ausgewählten Datensatztyp wird mit <!--<span class="preview"> in the Form tab</span>; add screen shot below with Configuration tab.--> geöffnet.

   ![](assets/campaigns-request-form-edit-mode.png)

   Das Anfrageformular enthält standardmäßig die folgenden Informationen:

   * In der Tabellenansicht des ausgewählten Datensatztyps verfügbare Datensatzfelder. <!--they are working on removing the limitation below-->

   >[!IMPORTANT]
   >
   > Je nachdem, welche Umgebung Sie zum Erstellen eines Anfrageformulars verwenden, gibt es die folgenden Szenarien:
   >
   >* Felder der folgenden Typen werden nicht im Anfrageformular <span class="preview">in der Vorschau </span>- oder Produktionsumgebung angezeigt:
   >
   >    * Erstellt von und zuletzt geändert von
   >    * Formel
   >    * Erstellungsdatum und Datum der letzten Änderung
   >    * Suchfelder für Workfront-Objekte
   >    * Workfront Planen der Suchfelder verbundener Datensätze
   >    * Mit AEM Assets verbundene Felder
   >* Felder der folgenden Typen werden nicht im Anfrageformular in der Produktionsumgebung angezeigt. <span class="preview">Sie werden in der Vorschau-Umgebung angezeigt:</span>
   >    * <span class="preview"> Verbindungsfelder der Workfront-Planungsdatensätze</span>
   >    * <span class="preview">Personen </span>
   >    * <span class="preview">Verbindungsfelder der Workfront-Objekte</span>
   >    * <span class="preview">AEM Assets-verbundene Felder </span>


   * **Standardabschnitt**: Dies ist der standardmäßige Abschnittsumbruch, den Workfront auf das Anforderungsformular anwendet. Der Abschnitt Standard kann nicht umbenannt oder entfernt werden.
   * Feld **Betreff** : Das Feld, das die Anforderung in Workfront identifiziert. Diese Funktion ist noch nicht verfügbar. Die Konfiguration und der Wert des Felds Betreff können nicht bearbeitet werden.
   * Alle mit dem Datensatztyp verknüpften Felder.

     Die im Anfrageformular enthaltenen Felder sind für alle sichtbar, die eine Anfrage an diesen Datensatztyp senden.

1. (Optional) Bewegen Sie den Mauszeiger über alle Felder im Formular, die Sie entfernen möchten, und klicken Sie dann auf das Symbol **x** , um sie zu entfernen. Sie werden der Registerkarte **Felder** links neben dem Formular hinzugefügt.

   Entfernen Sie beispielsweise das Feld **Betreff** , da dies in der Workfront-Planung nicht sichtbar ist. <!--remove this step when we connect intake with the Requests area in Workfront-->
1. Klicken Sie auf ein beliebiges Feld und verwenden Sie dann die Steuerelemente im rechten Bereich im Formular, um deren Größe oder eine der folgenden Informationen zu definieren:

   * **Beschriftung**: Dies ist der Name des Felds, wie es im Anfrageformular angezeigt wird. Dadurch wird der Name des Datensatzfelds nicht geändert.
   * **Anweisungen**: Fügen Sie weitere Informationen zum Feld hinzu.
   * **Machen Sie ein erforderliches Feld**: Wenn ausgewählt, muss das Feld einen Wert enthalten. Andernfalls kann das Formular nicht gesendet werden.
   * **Logik hinzufügen**: Definieren Sie, welche Bedingungen erfüllt sein müssen, damit das Feld angezeigt oder ausgeblendet wird.

   >[!NOTE]
   >
   >   Der Feldtyp jedes Felds wird oben im rechten Bereich angezeigt, nachdem Sie das Feld im Formular ausgewählt haben.
   >   
   >
   >   Die Felder Währung, Zahl und Prozentsatz werden als einzeiliger Textfeldtyp angezeigt. Das Feldformat wird jedoch beibehalten und die Werte in diesen Feldern werden als Währungs-, Zahlungs- und Prozentwerte angezeigt.

1. (Optional) Klicken Sie auf die Registerkarte **Inhaltselemente** auf der linken Seite des Formulars und fügen Sie eines der folgenden Elemente hinzu:

   * **Beschreibender Text**
   * **Abschnittsumbruch**

   Weitere Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. (Optional) Klicken Sie auf **Vorschau** , um anzuzeigen, wie das Formular für andere Benutzer angezeigt wird, wenn diese es zum Senden eines neuen Datensatzes verwenden werden.

   <!--
   <div class="preview">
   1. (Optional) Click the **Configuration** tab, then add at least one user to the **Approvers** field to approve new requests for this record form. 
      When you associate a request form with approvers, any new request must first be approved by all approvers before it generates a new record. 
      You can add one or several approvers to a request form. If at least one approver rejects the request, the request is rejected and the record is not created.
   For more information about adding approvals to request forms, see [Add approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md). 
   </div>
   -->

1. (Optional) Klicken Sie auf das Menü **Mehr** rechts neben dem Namen des Formulars in der Kopfzeile und dann auf **Bearbeiten** , um den Namen des Formulars zu aktualisieren.![](assets/more-menu.png)
1. Klicken Sie auf **Publish** , um das Formular zu veröffentlichen und einen eindeutigen Link dafür zu erhalten.

   Folgendes geschieht:

   * Die Schaltfläche **Publish** wurde entfernt.
   * Die Schaltfläche **Veröffentlichung rückgängig machen** wird dem Formular hinzugefügt. Wenn Sie darauf klicken, wird der Zugriff auf das Formular verhindert.
   * Dem Formular wird eine Schaltfläche **Freigabe** hinzugefügt.

1. Klicken Sie auf **Freigeben** , um das Formular für andere freizugeben.

   ![](assets/share-box-for-request-form.png)

1. Wählen Sie aus den folgenden Optionen aus, um anzugeben, welche Benutzertypen auf dieses Formular zugreifen können:

   * Jede Person mit Zugriff auf den Arbeitsbereich (Ansicht oder höher)
   * Jede Person mit Zugriff auf den Arbeitsbereich (Beitrag oder höher)
   * Jede Person mit dem Link

   >[!WARNING]
   >
   >
   >* Wenn Sie **Jeder, der über den Link** verfügt, auswählen, kann jeder auf das Formular zugreifen und einen neuen Datensatz senden, selbst Personen außerhalb Ihres Unternehmens, die kein Workfront-Konto haben.
   >
   > * <span class="preview">Ein Formular, das die folgenden Feldtypen enthält, kann nicht öffentlich freigegeben werden:</span>
   >
   >     * <span class="preview">Formel</span>
   >     * <span class="preview">Workfront- oder AEM Assets-Verbindungen</span>
   >     * <span class="preview">Suchfelder</span>
   >     * <span class="preview">Personen</span>
   >

1. (Bedingt) Wenn Sie im vorherigen Schritt **Jeder Benutzer mit dem Link** ausgewählt haben, wählen Sie im verfügbaren Kalender das **Ablaufdatum des Links** aus. Personen erhalten nach Ablauf des Links einen Fehler. Sie müssen das Link-Datum aktualisieren, bevor sie erneut auf das Formular zugreifen können.

   Sie können zukünftige Datumsangaben innerhalb von 180 Tagen ab dem aktuellen Datum auswählen.

1. Klicken Sie auf **Link speichern und kopieren** , um die Freigabedetails für das Formular zu speichern.

   Die Optionen zur Formularfreigabe werden gespeichert und der Link wird in die Zwischenablage kopiert. Sie können es jetzt für andere freigeben.

   Informationen zum Erstellen von Datensätzen mithilfe eines Links zu einem Anforderungsformular finden Sie unter [Planungsanforderungen für die Adobe Workfront übermitteln](/help/quicksilver/planning/requests/submit-requests.md).

1. Klicken Sie in der rechten unteren Ecke des Bildschirms auf **Speichern** , um das Formular zu speichern.
1. Klicken Sie in der Kopfzeile auf den linken Pfeil neben dem Formularnamen, um das Formular zu schließen.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Optional) Klicken Sie auf das Menü **Mehr** rechts neben dem Namen des Datensatztyps in der Kopfzeile und führen Sie einen der folgenden Schritte aus:![](assets/more-menu.png)
   * Klicken Sie auf **Anforderungsformular aktualisieren** , um Änderungen am Anforderungsformular vorzunehmen.
   * Klicken Sie auf **Link zum Anforderungsformular kopieren** , um den Link zum Formular für andere freizugeben.

   >[!TIP]
   >
   >Es gibt einen Hinweis darauf, dass der Link öffentlich freigegeben wird, wenn dies der Fall ist.
   >![](assets/publicly-shared-link-to-form-on-record-type-menu-highlighted.png)
