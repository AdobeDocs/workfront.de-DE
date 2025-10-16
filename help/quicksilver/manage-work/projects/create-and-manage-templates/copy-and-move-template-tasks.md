---
product-area: templates
navigation-topic: templates-navigation-topic
title: Vorlagenaufgaben kopieren und verschieben
description: Sie können eine Vorlagenaufgabe in dieselbe Vorlage oder in eine andere Vorlage kopieren oder verschieben.
author: Alina
feature: Work Management
exl-id: a2e09e63-5c88-460c-9996-3a39fbb82150
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '2090'
ht-degree: 3%

---

# Vorlagenaufgaben kopieren und verschieben

Sie können eine Vorlagenaufgabe von einer Vorlage in eine andere Vorlage kopieren oder sie entweder in eine andere Vorlage oder an eine andere Stelle in derselben Vorlage verschieben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Vorlagen bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für eine Vorlage.</p> <p>Sie können eine Vorlagenaufgabe nicht freigeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a template.</p> <p>You cannot share a template task.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Überlegungen zum Kopieren oder Verschieben von Vorlagenaufgaben

Beachten Sie beim Kopieren von Vorlagenaufgaben Folgendes:

* Die folgenden Informationen werden nicht an die kopierte Aufgabe übertragen:

   * Meilensteine

* Sie haben die Möglichkeit, einige mit der Vorlagenaufgabe verknüpfte Elemente während des Kopiervorgangs in die kopierte Aufgabe zu kopieren. Standardmäßig werden die folgenden Objekte jedoch nicht an die kopierte Aufgabe übertragen:

   * Benutzerkommentare

* Benutzerdefinierte Formulare werden mit der Vorlagenaufgabe kopiert, wenn Sie eine Vorlagenaufgabe kopieren. Die Informationen in den benutzerdefinierten Feldern werden nur dann an die neue Vorlagenaufgabe übertragen, wenn Sie Benutzerdefinierte Daten kopieren.

* Die folgenden Elemente werden standardmäßig an die kopierte Vorlagenaufgabe übertragen:

   * Teilaufgaben

Beachten Sie beim Verschieben von Vorlagenaufgaben Folgendes:

* Die folgenden Informationen werden standardmäßig an die verschobene Aufgabe übertragen:

   * Benutzerdefinierte Formulare und Informationen zu benutzerdefinierten Feldern
   * Teilaufgaben
   * Benutzerkommentare

* Die folgenden Informationen werden nicht an die verschobene Aufgabe übertragen:

   * Meilensteine.

## Vorlagenaufgaben kopieren

Sie können eine einzelne Vorlagenaufgabe kopieren oder mehrere Vorlagenaufgaben stapelweise kopieren.

1. Wechseln Sie zu der Vorlage, die die Vorlagenaufgabe oder Vorlagenaufgaben enthält, die Sie kopieren möchten.
1. Klicken Sie **linken Bedienfeld** Vorlagenaufgaben“.
1. Führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf den Namen einer Vorlagenaufgabe, um sie zu öffnen.
   * Eine oder mehrere Vorlagenaufgaben in der Liste auswählen.
1. (Bedingt) Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/more-icon.png) oben in der Vorlagenaufgabenliste oder rechts neben dem Namen der Vorlagenaufgabe, wenn Sie die Aufgabe geöffnet haben. Klicken Sie dann je nachdem, von wo aus Sie auf die Option Kopieren zugreifen, auf **Kopieren nach** oder **Kopieren**.
Das Feld Vorlagenaufgabe kopieren wird geöffnet.
   ![Feld für Vorlagenaufgabe kopieren](assets/copy-template-task-box-unshimmed.png)
1. (Optional) Benennen Sie die Vorlagenaufgabe im Feld **Name der Vorlagenaufgabe** um.

   >[!TIP]
   >
   >Dieses Feld ist abgeblendet und kann nicht bearbeitet werden, wenn mehrere Vorlagenaufgaben in einer Liste kopiert werden sollen. Sie können den Mauszeiger über das Feld Name der Vorlagenaufgabe bewegen, und eine Liste aller ausgewählten Vorlagenaufgaben wird angezeigt.

