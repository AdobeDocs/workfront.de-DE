---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopieren und Verschieben von Vorlagenaufgaben
description: Sie können eine Vorlagenaufgabe kopieren oder in dieselbe Vorlage oder in eine andere Vorlage verschieben.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '2138'
ht-degree: 3%

---

# Kopieren und Verschieben von Vorlagenaufgaben

Sie können eine Vorlagenaufgabe von einer Vorlage in eine andere Vorlage kopieren oder entweder in eine andere Vorlage oder an eine andere Stelle in derselben Vorlage verschieben.

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
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für eine Vorlage und die Vorlagenaufgabe verwalten </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Kopieren oder Verschieben von Vorlagenaufgaben

Beachten Sie beim Kopieren einer Vorlagenaufgabe Folgendes:

* Meilensteine werden nicht in die kopierte oder verschobene Vorlagenaufgabe übertragen.

* Teilaufgaben werden an die neue Vorlagenaufgabe übertragen.
* Benutzerdefinierte Formulare werden mit der Vorlagenaufgabe kopiert. Die Informationen in den benutzerdefinierten Feldern werden nur dann an die neue Vorlagenaufgabe übertragen, wenn Sie die Option zum Kopieren benutzerdefinierter Daten auswählen.
* Sie haben die Möglichkeit, während des Kopiervorgangs einige mit der Vorlagenaufgabe verknüpfte Elemente in die kopierte Aufgabe zu kopieren. Die folgenden Objekte werden jedoch standardmäßig nicht an die kopierte Aufgabe übertragen:

   * Benutzerkommentare

* Sie können eine Vorlagenaufgabe in die folgenden Bereiche der Adobe Workfront-Webanwendung kopieren:

   * Auf der Ebene der Vorlagenaufgaben über die **Weitere Symbole** ![](assets/more-icon.png) rechts neben dem Namen der Vorlagenaufgabe.

   * In einer Aufgabenliste einer Vorlage.
* Sie können Vorlagenaufgaben entweder nacheinander kopieren oder verschieben oder mehrere Vorlagenaufgaben auswählen.

## Vorlagenaufgaben kopieren

1. Wechseln Sie zu der Vorlage, die die Vorlagenaufgabe oder Vorlagenaufgaben enthält, die Sie kopieren möchten.
1. Klicks **Vorlagenaufgaben** im linken Bereich.
1. Führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf den Namen einer Vorlagenaufgabe, um sie zu öffnen.
   * Wählen Sie eine oder mehrere Vorlagenaufgaben in der Liste aus.
1. (Bedingt) Klicken Sie auf die **Mehr** Menü ![](assets/more-icon.png) oben in der Aufgabenliste der Vorlage oder rechts neben dem Namen der Vorlagenaufgabe, wenn Sie die Aufgabe geöffnet haben, klicken Sie auf **Kopieren nach** oder **Kopieren**, je nachdem von wo aus Sie auf die Option Kopieren zugreifen.
Das Feld Vorlage kopieren wird geöffnet.
   ![](assets/copy-template-task-box-unshimmed.png)
1. (Optional) Benennen Sie die Vorlagenaufgabe in der **Vorlagenname** -Feld.

   >[!TIP]
   >
   >Dieses Feld ist abgeblendet und kann nicht bearbeitet werden, wenn Sie mehrere Vorlagenaufgaben in eine Liste kopieren möchten. Sie können den Mauszeiger über das Feld &quot;Vorlagenname&quot;bewegen und eine Liste aller ausgewählten Vorlagenaufgaben wird angezeigt.

1. Geben Sie den Namen der **Zielvorlage** wo Sie die Vorlagenaufgabe in die **Zielvorlage auswählen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   Der aktuelle Vorlagenname wird standardmäßig angezeigt. Wenn Sie die Vorlagenaufgabe in dieselbe Vorlage kopieren möchten, lassen Sie dieses Feld unverändert.

   >[!TIP]
   >
   >Sie können auch mit der Eingabe der Referenznummer beginnen oder die Kennung der Vorlage eingeben. Auf diese Weise können Sie zwischen Vorlagen mit identischen Namen unterscheiden.

1. (Bedingt) Klicken Sie auf **Zugriff anfordern** , um Zugriff auf die Zielvorlage anzufordern, wenn Sie keinen Zugriff auf die ausgewählte Vorlage haben.
1. (Bedingt) Kopieren Sie die Vorlagenaufgabe weiterhin in die ausgewählte Zielvorlage, ohne Zugriff anzufordern, wenn Sie Zugriff haben, um Vorlagenaufgaben zu einer der Vorlagenaufgaben in der Zielvorlage hinzuzufügen.

