---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Smart-Zuweisungen vornehmen
description: Sie können Smart-Zuweisungen verwenden, um zu ermitteln, wer der beste Benutzer ist, um die Arbeit abzuschließen. Smart-Zuweisungen sind Vorschläge für Benutzer, Rollen oder Teams, die Ihnen Adobe Workfront präsentiert, wenn Sie Arbeitselemente Ressourcen zuweisen, die auf einem Algorithmus basieren, der die am besten geeignete Ressource für den Auftrag bestimmt. Informationen zu Smart-Zuweisungen finden Sie unter Übersicht über Smart-Zuweisungen .
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Smart-Zuweisungen vornehmen

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnelle Versionen für Ihre Organisation aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Übersicht über die Version 2024 im dritten Quartal](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Sie können Smart-Zuweisungen verwenden, um zu ermitteln, wer der beste Benutzer ist, um die Arbeit abzuschließen.

Smart-Zuweisungen sind Vorschläge für Benutzer, Rollen oder Teams, die Ihnen Adobe Workfront präsentiert, wenn Sie Ressourcen Arbeitselemente zuweisen. Workfront basiert seine Vorschläge auf einem Algorithmus, der die am besten geeignete Ressource für den Auftrag bestimmt.

<span class="preview">Es gibt zwei separate Algorithmen in Workfront, die Smart-Zuweisungen berechnen, die für Aufgaben und Probleme unterschiedlich funktionieren. </span>

Weitere Informationen zu den Kriterien für die Bestimmung von Smart-Zuweisungen finden Sie unter [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p>
      Oder
      <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Projekte</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen oder höhere Berechtigungen mit der Möglichkeit, Zuweisungen zu Aufgaben und Problemen vorzunehmen</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Smart-Zuweisungen vornehmen

Smart-Zuweisungen sind an den meisten Stellen verfügbar, an denen Sie Zuweisungen in Workfront vornehmen können.

1. Klicken Sie in den folgenden Bereichen auf die Schaltfläche **Zuweisungen** oder **Zuweisen** -Feld:

   * Aufgabe oder Problemliste oder Bericht
   * Aufgaben- oder Problemkopfzeile
   * Das Bedienfeld &quot;Aufgabe oder Problem-Zusammenfassung&quot;
   * <span class="preview">Ein Feld &quot;Neue Aufgabe&quot;oder &quot;Neues Problem&quot;, wenn Sie eine neue Aufgabe oder ein neues Problem zu einem Projekt hinzufügen</span>
   * Das Feld Zuweisungen für ein Element, das im Startbereich aufgeführt ist
   * Eine Aufgabe oder ein Problem im Arbeitslastausgleich

1. Platzieren Sie den Cursor im Feld Zuweisungen und warten Sie zwei Sekunden.

   <div class="preview">
   Ein oder mehrere der folgenden Abschnitte mit Vorschlägen für die intelligente Zuweisung werden angezeigt:

   * **Vorgeschlagene Zuweisungen**: Wird für Aufgaben angezeigt. <!--remove the note when we go to production with smarter assignments-->

     >[!TIP]
     >
     >   Die Listenüberschrift wird angezeigt **Im Folgenden finden Sie einige Empfehlungen** anstelle von **Vorgeschlagene Zuweisungen** in der Produktionsumgebung.
     >
   * **Benutzer und Teams**: Wird für Aufgaben und Probleme angezeigt.
   * **Vorgangsrollen**: Zeigt Aufgaben und Probleme an.
   * **Auftragsrollen auf Ratenkarten**: Wird für Aufgaben angezeigt. Weitere Informationen finden Sie unter [Ratenkarten verwalten](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   Bei Aufgaben werden die Smart-Zuweisungen in den folgenden Abschnitten angezeigt, je nachdem, in welcher Phase der Algorithmusberechnung die Zuweisungen identifiziert wurden:

   * **Vorgeschlagene Zuweisungen**: Zuweisungen, die in der ersten Phase der Algorithmusberechnung der intelligenten Aufgabenzuweisung identifiziert wurden. <span class="preview">Dieser Abschnitt ist nicht für Probleme verfügbar.</span>
   * <span class="preview">**Benutzer und Teams**, **Vorgangsrollen** oder **Auftragsrollen auf Ratenkarten**: Zuweisungen, die in der zweiten Phase der Algorithmusberechnung der intelligenten Aufgabenzuweisung identifiziert werden. <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Weitere Informationen finden Sie unter [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Wählen Sie den Benutzer in der Empfehlungsliste aus, indem Sie auf seinen Namen klicken.

1. (Optional) Klicken Sie auf **Zuweisen** , um sich das Arbeitselement zuzuweisen.

   >[!TIP]
   >
   >Wenn keine Vorschläge vorhanden sind, wird die Vorschlagsliste nicht geöffnet.

1. (Optional) Wenn Sie keinen der empfohlenen Benutzer aus der Liste der intelligenten Zuweisungen verwenden möchten, geben Sie den Namen der gewünschten Ressource ein und wählen Sie den Namen aus, wenn er in der Liste angezeigt wird.
1. Klicks **Eingabe** , um die Zuweisung vorzunehmen.

   Der ausgewählte Benutzer wird der Aufgabe oder dem Problem zugewiesen.