1. Geben Sie zunächst den Namen der **Zielvorlage** in das Feld **Zielvorlage auswählen** ein, in das Sie die Vorlagenaufgabe kopieren möchten, und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

   Der aktuelle Vorlagenname wird standardmäßig angezeigt. Wenn Sie die Vorlagenaufgabe in dieselbe Vorlage kopieren möchten, lassen Sie dieses Feld unverändert.

   >[!TIP]
   >
   >Sie können auch mit der Eingabe der Referenznummer beginnen oder die ID der Vorlage eingeben. Auf diese Weise können Sie zwischen Vorlagen mit identischen Namen unterscheiden.

1. (Bedingt) Klicken Sie auf **Zugriff anfordern** um Zugriff auf die Zielvorlage anzufordern, wenn Sie keinen Zugriff auf die ausgewählte Vorlage haben.
1. (Bedingt) Kopieren Sie die Vorlagenaufgabe weiterhin in die ausgewählte Zielvorlage, ohne Zugriff anzufordern, wenn Sie Zugriff zum Hinzufügen von Vorlagenaufgaben zu einer der Vorlagenaufgaben in der Zielvorlage haben.

1. Klicken Sie **linken** auf „Optionen“ und heben Sie dann die Auswahl der Vorlagenaufgabenattribute auf, die Sie nicht mit der Vorlagenaufgabe kopieren möchten. Alle Optionen sind standardmäßig ausgewählt.

   >[!TIP]
   >
   >Wenn Sie **Alle auswählen** deaktivieren, werden alle Optionen deaktiviert.

   Deaktivieren Sie die Auswahl aus den folgenden Optionen, um sie nicht in die kopierte Vorlagenaufgabe zu übertragen. In der folgenden Tabelle wird beschrieben, was passiert, wenn die Optionen deaktiviert sind:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td>Deaktivieren Sie diese Option, um alle Informationen aus der Vorlagenaufgabe zu entfernen, wenn Sie sie an den neuen Speicherort kopieren. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Beschränkung</td> 
      <td> <p>Die Vorlagenaufgabe-Einschränkung wird auf So bald wie möglich oder So spät wie möglich basierend auf der Einstellung des Vorlagenzeitplanmodus festgelegt.</p> <p> Wenn diese Option aktiviert ist, wird die aktuelle Einschränkung der Vorlagenaufgabe auf die kopierte Vorlagenaufgabe übertragen. </p> 
      <p><b>NOTIZ</b>

   Wenn eine Vorlagenaufgabe mit datumsspezifischen Einschränkungen in eine andere Vorlage kopiert wird und die Einschränkungstermine der Vorlagenaufgabe außerhalb der Termine der neuen Vorlage liegen, wird entweder die Vorlagenaufgaben-Einschränkung auf „So bald wie möglich“ oder „So spät wie möglich“ geändert oder die geplanten Start- oder Abschlussdaten der Vorlagen werden angepasst.

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
      <td> <p>Das bedeutet, dass die Abhängigkeiten nicht auf die kopierten Vorlagenaufgaben übertragen werden. </p> <p>Wenn diese Option aktiviert ist, werden die Vorgänger innerhalb der Gruppe kopierter Vorlagenaufgaben beibehalten, andere werden gelöscht.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td> <p>Die Werte für die benutzerdefinierten Felder werden gelöscht und die benutzerdefinierten Formulare werden in die kopierte Vorlagenaufgabe übertragen. </p> <p>Wenn diese Option aktiviert ist, werden sowohl die Formulare als auch die Werte für die benutzerdefinierten Felder an die kopierte Vorlagenaufgabe übertragen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td>Die Finanzinformationen der kopierten Vorlagenaufgabe werden entfernt und Workfront aktualisiert den Vorlagenaufgaben-Kostentyp auf „Keine Kosten“ und den Vorlagenaufgaben-Umsatztyp auf „Nicht fakturierbar“.
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Die an die Vorlagenaufgabe angehängten Dokumente werden nicht an die kopierte Vorlagenaufgabe übertragen. Dazu gehören Versionen, Testsendungen und verknüpfte Dokumente.</p> <p><b>NOTIZ</b></p>

   <p>Dies umfasst keine Dokumentengenehmigungen. Dokumentgenehmigungen können niemals kopiert werden, wenn eine Vorlagenaufgabe kopiert wird.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td>Die Vorlagenaufgaben-Erinnerungen werden nicht an die kopierte Vorlagenaufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Die für die Vorlagenaufgabe protokollierten Ausgaben werden nicht auf die kopierte Vorlagenaufgabe übertragen. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Optional) Klicken Sie **linken Bereich auf**&#x200B;Übergeordnetes Element auswählen) und wählen Sie dann die Vorlagenaufgabe in der Zielvorlage aus, die Sie zum übergeordneten Element der kopierten Vorlagenaufgabe werden möchten.

   >[!TIP]
   >
   >Wenn Sie auswählen, mehrere Vorlagenaufgaben in eine Liste zu kopieren, werden alle ausgewählten Vorlagenaufgaben zu untergeordneten Aufgaben des ausgewählten übergeordneten Elements und werden nach den vorhandenen untergeordneten Aufgaben hinzugefügt.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste eine der übergeordneten Elemente im Vorlagenplan aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie nach einer übergeordneten Vorlagenaufgabe anhand des Namens.

   Die Vorlagenaufgabe sollte in der Liste angezeigt werden.

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Vorlagenaufgabe auswählen, werden die Vorlagenaufgaben nicht als Unteraufgaben, sondern als Hauptvorlagenaufgaben kopiert und an das Ende der Vorlagenaufgabenliste in der Zielvorlage gesetzt.

