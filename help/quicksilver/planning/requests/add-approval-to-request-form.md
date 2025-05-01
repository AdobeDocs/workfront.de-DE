---
title: Hinzufügen einer Genehmigung zu einem Anforderungsformular in Adobe Workfront Planning
description: Sie können einem Adobe Workfront Planning-Anforderungsformular einen Genehmigungsprozess hinzufügen, um für jede gesendete Anforderung eine Genehmigung zu starten, bevor ein Datensatz erstellt wird.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 1%

---

# Hinzufügen einer Genehmigung zu einem Anforderungsformular in Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können einem Adobe Workfront Planning-Anforderungsformular einen Genehmigungsprozess hinzufügen, um für jede gesendete Anforderung eine Genehmigung zu starten, bevor ein Datensatz erstellt wird.

In diesem Artikel wird beschrieben, wie ein Workspace-Manager einem Anfrageformular, das mit einem Datensatztyp verknüpft ist, eine Genehmigung hinzufügen kann.

Informationen zum Erstellen eines Anfrageformulars in Workfront Planning finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Weitere Informationen zum Senden einer Anfrage an einen Datensatztyp zum Erstellen eines Datensatzes finden Sie unter [Senden von Adobe Workfront Planning-Anfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
<p>Einer der folgenden Workfront-Pläne:</p>
<ul><li>Auswählen</li>
<li>Erstklassig</li>
<li>Ultimativ</li></ul>
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p>
   </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td>
   <td>
<p>Beliebig </p>  
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </td>

<tr>
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td>
   <td>
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Standard</p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Objektberechtigungen</p></td>
   <td>
   <ul>
   <li><p>Verwalten von Berechtigungen für einen Arbeitsbereich <span class="preview">und Datensatztyp</span></p></li>
    <li><p>Systemadministratoren können Arbeitsbereiche verwalten, die sie nicht erstellt haben. </p></li>
    </ul>
   <p>Informationen zu Freigabeberechtigungen für Workfront Planning-Objekte finden Sie unter  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Übersicht über Freigabeberechtigungen in Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>In der Produktionsumgebung müssen alle Benutzer, einschließlich der Systemadministratoren, einer Layoutvorlage zugewiesen werden, die Planning enthält.</p>
<p><span class="preview">In der Vorschau-Umgebung ist für Standardbenutzer und Systemadministratoren „Planung“ standardmäßig aktiviert.</span></p>
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Hinzufügen von Genehmigungen zu einem Anfrageformular

* Sie können einem Anfrageformular eine oder mehrere genehmigende Personen hinzufügen. Sie können nur Benutzer als genehmigende Personen hinzufügen.
* Wenn Sie einem Anfrageformular mehrere genehmigende Personen hinzufügen, müssen alle genehmigenden Personen die Anfrage akzeptieren, bevor in Workfront Planning ein Datensatz erstellt wird.
* Wenn alle genehmigenden Personen die Anfrage genehmigen, wird ein Datensatz für den mit dem Anfrageformular verknüpften Datensatztyp erstellt.
* Wenn mindestens eine genehmigende Person die Anforderung ablehnt und alle anderen sie genehmigen, wird eine Anforderung für den Bereich Anfragen in Workfront erstellt, aber es wird kein Datensatz für den Datensatztyp erstellt, der mit dem Anfrageformular verknüpft ist.
* Das Hinzufügen von Genehmigungen zu einem Anfrageformular ist optional. Workfront Planning erstellt beim Senden einer Anfrage sofort einen Datensatz, wenn das Anforderungsformular nicht mit einer Genehmigung verknüpft ist.

## Hinzufügen einer Genehmigung zu einem Anfrageformular

1. Erstellen Sie zunächst ein Anfrageformular für einen Datensatztyp, wie in [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md) beschrieben.
1. Klicken Sie **Konfiguration**.

   Der **Konfiguration** wird angezeigt.

   ![Registerkarte „Konfiguration“](assets/configuration-tab.png)
1. Klicken **im Feld** auf das Dropdown-Symbol und wählen Sie einen oder mehrere Namen aus der Liste aus

   Oder

   Beginnen Sie mit der Eingabe des Namens einer genehmigenden Person und wählen Sie diese aus, wenn sie in der Liste angezeigt wird.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Sie können einem Anfrageformular eine oder mehrere genehmigende Personen hinzufügen.
   >
   >* Wenn Sie mehr als eine genehmigende Person hinzufügen, müssen alle genehmigenden Personen die Anfrage genehmigen, bevor Workfront Planning einen Datensatz erstellt.
   >
   >* Wenn mindestens eine genehmigende Person die Anforderung ablehnt, wird die Anforderung abgelehnt und der Datensatz nicht erstellt. Die Anfrage verbleibt auf der Registerkarte Planung im Abschnitt Gesendet im Bereich Anfragen in Workfront.
   >
   >* Alle genehmigenden Personen müssen eine Entscheidung treffen, bevor eine Anfrage genehmigt oder abgelehnt wird.


1. (Optional) Klicken Sie auf **Veröffentlichen** wenn Sie das Anfrageformular noch nie zuvor freigegeben haben

   Oder

   Klicken Sie auf **Freigeben**, um das Formular freizugeben, und **Link kopieren**.
1. (Optional) Nachdem ein(e) Benutzende(r) den von Ihnen freigegebenen Link verwendet und eine Anfrage gesendet hat, sendet Workfront Planning eine In-App-Benachrichtigung über die Genehmigung und eine E-Mail an die genehmigenden Personen.

   >[!NOTE]
   >
   >   Damit Benutzerinnen und Benutzer E-Mail- und In-App-Benachrichtigungen empfangen können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.


   Informationen zum Genehmigen von Anfragen finden Sie unter [Genehmigen einer Anfrage](/help/quicksilver/planning/requests/approve-request.md).
