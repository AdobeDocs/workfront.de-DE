---
product-area: templates
navigation-topic: templates-navigation-topic
title: Kopieren und Verschieben von Vorlagenaufgaben
description: Sie können eine Vorlagenaufgabe kopieren oder in dieselbe Vorlage oder in eine andere Vorlage verschieben.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '2128'
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
   <td> <p>Alle</p> </td> 
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
   <td> <p>Berechtigungen für eine Vorlage und die Vorlagenaufgabe verwalten </p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen zum Kopieren oder Verschieben von Vorlagenaufgaben

Beachten Sie beim Kopieren von Vorlagenaufgaben Folgendes:

* Die folgenden Informationen werden nicht an die kopierte Aufgabe übertragen:

   * Meilensteine

* Sie haben die Möglichkeit, während des Kopiervorgangs einige mit der Vorlagenaufgabe verknüpfte Elemente in die kopierte Aufgabe zu kopieren. Die folgenden Objekte werden jedoch standardmäßig nicht an die kopierte Aufgabe übertragen:

   * Benutzerkommentare

* Benutzerdefinierte Formulare werden mit der Vorlagenaufgabe kopiert, wenn Sie eine Vorlagenaufgabe kopieren. Die Informationen in den benutzerdefinierten Feldern werden nur dann an die neue Vorlagenaufgabe übertragen, wenn Sie die Option zum Kopieren benutzerdefinierter Daten auswählen.

* Die folgenden Elemente werden standardmäßig an die kopierte Vorlagenaufgabe übertragen:

   * Teilaufgaben

Beachten Sie beim Verschieben von Vorlagenaufgaben Folgendes:

* Die folgenden Informationen werden standardmäßig an die verschobene Aufgabe übertragen:

   * Benutzerdefinierte Formulare und benutzerdefinierte Feldinformationen
   * Teilaufgaben
   * Benutzerkommentare

* Die folgenden Informationen werden nicht an die verschobene Aufgabe übertragen:

   * Meilensteine

## Vorlagenaufgaben kopieren

Sie können eine einzelne Vorlagenaufgabe kopieren oder mehrere Vorlagenaufgaben stapelweise kopieren.

1. Wechseln Sie zu der Vorlage, die die Vorlagenaufgabe oder Vorlagenaufgaben enthält, die Sie kopieren möchten.
1. Klicken Sie im linken Bereich auf **Vorlagenaufgaben** .
1. Führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf den Namen einer Vorlagenaufgabe, um sie zu öffnen.
   * Wählen Sie eine oder mehrere Vorlagenaufgaben in der Liste aus.
1. (Bedingt) Klicken Sie oben in der Vorlagenaufgabenliste auf das Menü **Mehr** ![](assets/more-icon.png) oder bei geöffneter Aufgabe rechts vom Vorlagennamen, und klicken Sie dann auf **Kopieren nach** oder **Kopieren**, je nachdem, von wo aus Sie auf die Option Kopieren zugreifen.
Das Feld Vorlage kopieren wird geöffnet.
   ![](assets/copy-template-task-box-unshimmed.png)
1. (Optional) Benennen Sie die Vorlagenaufgabe im Feld **Vorlagenstammname** um.

   >[!TIP]
   >
   >Dieses Feld ist abgeblendet und kann nicht bearbeitet werden, wenn Sie mehrere Vorlagenaufgaben in eine Liste kopieren möchten. Sie können den Mauszeiger über das Feld &quot;Vorlagenname&quot;bewegen und eine Liste aller ausgewählten Vorlagenaufgaben wird angezeigt.

1. Beginnen Sie mit der Eingabe des Namens der **Zielvorlage**, in die Sie die Vorlagenaufgabe kopieren möchten, im Feld **Zielvorlage auswählen** und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

   Der aktuelle Vorlagenname wird standardmäßig angezeigt. Wenn Sie die Vorlagenaufgabe in dieselbe Vorlage kopieren möchten, lassen Sie dieses Feld unverändert.

   >[!TIP]
   >
   >Sie können auch mit der Eingabe der Referenznummer beginnen oder die Kennung der Vorlage eingeben. Auf diese Weise können Sie zwischen Vorlagen mit identischen Namen unterscheiden.

1. (Bedingt) Klicken Sie auf **Zugriffsanfrage** , um den Zugriff auf die Zielvorlage anzufordern, wenn Sie keinen Zugriff auf die ausgewählte Vorlage haben.
1. (Bedingt) Kopieren Sie die Vorlagenaufgabe weiterhin in die ausgewählte Zielvorlage, ohne Zugriff anzufordern, wenn Sie Zugriff haben, um Vorlagenaufgaben zu einer der Vorlagenaufgaben in der Zielvorlage hinzuzufügen.

1. Klicken Sie im linken Bereich auf **Optionen** und deaktivieren Sie dann die VorlagenAufgabenattribute, die Sie nicht mit der Vorlagenaufgabe kopieren möchten. Alle Optionen sind standardmäßig ausgewählt.

   >[!TIP]
   >
   >Wenn Sie die Option **Alle auswählen** deaktivieren, werden alle Optionen deaktiviert.

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