1. Klicken Sie **Vorlagenaufgabe kopieren**.

   Die kopierten Vorlagenaufgaben befinden sich nun auf der angegebenen Vorlage und sind entweder Teilaufgaben der ausgewählten übergeordneten Vorlagenaufgabe oder die letzten Vorlagenaufgaben auf der Vorlage.


## Vorlagenaufgaben verschieben

Sie können eine Vorlagenaufgabe entweder in eine andere Vorlagenaufgabe in derselben Vorlage oder in eine andere Vorlage verschieben. Sie können eine Vorlagenaufgabe oder mehrere Vorlagenaufgaben in großen Mengen verschieben.

1. Wechseln Sie zu der Vorlage, die die Vorlagenaufgabe oder Vorlagenaufgaben enthält, die Sie verschieben möchten.
1. Klicken Sie **linken Bedienfeld** Vorlagenaufgaben“.
1. Führen Sie einen der folgenden Schritte aus:
   * Klicken Sie auf den Namen einer Vorlagenaufgabe, um sie zu öffnen.
   * Eine oder mehrere Vorlagenaufgaben in der Liste auswählen.
1. (Bedingt) Klicken Sie auf das **Mehr**-Menü ![Mehr-Symbol](assets/more-icon.png) oben in der Vorlagenaufgabenliste oder rechts neben dem Namen der Vorlagenaufgabe, wenn Sie die Aufgabe geöffnet haben, und klicken Sie dann auf **Verschieben nach** oder **Verschieben**, je nachdem, von wo aus Sie auf die Option Verschieben zugreifen.
Das Feld Vorlagenaufgabe verschieben wird geöffnet.
   ![Feld für Vorlagenaufgabe verschieben](assets/move-template-task-box-unshimmed.png)