1. Klicks **Optionen** Deaktivieren Sie dann im linken Bereich die VorlagenAufgabenattribute, die Sie nicht mit der Vorlagenaufgabe kopieren möchten. Alle Optionen sind standardmäßig ausgewählt.

   >[!TIP]
   >
   >Auswahl aufheben **Alle auswählen** Deaktiviert alle Optionen.

   Deaktivieren Sie die folgenden Optionen, um sie nicht in die kopierte Vorlagenaufgabe zu übertragen. In der folgenden Tabelle wird beschrieben, was passiert, wenn die Optionen deaktiviert werden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td>Deaktivieren Sie diese Option, um alle Informationen aus der Vorlagenaufgabe zu entfernen, wenn sie an ihren neuen Speicherort kopiert wird. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Einschränkung</td> 
      <td> <p>Die Aufgabenbegrenzung der Vorlage wird auf "Sofort wie möglich"oder "So spät wie möglich"festgelegt, basierend auf der Einstellung "Vorlagenzeitplanmodus".</p> <p> Wenn diese Option aktiviert ist, wird die aktuelle Einschränkung der Vorlagenaufgabe an die kopierte Vorlagenaufgabe übertragen. </p> 
      <p><b>NOTIZ</b>

   Wenn beim Kopieren einer Vorlagenaufgabe mit datumsspezifischen Begrenzungen in eine andere Vorlage die Beschränkungsdaten der Vorlagenaufgabe außerhalb der Daten der neuen Vorlage liegen, wird entweder die Vorlagenaufgabe-Beschränkung so bald wie möglich oder so spät wie möglich geändert oder die geplanten Start- oder Abschlussdaten der Vorlagen werden angepasst.

   Im Folgenden finden Sie Beispiele für datumsspezifische Einschränkungen:
   <ul>
      <li> Muss beginnen am</li>
      <li> Muss beendet werden am</li>
      <li> Nicht früher anfangen als</li>
      <li> Nicht später anfangen als</li>
      </ul>
     </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td> <p>Alle Zuweisungen werden aus der Vorlagenaufgabe entfernt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsprozess</td> 
      <td>Alle Genehmigungsprozesse werden aus der Vorlagenaufgabe entfernt.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Alle Vorgänger</td> 
      <td> <p>Dies bedeutet, dass die Abhängigkeiten nicht in die kopierten Vorlagenaufgaben übertragen werden. </p> <p>Wenn diese Option aktiviert ist, bleiben die Vorgänger in der Gruppe der kopierten Vorlagenaufgaben erhalten, andere werden gelöscht.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td> <p>Die Werte für die benutzerdefinierten Felder werden gelöscht und die benutzerdefinierten Formulare werden in die kopierte Vorlagenaufgabe übertragen. </p> <p>Wenn diese Option aktiviert ist, werden sowohl die Formulare als auch die Werte für die benutzerdefinierten Felder an die kopierte Vorlagenaufgabe übertragen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td>Die Finanzinformationen der kopierten Vorlagenaufgabe werden entfernt und die Workfront aktualisiert die Vorlagenaufgabe "Kostentyp"auf "Keine Kosten"und die Vorlagenaufgabe "Umsatztyp"auf "Nicht abrechenbar".
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Die der Vorlagenaufgabe angehängten Dokumente werden nicht an die kopierte Vorlagenaufgabe übertragen. Dazu gehören Versionen, Testsendungen und verknüpfte Dokumente.</p> <p><b>NOTIZ</b></p>

   <p>Dokumentgenehmigungen sind nicht enthalten. Dokumentgenehmigungen können nie kopiert werden, wenn eine Vorlagenaufgabe kopiert wird.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td>Die Erinnerungen an Vorlagenaufgaben werden nicht an die kopierte Vorlagenaufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Die in der Vorlagenaufgabe protokollierten Ausgaben werden nicht an die kopierte Vorlagenaufgabe übertragen. </td> 
     </tr>  
    </tbody> 
   </table>

(FRAGEN ZUR LETZTEN ZEILE: VORLAGENAUFGABE SCHEINT NICHT &quot;FREIGABE&quot;ZU HABEN)

1. (Optional) Klicken Sie auf **Übergeordnetes Element auswählen** Wählen Sie im linken Bereich die Vorlagenaufgabe in der Zielvorlage aus, die Sie zur übergeordneten Aufgabe der kopierten Vorlagenaufgabe werden möchten.

   >[!TIP]
   >
   >Bei der Auswahl, mehrere Vorlagenaufgaben in eine Liste zu kopieren, werden alle ausgewählten Vorlagenaufgaben zu den untergeordneten Elementen des ausgewählten übergeordneten Objekts und werden nach den vorhandenen untergeordneten Aufgaben hinzugefügt.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste der Vorlage einen der übergeordneten Elemente im Vorlagenplan aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie anhand des Namens nach einer übergeordneten Vorlagenaufgabe.

   Die Vorlagenaufgabe sollte in der Liste angezeigt werden.

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Vorlagenaufgabe auswählen, werden die Vorlagenaufgaben als Hauptvorlagenaufgaben und nicht als Unteraufgaben kopiert und am Ende der Vorlagenaufgabenliste in der Zielvorlage platziert.

