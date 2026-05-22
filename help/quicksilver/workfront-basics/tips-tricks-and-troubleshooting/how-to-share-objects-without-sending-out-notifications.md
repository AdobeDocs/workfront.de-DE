---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Freigeben von Objekten ohne Generieren von Benachrichtigungen
description: Erfahren Sie, wie Sie Objekte freigeben und verhindern können, dass Benachrichtigungen über diese Änderung gesendet werden. Dies ist besonders hilfreich, wenn Sie Objekte stapelweise freigeben.
author: Alina
feature: Get Started with Workfront
exl-id: 02106282-addb-4bdd-82d2-9da5a5f6a687
source-git-commit: 14b3bfaf16a4ab8749538b32100ce6363a3a9335
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 11%

---

# Freigeben von Objekten ohne Generieren von Benachrichtigungen

<!--Audited: 12/2024-->

Wenn Sie ein Objekt in Adobe Workfront freigeben, erhalten die Personen, für die Sie das Objekt freigeben, eine E-Mail-Benachrichtigung über die Freigabe.

Es ist wichtig, sich dieser Änderung bewusst zu sein, dass Sie eine E-Mail-Benachrichtigung erhalten, wenn jemand ein Objekt mit Ihnen teilt. Zu viele Benachrichtigungen können jedoch für Benutzende zu verwirrend sein. Wenn Sie eine große Anzahl von Objekten gleichzeitig für Benutzende freigeben möchten, hilft Ihnen das vorübergehende Deaktivieren von Benachrichtigungen, die Verwirrung zu vermeiden.

Personen erhalten E-Mail-Benachrichtigungen, wenn die folgenden Einstellungen gleichzeitig aktiviert sind:

* Eine oder beide der folgenden Ereignisbenachrichtigungen sind auf System- oder Gruppenebene aktiviert:

   * Objektfreigabe an Benutzer
   * Die Objektfreigabe für Team wird auf System- oder Gruppenebene aktiviert.
* Eine oder beide der folgenden E-Mail-Benachrichtigungen sind im Benutzerprofil aktiviert:

   * Jemand hat ein Objekt für mich freigegeben
   * Jemand hat ein Objekt für mein Team freigegeben

Wenn Sie mehrere Objekte für mehrere Personen (in großen Mengen) freigeben müssen, sie jedoch keine E-Mail-Benachrichtigungen über diese Änderung erhalten sollen, gehen Sie wie folgt vor:

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Abo</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Ansichtszugriff oder höher auf die Objekte, die Sie freigeben möchten</p>
   <p>Zugriff auf Benutzer bearbeiten</p>
   <p><b>NOTIZ</b></p>
   <p> Sie müssen System- oder Gruppenadministrator sein, um den Status von Ereignisbenachrichtigungen für das System oder die Gruppe zu überprüfen</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigung zum Anzeigen oder höher für die Objekte, die Sie freigeben möchten</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Freigeben von Objekten ohne Generieren von Benachrichtigungen

1. Stellen Sie sicher **dass die folgenden** (Ereignisbenachrichtigungen) auf System- oder Gruppenebene aktiviert sind:

   * **Objektfreigabe für Benutzer**
   * **Objektfreigabe für Team wird auf System- oder Gruppenebene aktiviert**.

   Weitere Informationen finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Wenn diese Ereignisbenachrichtigungen nicht aktiviert sind, werden die Benachrichtigungen über die Freigabe eines Objekts nicht an die Benutzer gesendet. Wenn eine oder beide aktiviert sind, fahren Sie mit den folgenden Schritten fort.

{{step-1-to-users}}

1. Wählen Sie mehrere Benutzer in der Liste aus und klicken Sie dann auf **Benachrichtigungen** > **Verschiedenes**.
1. Deaktivieren Sie eine oder beide der folgenden Benachrichtigungen (je nachdem, welche auf System- oder Gruppenebene aktiviert sind):

   * **Jemand hat ein Objekt für mich freigegeben**
   * **Jemand hat ein Objekt für mein Team freigegeben**

   Stellen Sie sicher, dass diese Benachrichtigungen für alle ausgewählten Benutzer ausgewählt sind, bevor Sie sie deaktivieren. Auf diese Weise können Sie sie nach der Freigabe der Objekte stapelweise für alle erneut aktivieren.

1. Klicken Sie auf **Änderungen speichern**.
1. Navigieren Sie zu einer Liste von Objekten, die Sie freigeben möchten, wählen Sie die Objekte aus und klicken Sie dann oben in **Liste auf** Symbol „Freigeben“.

   Weitere Informationen zum Massenfreigeben von Objekten finden Sie unter [Freigeben eines Objekts](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

1. Gehen Sie zurück zur Liste der Benutzer, für die Sie die Benachrichtigungen deaktiviert haben, und wählen Sie dieselben Benutzer aus.
1. Wählen Sie dieselben Benutzer in der Liste aus und klicken Sie dann auf **Benachrichtigungen** > **Verschiedenes**.
1. Aktivieren Sie eine oder beide der folgenden Benachrichtigungen (je nachdem, welche auf System- oder Gruppenebene aktiviert sind):

   * **Jemand hat ein Objekt für mich freigegeben**
   * **Jemand hat ein Objekt für mein Team freigegeben**

1. Klicken Sie auf **Änderungen speichern**.

   Die Objekte wurden für die ausgewählten Benutzer freigegeben, und keiner von ihnen erhielt E-Mail-Benachrichtigungen über diese Änderung.
