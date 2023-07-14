---
title: Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer sehen, wenn sie auf eine Aufgabe oder ein Problem in der Startseite und in der Zusammenfassung klicken. Jede Konfiguration, die Sie mithilfe der folgenden Schritte vornehmen, wirkt sich auf die gleiche Weise auf den Startbereich und den Zusammenfassungsbereich aus. Diese Anpassungen gelten nicht für das Bedienfeld "Dokumentzusammenfassung".
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 2%

---

# Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage

Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer sehen, wenn sie auf eine Aufgabe oder ein Problem in der Startseite und in der Zusammenfassung klicken. Jede Konfiguration, die Sie mithilfe der folgenden Schritte vornehmen, wirkt sich auf die gleiche Weise auf den Startbereich und den Zusammenfassungsbereich aus. Diese Anpassungen gelten nicht für das Bedienfeld &quot;Dokumentzusammenfassung&quot;.

Sie können Folgendes konfigurieren:

* Welche Felder werden für eine Aufgabe oder ein Problem im Bereich Details angezeigt und in welcher Reihenfolge
* Ob Aktualisierungen, aufgezeichnete Zeit, angehängte Dokumente und Zeitstempel für eine ausgewählte Aufgabe oder ein ausgewähltes Problem angezeigt werden

Sie können auch die Felder anpassen, die Benutzern im Bereich Startseite angezeigt werden, wenn Benutzer auf eine ihnen zugewiesene Projektgenehmigung, Dokumentgenehmigung oder Dokumentversionsgenehmigung klicken.

