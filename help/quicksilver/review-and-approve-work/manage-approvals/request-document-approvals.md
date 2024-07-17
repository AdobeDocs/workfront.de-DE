---
product-area: documents
navigation-topic: approvals
title: Dokumentgenehmigungen anfordern
description: Sie können die Genehmigung von Managern oder anderen Benutzern für ein Dokument in Adobe Workfront anfordern. Sie können auch Dokumentgenehmigungen von Personen ohne Workfront-Konten anfordern, wenn Ihr Workfront-Administrator diese Funktion aktiviert hat, wie unter Systemsicherheitseinstellungen konfigurieren beschrieben.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 1%

---

# Dokumentgenehmigungen anfordern

Sie können die Genehmigung von Managern oder anderen Benutzern für ein Dokument in Adobe Workfront anfordern. Sie können auch Dokumentgenehmigungen von Personen ohne Workfront-Konten anfordern, wenn Ihr Workfront-Administrator diese Funktion aktiviert hat, wie in [Systemsicherheitseinstellungen konfigurieren](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) beschrieben.

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
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards und Kalender, Dokumente anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf das Objekt verwalten, das mit dem Anforderungszugriff oder der Genehmigung verknüpft ist </p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Dokumentgenehmigung anfordern

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente** aus.
1. Suchen Sie das gewünschte Dokument.

1. Scrollen Sie in der Zusammenfassung nach unten zum Abschnitt **Genehmigungen** und beginnen Sie mit der Eingabe in das Textfeld **Genehmiger hinzufügen** . Sie können Workfront-Benutzer nach Namen oder externe Benutzer per E-Mail hinzufügen.

1. Wenn Ihr Adobe Workfront-Administrator die Möglichkeit zur Zusammenarbeit mit Personen aktiviert hat, die Workfront nicht verwenden, wie unter [Systemsicherheitseinstellungen konfigurieren](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) beschrieben, können Sie ihre E-Mail-Adressen eingeben, um sie einzuschließen.

   Sie können die Genehmigung nicht von Teams oder Gruppen anfordern.

1. Wiederholen Sie den vorherigen Schritt, um weitere Genehmiger hinzuzufügen.

## Genehmigung für eine neue Version erneut einreichen

Entscheidungen zur Dokumentgenehmigung werden beim Hochladen einer neuen Version nicht automatisch zurückgesetzt. Wenn Ihr Dokument beispielsweise mit Änderungen genehmigt wurde, zeigt die Entscheidung &quot;Änderungen&quot;als Entscheidung an, selbst wenn Sie eine neue Version mit den angegebenen Änderungen hochladen. Sie können die Entscheidung über eine neue Version löschen, wenn Sie die Genehmigung manuell erneut einreichen.

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente** aus.
1. Suchen Sie das gewünschte Dokument.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung, klicken Sie auf das Symbol Mehr und dann auf Neu senden .

   ![](assets/nwe-resubmit-approval-350x149.png)

## Anforderung einer Dokumentgenehmigung löschen

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente** aus.
1. Suchen Sie das gewünschte Dokument.

1. Scrollen Sie in der Zusammenfassung nach unten zum Abschnitt **Genehmigungen** , klicken Sie dann auf das Menü **Mehr** , das dem Namen des Genehmigers entspricht, und wählen Sie **Löschen** aus.

   Die Validierungsanfrage wird entfernt und der Validierer erhält eine Benachrichtigung, dass seine Validierung nicht mehr erforderlich ist. Auch der genehmigungsbezogene Freigabe-Zugriff wurde entfernt.

## Senden einer Erinnerung an einen Genehmiger

Sie können eine Nachricht senden, um einen Genehmiger daran zu erinnern, dass Sie auf sein Feedback warten.

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente** aus.
1. Suchen Sie das gewünschte Dokument.

1. Scrollen Sie in der Zusammenfassung nach unten zum Abschnitt **Genehmigungen** , klicken Sie dann auf das Menü **Mehr** , das dem Namen des Genehmigers entspricht, und wählen Sie **Erinnerung** aus.

   Der Validierer erhält eine Benachrichtigung, in der er darüber informiert wird, dass die Validierung noch aussteht. Sie können auch eine E-Mail-Erinnerung erhalten, wenn diese aktiviert ist.
