---
title: Übermitteln von Adobe Workfront-Planungsanfragen
description: Nachdem Sie von einer Datensatztyp-Seite in der Adobe Workfront-Planung einen Link zu einem Anfrageformular für eine Person freigegeben haben, können Sie eine Anforderung hinzufügen, um Datensätze für den mit dem Anfrageformular verknüpften Datensatztyp zu erstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: d7c7b09b033705142b2c658c9d275e63299d3fd0
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---


# Planungsanfragen für Adobe Workfront zur Erstellung von Datensätzen übermitteln

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

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
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td>
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

   * Wenn Sie über ein Workfront-Konto verfügen, wurde der Link nur für interne Personen freigegeben, und Sie haben einen Beitrag oder einen höheren Zugriff auf den Arbeitsbereich. Personen außerhalb von Workfront können nicht auf einen intern freigegebenen Link zugreifen.
   * Wenn Sie kein Workfront-Konto haben, wurde der Link für externe Personen freigegeben. Workfront-Benutzer können auch auf einen Link zugreifen, der für externe Personen freigegeben wurde.

* Der Link zum Formular darf nicht abgelaufen sein.

## Überlegungen zum Senden von Anfragen an die Workfront-Planung

* Sie können auf ein Anforderungsformular für Workfront-Planungsanfragen nur über einen bestimmten Link zum Formular zugreifen.
* Sie können eine Anforderung nicht bearbeiten, nachdem Sie sie an die Workfront-Planung übermittelt haben.
* Jede gesendete Anfrage erstellt einen Datensatz für den Datensatztyp, der mit dem Formular verknüpft ist, das Sie <!--<span class="preview">if the form is not associated with an approval, or if the approval has been granted.</span> --> verwenden
* Datensätze, die durch die Übermittlung von Anfrageformularen erstellt wurden, können nicht von Datensätzen unterschieden werden, die über eine andere Methode hinzugefügt wurden. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* <span class="preview">Gesendete Anforderungen werden auf der Registerkarte &quot;Planung&quot;des Abschnitts &quot;Gesendet&quot;im Bereich &quot;Anforderungen&quot;von Workfront angezeigt </span>.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some incosistency between unified-approvals-service and intake-approvals-flow.-->


## Anfrage an die Workfront-Planung senden

1. Wechseln Sie von einem Workfront Planning-Record-Typ zu dem für Sie freigegebenen Link.

1. Aktualisieren Sie die im Formular verfügbaren Felder. Felder mit einem Sternchen sind erforderlich.

   >[!TIP]
   >
   >   Wenn das Feld **Betreff** verfügbar ist, wird es nach dem Senden der Anfrage in der Workfront-Planung nicht mehr angezeigt.
   >
   >Es wird empfohlen, so viele Felder in Ihrer Anfrage wie möglich zu aktualisieren, damit der neue Datensatz beim Hinzufügen zum Datensatztyp in der Workfront-Planung identifizierbar ist.

1. Klicken Sie auf **Senden**.

   Ihr Formular wird gesendet und die folgenden Vorgänge treten auf:

   * <!--If the request form was not associated with an approval, or <span class="preview">if the approval was granted</span>, a-->Dem mit dem Formular verknüpften Datensatztyp wird ein neuer Datensatz hinzugefügt.


   * <!--If the request form was not associated with an approval, the--> <span class="preview"> Die Anforderung wird zum Abschnitt &quot;Gesendet&quot;des Workfront-Anforderungsbereichs hinzugefügt und der Seite mit dem Datensatztyp wird ein neuer Datensatz hinzugefügt.</span>

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     ><span class="preview">Alle Benutzer, die Zugriff auf mindestens einen Arbeitsbereich haben, können die Registerkarte Planung im Bereich Anforderungen anzeigen. Sie können nur die von Ihnen gesendeten Anfragen anzeigen. Workfront-Administratoren können alle Anforderungen im System anzeigen. </span> <!--ensure this is correct; asking team in slack-->

   <!--
   * <span class="preview">If the request form was associated with an approval, the request is temporarily saved to the Planning tab in the Submitted section of the Workfront Requests area. No record is created for the record type associated with the request form.</span>

      <span class="preview">For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).</span>  
   -->
   <!--

   * <span class="preview">You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.</span> 
   * <span class="preview">If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.</span> 
   -->