Informationen zum Startbereich finden Sie unter [Verwenden des Startbereichs](../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md). Weitere Informationen zum Bedienfeld &quot;Zusammenfassung&quot;finden Sie unter [Zusammenfassungsübersicht](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Informationen zum Erstellen von Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Gruppenlayoutvorlagen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layoutvorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layoutvorlage zu Benutzern finden Sie unter [Benutzer einer Layoutvorlage zuweisen](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassen von Startseite und Zusammenfassung mithilfe einer Layoutvorlage

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie beschrieben in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

1. Klicken Sie auf den Abwärtspfeil. ![](assets/dropdown-arrow.png) under **Anpassen der Ansicht von Benutzern** Klicken Sie auf **Startseite und Zusammenfassung**.

1. Klicken Sie in der Liste auf der linken Seite auf den Objekttyp (**Aufgaben**, **Probleme**, **Projekte**, **Dokumente** oder **Dokumentversionen**), die Sie in Startseite und Zusammenfassung anpassen möchten.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aufgaben</td> 
      <td> <p>Auf der Startseite wirkt sich Ihre Konfiguration für diese Einstellung auf den Bereich rechts neben einer Aufgabe aus, wenn ein Benutzer auf die Aufgabe klickt. In einer Aufgabenliste wirkt sich dies auf das Bedienfeld Zusammenfassung aus, das rechts auf der Seite angezeigt wird, wenn ein Benutzer eine Aufgabe auswählt, und dann auf das Symbol Zusammenfassung öffnen <img src="assets/summary-panel-icon.png">.</p> <p>Sie können beispielsweise festlegen, welche Felder Benutzern im Bereich Details angezeigt werden, wenn Benutzer Aufgaben auf der Startseite auswählen:</p> <p><img src="assets/home-details-adobe branding.jpg"></p> <p>Und wenn sie eine Aufgabe in der Zusammenfassung auswählen:</p> <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Probleme</td> 
      <td> <p>Auf der Startseite wirkt sich Ihre Konfiguration für diese Einstellung auf den Bereich rechts neben einem Problem aus, wenn ein Benutzer auf das Problem klickt.</p> <p>In einer Liste von Problemen wirkt sich diese Einstellung auf das Bedienfeld Zusammenfassung aus, das rechts auf der Seite angezeigt wird, wenn ein Benutzer ein Problem auswählt, und dann auf das Symbol Zusammenfassung öffnen <img src="assets/summary-panel-icon.png">.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projekte</td> 
      <td>Wenn auf der Startseite ein Benutzer auf eine ihm zugewiesene Projektgenehmigung klickt, wirkt sich Ihre Konfiguration für diese Einstellung auf den Bereich rechts neben der Genehmigung aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td>Wenn auf der Startseite ein Benutzer auf eine ihm zugewiesene Dokumentgenehmigung klickt, wirkt sich Ihre Konfiguration für diese Einstellung auf den Bereich rechts neben der Genehmigung aus.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumentversionen</td> 
      <td>Wenn auf der Startseite ein Benutzer auf eine Genehmigung klickt, die ihm für eine bestimmte Version eines Dokuments zugewiesen wurde, wirkt sich Ihre Konfiguration für diese Einstellung auf den Bereich rechts neben der Genehmigung aus.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Wenn die Zuweisung einer Aufgabe aufgehoben wird, werden dem Benutzer, der der Layoutvorlage zugewiesen ist, die Feldanpassungen in der Zusammenfassung nicht angezeigt.

1. (Bedingt) Wenn Sie im vorherigen Schritt auf Aufgaben oder Probleme geklickt haben, wählen Sie die Kategorie der Aufgabe oder des Problems aus, die Sie anpassen möchten.

   ![](assets/choose-cat-cstmz-nwe-adobe-branding.png)

1. (Bedingt) Wenn die Variable **Schaltfläche &quot;Primäre Aktion festlegen&quot;** Dropdown-Menü angezeigt (wenn Sie **Aufgaben** oder **Probleme** Klicken Sie links in der Liste auf die primäre Aktion (**Fertig** oder **Status**), die Sie Benutzern im Bereich Startseite und im Bereich Zusammenfassung zur Verfügung stellen möchten, wenn sie eine Aufgabe oder ein Problem anzeigen.

   ![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)

1. Hinzufügen ![](assets/add-item-plus-in-circle-blue.png) oder ausblenden ![](assets/close-or-hide---x.png) -Felder für den ausgewählten Objekttyp.

   ![](assets/lt-home-add-hide-fields-adobe-branding.png)

1. Wiederholen Sie die Schritte 3 bis 6, um den Startbereich und das Bedienfeld &quot;Zusammenfassung&quot;für alle anderen Objekttypen anzupassen.
1. Klicken **Globale Einstellungen** in der Nähe der linken unteren Ecke eine der folgenden Optionen für Adobe Workfront-Objekte in Startseite und Zusammenfassung aktivieren oder deaktivieren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Updates für Arbeiten anzeigen</td> 
      <td>Zeigt alle Aktualisierungen an, die an einer ausgewählten Aufgabe oder einem Problem in der Startseite oder Zusammenfassung vorgenommen wurden. Dies umfasst sowohl Systemaktualisierungen als auch Aktualisierungen, die von einem Benutzer vorgenommen werden. Benutzer können Systemaktualisierungen weiterhin herausfiltern, wie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Systemaktualisierungen aktivieren oder deaktivieren</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Update der Arbeit</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeit für Arbeit erfassen</td> 
      <td>Zeigt die Option Arbeitszeit bei Arbeit protokollieren an, wenn eine Aufgabe oder ein Problem ausgewählt ist. Dadurch können Benutzer die Arbeitszeit für Arbeitselemente direkt über die Bereiche Startseite und Zusammenfassung protokollieren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anzeigen von Dokumenten, die mit Arbeiten verknüpft sind</td> 
      <td>Zeigt den Bereich "Dokumente"in Startseite und Zusammenfassung an, wenn eine Aufgabe oder ein Problem ausgewählt ist, und listet alle Dokumente auf, die mit der Aufgabe oder dem Problem verbunden sind. Benutzer können auf Dokumente klicken, um sie in einem Vorschaufenster anzuzeigen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeitstempel ausblenden</td> 
      <td>Blendet Zeitstempel für die folgenden Datumsfelder in Startseite und Zusammenfassung aus:
       <ul>
        <li>Geplantes Abschlussdatum</li>
        <li>Verpflichtungsdatum</li>
        <li><p>Gesendetes Datum</p></li>
       </ul><p><b>NOTE</b>: Wenn diese Option aktiviert ist, werden Arbeitselemente, die überfällig werden, in die verspätete Gruppierung in der Hausarbeitsliste verschoben, wobei nur das Datum und nicht die Uhrzeit verwendet wird.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