1. (Optional) Benennen Sie die Vorlagenaufgabe im Feld **Name der Vorlagenaufgabe** um.

   >[!TIP]
   >
   >Dieses Feld ist abgeblendet und kann nicht bearbeitet werden, wenn ausgewählt wird, mehrere Vorlagenaufgaben in einer Liste zu verschieben. Sie können den Mauszeiger über das Feld Name der Vorlagenaufgabe bewegen, und eine Liste aller ausgewählten Vorlagenaufgaben wird angezeigt.

1. Geben Sie zunächst den Namen der **Zielvorlage** in das Feld **Zielvorlage auswählen** ein, in das Sie die Vorlagenaufgabe verschieben möchten, und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

   >[!TIP]
   >
   >Sie können auch mit der Eingabe der Referenznummer beginnen oder die ID der Vorlage eingeben. Auf diese Weise können Sie zwischen Vorlagen mit identischen Namen unterscheiden.

1. (Bedingt) Klicken Sie auf **Zugriff anfordern** um Zugriff auf die Vorlage anzufordern, wenn Sie keinen Zugriff auf die Zielvorlage haben.
1. (Bedingt) Verschiebt die Vorlagenaufgabe weiterhin in die ausgewählte Zielvorlage, ohne Zugriff anzufordern, wenn ihr Zugriff zum Hinzufügen von Vorlagenaufgaben zu einer der Vorlagenaufgaben in der Zielvorlage habt.

1. Klicken Sie **linken** auf „Optionen“ und heben Sie dann die Auswahl der Vorlagenaufgabenattribute auf, die Sie nicht mit der Vorlagenaufgabe kopieren möchten. Alle Optionen sind standardmäßig ausgewählt.

   >[!TIP]
   >
   >* Der Abschnitt Optionen ist erst verfügbar, nachdem Sie eine Zielvorlage ausgewählt haben.
   >* Wenn Sie **Alle auswählen** deaktivieren, werden alle Optionen deaktiviert.

   Deaktivieren Sie die Auswahl aus den folgenden Optionen, um die Informationen nicht an die verschobene Vorlagenaufgabe zu übertragen. In der folgenden Tabelle wird beschrieben, was passiert, wenn die Optionen deaktiviert sind:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
    <tr> 
      <td role="rowheader">Alle auswählen</td> 
      <td>Deaktivieren Sie diese Option, um alle Informationen aus der Vorlagenaufgabe zu entfernen, wenn Sie sie an die neue Position verschieben. </td> 
     </tr>
     <tr> 
      <td role="rowheader">Beschränkung</td> 
      <td> <p>Die Vorlagenaufgabe-Einschränkung wird auf So bald wie möglich oder So spät wie möglich basierend auf der Einstellung des Vorlagenzeitplanmodus festgelegt.</p> <p> Wenn diese Option aktiviert ist, wird die aktuelle Einschränkung der Vorlagenaufgabe auf die verschobene Vorlagenaufgabe übertragen. </p>

   <p><b>NOTIZ</b>

   Wenn eine Vorlagenaufgabe mit datumsspezifischen Einschränkungen in eine andere Vorlage verschoben wird und die Einschränkungstermine der Vorlagenaufgabe außerhalb der Termine der neuen Vorlage liegen, wird entweder die Vorlagenaufgabenbeschränkung auf So bald wie möglich oder So spät wie möglich geändert oder die geplanten Start- oder Abschlussdaten der Vorlagen werden angepasst.

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
      <td> <p>Das bedeutet, dass die Abhängigkeiten mit den verschobenen Vorlagenaufgaben nicht übernommen werden. </p> <p>Wenn diese Option aktiviert ist, werden die Vorgänger innerhalb der Gruppe verschobener Vorlagenaufgaben beibehalten, andere werden gelöscht.</p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Benutzerdefinierte Daten</td> 
      <td> <p>Die Werte für die benutzerdefinierten Felder werden gelöscht und die benutzerdefinierten Formulare werden mit der verschobenen Vorlagenaufgabe übertragen. </p> <p>Wenn diese Option aktiviert ist, werden sowohl die Formulare als auch die Werte für die benutzerdefinierten Felder mit der verschobenen Vorlagenaufgabe übertragen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Finanzinformationen</td> 
      <td>Die Finanzinformationen der verschobenen Vorlagenaufgabe werden entfernt und Workfront aktualisiert den Vorlagenaufgaben-Kostentyp auf „Keine Kosten“ und den Vorlagenaufgaben-Umsatztyp auf „Nicht fakturierbar“.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td> <p>Die an die Vorlagenaufgabe angehängten Dokumente werden nicht mit der verschobenen Vorlagenaufgabe übertragen. Dazu gehören Versionen, Testsendungen und verknüpfte Dokumente.</p>

   <p><b>NOTIZ</b></p>

   <ul><li>
      <p>Dies umfasst keine Dokumentengenehmigungen. Dokumentgenehmigungen können beim Verschieben einer Vorlagenaufgabe nicht verschoben werden.</p> </li>
      <li>Wenn Sie sich dafür entscheiden, die Dokumente nicht mit der Vorlagenaufgabe verschieben zu lassen, werden die Dokumente gelöscht und für 30 Tage in den Papierkorb gelegt. Ein Administrator kann sie wiederherstellen und sie werden bei der verschobenen Vorlagenaufgabe wiederhergestellt.

   Wenn die Vorlagenaufgabe nach dem Verschieben gelöscht wird, werden die wiederhergestellten Dokumente im Bereich Dokumente auf der Benutzerseite des Administrators platziert, der sie wiederherstellt. </li> </ul>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erinnerungsnachrichten</td> 
      <td>Die Vorlagenaufgabenerinnerungen werden nicht an die verschobene Vorlagenaufgabe übertragen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ausgaben</td> 
      <td>Die in der Vorlagenaufgabe protokollierten Ausgaben werden nicht mit der verschobenen Vorlagenaufgabe übertragen. </td> 
     </tr>  
    </tbody> 
   </table>


