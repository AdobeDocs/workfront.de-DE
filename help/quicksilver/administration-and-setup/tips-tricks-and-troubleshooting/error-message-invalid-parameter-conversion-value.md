---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: Ungültiger Parameter: Konversionswert'
description: '"Sie erhalten die folgende Fehlermeldung, wenn Sie versuchen, das Format eines benutzerdefinierten Felds in einem vorhandenen benutzerdefinierten Formular zu ändern: "Ungültiger Parameter: Konversionswert `&lt;...&gt;`"'
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7aac95-4afb-422d-877b-0fa49ef43883
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 1%

---

# Fehlermeldung: Ungültiger Parameter: Konversionswert

## Problem

Sie erhalten die folgende Fehlermeldung, wenn Sie versuchen, das Format eines benutzerdefinierten Felds in einem vorhandenen benutzerdefinierten Formular zu ändern: &quot;Ungültiger Parameter: Konversionswert &quot;&lt;..>&quot;&quot;\
![custom_field_format_invalid_parameter_error.png](assets/custom-field-format-invalid-parameter-error-350x148.png)

## Ursache

Diese Meldung tritt im folgenden Szenario auf:

Sie haben beispielsweise ein als Text formatiertes benutzerdefiniertes Feld.  Jetzt möchten Sie das Format des benutzerdefinierten Felds in Währung ändern. Irgendwo in Ihrem [!DNL Adobe Workfront] -Instanz ist dieses Feld bereits an ein Objekt angehängt und enthält bereits Informationen, die darin angegeben sind. Die vorhandenen Informationen in mindestens einem dieser Felder sind bereits als Text formatiert. Daher kann das Format des Felds nicht in Währung geändert werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Workfront] Plan</a>*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] Lizenzübersicht</a>*</p> </td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Erstellen von Berichten, Dashboards und Kalendern</p> </li> 
     <li> <p>Erstellen von Filtern, Ansichten und Gruppierungen</p> </li> 
    </ul> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Gehen Sie wie folgt vor:

1. Erstellen Sie Berichte für alle Objekte, denen dieses Feld möglicherweise mit dem benutzerdefinierten Forms zugeordnet ist.\
   Informationen zum Erstellen eines Berichts finden Sie unter [Benutzerdefinierten Bericht erstellen](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Schließen Sie das benutzerdefinierte Feld, das Sie bearbeiten möchten, in die Ansicht des Berichts ein, damit Sie sehen können, für welches Objekt dieses Feld einen Textwert enthält.
1. Korrigieren Sie die Werte des benutzerdefinierten Felds der Objekte, die in einem Textformat angezeigt werden, und geben Sie ihnen einen Wert, der als Währung formatiert ist. Versuchen Sie dann erneut, das Feld Format im benutzerdefinierten Formular zu ändern.\
   Oder\
   Wenn Sie bereits zu viele Feldwerte mit textformatierten Informationen ausgefüllt haben, sollten Sie ein neues benutzerdefiniertes Feld zu Ihrem benutzerdefinierten Formular hinzufügen und es als Währung formatieren.
