---
title: Übermitteln von Adobe Workfront-Planungsanfragen
description: Nachdem Sie von einer Datensatztyp-Seite in der Adobe Workfront-Planung einen Link zu einem Anfrageformular für eine Person freigegeben haben, können Sie eine Anforderung hinzufügen, um Datensätze für den mit dem Anfrageformular verknüpften Datensatztyp zu erstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 1%

---

# Planungsanfragen für Adobe Workfront zur Erstellung von Datensätzen übermitteln

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

{{planning-important-intro}}

Nachdem Sie von einer Datensatztyp-Seite in der Adobe Workfront-Planung einen Link zu einem Anfrageformular für eine Person freigegeben haben, können Sie eine Anforderung hinzufügen, um Datensätze für den mit dem Anfrageformular verknüpften Datensatztyp zu erstellen.

Workfront-Benutzer und externe Benutzer können Anfragen an die Planung von Datensatztypen senden und Datensätze erstellen. <!--double check on the external users-->

In diesem Artikel wird beschrieben, wie Sie eine Anfrage zum Hinzufügen neuer Datensätze zu einem Datensatztyp senden können.

Informationen dazu, wie ein Workspace-Manager ein Anforderungsformular erstellen und mit einem Datensatztyp verknüpfen kann, finden Sie unter [Erstellen und Verwalten eines Anforderungsformulars in der Adobe Workfront-Planung](/help/quicksilver/planning/requests/create-request-form.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkte</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Adobe Workfront-Planung<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td>
   <td>
<p>Die folgenden Workfront-Pläne:</p>
<ul><li>Auswählen</li>
<li>Erstklassig</li>
<li>Ultimativ</li></ul>
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p>
   </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td>
   <td>
<p>Alle </p>  
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td>
   <td>
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Externe, Mitarbeiter-, Licht- oder Standardlizenz</p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <p>Anzeigen von oder höheren Berechtigungen für einen Arbeitsbereich, wenn Sie Workfront-Benutzer sind</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Für den Zugriff auf den Planungsbereich in Workfront muss Ihnen eine Layout-Vorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p>
   <p> Der Zugriff auf den Planungsbereich ist jedoch nicht erforderlich, um Anfragen an die Workfront-Planung zu senden. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie eine Anfrage an ein Workfront Planning-Anfrageformular senden können, müssen Sie Folgendes einrichten:

* Folgendes muss in der Workfront-Planung vorhanden sein:

   * Arbeitsbereich
   * Ein mit einem Anfrageformular verknüpfter Datensatztyp. Weitere Informationen finden Sie unter [Anforderungsformular in der Adobe Workfront-Planung erstellen](/help/quicksilver/planning/requests/create-request-form.md).

* Das Anfrageformular muss für einen Link freigegeben werden, damit Sie darauf zugreifen können. Die folgenden Szenarien existieren:

   * Wenn Sie über ein Workfront-Konto verfügen, wurde der Link nur für interne Personen freigegeben und Sie haben Zugriff auf den Arbeitsbereich. Personen außerhalb von Workfront können nicht auf einen intern freigegebenen Link zugreifen.
   * Wenn Sie kein Workfront-Konto haben, wurde der Link für externe Personen freigegeben. Workfront-Benutzer können auch auf einen Link zugreifen, der für externe Personen freigegeben wurde.

* Der Link zum Formular darf nicht abgelaufen sein.

## Überlegungen zum Senden von Anfragen an die Workfront-Planung

* Sie können nicht auf die Anforderungsformulare für Workfront-Planungsanfragen zugreifen, ohne dass ein bestimmter Link zu den Formularen vorhanden ist.
* Sie können eine Anforderung nicht bearbeiten, nachdem Sie sie an die Workfront-Planung übermittelt haben.
* Jede gesendete Anfrage erstellt einen Datensatz für den Datensatztyp, der mit dem von Ihnen verwendeten Formular verknüpft ist.
* Datensätze, die durch die Übermittlung von Anfrageformularen erstellt wurden, können nicht von Datensätzen unterschieden werden, die über eine andere Methode hinzugefügt wurden. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

## Anfrage an die Workfront-Planung senden

1. Wechseln Sie von einem Workfront Planning-Record-Typ zu dem für Sie freigegebenen Link.

1. Aktualisieren Sie die im Formular verfügbaren Felder. Felder mit einem Sternchen sind erforderlich.

   >[!TIP]
   >
   >   Wenn das Feld Workfront **Betreff** verfügbar ist, ist es möglicherweise nicht in der Workfront-Planung sichtbar. Es wird empfohlen, so viele Felder in Ihrer Anfrage wie möglich zu aktualisieren, damit der neue Datensatz beim Hinzufügen zum Datensatztyp identifizierbar ist.

1. Klicken Sie auf **Senden**.

   Ihr Formular wird gesendet und dem mit dem Formular verknüpften Datensatztyp wird ein neuer Datensatz hinzugefügt.
