---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filter: mehrere Filterregeln erstellen, die auf dasselbe Feld verweisen ('AND'-Anweisungen)"
description: Wenn Sie in der Benutzeroberfläche des Standardmodus versuchen, mehrere Filter zu erstellen, die auf dasselbe Feld verweisen (mithilfe des AND-Qualifizierers), wird einer der Filter beim Speichern des Berichts und Beenden des ReportBuilder gelöscht.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Filter: mehrere Filterregeln erstellen, die auf dasselbe Feld verweisen (&quot;AND&quot;-Anweisungen)

Wenn Sie in der Benutzeroberfläche des Standardmodus versuchen, mehrere Filter zu erstellen, die auf dasselbe Feld verweisen (mithilfe des AND-Qualifizierers), wird einer der Filter beim Speichern des Berichts und Beenden des ReportBuilder gelöscht.

**Beispiel:** Möglicherweise möchten Sie nur Aufgaben anzeigen, die das Wort &quot;grün&quot;enthalten, im Namen jedoch nicht das Wort &quot;rot&quot;enthalten. Adobe Workfront ermöglicht es Ihnen nicht, die folgenden Filterregeln mithilfe der Benutzeroberfläche des Standardmodus zu speichern, da sie dasselbe Feld (Aufgabenname) referenziert, aber unterschiedliche Modifikatoren verwendet und sich auf unterschiedliche Werte bezieht:

* Aufgabenname > Enthält > Grün
* Aufgabenname > enthält nicht > Rot

Sie können diesen Filter jedoch im Textmodus erstellen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Filteränderung anfordern </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Mehrere Filterregeln erstellen, die auf dasselbe Feld verweisen

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Filter** Dropdown-Menü auswählen **Neuer Filter**.
1. Klicken **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Fügen Sie im Bereich Filterregeln für Ihren Bericht festlegen den folgenden Code hinzu:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Um ähnliche Filter zu erstellen, erstellen Sie zuerst die erste Anweisung. Beispiel:
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Kopieren Sie die Anweisung und fügen Sie sie beliebig oft ein. Anschließend können Sie so viele Anweisungen hinzufügen, wie Sie benötigen, um auf dasselbe Feld zu verweisen (in unserem Fall &quot;name&quot;), und die folgenden Änderungen an den zusätzlichen Anweisungen vornehmen:
   >
   >1. Stellen Sie den beiden kopierten Zeilen den Vorrang vor &quot;AND&quot;.:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot;, etc für jeden neuen Feld möglichen Wert.
   >1. Ersetzen Sie die Feldzeile durch den neuen Feldwert (nach dem Zeichen &quot;=&quot;).
   >1. Ersetzen Sie die Modifikatorzeile (_Mod) durch den neuen Modifikator.

   >   
   >Bei diesen Anweisungen wird zwischen Groß- und Kleinschreibung unterschieden.

1. Klicken **Fertig**, dann **Filter speichern**.
