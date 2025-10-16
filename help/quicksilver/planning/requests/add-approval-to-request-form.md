---
title: Hinzufügen einer Genehmigung zu einem Anforderungsformular in Adobe Workfront Planning
description: Sie können einem Adobe Workfront Planning-Anforderungsformular einen Genehmigungsprozess hinzufügen, um für jede gesendete Anforderung eine Genehmigung zu starten, bevor ein Datensatz erstellt wird.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: c06baa45e52d77463f9f886b6f6eae4ff68e4ccd
workflow-type: tm+mt
source-wordcount: '690'
ht-degree: 0%

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

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<ul><li><p>Beliebiges Workfront-Paket</p></li>
Und
<li><p>Beliebiges Planungspaket</p></li></ul>
Oder
<ul><li><p>Beliebiges Workflow-Paket</p></li>
Und
<li><p>Beliebiges Planungspaket</p></li></ul>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich und Datensatztyp</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Hinzufügen von Genehmigungen zu einem Anfrageformular

* Sie können einem Anfrageformular eine oder mehrere genehmigende Personen hinzufügen. Sie können nur Benutzer als genehmigende Personen hinzufügen.
* Sie können Genehmigungsinformationen zu einem Datensatz anzeigen, der durch Senden eines Anforderungsformulars in den Feldern Genehmigt von und Genehmigt am erstellt wurde. Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).
* Wenn Sie einem Anfrageformular mehrere genehmigende Personen hinzufügen, müssen alle genehmigenden Personen die Anfrage akzeptieren, bevor in Workfront Planning ein Datensatz erstellt wird.
* Wenn alle genehmigenden Personen die Anfrage genehmigen, wird ein Datensatz für den mit dem Anfrageformular verknüpften Datensatztyp erstellt.
* Wenn mindestens eine genehmigende Person die Anforderung ablehnt und alle anderen sie genehmigen, wird eine Anforderung für den Bereich Anfragen in Workfront erstellt, aber es wird kein Datensatz für den Datensatztyp erstellt, der mit dem Anfrageformular verknüpft ist.
* Das Hinzufügen von Genehmigungen zu einem Anfrageformular ist optional. Workfront Planning erstellt beim Senden einer Anfrage sofort einen Datensatz, wenn das Anforderungsformular nicht mit einer Genehmigung verknüpft ist.

## Hinzufügen einer Genehmigung zu einem Anfrageformular

1. Erstellen Sie zunächst ein Anfrageformular für einen Datensatztyp, wie in [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md) beschrieben.
1. Klicken Sie **Konfiguration**.

   Der **Konfiguration** wird angezeigt.

   ![Registerkarte „Konfiguration“](assets/configuration-tab.png)
1. Klicken **im Feld** auf das Dropdown-Symbol und wählen Sie einen oder mehrere Benutzer oder Teams in der Liste aus

   Oder

   Geben Sie den Namen eines Benutzers oder Teams ein, den Sie als genehmigende Person festlegen möchten, und wählen Sie ihn aus, wenn er/sie in der Liste angezeigt wird.

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
   >
   >* Wenn ein Team als genehmigende Person festgelegt ist, ist nur eine Entscheidung vom Team erforderlich.


1. (Optional) Klicken Sie auf **Veröffentlichen** wenn Sie das Anfrageformular noch nie zuvor freigegeben haben

   Oder

   Klicken Sie auf **Freigeben**, um das Formular freizugeben, und **Link kopieren**.
1. (Optional) Nachdem ein(e) Benutzende(r) den von Ihnen freigegebenen Link verwendet und eine Anfrage gesendet hat, sendet Workfront Planning eine In-App-Benachrichtigung über die Genehmigung und eine E-Mail an die genehmigenden Personen.

   >[!NOTE]
   >
   >   Damit Benutzerinnen und Benutzer E-Mail- und In-App-Benachrichtigungen empfangen können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.


   Informationen zum Genehmigen von Anfragen finden Sie unter [Genehmigen einer Anfrage](/help/quicksilver/planning/requests/approve-request.md).
