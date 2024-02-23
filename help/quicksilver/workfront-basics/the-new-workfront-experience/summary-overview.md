---
content-type: overview
title: Zusammenfassungsübersicht
description: Sie können das Bedienfeld "Zusammenfassung"verwenden, um Arbeitselementinformationen direkt aus einer Liste von Aufgabenproblemen, Dokumenten oder aus anderen Bereichen von [!DNL Adobe Workfront] die Aufgaben und Probleme anzeigen.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: ba81706f457e41c989bc34d9bdff81223b0d745e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 1%

---

# [!UICONTROL Zusammenfassung] Übersicht

{{highlighted-preview}}

Sie können die [!UICONTROL Zusammenfassung] -Bedienfeld zum Überprüfen und Aktualisieren von Arbeitselementinformationen direkt aus einer Liste von Aufgabenproblemen, Dokumenten oder aus anderen Bereichen von [!DNL Adobe Workfront] die Aufgaben und Probleme anzeigen.

Die folgende Tabelle zeigt die Bereiche, in denen Sie die [!UICONTROL Zusammenfassung] Bereich:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>Aufgaben</td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabenlisten innerhalb einer</p> 
    <ul> 
     <li>Projekt</li> 
     <li>Teilaufgabe</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Aufgaben in den Arbeitsbereichen [!UICONTROL Nicht zugewiesen] und [!UICONTROL Zugewiesene] Arbeitsbereiche des [!UICONTROL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Probleme</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Problemlisten in einer</p> 
    <ul> 
     <li>Projekt</li> 
     <li>Aufgabe</li> 
     <li>Teilaufgabe</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Probleme im Bereich [!UICONTROL Zugewiesene Arbeit] des [!UICONTROL Workload Balancer]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Probleme im Abschnitt [!UICONTROL Gesendet] des Bereichs [!UICONTROL Anforderungen]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Dokumente</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dokumente] Bereich</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dokumente] Abschnitt jedes Objekts (Projekt, Aufgabe, Problem, Programm, Portfolio, Vorlage, Vorlagenaufgabe, Benutzer)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

In diesem Artikel wird beschrieben, wie Sie auf die [!UICONTROL Zusammenfassung] Bedienfeld für Aufgaben und Probleme in Listen.

