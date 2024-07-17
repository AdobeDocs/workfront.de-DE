---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: ungültiger Parameter: Konversionswert'
description: "Sie erhalten die folgende Fehlermeldung, wenn Sie versuchen, das Format eines benutzerdefinierten Felds in einem vorhandenen benutzerdefinierten Formular zu ändern: 'Ungültiger Parameter: Konvertierungswert `&lt;..&gt;`'"
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Fehlermeldung: ungültiger Parameter: Konversionswert

## Problem

Sie erhalten die folgende Fehlermeldung, wenn Sie versuchen, das Format eines benutzerdefinierten Felds in einem vorhandenen benutzerdefinierten Formular zu ändern: &quot;Ungültiger Parameter: Konvertierungswert &quot;&lt;..>&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Ursache

Diese Meldung tritt im folgenden Szenario auf:

Sie haben beispielsweise ein als Text formatiertes benutzerdefiniertes Feld.  Jetzt möchten Sie das Format des benutzerdefinierten Felds in Währung ändern. Irgendwo in Ihrer Adobe Workfront-Instanz ist dieses Feld bereits an ein Objekt angehängt und enthält bereits Informationen. Die vorhandenen Informationen in mindestens einem dieser Felder sind bereits als Text formatiert. Daher kann das Format des Felds nicht in Währung geändert werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">Workfront-Plan</a>*</p> </td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Überblick über Lizenzen</a>*</p> </td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Erstellen von Berichten, Dashboards und Kalendern</p> </li> 
     <li> <p>Erstellen von Filtern, Ansichten und Gruppen</p> </li> 
    </ul> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Gehen Sie wie folgt vor:

1. Erstellen Sie Berichte für alle Objekte, denen dieses Feld möglicherweise mit dem benutzerdefinierten Forms zugeordnet ist.\
   Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerspezifischen Bericht erstellen](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Schließen Sie das benutzerdefinierte Feld, das Sie bearbeiten möchten, in die Ansicht des Berichts ein, damit Sie sehen können, für welches Objekt dieses Feld einen Textwert enthält.
1. Korrigieren Sie die Werte für das benutzerdefinierte Feld der Objekte, die in einem Textformat angezeigt werden, und geben Sie ihnen einen als Währung formatierten Wert. Versuchen Sie dann erneut, das Feld Format im benutzerdefinierten Formular zu ändern.\
   Oder\
   Wenn Sie bereits zu viele Feldwerte mit textformatierten Informationen ausgefüllt haben, sollten Sie ein neues benutzerdefiniertes Feld zu Ihrem benutzerdefinierten Formular hinzufügen und es als Währung formatieren.