1. Klicks **Aufgabe &quot;Vorlage kopieren&quot;**.

   Die kopierten Vorlagenaufgaben befinden sich nun in der angegebenen Vorlage und sind entweder Unteraufgaben der ausgewählten übergeordneten Vorlagenaufgabe oder der letzten Vorlagenaufgaben in der Vorlage.


## Vorlagenaufgaben verschieben

Neben dem Kopieren von Vorlagenaufgaben können Sie auch eine Vorlagenaufgabe in eine andere Vorlagenaufgabe in derselben Vorlage oder in eine andere Vorlage verschieben.


1. Markieren Sie die Vorlage, die die zu verschiebenden Vorlagenaufgaben enthält.
1. Klicks **Vorlagenaufgaben** im linken Bereich.
1. Führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf den Namen einer Vorlagenaufgabe, um sie zu öffnen.
   * Wählen Sie eine oder mehrere Vorlagenaufgaben in der Liste aus.
1. (Bedingt) Klicken Sie auf die **Mehr** Menü ![](assets/more-icon.png) oben in der Aufgabenliste der Vorlage oder rechts neben dem Namen der Vorlagenaufgabe, wenn Sie die Aufgabe geöffnet haben, klicken Sie auf **Verschieben nach** oder **Verschieben**, je nachdem, von wo aus Sie auf die Option Verschieben zugreifen.
Das Feld Vorlage verschieben wird geöffnet.
   ![](assets/move-template-task-box-unshimmed.png)

1. (Optional) Benennen Sie die Vorlagenaufgabe in der **Vorlagenname** -Feld.

   >[!TIP]
   >
   >Dieses Feld ist abgeblendet und kann nicht bearbeitet werden, wenn Sie mehrere Vorlagenaufgaben in eine Liste verschieben möchten. Sie können den Mauszeiger über das Feld &quot;Vorlagenname&quot;bewegen und eine Liste aller ausgewählten Vorlagenaufgaben wird angezeigt.

1. Geben Sie den Namen der **Zielvorlage** wo Sie die Vorlagenaufgabe in die **Zielvorlage auswählen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können auch mit der Eingabe der Referenznummer beginnen oder die Kennung der Vorlage eingeben. Auf diese Weise können Sie zwischen Vorlagen mit identischen Namen unterscheiden.

1. (Bedingt) Klicken Sie auf **Zugriff anfordern** , um Zugriff auf die Vorlage anzufordern, wenn Sie keinen Zugriff auf die Zielvorlage haben.
1. (Bedingt) Verschieben Sie die Vorlagenaufgabe weiterhin in die ausgewählte Zielvorlage, ohne Zugriff anzufordern, wenn Sie Zugriff haben, um Vorlagenaufgaben zu einer der Vorlagenaufgaben in der Zielvorlage hinzuzufügen.

