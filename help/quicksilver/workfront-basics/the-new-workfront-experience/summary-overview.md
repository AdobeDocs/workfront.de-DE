---
content-type: overview
title: Zusammenfassungsübersicht
description: Sie können das Bedienfeld "Zusammenfassung"verwenden, um Arbeitselementinformationen direkt aus einer Liste von Aufgabenproblemen, Dokumenten oder aus anderen Bereichen von [!DNL Adobe Workfront] die Aufgaben und Probleme anzeigen.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 5d6e9788ccbae7a8970cff56558233a57ceee1ab
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 2%

---

# [!UICONTROL Zusammenfassung] Übersicht

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

Sie können die [!UICONTROL Zusammenfassung] -Bedienfeld zum Überprüfen und Aktualisieren von Arbeitselementinformationen direkt aus einer Liste von Aufgaben, Problemen, Dokumenten oder anderen Bereichen von [!DNL Adobe Workfront] die Aufgaben und Probleme anzeigen.

Ihr Workfront- oder Gruppenadministrator kann die Bereiche und Felder ändern, die im Bedienfeld &quot;Zusammenfassung&quot;angezeigt werden. Sie können dem Bedienfeld &quot;Zusammenfassung&quot;bis zu 16 Felder hinzufügen.

>[!IMPORTANT]
>
>Es wird empfohlen, Felder hinzuzufügen, die Sie häufig im Bedienfeld &quot;Zusammenfassung&quot;aktualisieren müssen, damit Sie einfach darauf zugreifen und sie aktualisieren können, ohne auf die Hauptseite des Objekts zugreifen zu müssen.
>
>Sie können beispielsweise die folgenden häufig aktualisierten Felder zu den Aufgaben und Problemen in den Bedienfeldern &quot;Zusammenfassung&quot;hinzufügen:
>
>* Status
>* Prozent abgeschlossen
>* Verpflichtungsdatum
>* Geplantes Abschlussdatum
>* Bedingung



Die folgende Tabelle zeigt die Bereiche, in denen Sie die [!UICONTROL Zusammenfassung] Bereich:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>Aufgaben</b></td> 
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
   <tr> 
   <td>Aufgaben in einem [!UICONTROL Zeitblatt]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>Probleme</b></td> 
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
</tr> 
   <tr> 
   <td>Probleme in einem [!UICONTROL Timesheet]</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>Dokumente</b></td> 
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
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Neu: Mitarbeiter oder höher</p>
   Oder
   <p>Aktuell:[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfiguration der Zugriffsebene</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höher Zugriff auf Aufgaben, Probleme, Dokumente</p> <p>[!UICONTROL Ansicht] oder höher Zugriff auf Objekte, für die Sie Dokumente anzeigen möchten [!UICONTROL Zusammenfassung]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für Aufgaben, Probleme oder Dokumente</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren [!DNL Workfront] Administrator. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Anzeigen der [!UICONTROL Zusammenfassung] in einer Liste von Aufgaben oder Problemen

1. Markieren Sie eine Aufgabe oder ein Problem und wählen Sie ein Element in der Liste aus.
1. Klicken Sie auf **[!UICONTROL Zusammenfassung]** icon ![](assets/qs-summary-in-new-toolbar-small.png)

   oder

   Klicken Sie auf **[!UICONTROL Zusammenfassung öffnen]** icon ![](assets/open-summary-with-text-nwe.png) im [!UICONTROL Gesendet] Abschnitt [!UICONTROL Anforderungen] Bereich.

   Nachdem Sie die Zusammenfassung geöffnet haben, bleibt sie beim Klicken oder Auswählen anderer Aufgaben oder Probleme geöffnet und bleibt geöffnet, bis Sie sie manuell schließen.

   >[!TIP]
   >
   >Sie können nur eine Aufgabe oder ein Problem gleichzeitig auswählen, um ihre Details im [!UICONTROL Zusammenfassung] Bedienfeld.

   ![Zusammenfassungsbereich](assets/summary-panel-for-task-new-comments.png)

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

![Abschnitt &quot;Aktualisierungen&quot;im Bereich &quot;Zusammenfassung&quot;](assets/summary-updates-section.png)

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
