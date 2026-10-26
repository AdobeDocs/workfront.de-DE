---
title: Benutzer löschen
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Wenn ein(e) Benutzende(r) Ihre Organisation verlässt, kann er/sie diesen Benutzenden aus Workfront entfernen. Wir empfehlen jedoch, Benutzende zu deaktivieren, anstatt sie zu löschen.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 9%
---
# Löschen von Benutzenden

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren galt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Da sich Ihr Unternehmen in die Adobe Admin Console integriert hat, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
>
>  Anweisungen zum Löschen von Benutzenden in der Adobe Admin Console finden Sie im Abschnitt „Dauerhaftes Löschen von Benutzenden“ im Artikel [Einzelne Benutzende verwalten](https://helpx.adobe.com/de/enterprise/using/manage-users-individually.html) oder wenden Sie sich an Ihren Adobe Admin Console-Administrator.

Wenn ein(e) Benutzende(r) Ihre Organisation verlässt, können Sie diesen/diese Benutzende aus Adobe Workfront entfernen.

Das Löschen eines Benutzers muss über die Adobe Admin Console durchgeführt werden. Anweisungen finden Sie im Abschnitt „Dauerhaftes Löschen von Benutzern“ im Artikel [Benutzer einzeln verwalten](https://helpx.adobe.com/de/enterprise/using/manage-users-individually.html) oder wenden Sie sich an Ihren Adobe Admin Console-Administrator.

>[!IMPORTANT]
>
>Beim Löschen eines Benutzers aus dem System werden auch mit dem Benutzer verknüpfte Informationen gelöscht, die Sie möglicherweise beibehalten möchten. Es wird empfohlen, Benutzer zu deaktivieren, anstatt sie zu löschen. Weitere Informationen finden Sie unter [Deaktivieren oder Reaktivieren eines Benutzers](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <td><p>Standard</p><p>Abo</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen Administrator der Adobe Admin Console sein.</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Löschen oder Deaktivieren von Benutzern

Wenn Sie einen Benutzer deaktivieren, passiert Folgendes:

* Entfernt die Benutzerlizenzen für Workfront und Workfront Proof, wenn die Workfront Proof-Komponente mit Ihrem Workfront-Konto verknüpft ist. Weitere Informationen zu Workfront Proof finden Sie unter [Workfront Proof: Artikelindex](../../../workfront-proof/workfront-proof.md).
* Dem Benutzer kann keine Arbeit mehr zugewiesen werden.
* Der Benutzer kann nicht mehr zu Aktualisierungen hinzugefügt werden.
* Der Benutzer kann nicht mehr zu Teams oder Gruppen hinzugefügt werden.
* Objekte können nicht mehr für Benutzende freigegeben werden.
* Ihre Zuordnung zu den folgenden Objekten bleibt intakt:

  * Aufgaben, Probleme, Projekte, Portfolios
  * Dashboards

    >[!NOTE]
    >
    >Wenn Sie einen Benutzer deaktivieren und die mit einem Benutzer verknüpften Berichte oder Dashboards nicht mehr anzeigen können, müssen Sie möglicherweise das Feld **Diesen Bericht ausführen mit den Zugriffsrechten von:** aktualisieren.\
    >Weitere Informationen finden Sie unter [Warum kann ich nicht auf einen Bericht zugreifen, der einem deaktivierten Benutzer gehört?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) -Abschnitt des Artikels [Häufig gestellte Fragen zu ](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) .

  * Dokumente
  * Updates
  * Stunden

* Wenn der Benutzer Dokumente ausgecheckt hat, bleiben die Dokumente ausgecheckt, sobald Sie sie deaktivieren. Nur ein Workfront-Administrator kann sie wieder einchecken. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Auschecken von Dokumenten](../../../documents/managing-documents/check-out-documents.md).

Beim Löschen eines Benutzers passiert Folgendes:

* Entfernt die Benutzerlizenzen für Workfront und Workfront Proof, wenn die Workfront Proof-Komponente mit Ihrem Workfront-Konto verknüpft ist. Weitere Informationen zu Workfront Proof finden Sie unter [Workfront Proof: Artikelindex](../../../workfront-proof/workfront-proof.md).
* Dem Benutzer kann keine Arbeit mehr zugewiesen werden.
* Der Benutzer kann nicht mehr zu Aktualisierungen hinzugefügt werden.
* Der Benutzer kann nicht mehr zu Teams oder Gruppen hinzugefügt werden.
* Objekte können nicht mehr für Benutzende freigegeben werden.
* Löscht die Verknüpfung dieses Benutzers mit den folgenden Objekten:

  * Aufgaben, Probleme, Projekte, Portfolio
  * Dashboards

<!--

     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.

-->
* Updates
* Stunden

  >[!NOTE]
  >
  >Diese Objekte verbleiben in Workfront, aber der Eigentümer des Objekts ist jetzt leer.

* Wenn der Benutzer Dokumente unter dem Bereich Dokumente in der globalen Navigationsleiste hochgeladen hat, werden die Dokumente ebenfalls gelöscht.
* Wenn der/die Benutzende Dokumente ausgecheckt hat, deren Inhaber er/sie ist, und die Dokumente im Hauptdokumentenbereich hochgeladen wurden (der Zugriff erfolgt über das Hauptmenü), werden die Dokumente mit dem/der Benutzenden gelöscht. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Auschecken von Dokumenten](../../../documents/managing-documents/check-out-documents.md).

Weitere Informationen zum Deaktivieren von Benutzern finden Sie unter [Deaktivieren oder Reaktivieren von Benutzern](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
