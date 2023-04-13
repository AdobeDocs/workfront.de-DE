---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Konfigurieren des Rückstands auf einer Workstream-Pinnwand
description: Sie können festlegen, dass in einem Workstream eine Spalte mit dem Rückstand auf einer Pinnwand angezeigt werden soll, und eine Abfrage für die Karten definieren, die aus der Liste der Workstream-Karten in den Pinnwandspeicher gezogen werden.
author: Lisa
source-git-commit: b58831d50c2be421c666515808091aa4863bb471
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 1%

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
1. Klicken [!UICONTROL **Bedingung hinzufügen**] und klicken Sie in das Feld &quot;leer&quot;.
1. Wählen Sie das Feld aus, nach dem abgefragt werden soll.

   Die Felder, aus denen Sie auswählen können, sind die Standardfelder auf einer Karte.

1. Wählen Sie den Abfragemodifikator aus.

   Die Optionen sind: ist gleich, ist nicht gleich, existiert und existiert nicht.

   Beispiel: Wenn Sie Fälligkeitsdatum wählen und bereits vorhanden ist, zeigt der Rückstand Karten mit zugewiesenen Fälligkeitsdaten an. Jede Karte ohne Fälligkeitsdatum wird nicht in den Rückstand gezogen.

1. Wählen Sie den Wert aus.

   Der Wert ist nur verfügbar, wenn Sie als Modifikator &quot;Gleich&quot;oder &quot;Gleich&quot;verwenden.

1. (Optional) Klicken Sie auf [!UICONTROL **Bedingung hinzufügen**] , um der Abfrage eine weitere Bedingung hinzuzufügen.

   ![Rückstandsabfrage](assets/backlog-query-wrkstrm-board.png)

1. (Optional) Klicken Sie auf [!UICONTROL **Gruppe erstellen**] , um eine Gruppe von Bedingungen hinzuzufügen, die mit der ersten Bedingung mit einem ODER -Operator verbunden sind.
1. Klicken [!UICONTROL **Abfrage speichern**].

   Die Abfrage wird angewendet und die den Kriterien entsprechenden Karten werden in der Spalte &quot;Rückstand&quot;angezeigt.
