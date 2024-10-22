---
content-type: overview
title: Zusammenfassungsübersicht
description: Sie können das Bedienfeld "Zusammenfassung"verwenden, um Arbeitselementinformationen direkt aus einer Liste von Aufgabenproblemen, Dokumenten oder aus anderen Bereichen von [!DNL Adobe Workfront] zu überprüfen und zu aktualisieren, in denen Aufgaben und Probleme angezeigt werden.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '960'
ht-degree: 2%

---

# [!UICONTROL Zusammenfassung] - Übersicht

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

Sie können das Bedienfeld [!UICONTROL Zusammenfassung] verwenden, um Arbeitselementinformationen direkt aus einer Liste von Aufgaben, Problemen, Dokumenten oder aus anderen Bereichen von [!DNL Adobe Workfront] zu überprüfen und zu aktualisieren, in denen Aufgaben und Probleme angezeigt werden.

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



Die folgende Tabelle zeigt die Bereiche, in denen Sie den Bereich [!UICONTROL Zusammenfassung] finden und verwenden können:

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

In diesem Artikel wird beschrieben, wie Sie auf das Bedienfeld [!UICONTROL Zusammenfassung] für Aufgaben und Probleme in Listen zugreifen und es verwenden.

Weitere Informationen zum Zugriff auf die [!UICONTROL Zusammenfassung] im [!UICONTROL Arbeitslade-Balancer] finden Sie unter [Aktualisieren von Arbeitselementen im [!UICONTROL Arbeitslade-Balancer] mithilfe der [!UICONTROL Zusammenfassung]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Informationen zum Zugriff auf die [!UICONTROL Zusammenfassung] für Dokumente finden Sie unter [[!UICONTROL Zusammenfassung] für die Dokumentübersicht](../../documents/managing-documents/summary-for-documents.md).

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

*Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Anzeigen des Bereichs [!UICONTROL Zusammenfassung] in einer Liste von Aufgaben oder Problemen

1. Markieren Sie eine Aufgabe oder ein Problem und wählen Sie ein Element in der Liste aus.
1. Klicken Sie auf das Symbol **[!UICONTROL Zusammenfassung]** ![](assets/qs-summary-in-new-toolbar-small.png)

   oder

   Klicken Sie auf das Symbol **[!UICONTROL Zusammenfassung öffnen]** ![](assets/open-summary-with-text-nwe.png) im Abschnitt [!UICONTROL Gesendet] des Bereichs [!UICONTROL Anforderungen] .

   Nachdem Sie die Zusammenfassung geöffnet haben, bleibt sie beim Klicken oder Auswählen anderer Aufgaben oder Probleme geöffnet und bleibt geöffnet, bis Sie sie manuell schließen.

   >[!TIP]
   >
   >Sie können jeweils nur eine Aufgabe oder ein Problem auswählen, um ihre Details im Bedienfeld [!UICONTROL Zusammenfassung] anzuzeigen.

   ![Bedienfeld &quot;Zusammenfassung&quot;](assets/summary-panel-for-task-new-comments.png)

1. (Optional) Führen Sie einen der folgenden Schritte aus, um das Bedienfeld [!UICONTROL Zusammenfassung] zu schließen:

   * Klicken Sie in einer Aufgaben- oder Problemliste auf das Symbol **[!UICONTROL Zusammenfassung öffnen]** ![](assets/summary-panel-icon.png)

     Oder

     Klicken Sie auf das Symbol **X** oben rechts im Bedienfeld [!UICONTROL Zusammenfassung].

   * Klicken Sie im Abschnitt [!UICONTROL Gesendet] im Bereich [!UICONTROL Anforderungen] auf das Symbol **[!UICONTROL Zusammenfassung schließen]** ![](assets/close-summary-with-text-nwe.png)

     Oder

     Klicken Sie auf das Symbol **X** oben rechts im Bedienfeld &quot;Zusammenfassung&quot;.

## [!UICONTROL Prozent abgeschlossen]

Verwenden Sie die Fortschrittsleiste oben in der [!UICONTROL Zusammenfassung] , um den Prozentsatz zu aktualisieren, der für die ausgewählte Aufgabe oder das ausgewählte Problem abgeschlossen ist. Geben Sie eine Zahl ein oder ziehen Sie die Leiste auf den richtigen Prozentsatz.

![Prozent abgeschlossen im Zusammenfassungsbereich](assets/summary-overview-percent-complete.png)

## [!UICONTROL Updates]

Verwenden Sie den Abschnitt [!UICONTROL Aktualisierungen] der [!UICONTROL Zusammenfassung] , um aktuelle Aktualisierungen anzuzeigen und Aktualisierungen zu der ausgewählten Aufgabe oder dem ausgewählten Problem vorzunehmen. Klicken Sie auf &quot;**[!UICONTROL See all]**&quot;, um direkt zur Registerkarte &quot;[!UICONTROL Updates]&quot;der Aufgabe zu gelangen.

Abschnitt ![Aktualisierungen im Zusammenfassungsbereich](assets/summary-updates-section.png)

## [!UICONTROL Dokumente]

Verwenden Sie den Abschnitt [!UICONTROL Dokumente] der [!UICONTROL Zusammenfassung], um Dokumente anzuzeigen, die an die ausgewählte Aufgabe oder das ausgewählte Problem angehängt sind. Klicken Sie auf die Miniaturansicht, um eine Dokumentvorschau zu öffnen. Um direkt zur Registerkarte [!UICONTROL Dokumente] für die Aufgabe oder das Problem zu wechseln, klicken Sie auf den Titel **[!UICONTROL Dokumente]** .

Abschnitt &quot;![Dokumente&quot;im Bereich &quot;Zusammenfassung&quot;](assets/summary-documents-section.png)

## [!UICONTROL Details]

Verwenden Sie den Abschnitt [!UICONTROL Details] der [!UICONTROL Zusammenfassung], um allgemeine Details zu Arbeitselementen anzuzeigen, Zuweisungen vorzunehmen oder Startdaten hinzuzufügen. Klicken Sie auf **[!UICONTROL Alle anzeigen]** , um direkt zur Registerkarte [!UICONTROL Details] der Aufgabe oder des Problems zu gelangen.



![Detailabschnitt im Zusammenfassungsbereich](assets/summary-details-section.png)

## [!UICONTROL Unteraufgaben]

Dieser Abschnitt ist nur für Aufgaben verfügbar. Verwenden Sie den Abschnitt [!UICONTROL Unteraufgaben] der [!UICONTROL Zusammenfassung], um die Unteraufgaben [!UICONTROL Neu], [!UICONTROL In Bearbeitung] und [!UICONTROL Geschlossen] für die ausgewählte Aufgabe anzuzeigen. Klicken Sie auf das Dropdown-Menü **[!UICONTROL Status]** , um zwischen Status zu wechseln. Um direkt zur Registerkarte [!UICONTROL Unteraufgaben] der Aufgabe zu wechseln, klicken Sie auf den &#x200B; Titel **[!UICONTROL Unteraufgaben]** .

Wenn Sie der Aufgabe keine Unteraufgaben hinzugefügt haben, klicken Sie auf **[!UICONTROL Hier hinzufügen]** , um direkt zur Registerkarte [!UICONTROL Unteraufgaben] der Aufgabe zu wechseln.

![Abschnitt &quot;Unteraufgaben&quot;im Bereich &quot;Zusammenfassung&quot;](assets/summary-subtasks-section.png)

## [!UICONTROL Stunden]

Verwenden Sie den Abschnitt [!UICONTROL Stunden] der [!UICONTROL Zusammenfassung], um Stunden für die ausgewählte Aufgabe oder das ausgewählte Problem zu protokollieren. Klicken Sie auf **[!UICONTROL Login Time]** und geben Sie Ihre Stunden ein. Um direkt zur Registerkarte Stunden für die Aufgabe oder das Problem zu wechseln, klicken Sie auf den Titel **[!UICONTROL Stunden]** .

Die Stundenzahl in der [!UICONTROL Zusammenfassung] zeigt die Stunden an, die Sie protokollieren. Andere Benutzer verfügen in der [!UICONTROL Zusammenfassung] je nach dem Zeitpunkt, zu dem sie sich bei der Aufgabe anmelden, über unterschiedliche Stundensummen.

Wenn für die Aufgabe oder das Problem keine [!UICONTROL Stunden] geplant sind und Sie die Zeit protokolliert haben, wird die Stunden-Leiste rot angezeigt.

Abschnitt &quot;![Stunden&quot;im Zusammenfassungsbereich](assets/summary-hours-section.png)

## Genehmigungen

Verwenden Sie den Abschnitt [!UICONTROL Validierungen] der [!UICONTROL Zusammenfassung], um die mit der ausgewählten Aufgabe bzw. dem ausgewählten Problem verbundenen Genehmigungen anzuzeigen. Wenn Sie keine Genehmigungen hinzugefügt haben, wählen Sie eine vorhandene Genehmigung aus dem Dropdown-Menü aus oder klicken Sie auf **[!UICONTROL Validierungsprozess für einmalige Verwendung erstellen]** , um direkt zur Registerkarte [!UICONTROL Validierungen] der Aufgabe oder des Problems zu gelangen.

Um direkt zur Registerkarte [!UICONTROL Genehmigungen] für die Aufgabe oder das Problem zu wechseln, klicken Sie auf den Titel **[!UICONTROL Genehmigungen]** .

![Abschnitt &quot;Genehmigungen&quot;im Zusammenfassungsbereich](assets/summary-approvals-section.png)
