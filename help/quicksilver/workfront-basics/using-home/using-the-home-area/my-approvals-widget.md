---
product-area: home
navigation-topic: use-the-home-area
title: Verwalten Ihrer Genehmigungen mit dem Widget „Meine Genehmigungen“
description: Das Widget Meine Genehmigungen zeigt alle ausstehenden, zugewiesenen, delegierten und gesendeten Genehmigungen an einer Stelle an. Hier können Sie Ihre Genehmigungen filtern und organisieren, Entscheidungen treffen und Genehmigungen nach Bedarf delegieren.
author: Courtney
feature: Get Started with Workfront
exl-id: 276a33f5-92de-440c-ae3a-8cd01731434f
TQID: https://experienceleague.adobe.com/wfTP8CMqgTZtTLshO239HNrDAUbyrHNbOhs3ZKlMXGg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 415
ht-degree: 17%

---

# Verwalten Ihrer Genehmigungen mit dem Widget „Meine Genehmigungen“

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

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <p>Mitwirkende oder höher</p>
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Genehmigen von Arbeit über das Widget Meine Genehmigungen

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) Klicken Sie auf **Anpassen**, um das Widget **Meine Genehmigungen** hinzuzufügen.
1. (Bedingt) Klicken Sie auf das **Filter** Dropdown-Menü und wählen Sie **Alle**, um die Ihnen zugewiesenen und delegierten Genehmigungen anzuzeigen.

   >[!NOTE]
   >
   >Genehmigungen, die Aufgabengebieten oder Gruppen zugewiesen wurden, werden nicht auf der Startseite angezeigt. Genehmigungen, die Teams zugewiesen wurden, werden für jedes Teammitglied im Widget Meine Genehmigungen angezeigt.


1. (Bedingt) Klicken Sie auf das **Sortieren** Dropdown-Menü und wählen Sie dann **Neueste zuerst**, um die zuletzt hinzugefügten Genehmigungen anzuzeigen.


1. (Optional) Klicken Sie auf das Vollbildsymbol ![Vollbildsymbol), ](assets/full-screen.png) das Widget Meine Genehmigungen im Vollbildmodus zu öffnen.

1. Wählen Sie das Element aus, für das Sie eine Genehmigungsentscheidung treffen möchten.

   ![Widget „Meine Genehmigungen“](assets/my-approvals-widget.png)

   <!--update screenshot after production release-->

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
