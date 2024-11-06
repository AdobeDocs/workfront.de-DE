---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Dokumentbericht mit Link zu einem Testversand"
description: "Ansicht: Dokumentbericht mit Link zu einem Testversand"
author: Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '313'
ht-degree: 1%

---

# Anzeigen: Dokumentbericht mit Link zu einem Testversand

<!--Audited: 11/2024-->

In dieser Dokumentansicht können Sie einen Link zu einem Testversand der aktuellen Dokumentversion einfügen.

![](assets/view-document-with-proof-link-350x92.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dokumentbericht mit Link zu einem Testversand anzeigen

So wenden Sie diese Ansicht an:

1. Gehen Sie zu einer Liste von Dokumenten.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.
1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie auf **Wechseln zum Textmodus** und dann auf **Textmodus bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus bearbeiten** finden, und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Proof Link
   shortview=true
   textmode=true
   valueexpression=CONCAT("https://Your domain.my.workfront.com/document/",{currentVersion}.{ID},"/proof/",{currentVersion}.{proofID},"/view")
   valueformat=HTML
   ```

   >[!TIP]
   >
   >Ersetzen Sie &quot;Ihre Domäne&quot;durch Ihre eigentliche Workfront-Domäne. Wenn die Workfront-URL Ihres Unternehmens beispielsweise *Company.my.workfront.com* lautet, lautet Ihre Domäne &quot;Unternehmen&quot;.

1. Klicken Sie auf **Fertig** und dann auf **Ansicht speichern**.
1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
1. (Optional) Um sicherzustellen, dass nur Dokumente mit Testsendungen angezeigt werden, fügen Sie einen Filter hinzu, indem Sie Folgendes durchführen:

   1. Klicken Sie auf das Dropdown-Menü **Filter** und dann auf **Neuer Filter**.
   1. Klicken Sie auf **Filterregel hinzufügen** und beginnen Sie mit der Eingabe von &quot;Testversand-Inhaber&quot;und wählen Sie dann **Kennung des Testversands-Eigentümers** aus, wenn sie in der Liste angezeigt wird.
   1. Wählen Sie für den Filtermodifikator **Ist nicht leer** aus.
   1. Klicken Sie auf **Filter speichern**.
   1. (Optional) Aktualisieren Sie den Filternamen und klicken Sie dann auf **Filter speichern**.

1. Klicken Sie auf den Link in der Spalte Testversand-Link , um auf den Testversand der letzten Version des Dokuments zuzugreifen.
