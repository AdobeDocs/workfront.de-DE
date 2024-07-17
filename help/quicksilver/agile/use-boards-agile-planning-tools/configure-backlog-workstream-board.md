---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Konfigurieren des Rückstands auf einer Arbeitsfläche
description: Sie können festlegen, dass in einem Workstream eine Spalte mit dem Rückstand auf einer Pinnwand angezeigt werden soll, und eine Abfrage für die Karten definieren, die aus der Liste der Workstream-Karten in den Pinnwandspeicher gezogen werden.
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 0%

---

# Konfigurieren des Rückstands auf einer Arbeitsfläche

>[!IMPORTANT]
>
>Workflows stehen nur einer bestimmten Kundengruppe zur Verfügung.

Sie können festlegen, dass in einem Workstream eine Spalte mit dem Rückstand auf einer Pinnwand angezeigt werden soll, und eine Abfrage für die Karten definieren, die aus der Liste der Workstream-Karten in den Pinnwandspeicher gezogen werden.

>[!NOTE]
>
>Wenn Sie eine neue Karte in die Spalte &quot;Backlog&quot;einfügen, die nicht den Abfragekriterien entspricht, verschwindet die Karte beim Aktualisieren der Pinnwand aus dem Backlog und ist nur in der Kartenliste verfügbar. Sie können die Abfrage jederzeit ändern, um die Karten anzupassen, die in der Spalte &quot;Rückstand&quot;angezeigt werden.

Die Spalte mit dem Rückstand und die Abfrage sind auf Standalone-Pinnwänden nicht verfügbar. Weitere Informationen zum Hinzufügen einer Ansaugspalte zu einer Standalone-Pinnwand finden Sie unter [Hinzufügen einer Annahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Konfigurieren des Rückstands auf einer Arbeitsfläche

{{step1-to-boards}}

1. Öffnen Sie den Workflow, in dem Sie arbeiten möchten. Um einen Workstream zu öffnen, klicken Sie auf [!UICONTROL **Workflow anzeigen**].
1. Klicken Sie auf eine beliebige Pinnwand im Workstream, um sie zu öffnen.
1. Klicken Sie rechts auf der Pinnwand auf [!UICONTROL **Konfigurieren**] , um den Bereich &quot;Konfigurieren&quot;zu öffnen.
1. Aktivieren Sie [!UICONTROL **Fügen Sie eine Rückstagespalte auf dieser Pinnwand ein**].

   Die Spalte &quot;backlog&quot;wird links auf der Pinnwand hinzugefügt. Sie bleibt leer, bis Sie eine Abfrage darauf anwenden.

1. Erweitern Sie [!UICONTROL **Backlog-Abfrage**].

   >[!NOTE]
   >
   >Eine Standardabfrage kann bereits auf den Rückstand angewendet werden, um alle Arbeitselemente aus der Kartenliste anzuzeigen, die einen Status haben und deren Status nicht abgeschlossen ist.

1. Klicken Sie auf [!UICONTROL **Bedingung hinzufügen**] und klicken Sie auf das Feld &quot;leer&quot;.
1. Wählen Sie das Feld aus, nach dem abgefragt werden soll.

   Die Felder, aus denen Sie auswählen können, sind die Standardfelder auf einer Karte.

1. Wählen Sie den Abfragemodifikator aus.

   Die Modifikatoroptionen hängen von den Feldern ab, auf die sie angewendet werden können. Beispielsweise verfügt das Feld &quot;Name&quot;nicht über &quot;größer als&quot;oder &quot;kleiner als&quot; als Modifikatoroptionen, da diese Modifikatoren nur für Zahlen gelten.

1. Wählen Sie den Wert aus.

   Der Wert ist nicht verfügbar, wenn Sie &quot;vorhanden&quot;oder &quot;nicht vorhanden&quot;als Modifikator verwenden.

   Wenn Sie beispielsweise &quot;Fälligkeitsdatum&quot;und &quot;Vorhanden&quot;wählen, zeigt der Rückstand Karten mit zugewiesenen Fälligkeitsdaten an. Jede Karte ohne Fälligkeitsdatum wird nicht in den Rückstand gezogen.

1. (Optional) Klicken Sie auf [!UICONTROL **Bedingung hinzufügen**] , um der Abfrage eine weitere Bedingung hinzuzufügen.

   ![Rücklog-Abfrage](assets/backlog-query-wrkstrm-board.png)

1. (Optional) Klicken Sie auf [!UICONTROL **Gruppe erstellen**] , um eine Gruppe von Bedingungen hinzuzufügen, die mit der ersten Bedingung mit einem ODER-Operator verbunden sind.
1. Klicken Sie auf [!UICONTROL **Abfrage speichern**].

   Die Abfrage wird angewendet und die den Kriterien entsprechenden Karten werden in der Spalte &quot;Rückstand&quot;angezeigt.
