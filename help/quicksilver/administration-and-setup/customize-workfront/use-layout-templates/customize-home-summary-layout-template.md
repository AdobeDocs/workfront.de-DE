---
title: Anpassen des Zusammenfassungsbereichs mithilfe einer Layoutvorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer sehen, wenn sie auf eine Aufgabe oder ein Problem in der Zusammenfassung klicken. Jede Konfiguration, die Sie mithilfe der folgenden Schritte vornehmen, wirkt sich auf das Bedienfeld "Zusammenfassung"aus. Diese Anpassungen gelten nicht für das Bedienfeld "Dokumentzusammenfassung".
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 8f64c009-09ad-45f6-8b59-5c1b4024532e
source-git-commit: 8880891c0f5fd8fecad6c2f58136d36a943105ae
workflow-type: tm+mt
source-wordcount: '1027'
ht-degree: 2%

---

# Anpassen des Zusammenfassungsbereichs mithilfe einer Layoutvorlage

<!--Audited: 11/2024-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.


Sie können eine Layout-Vorlage verwenden, um zu konfigurieren, was Benutzer beim Klicken auf eine Aufgabe oder ein Problem im Bedienfeld &quot;Zusammenfassung&quot;sehen. Jede Konfiguration, die Sie mithilfe der folgenden Schritte vornehmen, wirkt sich auf das Bedienfeld &quot;Zusammenfassung&quot;aus. Diese Anpassungen gelten nicht für das Bedienfeld &quot;Dokumentzusammenfassung&quot;.

Sie können Folgendes konfigurieren:

* Welche Felder werden für eine Aufgabe oder ein Problem im Bereich Details angezeigt und in welcher Reihenfolge
* Ob Aktualisierungen, aufgezeichnete Zeit, angehängte Dokumente und Zeitstempel für eine ausgewählte Aufgabe oder ein ausgewähltes Problem angezeigt werden

Sie können auch die Felder anpassen, die Benutzern im Bereich Startseite angezeigt werden, wenn Benutzer auf eine ihnen zugewiesene Projektgenehmigung, Dokumentgenehmigung oder Dokumentversionsgenehmigung klicken.

Weitere Informationen zum Bedienfeld &quot;Zusammenfassung&quot;finden Sie unter [Übersicht&quot;](../../../workfront-basics/the-new-workfront-experience/summary-overview.md).

