---
product-area: documents
navigation-topic: approvals
title: Dokumentgenehmigungen anfordern
description: Sie können eine Genehmigung von Managern oder anderen Benutzern für ein Dokument in Adobe Workfront anfordern. Sie können auch Dokumentgenehmigungen von Personen ohne Workfront-Konten anfordern, wenn Ihr Workfront-Administrator diese Funktion aktiviert hat, wie in Konfigurieren von Systemsicherheitseinstellungen beschrieben.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 2503b6e628e4860a5652c620d8e4d0eea2414443
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 1%

---

# Dokumentgenehmigungen anfordern

Sie können eine Genehmigung von Managern oder anderen Benutzern für ein Dokument in Adobe Workfront anfordern. Sie können auch Dokumentgenehmigungen von Personen ohne Workfront-Konten anfordern, wenn Ihr Workfront-Administrator diese Funktion aktiviert hat, wie in [Konfigurieren von Systemsicherheitseinstellungen](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) beschrieben.

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
   <p>Beitragen oder höher</p>
   <p>Überprüfen oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Projekte, Aufgaben, Probleme, Vorlagen, Portfolios, Programme, Berichte, Dashboards, Kalender und Dokumente</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten des Zugriffs auf das Objekt, das mit der Zugriffsanforderung oder Genehmigung verknüpft ist </p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Dokumentengenehmigung anfordern

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung und beginnen Sie mit der Eingabe in das Textfeld **Genehmigende Person hinzufügen**. Sie können Workfront-Benutzer nach Namen oder externe Benutzer nach E-Mail hinzufügen.

1. Wenn Ihr Adobe Workfront-Administrator die Funktion zur Zusammenarbeit mit Personen aktiviert hat, die Workfront nicht verwenden, wie in [Konfigurieren von Systemsicherheitseinstellungen](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md) beschrieben, können Sie deren E-Mail-Adressen eingeben, um sie einzuschließen.

   Sie können keine Genehmigung von Teams oder Gruppen anfordern.

1. Wiederholen Sie den vorherigen Schritt, um weitere genehmigende Personen hinzuzufügen.

## Erneutes Senden einer Genehmigung für eine neue Version

Entscheidungen zu Dokumentgenehmigungen werden beim Hochladen einer neuen Version nicht automatisch zurückgesetzt. Wenn Ihr Dokument beispielsweise mit Änderungen genehmigt wurde, zeigt die Entscheidung „Änderungen“ als Entscheidung an, auch wenn Sie eine neue Version mit den angegebenen Änderungen hochladen. Sie können die Entscheidung für eine neue Version löschen, wenn Sie die Genehmigung manuell erneut übermitteln.

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung, klicken Sie auf das Symbol Mehr und dann auf Erneut übermitteln .

   ![Genehmigung erneut übermitteln](assets/nwe-resubmit-approval-350x149.png)

## Löschen einer Dokumentgenehmigungsanfrage

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung, klicken Sie dann auf das Menü **Mehr** , das den Namen der genehmigenden Person enthält, und wählen Sie **Löschen**.

   Die Genehmigungsanforderung wird entfernt und die genehmigende Person erhält eine Benachrichtigung, dass ihre Genehmigung nicht mehr erforderlich ist. Ihr genehmigungsbezogener Freigabezugang wird ebenfalls entfernt.

## Erinnerung an eine genehmigende Person senden

Sie können eine Nachricht senden, um eine genehmigende Person daran zu erinnern, dass Sie auf ihr Feedback warten.

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Suchen Sie das Dokument, das Sie benötigen.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** in der Zusammenfassung, klicken Sie dann auf das Menü **Mehr** , das den Namen der genehmigenden Person enthält, und wählen Sie **Erinnern** aus.

   Die genehmigende Person erhält eine Benachrichtigung, in der sie darüber informiert wird, dass die Genehmigung noch aussteht. Sie erhalten möglicherweise auch eine E-Mail-Erinnerung, wenn sie diese aktiviert haben.
