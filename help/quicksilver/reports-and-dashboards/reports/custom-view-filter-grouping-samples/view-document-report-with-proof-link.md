---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Dokumentbericht mit Link zu einem Testversand"
description: "Ansicht: Dokumentbericht mit Link zu einem Testversand"
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: a38c5e86-9789-41ca-a832-2ee5eb0a570b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Anzeigen: Dokumentbericht mit Link zu einem Testversand

In dieser Dokumentansicht können Sie einen Link zu einem Testversand der aktuellen Dokumentversion einfügen.

![](assets/view-document-with-proof-link-350x92.png)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Dokumentbericht mit Link zu einem Testversand anzeigen

So wenden Sie diese Ansicht an:

1. Gehen Sie zu einer Liste von Dokumenten.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Klicken Sie auf **Spalte hinzufügen**.
1. Klicken Sie auf **Wechseln zum Textmodus**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:

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

1. Klicken Sie auf **Speichern** und dann auf **Ansicht speichern**.
1. Geben Sie einen Namen für die Ansicht ein und klicken Sie dann auf **Ansicht speichern**.
1. (Optional) Um sicherzustellen, dass nur Dokumente mit Testsendungen angezeigt werden, fügen Sie einen Filter hinzu, indem Sie Folgendes durchführen:

   1. Klicken Sie auf das Dropdown-Menü **Filter** und dann auf **Neuer Filter**.
   1. Klicken Sie auf **Filterregel hinzufügen** und beginnen Sie mit der Eingabe des Testversandinhabers. Wählen Sie dann **Kennung des Testversands des Eigentümers** aus, wenn er in der Liste angezeigt wird.
   1. Wählen Sie für den Filtermodifikator **Ist nicht leer** aus.
   1. Klicken Sie auf **Filter speichern**, geben Sie den Namen des Filters ein und klicken Sie dann auf **Filter speichern**.

1. Klicken Sie auf den Link in der Spalte Testversand-Link , um auf den Testversand der letzten Version des Dokuments zuzugreifen.