1. (Optional) Klicken Sie **linken Bereich auf**&#x200B;Übergeordnetes Element auswählen) und wählen Sie dann die Vorlagenaufgabe in der Zielvorlage aus, die Sie zum übergeordneten Element der verschobenen Vorlagenaufgabe werden möchten.

   >[!TIP]
   >
   >Wenn Sie auswählen, dass mehrere Vorlagenaufgaben in einer Liste verschoben werden sollen, werden alle ausgewählten Vorlagenaufgaben zu untergeordneten Aufgaben des ausgewählten übergeordneten Elements und werden nach den vorhandenen untergeordneten Aufgaben hinzugefügt.

   Wählen Sie ein übergeordnetes Element aus, indem Sie einen der folgenden Schritte ausführen:

   * Wählen Sie in der Aufgabenliste eine der übergeordneten Elemente im Vorlagenplan aus.
   * Klicken Sie auf das Suchsymbol ![Suchsymbol](assets/search-icon.png) und suchen Sie nach einer übergeordneten Vorlagenaufgabe anhand des Namens.

   Die Vorlagenaufgabe sollte in der Liste angezeigt werden.

1. Wählen Sie das Optionsfeld für das übergeordnete Element aus, nachdem Sie es gefunden haben.

   Wenn Sie keine übergeordnete Vorlagenaufgabe auswählen, werden die Vorlagenaufgaben nicht als Unteraufgaben, sondern als Hauptvorlagenaufgaben verschoben und an das Ende der Vorlagenaufgabenliste in der Zielvorlage platziert.

1. Klicken Sie **Vorlagenaufgabe verschieben**.

   Die verschobenen Vorlagenaufgaben befinden sich nun auf der angegebenen Vorlage und sind entweder Teilaufgaben der ausgewählten übergeordneten Vorlagenaufgabe oder die letzten Vorlagenaufgaben auf der Vorlage.