1. Klicks **Optionen** Deaktivieren Sie dann im linken Bereich die VorlagenAufgabenattribute, die Sie nicht mit der Vorlagenaufgabe kopieren möchten. Alle Optionen sind standardmäßig ausgewählt.

   >[!TIP]
   >
   >* Der Abschnitt Optionen ist erst verfügbar, nachdem Sie eine Zielvorlage ausgewählt haben.
   >* Auswahl aufheben **Alle auswählen** Deaktiviert alle Optionen.

   Deaktivieren Sie die Option aus den folgenden Optionen, um die Informationen nicht an die verschobene Vorlagenaufgabe zu übertragen. In der folgenden Tabelle wird beschrieben, was passiert, wenn die Optionen deaktiviert werden:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td>Deaktivieren Sie diese Option, um alle Informationen aus der Vorlagenaufgabe zu entfernen, wenn sie an die neue Position verschoben wird. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Einschränkung</td> 
      <td> <p>Die Aufgabenbegrenzung der Vorlage wird auf "Sofort wie möglich"oder "So spät wie möglich"festgelegt, basierend auf der Einstellung "Vorlagenzeitplanmodus".</p> <p> Wenn diese Option aktiviert ist, wird die aktuelle Einschränkung der Vorlagenaufgabe an die verschobene Vorlagenaufgabe übertragen. </p>

   <p><b>NOTIZ</b>

   Wenn Sie eine Vorlagenaufgabe mit datumsspezifischen Begrenzungen auf eine andere Vorlage verschieben und die Beschränkungsdaten der Vorlagenaufgabe außerhalb der Daten der neuen Vorlage liegen, wird entweder die Vorlagenaufgabe-Beschränkung so bald wie möglich oder so spät wie möglich geändert oder die geplanten Start- oder Abschlussdaten der Vorlagen werden angepasst.

   Im Folgenden finden Sie Beispiele für datumsspezifische Einschränkungen:
   <ul>
      <li> Starten am</li>
      <li> Muss beendet werden am</li>
      <li> Nicht früher anfangen als</li>
      <li> Nicht später anfangen als</li>
      </ul>


   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Arbeitsaufträge</td> 
      <td> <p>Alle Zuweisungen werden aus der Vorlagenaufgabe entfernt. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsprozess</td> 
      <td>Alle Genehmigungsprozesse werden aus der Vorlagenaufgabe entfernt.</td> 
     </tr>

   <tr> 
      <td role="rowheader">Alle Vorgänger</td> 
      <td> <p>Dies bedeutet, dass die Abhängigkeiten nicht mit den verschobenen Vorlagenaufgaben übernommen werden. </p> <p>Wenn diese Option aktiviert ist, bleiben die Vorgänger in der Gruppe der verschobenen Vorlagenaufgaben erhalten, andere werden gelöscht.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td> <p>Die Werte für die benutzerdefinierten Felder werden gelöscht und die benutzerdefinierten Formulare werden mit der verschobenen Vorlagenaufgabe übertragen. </p> <p>Wenn diese Option aktiviert ist, werden sowohl die Formulare als auch die Werte für die benutzerdefinierten Felder mit der Aufgabe "Verschieben einer Vorlage"übertragen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td>Die Finanzinformationen der verschobenen Vorlagenaufgabe werden entfernt und die Workfront aktualisiert die Vorlagenaufgabe "Kostentyp"auf "Keine Kosten"und die Vorlagenaufgabe "Umsatztyp"auf "Nicht abrechenbar".</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Die der Vorlagenaufgabe angehängten Dokumente werden nicht mit der verschobenen Vorlagenaufgabe übertragen. Dazu gehören Versionen, Testsendungen und verknüpfte Dokumente.</p>

   <p><b>NOTIZ</b></p>

   <ul><li>
      <p>Dokumentgenehmigungen sind nicht enthalten. Dokumentgenehmigungen können beim Verschieben einer Vorlagenaufgabe nie verschoben werden.</p> </li>
      <li>Wenn Sie sich dafür entscheiden, die Dokumente nicht mit der Vorlagenaufgabe verschieben zu lassen, werden die Dokumente gelöscht und 30 Tage lang im Papierkorb abgelegt. Ein Administrator kann sie wiederherstellen und wird in der verschobenen Vorlagenaufgabe wiederhergestellt.

   Wenn die Vorlagenaufgabe nach dem Verschieben gelöscht wird, werden die wiederhergestellten Dokumente im Bereich &quot;Dokumente&quot;der Benutzerseite des Administrators platziert, der sie wiederherstellt. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td>Die Erinnerungen an Vorlagenaufgaben werden nicht an die verschobene Vorlagenaufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Die in der Vorlagenaufgabe protokollierten Ausgaben werden nicht mit der verschobenen Vorlagenaufgabe übertragen. </td> 
     </tr>  
    </tbody> 
   </table>

(FRAGEN ZUR LETZTEN ZEILE: VORLAGENAUFGABE SCHEINT NICHT &quot;FREIGABE&quot;ZU HABEN)

1. (Optional) Klicken Sie auf **Übergeordnetes Element auswählen** Wählen Sie im linken Bereich die Vorlagenaufgabe in der Zielvorlage aus, die Sie zur übergeordneten Aufgabe der verschobenen Vorlage werden möchten.

   >[!TIP]
   >
   >Bei der Auswahl, mehrere Vorlagenaufgaben in eine Liste zu verschieben, werden alle ausgewählten Vorlagenaufgaben zu den untergeordneten Elementen des ausgewählten übergeordneten Objekts und werden nach den vorhandenen untergeordneten Aufgaben hinzugefügt.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste der Vorlage einen der übergeordneten Elemente im Vorlagenplan aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie anhand des Namens nach einer übergeordneten Vorlagenaufgabe.

   Die Vorlagenaufgabe sollte in der Liste angezeigt werden.

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Vorlagenaufgabe auswählen, werden die Vorlagenaufgaben als Hauptvorlagenaufgaben und nicht als Unteraufgaben verschoben und am Ende der Vorlagenaufgabenliste auf der Zielvorlage platziert.

1. Klicks **Vorlagenaufgabe verschieben**.

   Die verschobenen Vorlagenaufgaben befinden sich nun in der angegebenen Vorlage und sind entweder Unteraufgaben der ausgewählten übergeordneten Vorlagenaufgabe oder der letzten Vorlagenaufgaben in der Vorlage.