1. (Optional) Klicken Sie im linken Bereich auf **Übergeordnetes Element auswählen** und wählen Sie dann die Vorlagenaufgabe in der Zielvorlage aus, die Sie zum übergeordneten Element der kopierten Vorlagenaufgabe werden möchten.

   >[!TIP]
   >
   >Bei der Auswahl, mehrere Vorlagenaufgaben in eine Liste zu kopieren, werden alle ausgewählten Vorlagenaufgaben zu den untergeordneten Elementen des ausgewählten übergeordneten Objekts und werden nach den vorhandenen untergeordneten Aufgaben hinzugefügt.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste der Vorlage einen der übergeordneten Elemente im Vorlagenplan aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie nach einer übergeordneten Vorlagenaufgabe anhand des Namens.

   Die Vorlagenaufgabe sollte in der Liste angezeigt werden.

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Vorlagenaufgabe auswählen, werden die Vorlagenaufgaben als Hauptvorlagenaufgaben und nicht als Unteraufgaben kopiert und am Ende der Vorlagenaufgabenliste in der Zielvorlage platziert.

1. Klicken Sie auf **Vorlagenaufgabe kopieren**.

   Die kopierten Vorlagenaufgaben befinden sich nun in der angegebenen Vorlage und sind entweder Unteraufgaben der ausgewählten übergeordneten Vorlagenaufgabe oder der letzten Vorlagenaufgaben in der Vorlage.


## Vorlagenaufgaben verschieben

Sie können eine Vorlagenaufgabe entweder in eine andere Vorlagenaufgabe in derselben Vorlage oder in eine andere Vorlage verschieben. Sie können eine Vorlagenaufgabe oder mehrere Vorlagenaufgaben stapelweise verschieben.

1. Markieren Sie die Vorlage, die die zu verschiebenden Vorlagenaufgaben enthält.
1. Klicken Sie im linken Bereich auf **Vorlagenaufgaben** .
1. Führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf den Namen einer Vorlagenaufgabe, um sie zu öffnen.
   * Wählen Sie eine oder mehrere Vorlagenaufgaben in der Liste aus.
1. (Bedingt) Klicken Sie oben in der Vorlagenaufgabenliste auf das Menü **Mehr** ![](assets/more-icon.png) oder bei geöffneter Aufgabe rechts vom Vorlagenstammnamen, und klicken Sie dann auf **Verschieben nach** oder **Verschieben**, je nachdem, von wo aus Sie auf die Option Verschieben zugreifen.
Das Feld Vorlage verschieben wird geöffnet.
   ![](assets/move-template-task-box-unshimmed.png)

1. (Optional) Benennen Sie die Vorlagenaufgabe im Feld **Vorlagenstammname** um.

   >[!TIP]
   >
   >Dieses Feld ist abgeblendet und kann nicht bearbeitet werden, wenn Sie mehrere Vorlagenaufgaben in eine Liste verschieben möchten. Sie können den Mauszeiger über das Feld &quot;Vorlagenname&quot;bewegen und eine Liste aller ausgewählten Vorlagenaufgaben wird angezeigt.

1. Geben Sie den Namen der **Zielvorlage** ein, in die Sie die Vorlagenaufgabe in das Feld **Zielvorlage auswählen** verschieben möchten, und wählen Sie sie dann aus, wenn sie in der Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können auch mit der Eingabe der Referenznummer beginnen oder die Kennung der Vorlage eingeben. Auf diese Weise können Sie zwischen Vorlagen mit identischen Namen unterscheiden.

1. (Bedingt) Klicken Sie auf **Zugriffsanfrage** , um den Zugriff auf die Vorlage anzufordern, wenn Sie keinen Zugriff auf die Zielvorlage haben.
1. (Bedingt) Verschieben Sie die Vorlagenaufgabe weiterhin in die ausgewählte Zielvorlage, ohne Zugriff anzufordern, wenn Sie Zugriff haben, um Vorlagenaufgaben zu einer der Vorlagenaufgaben in der Zielvorlage hinzuzufügen.

1. Klicken Sie im linken Bereich auf **Optionen** und deaktivieren Sie dann die VorlagenAufgabenattribute, die Sie nicht mit der Vorlagenaufgabe kopieren möchten. Alle Optionen sind standardmäßig ausgewählt.

   >[!TIP]
   >
   >* Der Abschnitt Optionen ist erst verfügbar, nachdem Sie eine Zielvorlage ausgewählt haben.
   >* Wenn Sie die Option **Alle auswählen** deaktivieren, werden alle Optionen deaktiviert.

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


1. (Optional) Klicken Sie im linken Bereich auf **Übergeordnetes Element auswählen** und wählen Sie dann die Vorlagenaufgabe in der Zielvorlage aus, die Sie zum übergeordneten Element der verschobenen Vorlagenaufgabe werden möchten.

   >[!TIP]
   >
   >Bei der Auswahl, mehrere Vorlagenaufgaben in eine Liste zu verschieben, werden alle ausgewählten Vorlagenaufgaben zu den untergeordneten Elementen des ausgewählten übergeordneten Objekts und werden nach den vorhandenen untergeordneten Aufgaben hinzugefügt.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste der Vorlage einen der übergeordneten Elemente im Vorlagenplan aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie nach einer übergeordneten Vorlagenaufgabe anhand des Namens.

   Die Vorlagenaufgabe sollte in der Liste angezeigt werden.

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Vorlagenaufgabe auswählen, werden die Vorlagenaufgaben als Hauptvorlagenaufgaben und nicht als Unteraufgaben verschoben und am Ende der Vorlagenaufgabenliste auf der Zielvorlage platziert.

1. Klicken Sie auf **Vorlagenaufgabe verschieben**.

   Die verschobenen Vorlagenaufgaben befinden sich nun in der angegebenen Vorlage und sind entweder Unteraufgaben der ausgewählten übergeordneten Vorlagenaufgabe oder der letzten Vorlagenaufgaben in der Vorlage.
