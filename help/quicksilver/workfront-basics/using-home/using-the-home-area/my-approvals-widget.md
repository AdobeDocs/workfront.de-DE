---
product-area: home
navigation-topic: use-the-home-area
title: Verwalten Sie Ihre Genehmigungen mit dem Widget Meine Genehmigungen .
description: Das Widget Meine Genehmigungen zeigt alle ausstehenden, zugewiesenen, delegierten und gesendeten Genehmigungen an einer Stelle an. Hier können Sie Ihre Genehmigungen filtern und organisieren, Entscheidungen treffen und Genehmigungen nach Bedarf delegieren.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 5%

---

# Verwalten Sie Ihre Genehmigungen mit dem Widget Meine Genehmigungen .

Das Widget Meine Genehmigungen zeigt alle ausstehenden, zugewiesenen, delegierten und gesendeten Genehmigungen an einer Stelle an. Hier können Sie Ihre Genehmigungen filtern und organisieren, Entscheidungen treffen und Genehmigungen nach Bedarf delegieren.

Das Widget Meine Genehmigungen unterstützt Genehmigungen von den folgenden Workfront-Objekten:

* Aufgaben
* Probleme
* Projekte
* Dokumente
* Korrekturabzüge
* Planen von Datensatzanfragen
* Arbeitszeittabellen

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
   <td> 
   <p>Mitwirkender oder höher</p>
   <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Objekte, die mit Genehmigungen verknüpft sind, anzeigen oder höher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die mit Genehmigungen verbunden sind</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Genehmigen von Arbeit über das Widget Meine Genehmigungen

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) Klicken Sie auf **Anpassen**, um das Widget **Meine Genehmigungen** hinzuzufügen.
1. (Bedingt) Klicken Sie auf das **Filter** Dropdown-Menü und wählen Sie **Alle**, um die Ihnen zugewiesenen und delegierten Genehmigungen anzuzeigen.

   >[!NOTE]
   >
   >Genehmigungen, die Aufgabengebieten oder Gruppen zugewiesen wurden, werden nicht auf der Startseite angezeigt. Genehmigungen, die Teams zugewiesen wurden, werden für jedes Teammitglied im Widget Meine Genehmigungen angezeigt.


1. Wählen Sie das Element aus, für das Sie eine Genehmigungsentscheidung treffen möchten.

   ![Widget „Meine Genehmigungen“](assets/my-approvals-widget.png)

1. Klicken Sie im rechten Bedienfeld auf eine der verfügbaren Optionen, wenn Sie eine Genehmigungsentscheidung treffen. Die folgenden Optionen werden je nach Art des zu genehmigenden Elements in der rechten oberen Ecke der Seite angezeigt:

   <table>
   <tr>
      <td>
      <p><strong>Zugriff</strong></p>
      </td>
      <td>
      <p><strong>Arbeitselemente</strong></p>
      </td>
      <td>
      <p><strong>Dokumente</strong></p>
      </td>
      <td>
      <p><strong>Korrekturabzüge</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>erteilen</li>
      <li>Ignorieren</li>
      </ul>
      Sie können die Zugriffsebene bei Bedarf im Dropdown-Menü <b>Zugriff ändern</b> anpassen.
      </td>
      <td>
         <ul>
         <li>Genehmigen</li>
         <li>Ablehnen</li>
         </ul>
      Sie können eine Entscheidung kommentieren, indem Sie auf das Dropdown-Menü in der Entscheidungsschaltfläche klicken.
      </td>
      <td>
   Als genehmigende Person zugewiesen
         <ul>
         <li>Genehmigen</li>
         <li>Mit Änderungen genehmigt</li>
         <li>Muss bearbeitet werden</li>
         </ul>
   Als Prüfer zugewiesen
         <ul>
         <li>Überprüfung abschließen</li>
         </ul>
      Die Optionen in dieser Spalte gelten nur für einheitliche Genehmigungen. Legacy-Dokumentgenehmigungen erscheinen genauso wie Arbeitselementgenehmigungen. 
      </td>
      <td>
         <ul>
         <li>Zum Korrekturabzug gehen</li>
         </ul>
         Sie treffen Ihre Entscheidung in der Korrekturabzugsansicht. Informationen zur Überprüfung eines Korrekturabzugs finden Sie unter <a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Testsendungen in Adobe Workfront </a>.
      </td>
   </tr>
   </table>

Nachdem Sie eine Entscheidung getroffen haben, wird die Genehmigung aus dem Widget Meine Genehmigung entfernt.