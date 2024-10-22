---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Smart-Zuweisungen vornehmen
description: Sie können Smart-Zuweisungen verwenden, um zu ermitteln, wer der beste Benutzer ist, um die Arbeit abzuschließen. Smart-Zuweisungen sind Vorschläge für Benutzer, Rollen oder Teams, die Ihnen Adobe Workfront präsentiert, wenn Sie Arbeitselemente Ressourcen zuweisen, die auf einem Algorithmus basieren, der die am besten geeignete Ressource für den Auftrag bestimmt. Informationen zu Smart-Zuweisungen finden Sie unter Übersicht über Smart-Zuweisungen .
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Smart-Zuweisungen vornehmen

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>.

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Überblick über die Version des vierten Quartals 2024](/help/quicksilver/product-announcements/product-releases/24-q4-release-activity/24-q4-release-overview.md).</span>

Sie können Smart-Zuweisungen verwenden, um zu ermitteln, wer der beste Benutzer ist, um die Arbeit abzuschließen.

Smart-Zuweisungen sind Vorschläge für Benutzer, Rollen oder Teams, die Ihnen Adobe Workfront präsentiert, wenn Sie Ressourcen Arbeitselemente zuweisen. Workfront basiert seine Vorschläge auf einem Algorithmus, der die am besten geeignete Ressource für den Auftrag bestimmt.

<span class="preview">Es gibt zwei separate Algorithmen in Workfront, die Smart-Zuweisungen berechnen, die für Aufgaben und Probleme unterschiedlich funktionieren.</span>

Weitere Informationen zu den Kriterien für die Bestimmung von Smart-Zuweisungen finden Sie unter [Übersicht über Smart-Zuweisungen](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td> <p>Contribute oder höhere Berechtigungen mit der Möglichkeit, Aufgaben und Probleme zuzuweisen</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Smart-Zuweisungen vornehmen

Smart-Zuweisungen sind an den meisten Stellen verfügbar, an denen Sie Zuweisungen in Workfront vornehmen können.

1. Gehen Sie in die folgenden Bereiche und klicken Sie auf das Feld **Zuweisungen** oder **Zuweisen zu** :

   * Aufgabe oder Problemliste oder Bericht
   * Aufgaben- oder Problemkopfzeile
   * Das Bedienfeld &quot;Aufgabe oder Problem-Zusammenfassung&quot;
   * <span class="preview">Eine neue Aufgabe </span> oder ein neues Problem, wenn Sie <span class="preview">eine neue Aufgabe hinzufügen</span> oder ein Problem zu einem Projekt hinzufügen
   * Eine Aufgabe oder ein Problem im Arbeitslastausgleich

1. Platzieren Sie den Cursor im Feld Zuweisungen und warten Sie zwei Sekunden.

   Bei Problemen werden die Smart-Zuweisungen in den folgenden Abschnitten angezeigt:

   * **Benutzer und Teams**
   * **Vorgangsrollen**

   ![](assets/smart-assignments-issue-header.png)

   Bei Aufgaben werden die Smart-Zuweisungen in den folgenden Abschnitten angezeigt, je nachdem, in welcher Phase der Algorithmusberechnung die Zuweisungen identifiziert wurden:

   * <span class="preview">**Vorgeschlagene Zuweisungen**: Zeigt Zuweisungen an, die in der ersten Phase des Algorithmus für die intelligente Aufgabenzuweisung identifiziert wurden.</span>
   * **Benutzer und Teams**, **Auftragsrollen** oder <span class="preview">**Auftragsrollen auf Ratenkarten**</span>: Zuweisungen, die in der zweiten Phase der Algorithmusberechnung der Aufgabe &quot;Smart-Zuweisung&quot;identifiziert wurden.

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   Weitere Informationen finden Sie unter [Übersicht über Smart-Zuweisungen](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

1. Wählen Sie die Ressource in der Empfehlungsliste aus, indem Sie auf ihren Namen klicken.

1. (Optional) Klicken Sie auf **Zuweisen** , um sich das Arbeitselement zuzuweisen.

   >[!TIP]
   >
   >Wenn keine Vorschläge vorhanden sind, wird die Vorschlagsliste nicht geöffnet.

1. (Optional) Wenn Sie keinen der empfohlenen Benutzer aus der Liste der intelligenten Zuweisungen verwenden möchten, geben Sie den Namen der gewünschten Ressource ein und wählen Sie den Namen aus, wenn er in der Liste angezeigt wird.
1. Klicken Sie auf **Enter** , um die Zuweisung vorzunehmen.

   Der ausgewählte Benutzer wird der Aufgabe oder dem Problem zugewiesen.
