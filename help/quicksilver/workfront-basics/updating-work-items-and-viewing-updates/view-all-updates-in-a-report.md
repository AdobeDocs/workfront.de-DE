---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Alle Aktualisierungen in einem Hinweis-Bericht anzeigen
description: Alle Aktualisierungen in einem Hinweis-Bericht anzeigen
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Alle Aktualisierungen in einem Hinweis-Bericht anzeigen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

Im Bereich Updates eines Objekts wird standardmäßig maximal 200 Updates angezeigt. Um alle Aktualisierungen anzuzeigen, die ein Benutzer für ein Objekt eingegeben hat, können Sie einen Hinweis-Bericht erstellen, der alle Aktualisierungen anzeigt.

>[!NOTE]
>
>Sie können einen Bericht erstellen, um mithilfe des Journaleintragsberichts Aktualisierungen zu Objekten in der Vorschau anzuzeigen. Weitere Informationen finden Sie unter [Bericht zum Bereich &quot;Updates&quot;](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Erstellen von Berichten, Dashboards und Kalendern</p> </li> 
     <li> <p>Erstellen von Filtern, Ansichten und Gruppierungen</p> </li> 
    </ul> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt.<br>Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Anzeigen</p> <p>Hinweis: Wenn Sie keine Ansichtsberechtigung oder eine höhere Berechtigung für ein Objekt haben, werden die Informationen für dieses Objekt nicht im Bericht angezeigt.</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen eines Berichts mit Anmerkungen

Das Erstellen eines Berichts für Anmerkungen für Objekte ist unabhängig vom Objekt identisch.

So erstellen Sie beispielsweise einen Notiz -Bericht für alle Notizen in einem Projekt:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) in der rechten oberen Ecke von Adobe Workfront.

1. Klicken **Berichte**.
1. Klicken **Neuer Bericht**, wählen Sie **Hinweis**.

1. (Optional) Klicken Sie auf **Ansichten**, dann **Spalte hinzufügen** , um **Name** des **Projekt** in der Ansicht des Berichts. 

1. (Optional) Klicken Sie auf **Gruppierungen**, dann **Gruppierung hinzufügen** um **Projektname**, wenn Sie über mehrere Projekte gleichzeitig berichten.\
   Dadurch wird sichergestellt, dass die Notizen nach ihren jeweiligen Projekten gruppiert werden, was das Lesen des Berichts erleichtert. 

1. (Optional) Klicken Sie auf **Filter,** then **Filterregel hinzufügen** , um nach nur einem Projekt oder spezifischen Projekten zu filtern.

1. (Bedingt und optional) Legen Sie die **Projektname** as **Gleich** zum Projektnamen des Projekts, für das Sie Updates anzeigen möchten.  

1. Klicken **Speichern und schließen**.\
   Alle Aktualisierungen, die im Projekt von allen Benutzern mit der Berechtigung zum Anzeigen des Projekts eingegeben wurden, werden im Bericht angezeigt.
