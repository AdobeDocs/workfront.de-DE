---
title: Benutzeroberflächen-Terminologie mithilfe einer Layoutvorlage anpassen
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Als Adobe Workfront-Administrator können Sie eine Layoutvorlage verwenden, um die Beschriftungen einiger Objekte in Workfront so zu ändern, dass sie mit den in Ihrem Unternehmen verwendeten Begriffen übereinstimmen.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 2%

---

# Benutzeroberflächenterminologie mithilfe einer Layoutvorlage anpassen

Als Adobe Workfront-Administrator können Sie eine Layoutvorlage verwenden, um die Beschriftungen einiger Objekte in Workfront so zu ändern, dass sie mit den in Ihrem Unternehmen verwendeten Begriffen übereinstimmen.

Nachdem Sie eine Layoutvorlage gespeichert haben, in der Sie die Terminologie geändert haben, melden Sie sich dann von Workfront ab und wieder an. Daraufhin werden die geänderten Bezeichnungen dort angezeigt, wo die Standardbezeichnungen in den meisten Bereichen von Workfront angezeigt werden:

* Hauptmenü
* Alle vom Hauptmenü aus zugänglichen Bereiche
* Alle Registerkarten
* Alle Menüs
* Report Builder- und Berichterstellungselemente (Ansichten, Filter und Gruppierungen)
* Schaltflächen speichern
* Exportierte Dateien
* E-Mails
* Mobile Apps

>[!NOTE]
>
>* Im Bereich Outlook-Add-in werden die angepassten Beschriftungen nicht angezeigt.
>* Bei der Anpassung von Bezeichnungen treten möglicherweise Grammatik- und andere Probleme auf. Wenn Sie beispielsweise &quot;Problem&quot;in &quot;Anfrage&quot;ändern, kann es in der Benutzeroberfläche Orte geben, an denen die Wortgruppe &quot;Anfrage&quot;angezeigt wird. Weitere Informationen finden Sie unter [Implikationen beim Anpassen von Objektnamen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) im Artikel [Grundlegendes zu Objekten in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

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

## Terminologie der Benutzeroberfläche anpassen

1. Beginnen Sie mit der Arbeit an einer Layoutvorlage, wie in [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) beschrieben.
1. Klicken Sie oben rechts auf der Seite auf **Terminologie festlegen** .
1. Führen Sie einen der folgenden Schritte aus:

   * Um einen von Workfront bereitgestellten alternativen Begriff zu verwenden, klicken Sie neben dem Titel auf den Abwärtspfeil ![](assets/dropdown-arrow.png) und dann auf die alternative Bezeichnung, die Sie in der Dropdownliste verwenden möchten.

     >[!NOTE]
     >
     >Alternative Beschriftungen, die in den Dropdownlisten bereitgestellt werden, werden in Versionen von Workfront unterstützt, die für nicht englische Sprachen lokalisiert sind.

   * Um eine eigene benutzerdefinierte Alternative für die Beschriftung anzugeben, die für ein Objekt angezeigt wird, klicken Sie auf **Benutzerdefinierten Namen festlegen** rechts neben der Beschriftung und geben Sie dann die Formulare **Singular** und **Plural** des benutzerdefinierten Begriffs ein. Sie können auf **Zurücksetzen** klicken, wenn Sie Ihre Meinung ändern.

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
        <td><p>Weitere Informationen zu diesen Objekten finden Sie unter <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Objekte in Adobe Workfront verstehen</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Workfront Goals-Objekte</p></td>
        <td>
         <ul>
          <p>Ziel</p>
          <p>Ergebnis</p>
          <p>Aktivität</p>
         </ul></td>
        <td><p>Für diese Objekte ist eine zusätzliche Lizenz erforderlich. Weitere Informationen finden Sie unter <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Übersicht über Adobe Workfront-Ziele</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Workfront Scario Planer-Objekte</p></td>
        <td>
         <ul>
          <p>Initiative</p>
          <p>Szenario</p>
          <p>Plan </p>
         </ul></td>
        <td><p>Für diese Objekte ist eine zusätzliche Lizenz erforderlich. Weitere Informationen finden Sie unter <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Erste Schritte mit dem Szenario-Planer</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Wenn Sie fertig sind, klicken Sie auf **Fertig**.

   >[!TIP]
   >
   >Nachdem Sie auf Fertig geklickt haben (und auch nach dem Speichern Ihrer Layoutvorlage), können Sie jederzeit zu den Einstellungen für &quot;Terminologie festlegen&quot;zurückkehren und neben allen benutzerdefinierten Begriffen auf &quot;Zurücksetzen&quot;klicken, um sie wieder in den Standardzustand zu versetzen.

1. Fahren Sie mit der Anpassung der Layoutvorlage fort.

   Oder

   Wenn Sie mit dem Anpassen fertig sind, klicken Sie auf **Speichern**.

1. So zeigen Sie Ihre Terminologieänderungen an:

   1. Melden Sie sich bei Workfront ab und wieder an.
   1. Schließen Sie alle Browser-Registerkarten, die Sie für Ihre Workfront-Umgebung geöffnet haben.

   >[!IMPORTANT]
   >
   >Dies ist auch für alle Benutzer erforderlich, die die Layoutvorlage vor der Terminologieänderung verwendet haben.

Weitere Informationen zu Layoutvorlagen finden Sie unter [Erstellen und Verwalten von Layoutvorlagen](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
