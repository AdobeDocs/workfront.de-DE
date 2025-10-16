---
title: Anpassen der Terminologie der Benutzeroberfläche mithilfe einer Layout-Vorlage
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator können Sie eine Layout-Vorlage verwenden, um die Beschriftungen einiger Objekte, die in Workfront angezeigt werden, an die in Ihrem Unternehmen verwendeten Begriffe anzupassen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 3%

---

# Anpassen der Terminologie der Benutzeroberfläche mithilfe einer Layout-Vorlage

Als Adobe Workfront-Administrator können Sie eine Layout-Vorlage verwenden, um die Beschriftungen einiger Objekte, die in Workfront angezeigt werden, an die in Ihrem Unternehmen verwendeten Begriffe anzupassen.

Nachdem Sie eine Layout-Vorlage gespeichert haben, in der Sie die Terminologie geändert haben, sich dann von Workfront abmelden und wieder anmelden, werden die von Ihnen geänderten Beschriftungen dort angezeigt, wo die Standardbeschriftungen in den meisten Bereichen von Workfront erscheinen würden:

* Hauptmenü
* Alle vom Hauptmenü aus zugänglichen Bereiche
* Alle Registerkarten
* Alle Menüs
* Report Builder und Reporting-Elemente (Ansichten, Filter und Gruppierungen)
* Schaltflächen speichern
* Exportierte Dateien
* E-Mails
* Mobile Apps

>[!NOTE]
>
>* Im Outlook-Add-In-Bereich werden die benutzerdefinierten Beschriftungen nicht angezeigt.
>* Beim Anpassen von Kennzeichnungen können Grammatikprobleme und andere Probleme auftreten. Wenn Sie z. B. „Problem“ in „Anfrage“ ändern, kann es an bestimmten Stellen der Benutzeroberfläche den Ausdruck „Eine Anfrage“ geben. Weitere Informationen finden Sie unter [Auswirkungen der Anpassung von Objektnamen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) im Artikel &quot;[ von Objekten in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

Weitere Informationen zu Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Weitere Informationen zu Layout-Vorlagen für Gruppen finden [ unter „Erstellen und Ändern der Layout-Vorlagen einer Gruppe](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Nachdem Sie eine Layout-Vorlage konfiguriert haben, müssen Sie sie Benutzern zuweisen, damit die von Ihnen vorgenommenen Änderungen für andere sichtbar sind. Informationen zum Zuweisen einer Layout-Vorlage an Benutzer finden Sie unter [Zuweisen von Benutzern zu einer Layout-Vorlage](../use-layout-templates/assign-users-to-layout-template.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Um diese Schritte auf Systemebene durchzuführen, benötigen Sie die Zugriffsebene „Systemadministrator“.</p>
        <p>Um sie für eine Gruppe auszuführen, müssen Sie ein Manager dieser Gruppe sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzeroberflächenterminologie anpassen

1. Beginnen Sie mit der Arbeit an einer Layout-Vorlage, wie unter [Erstellen und Verwalten von Layout-Vorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken **oben rechts** der Seite auf „Terminologie festlegen“.
1. Führen Sie einen der folgenden Schritte aus:

   * Um einen von Workfront bereitgestellten Alternativbegriff zu verwenden, klicken Sie auf den Abwärtspfeil ![Abwärtspfeil](assets/dropdown-arrow.png) neben der Bezeichnung und dann auf die gewünschte Alternativbezeichnung in der Dropdown-Liste.

     >[!NOTE]
     >
     >Alternative Bezeichnungen in den Dropdown-Listen werden in Versionen von Workfront unterstützt, die für nicht englische Sprachen lokalisiert sind.

   * Um Ihre eigene benutzerdefinierte Alternative für die für ein Objekt angezeigte Beschriftung bereitzustellen, klicken Sie auf **Benutzerdefinierten Namen festlegen** rechts neben der Beschriftung und geben Sie dann die **Singular** und **Plural**-Formulare des benutzerdefinierten Begriffs ein. Sie können auf **Zurücksetzen** klicken, wenn Sie es sich anders überlegen.

     Sie können die folgenden Objektnamen anpassen:

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Workfront-Objekte</p></td>
        <td>
          <p>Portfolio</p>
          <p>Programm</p>
          <p>Projekt</p>
          <p>Aufgabe</p>
          <p>Problem</p>
          <p>Ziel</p>
          <p>Ergebnis</p>
          <p>Aktivität</p>
         </ul></td>
        <td><p>Weitere Informationen zu diesen Objekten finden Sie unter <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objekte in Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront-Zielobjekte</p></td>
        <td>
         <ul>
          <p>Ziel</p>
          <p>Ergebnis</p>
          <p>Aktivität</p>
         </ul></td>
        <td><p>Diese Objekte erfordern eine zusätzliche Lizenz. Weitere Informationen finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Adobe Workfront-Ziele - Übersicht</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront Scenario Planner-Objekte</p></td>
        <td>
         <ul>
          <p>Initiative</p>
          <p>Szenario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Diese Objekte erfordern eine zusätzliche Lizenz. Weitere Informationen finden Sie <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Erste Schritte mit dem Szenario-Planer</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Klicken Sie abschließend auf **Fertig**.

   >[!TIP]
   >
   >Nachdem Sie auf Fertig geklickt haben (und auch nach dem Speichern der Layout-Vorlage), können Sie jederzeit zu den Einstellungen für Terminologie festlegen zurückkehren und neben den benutzerdefinierten Begriffen auf Zurücksetzen klicken, um sie wieder in den Standardzustand zu versetzen.

1. Passen Sie die Layout-Vorlage weiter an.

   Oder

   Wenn Sie mit der Anpassung fertig sind, klicken Sie auf **Speichern**.

1. So zeigen Sie Ihre Terminologieänderungen an:

   1. Melden Sie sich ab und wieder bei Workfront an.
   1. Schließen Sie alle Browser-Registerkarten, die für Ihre Workfront-Umgebung geöffnet sind.

   >[!IMPORTANT]
   >
   >Dies ist auch für alle Benutzer der Layout-Vorlage erforderlich, bevor Sie die terminologischen Änderungen vorgenommen haben.

Weitere Informationen zu Layout-Vorlagen finden Sie unter [Erstellen und Verwalten von Layout-](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
