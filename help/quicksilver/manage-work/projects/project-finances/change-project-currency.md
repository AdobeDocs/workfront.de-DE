---
product-area: projects
navigation-topic: financials
title: Projektwährung ändern
description: Als Projekt-Manager können Sie ein Projekt so konfigurieren, dass es eine andere Währung als die Standardwährung für Ihr Adobe Workfront-System verwendet. Auf diese Weise können Sie bei der Berechnung von Arbeitskosten und Umsatz Finanzinformationen zu Ihrem Projekt in der gewünschten Währung anzeigen.
author: Lisa
feature: Work Management
exl-id: c496fe92-5c17-41a5-972b-1c063643bde3
TQID: https://experienceleague.adobe.com/oI3Fu9-AAnKYBbnaI-7BNWWd5Js6eUpvwVQtEWJVPiY
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 570
ht-degree: 7%

---

# Ändern der Projektwährung

Als Projekt-Manager können Sie ein Projekt so konfigurieren, dass es eine andere Währung als die Standardwährung für Ihr Adobe Workfront-System verwendet. Auf diese Weise können Sie bei der Berechnung von Arbeitskosten und Umsatz Finanzinformationen zu Ihrem Projekt in der gewünschten Währung anzeigen.

Bevor Sie alternative Währungen wie in diesem Abschnitt beschrieben verwenden können, muss der Workfront-Administrator zunächst mehrere Währungen aktivieren und konfigurieren, wie im Artikel [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md) beschrieben.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Zugriff auf Projekte bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Verwalten von Berechtigungen für das Projekt</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Überlegungen zum Ändern der Projektwährung in Workfront

* Sie können die Währung eines Projekts nicht ändern, wenn im Projekt Finanzinformationen vorhanden sind.
* Die Sätze werden für Arbeitskosten, Umsatzberechnungen und Berichtszwecke verwendet.
* Wenn Sie für ein Projekt keine andere Währung angeben, geht Workfront davon aus, dass die Projektwährung die Standardwährung des Systems ist. Informationen zur Standardwährung auf Systemebene finden Sie unter [Einrichten von Wechselkursen](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Standardmäßig haben alle Benutzer mit Volllizenz Zugriff auf Währungen und Wechselkurse. Der Workfront-Administrator muss zusätzlichen administrativen Zugriff für **Wechselkurse“ gewähren** damit Benutzende bestimmte Kurse für Projekte festlegen können.
* Die Wechselkurse in Workfront sind nicht dynamisch. Der Wert wird von einem Administrator festgelegt und muss aktualisiert werden, wenn Wechselkursänderungen auftreten.
* Wenn auf eine Währung und ihre Wechselkurse ein Stichtag angewendet wird, kann sich der Wechselkurs während der Laufzeit des Projekts ändern. Informationen zu effektiven Wechselkursen finden Sie unter [Einrichten von Wechselkursen](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).
* Wenn Sie einen Bericht erstellen, der die Währung eines Projekts widerspiegelt, werden standardmäßig alle Berichte nach der Standardwährung des Projekts gruppiert. Wenn Sie einen Bericht mit mehreren Projekten mit unterschiedlichen Wechselkursen erstellen, spiegeln alle auf das Projekt angewendeten Gruppierungen den Standardwechselkurs auf Systemebene wider. Weitere Informationen finden Sie im Artikel [Erstellen von Finanzdatenberichten mit eindeutigen Wechselkursen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

## Währung für ein Projekt konfigurieren

1. Wechseln Sie zu dem Projekt, in dem Sie die Standardwährung ändern möchten.

   >[!TIP]
   >
   >Stellen Sie sicher, dass das Projekt noch über keine Finanzinformationen verfügt. Stellen Sie beispielsweise sicher, dass mit dem Projekt keine geplanten Kosten oder Istkosten verknüpft sind.

1. Klicken Sie **linken Bereich auf** Projektdetails“ und navigieren Sie dann zum Bereich **Finanzen**.
1. Klicken Sie **** Feld **Währung** auf „Hinzufügen“ und wählen Sie die Währung aus, die Sie als Standardwährung für das Projekt verwenden möchten. Alle Währungen, die Ihr Workfront-Administrator für Ihre Workfront-Instanz festgelegt hat, werden angezeigt.

   ![Währung des Projekts](assets/currency-on-project.png)

1. (Bedingt) Wenn Sie eine andere Währung als die Standardwährung auswählen, die für Ihr Workfront-System festgelegt wurde, geben Sie den Kurs für die ausgewählte Währung an, da sie sich auf die Währung bezieht, die im System als Basiswährung festgelegt wurde.

   >[!NOTE]
   >
   >Wenn die **Verwendung von Datumswechselkursen aus dem System** für dieses Projekt aktiviert ist, sind Wechselkursüberschreibungen nicht zulässig. Weitere Informationen finden Sie unter [Projekte bearbeiten](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

1. Klicken Sie auf **Änderungen speichern**.