Informationen zum Erstellen von Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layoutvorlagen für Gruppen finden Sie unter [Erstellen und Ändern von Layoutvorlagen für Gruppen](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layoutvorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layoutvorlage zu Benutzern finden Sie unter [Zuweisen von Benutzern zu einer Layoutvorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td><p>Neu: Standard</p>
  <p> Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene des Systemadministrators.
Um sie für eine Gruppe durchzuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anpassen des Zusammenfassungsbereichs mithilfe einer Layoutvorlage

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.

1. Klicken Sie auf den Abwärtspfeil ![](assets/dropdown-arrow.png) unter **Anpassen, was Benutzer sehen**, und klicken Sie dann auf **Zusammenfassungsbereich**.

1. Klicken Sie in der Liste, die darunter angezeigt wird, auf den Objekttyp, für den Sie das Bedienfeld &quot;Zusammenfassung&quot;anpassen möchten.

   In der folgenden Tabelle wird erläutert, was Sie für jedes Objekt anpassen können

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Aufgaben</td> 
      <td> <p>In einer Aufgabenliste wirkt sich diese Einstellung auf das Bedienfeld Zusammenfassung aus, das rechts auf der Seite angezeigt wird, wenn ein Benutzer eine Aufgabe auswählt und dann auf das Symbol "Zusammenfassung öffnen"<img src="assets/summary-panel-icon.png"> klickt.</p>

   <p> <img src="assets/summary-details.jpg"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Probleme</td> 
      <td><p>In einer Liste von Problemen wirkt sich diese Einstellung auf das Bedienfeld Zusammenfassung aus, das rechts auf der Seite angezeigt wird, wenn ein Benutzer ein Problem auswählt und dann auf das Symbol "Zusammenfassung öffnen"<img src="assets/summary-panel-icon.png"> klickt.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Projekte</td> 
      <td><ul><li><p>Wenn auf der Startseite ein Benutzer auf eine ihm zugewiesene Projektgenehmigung klickt, wirkt sich Ihre Konfiguration für diese Einstellung auf den Bereich rechts neben der Genehmigung aus.</p>
      <p><b>WICHTIG:</b> </p><p>Diese Funktion wird nicht mehr unterstützt. Alle Änderungen, die Sie an diesem Bereich vornehmen, beziehen sich auf eine Funktion, die von Workfront entfernt wurde. Diese Option wird mit einem späteren Wartungs-Update aus Workfront entfernt.</p></li>
      <li><span class="preview"><p>Dieser Bereich wurde aus der Vorschau-Umgebung entfernt.</p></li></span></ul> 
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumente</td> 
      <td>
     <ul><li><p>Wenn auf der Startseite ein Benutzer auf eine ihm zugewiesene Dokumentgenehmigung klickt, wirkt sich Ihre Konfiguration für diese Einstellung auf den Bereich rechts neben der Genehmigung aus.</p>
      <p><b>WICHTIG:</b> </p><p> Diese Funktion wird nicht mehr unterstützt. Alle Änderungen, die Sie an diesem Bereich vornehmen, beziehen sich auf eine Funktion, die von Workfront entfernt wurde. Diese Option wird mit einem späteren Wartungs-Update aus Workfront entfernt.</p></li>
      <li><span class="preview"><p>Dieser Bereich wurde aus der Vorschau-Umgebung entfernt.</p></li></span></ul>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokumentversionen</td> 
      <td><ul><li><p>Wenn auf der Startseite ein Benutzer auf eine Genehmigung klickt, die ihm für eine bestimmte Version eines Dokuments zugewiesen wurde, wirkt sich Ihre Konfiguration für diese Einstellung auf den Bereich rechts neben der Genehmigung aus.</p>
      <p><p><b>WICHTIG:</b></p> Diese Funktion wird nicht mehr unterstützt. Alle Änderungen, die Sie an diesem Bereich vornehmen, beziehen sich auf eine Funktion, die von Workfront entfernt wurde. Diese Option wird mit einem späteren Wartungs-Update aus Workfront entfernt.</p></li>
      <li><span class="preview"><p>Dieser Bereich wurde aus der Vorschau-Umgebung entfernt.</p></li></span></ul>
      </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Wenn die Zuweisung einer Aufgabe aufgehoben wird, werden dem Benutzer, der der Layoutvorlage zugewiesen ist, die Feldanpassungen in der Zusammenfassung nicht angezeigt.

1. (Bedingt) Wenn Sie im vorherigen Schritt auf Aufgaben oder Probleme geklickt haben, wählen Sie die Kategorie der Aufgabe oder des Problems aus, die Sie anpassen möchten.

   <span class="preview">![](assets/choose-cat-cstmz-nwe-adobe-branding.png)</span>

1. (Bedingt) Wenn das Dropdown-Menü **Schaltfläche &quot;Primäre Aktion festlegen&quot;** angezeigt wird (wenn Sie in der Liste auf der linken Seite die Option **Aufgaben** oder **Probleme** auswählen), klicken Sie auf die primäre Aktion (**Fertig** oder **Status**), die Benutzern im Zusammenfassungsbereich zur Verfügung stehen soll, wenn sie eine Aufgabe oder ein Problem anzeigen.

   <span class="preview">![](assets/set-primary-action-button-dropdown-pdf-adobe-branding.png)</span>

1. Fügen Sie ![](assets/add-item-plus-in-circle-blue.png) hinzu oder blenden Sie ![](assets/close-or-hide---x.png) -Felder für den ausgewählten Objekttyp aus.

   <span class="preview">![](assets/lt-home-add-hide-fields-adobe-branding.png)</span>

1. Wiederholen Sie die Schritte 3 bis 6, um den Bereich &quot;Zusammenfassung&quot;für alle anderen Objekttypen anzupassen.
1. Klicken Sie unten links auf **Globale Einstellungen** und aktivieren oder deaktivieren Sie dann eine der folgenden Optionen, die sich auf Adobe Workfront-Objekte in der Zusammenfassung beziehen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Updates für Arbeiten anzeigen</td> 
      <td>Zeigt alle Aktualisierungen an, die an einer ausgewählten Aufgabe oder einem ausgewählten Problem im Bereich "Zusammenfassung"vorgenommen wurden. Dies umfasst sowohl Systemaktualisierungen als auch Aktualisierungen, die von einem Benutzer vorgenommen werden. Benutzer können weiterhin Systemaktualisierungen herausfiltern, wie unter <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable" class="MCXref xref">Systemaktualisierungen aktivieren oder deaktivieren</a> in <a href="../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Arbeit aktualisieren</a> beschrieben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeit für Arbeit erfassen</td> 
      <td>Zeigt die Option Arbeitszeit bei Arbeit protokollieren an, wenn eine Aufgabe oder ein Problem ausgewählt ist. Dadurch können Benutzer die Arbeitszeit für Arbeitselemente direkt über die Bereiche Startseite und Zusammenfassung protokollieren.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anzeigen von Dokumenten, die mit Arbeiten verknüpft sind</td> 
      <td>Zeigt den Bereich Dokumente im Bereich Zusammenfassung an, wenn eine Aufgabe oder ein Problem ausgewählt ist, und listet alle Dokumente auf, die mit der Aufgabe oder dem Problem verbunden sind. Benutzer können auf Dokumente klicken, um sie in einem Vorschaufenster anzuzeigen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zeitstempel ausblenden</td> 
      <td>Blendet Zeitstempel für die folgenden Datumsfelder im Bereich "Zusammenfassung"aus:
       <ul>
        <li>Geplantes Abschlussdatum</li>
        <li>Verpflichtungsdatum</li>
        <li>Gesendetes Datum</li>
       </ul></td> 
     </tr> 
    </tbody> 
   </table>

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit dem Anpassen fertig sind, klicken Sie auf **Speichern**.

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
