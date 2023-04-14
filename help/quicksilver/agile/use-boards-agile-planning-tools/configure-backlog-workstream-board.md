---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Konfigurieren des Rückstands auf einer Workstream-Pinnwand
description: Sie können festlegen, dass in einem Workstream eine Spalte mit dem Rückstand auf einer Pinnwand angezeigt werden soll, und eine Abfrage für die Karten definieren, die aus der Liste der Workstream-Karten in den Pinnwandspeicher gezogen werden.
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 75bb5af9564947a39e1cb46f9d6be2c03eb07acc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Konfigurieren des Rückstands auf einer Workstream-Pinnwand

Sie können festlegen, dass in einem Workstream eine Spalte mit dem Rückstand auf einer Pinnwand angezeigt werden soll, und eine Abfrage für die Karten definieren, die aus der Liste der Workstream-Karten in den Pinnwandspeicher gezogen werden. Diese Optionen sind auf Standalone-Pinnwänden nicht verfügbar. Weitere Informationen zum Hinzufügen einer Ansaugspalte zu einer Standalone-Pinnwand finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Konfigurieren des Rückstands auf einer Workstream-Pinnwand

{{step1-to-boards}}

1. Öffnen Sie den Workflow, in dem Sie arbeiten möchten. Um einen Workflow zu öffnen, klicken Sie auf [!UICONTROL **Workflow anzeigen**].
1. Klicken Sie auf eine beliebige Pinnwand im Workstream, um sie zu öffnen.
1. Klicken [!UICONTROL **Konfigurieren**] auf der rechten Seite der Pinnwand, um den Bereich Konfigurieren zu öffnen.
1. Aktivieren [!UICONTROL **Eine Spalte im Rückstand auf dieser Pinnwand einschließen**].

   Die Spalte &quot;backlog&quot;wird links auf der Pinnwand hinzugefügt. Sie bleibt leer, bis Sie eine Abfrage darauf anwenden.

1. Erweitern [!UICONTROL **Backlog-Abfrage**].

   >[!NOTE]
   >
   >Möglicherweise wird bereits eine Standardabfrage auf den Rückstand angewendet, die alle Arbeitselemente aus der Kartenliste anzeigt, die nicht zu einer Iteration gehören und sich nicht im Status Abgeschlossen befinden.

1. Klicken [!UICONTROL **Bedingung hinzufügen**] und klicken Sie in das Feld &quot;leer&quot;.
1. Wählen Sie das Feld aus, nach dem abgefragt werden soll.

   Die Felder, aus denen Sie auswählen können, sind die Standardfelder auf einer Karte.

1. Wählen Sie den Abfragemodifikator aus.

   Die Modifikatoroptionen hängen von den Feldern ab, auf die sie angewendet werden können. Beispielsweise verfügt das Feld &quot;Name&quot;nicht über &quot;größer als&quot;oder &quot;kleiner als&quot; als Modifikatoroptionen, da diese Modifikatoren nur für Zahlen gelten.

1. Wählen Sie den Wert aus.

   Der Wert ist nicht verfügbar, wenn Sie &quot;vorhanden&quot;oder &quot;nicht vorhanden&quot;als Modifikator verwenden.

   Wenn Sie beispielsweise &quot;Fälligkeitsdatum&quot;und &quot;Vorhanden&quot;wählen, zeigt der Rückstand Karten mit zugewiesenen Fälligkeitsdaten an. Jede Karte ohne Fälligkeitsdatum wird nicht in den Rückstand gezogen.

1. (Optional) Klicken Sie auf [!UICONTROL **Bedingung hinzufügen**] , um der Abfrage eine weitere Bedingung hinzuzufügen.

   ![Rückstandsabfrage](assets/backlog-query-wrkstrm-board.png)

1. (Optional) Klicken Sie auf [!UICONTROL **Gruppe erstellen**] , um eine Gruppe von Bedingungen hinzuzufügen, die mit der ersten Bedingung mit einem ODER -Operator verbunden sind.
1. Klicken [!UICONTROL **Abfrage speichern**].

   Die Abfrage wird angewendet und die den Kriterien entsprechenden Karten werden in der Spalte &quot;Rückstand&quot;angezeigt.
