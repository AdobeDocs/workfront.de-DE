---
title: Hinzufügen einer Genehmigung zu einem Anforderungsformular
description: Sie können einem Adobe Workfront-Planungsanfrageformular einen Genehmigungsprozess hinzufügen, um eine Genehmigung für jede gesendete Anfrage zu initiieren, bevor ein Datensatz erstellt wird.
hide: true
hidefromTOC: true
source-git-commit: a999b805016361bdd101a6cd9c61967284a71014
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 1%

---


<!--

---
title: Add an Approval to a Request Form
description: You can add an approval process to an Adobe Workfront Planning request form, to initiate an approval for every submitted request, before it creates a record. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->

# Hinzufügen einer Validierung zu einem Anforderungsformular

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

Sie können einem Adobe Workfront-Planungsanfrageformular einen Genehmigungsprozess hinzufügen, um eine Genehmigung für jede gesendete Anfrage zu initiieren, bevor ein Datensatz erstellt wird.

In diesem Artikel wird beschrieben, wie ein Workspace-Manager einem Anforderungsformular, das mit einem Datensatztyp verknüpft ist, eine Genehmigung hinzufügen kann.

Informationen zum Erstellen eines Anfrageformulars in der Workfront-Planung finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in der Adobe Workfront-Planung](/help/quicksilver/planning/requests/create-request-form.md).

Weitere Informationen zum Senden einer Anfrage an einen Datensatztyp zum Erstellen eines Datensatzes finden Sie unter [Planungsanfragen zum Erstellen von Datensätzen durch Adobe Workfront übermitteln](/help/quicksilver/planning/requests/submit-requests.md).

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
   <p>Standard</p>
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
   <ul>
   <li><p>Berechtigungen für einen Arbeitsbereich verwalten</p></li>
    <li><p>Systemadministratoren können nicht erstellte Arbeitsbereiche verwalten. </p></li>
    </ul>
   <p>Informationen zum Freigeben von Berechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Überblick über die Freigabe von Berechtigungen in der Adobe Workfront-Planung</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Hinzufügen von Genehmigungen zu einem Anforderungsformular

* Sie können einem Anfrageformular einen oder mehrere Genehmiger hinzufügen. Sie können nur Benutzer als Genehmiger hinzufügen.
* Wenn Sie einem Anfrageformular mehrere Genehmiger hinzufügen, müssen alle Genehmiger die Anfrage akzeptieren, bevor in der Workfront-Planung ein Datensatz erstellt wird.
* Das Hinzufügen von Genehmigungen zu einem Anfrageformular ist optional. Workfront Planning erstellt sofort einen Datensatz, wenn eine Anforderung gesendet wird, wenn das Anfrageformular keiner Genehmigung zugeordnet ist.

## Hinzufügen einer Validierung zu einem Anforderungsformular

1. Beginnen Sie mit der Erstellung eines Anforderungsformulars für einen Datensatztyp, wie unter [Erstellen und Verwalten eines Anforderungsformulars in der Adobe Workfront-Planung](/help/quicksilver/planning/requests/create-request-form.md) beschrieben.
1. Klicken Sie auf **Konfiguration**.

   Der Bereich **Konfiguration** wird angezeigt.

   ![](assets/configuration-tab.png)
1. Klicken Sie im Feld **Genehmiger** auf das Dropdownsymbol und wählen Sie einen oder mehrere Namen in der Liste aus

   Oder

   Geben Sie den Namen eines Genehmigers ein und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   >[!TIP]
   >
   >    Wenn Sie mehr als einen Genehmiger hinzufügen, müssen alle Genehmiger die Anfrage genehmigen, bevor Workfront Planning einen Datensatz erstellt.

1. (Optional) Klicken Sie auf **Publish** , wenn Sie das Anforderungsformular noch nie freigegeben haben.

   Oder

   Klicken Sie auf **Freigeben** , um das Formular freizugeben, und dann auf **Link kopieren**.
1. (Optional) Nachdem ein Benutzer den von Ihnen freigegebenen Link verwendet und eine Anfrage gesendet hat, sendet Workfront Planning eine Validierungsbenachrichtigung und eine E-Mail an die Genehmiger.

   Informationen zum Genehmigen von Anforderungen finden Sie unter [Anfrage genehmigen](/help/quicksilver/planning/requests/approve-request.md).