Informationen zum Zugriff auf die [!UICONTROL Zusammenfassung] im [!UICONTROL Lastenausgleich], siehe [Arbeitselemente in der [!UICONTROL Lastenausgleich] mithilfe der [!UICONTROL Zusammenfassung]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Informationen zum Zugriff auf die [!UICONTROL Zusammenfassung] für Dokumente, siehe [[!UICONTROL Zusammenfassung] für Dokumentübersicht](../../documents/managing-documents/summary-for-documents.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höher Zugriff auf Aufgaben, Probleme, Dokumente</p> <p>[!UICONTROL Ansicht] oder höher Zugriff auf alle Objekte, für die Sie die Dokumentzusammenfassung anzeigen möchten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Informationen zur Verwendung von [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für Aufgaben, Probleme oder Dokumente</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Anzeigen der [!UICONTROL Zusammenfassung] in einer Liste von Aufgaben oder Problemen

1. Markieren Sie eine Aufgabe oder ein Problem und wählen Sie ein Element in der Liste aus.
1. Klicken Sie auf **[!UICONTROL Zusammenfassung]** icon ![](assets/qs-summary-in-new-toolbar-small.png)

   oder

   Klicken Sie auf **[!UICONTROL Zusammenfassung öffnen]** icon ![](assets/open-summary-with-text-nwe.png) im [!UICONTROL Gesendet] Abschnitt [!UICONTROL Anforderungen] Bereich.

   Nachdem Sie die Zusammenfassung geöffnet haben, bleibt sie beim Klicken oder Auswählen anderer Aufgaben oder Probleme geöffnet und bleibt geöffnet, bis Sie sie manuell schließen.

   >[!TIP]
   >
   >Sie können nur eine Aufgabe oder ein Problem gleichzeitig auswählen, um ihre Details im [!UICONTROL Zusammenfassung] Bedienfeld.

   <div class="preview">

   Beispiel des Zusammenfassungs-Bedienfelds in der Vorschau-Umgebung:
   ![Zusammenfassungsbereich](assets/summary-panel-for-task-new-comments.png)

   </div>

   Beispiel des Zusammenfassungsbereichs in der Produktionsumgebung:
   ![Zusammenfassungsbereich](assets/summary-panel-for-task.png)

1. (Optional) So schließen Sie die [!UICONTROL Zusammenfassung] einen der folgenden Schritte ausführen:

   * Klicken Sie in einer Aufgaben- oder Problemliste auf die **[!UICONTROL Zusammenfassung öffnen]** icon ![](assets/summary-panel-icon.png)

     Oder

     Klicken Sie auf **X** rechts oben im [!UICONTROL Zusammenfassung] Bedienfeld.

   * Im [!UICONTROL Gesendet] Abschnitt [!UICONTROL Anforderungen] Bereich, klicken Sie auf die **[!UICONTROL Zusammenfassung schließen]** icon ![](assets/close-summary-with-text-nwe.png)

     Oder

     Klicken Sie auf **X** in der oberen rechten Ecke des Bedienfelds &quot;Zusammenfassung&quot;angezeigt.

## [!UICONTROL Prozent abgeschlossen]

Verwenden Sie die Fortschrittsleiste oben im [!UICONTROL Zusammenfassung] , um den Prozentsatz zu aktualisieren, der für die ausgewählte Aufgabe oder das ausgewählte Problem abgeschlossen ist. Geben Sie eine Zahl ein oder ziehen Sie die Leiste auf den richtigen Prozentsatz.

![Prozent abgeschlossen im Bereich &quot;Zusammenfassung&quot;](assets/summary-overview-percent-complete.png)

## [!UICONTROL Updates]

Verwenden Sie die [!UICONTROL Updates] Abschnitt [!UICONTROL Zusammenfassung] , um aktuelle Aktualisierungen anzuzeigen und Aktualisierungen zu der ausgewählten Aufgabe oder Ausgabe vorzunehmen. Klicks **[!UICONTROL Alle anzeigen]** , um direkt zur [!UICONTROL Updates] Registerkarte der Aufgabe.

<div class="preview">

Beispiel für Aktualisierungen in der Vorschau-Umgebung:
![Abschnitt &quot;Aktualisierungen&quot;im Bereich &quot;Zusammenfassung&quot;](assets/summary-updates-section.png)

</div>

Beispiel für Aktualisierungen in der Produktionsumgebung:
![Abschnitt &quot;Aktualisierungen&quot;im Bereich &quot;Zusammenfassung&quot;](assets/summary-updates-with-block-quote-350x290.png)

## [!UICONTROL Dokumente]

Verwenden Sie die [!UICONTROL Dokumente] Abschnitt [!UICONTROL Zusammenfassung] , um Dokumente anzuzeigen, die an die ausgewählte Aufgabe oder das ausgewählte Problem angehängt sind. Klicken Sie auf die Miniaturansicht, um eine Dokumentvorschau zu öffnen. So wechseln Sie direkt zum [!UICONTROL Dokumente] auf der Registerkarte der Aufgabe oder des Problems auf **[!UICONTROL Dokumente]** title.

![Abschnitt &quot;Dokumente&quot;im Bedienfeld &quot;Zusammenfassung&quot;](assets/summary-documents-section.png)

## [!UICONTROL Details]

Verwenden Sie die [!UICONTROL Details] Abschnitt [!UICONTROL Zusammenfassung] , um allgemeine Details zu Arbeitselementen anzuzeigen, Zuweisungen vorzunehmen oder Startdaten hinzuzufügen. Klicks **[!UICONTROL Alle anzeigen]** , um direkt zur [!UICONTROL Details] auf die Aufgabe oder das Problem.

>[!NOTE]
>
>Die in diesem Abschnitt angezeigten Felder sind dieselben, die im rechten Bereich auf der Startseite angezeigt werden. Diese Felder können angepasst werden [Anpassen [!UICONTROL Startseite] und [!UICONTROL Zusammenfassung] Layout-Vorlage verwenden](../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).

![Detailabschnitt im Bereich &quot;Zusammenfassung&quot;](assets/summary-details-section.png)

## [!UICONTROL Unteraufgaben]

Dieser Abschnitt ist nur für Aufgaben verfügbar. Verwenden Sie die [!UICONTROL Unteraufgaben] Abschnitt [!UICONTROL Zusammenfassung] in der Ansicht [!UICONTROL Neu], [!UICONTROL In Bearbeitung], und [!UICONTROL Geschlossen] Unteraufgaben für die ausgewählte Aufgabe. Klicken Sie auf **[!UICONTROL Status]** Dropdown-Menü, um zwischen Status zu wechseln. So wechseln Sie direkt zum [!UICONTROL Unteraufgaben] auf der Registerkarte der Aufgabe klicken Sie auf **[!UICONTROL Unteraufgaben]**&#x200B; Titel.

Wenn Sie der Aufgabe keine Unteraufgaben hinzugefügt haben, klicken Sie auf **[!UICONTROL Einen hier hinzufügen]** , um direkt zur [!UICONTROL Unteraufgaben] Registerkarte der Aufgabe.

![Bereich &quot;Unteraufgaben&quot;im Bereich &quot;Zusammenfassung&quot;](assets/summary-subtasks-section.png)

## [!UICONTROL Stunden]

Verwenden Sie die [!UICONTROL Stunden] Abschnitt [!UICONTROL Zusammenfassung] , um Stunden zur ausgewählten Aufgabe oder Ausgabe zu protokollieren. Klicks **[!UICONTROL Protokollzeit]** und geben Sie Ihre Stunden ein. Um direkt zur Registerkarte Stunden der Aufgabe oder des Problems zu wechseln, klicken Sie auf die Schaltfläche **[!UICONTROL Stunden]** title.

Die Stundenanzahl in der [!UICONTROL Zusammenfassung] zeigt die Stunden an, die Sie protokollieren. Andere Benutzer haben unterschiedliche Stundensummen in der [!UICONTROL Zusammenfassung] abhängig von der Zeit, zu der sie sich bei der Aufgabe anmelden.

Wenn es keine Planung gibt [!UICONTROL Stunden] bei der Aufgabe oder dem Problem angezeigt und Sie die Zeit protokolliert haben, wird die Stunden-Leiste rot angezeigt.

![Abschnitt &quot;Stunden&quot;im Bedienfeld &quot;Zusammenfassung&quot;](assets/summary-hours-section.png)

## Genehmigungen

Verwenden Sie die [!UICONTROL Genehmigungen] Abschnitt [!UICONTROL Zusammenfassung] , um Genehmigungen anzuzeigen, die mit der ausgewählten Aufgabe oder Ausgabe verbunden sind. Wenn Sie noch keine Validierungen hinzugefügt haben, wählen Sie eine vorhandene Validierung aus dem Dropdown-Menü aus oder klicken Sie auf **[!UICONTROL Erstellen eines Validierungsprozesses für den einmaligen Einsatz]** , um direkt zur [!UICONTROL Genehmigungen] auf die Aufgabe oder das Problem.

So wechseln Sie direkt zum [!UICONTROL Genehmigungen] auf der Registerkarte der Aufgabe oder des Problems auf **[!UICONTROL Genehmigungen]** title.

![Abschnitt &quot;Genehmigungen&quot;im Bereich &quot;Zusammenfassung&quot;](assets/summary-approvals-section.png)
