---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Konfigurieren des Rückstands auf einer Workstream-Pinnwand
description: Sie können eine Rückstandsspalte auf einer Pinnwand in einem Arbeitsablauf anzeigen und eine Abfrage für die Karten definieren, die aus der Arbeitsablauf-Kartenliste in den Pinnwand-Rückstand gezogen werden.
author: Lisa
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Konfigurieren des Rückstands auf einer Workstream-Pinnwand

>[!IMPORTANT]
>
>Arbeitsabläufe stehen nur einer bestimmten Kundengruppe zur Verfügung.

Sie können eine Rückstandsspalte auf einer Pinnwand in einem Arbeitsablauf anzeigen und eine Abfrage für die Karten definieren, die aus der Arbeitsablauf-Kartenliste in den Pinnwand-Rückstand gezogen werden.

>[!NOTE]
>
>Wenn Sie in der Rückstandsspalte eine neue Karte hinzufügen, die nicht den Abfragekriterien entspricht, verschwindet die Karte aus dem Rückstand, wenn die Pinnwand aktualisiert wird, und sie ist nur in der Kartenliste verfügbar. Sie können die Abfrage jederzeit ändern, um anzupassen, welche Karten in der Spalte „Rückstand“ angezeigt werden.

Die Rückstandsspalte und die Abfrage sind auf eigenständigen Pinnwänden nicht verfügbar. Informationen zum Hinzufügen einer Aufnahmespalte zu einer eigenständigen Pinnwand finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neu: [!UICONTROL Contributor] oder höher</p> 
   <p>oder</p>
   <p>Aktuell: [!UICONTROL -Anfrage] oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren des Rückstands auf einer Workstream-Pinnwand

{{step1-to-boards}}

1. Öffnen Sie den Arbeitsablauf, in dem Sie arbeiten möchten. Um einen Arbeitsablauf zu öffnen, klicken Sie auf [!UICONTROL **Arbeitsablauf anzeigen**].
1. Klicken Sie auf eine beliebige Pinnwand im Arbeitsablauf, um sie zu öffnen.
1. Klicken Sie [!UICONTROL **rechts auf**] Pinnwand auf „Konfigurieren“, um das Bedienfeld „Konfigurieren“ zu öffnen.
1. Aktivieren Sie [!UICONTROL **Eine Rückstandsspalte auf dieser Pinnwand**].

   Die Rückstandsspalte wird links auf der Pinnwand hinzugefügt. Sie bleibt leer, bis Sie eine Abfrage darauf anwenden.

1. Erweitern Sie [!UICONTROL **Rückstandsabfrage**].

   >[!NOTE]
   >
   >Möglicherweise wurde bereits eine Standardabfrage auf den Rückstand angewendet, die alle Arbeitselemente aus der Kartenliste mit dem Status „Nicht abgeschlossen“ anzeigt.

1. Klicken Sie [!UICONTROL **„Bedingung hinzufügen**] und klicken Sie in das Feld „leer“.
1. Wählen Sie das Feld aus, nach dem abgefragt werden soll.

   Die Felder, aus denen Sie auswählen können, sind die Standardfelder auf einer Karte.

1. Wählen Sie den Abfragemodifikator aus.

   Die Modifikatoroptionen hängen von den Feldern ab, auf die sie angewendet werden können. Beispielsweise verfügt das Feld „Name“ nicht über die Modifikatoroptionen „größer als“ oder „kleiner als“, da diese Modifikatoren nur für Zahlen gelten.

1. Wählen Sie den Wert.

   Der Wert ist nicht verfügbar, wenn Sie „exists“ oder „NOT EXIST“ als Modifikator verwenden.

   Wenn Sie beispielsweise „Fälligkeitsdatum“ und „vorhanden“ wählen, zeigt der Rückstand Karten mit zugewiesenen Fälligkeitsdaten an. Karten ohne Fälligkeitsdatum werden nicht in den Rückstand gezogen.

1. (Optional) Klicken Sie auf [!UICONTROL **Bedingung hinzufügen**], um der Abfrage eine weitere Bedingung hinzuzufügen.

   ![Rückstandsabfrage](assets/backlog-query-wrkstrm-board.png)

1. (Optional) Klicken Sie auf [!UICONTROL **Gruppe erstellen**], um eine Gruppe von Bedingungen hinzuzufügen, die mit der ersten Bedingung mit einem OR-Operator verbunden sind.
1. Klicken Sie [!UICONTROL **Abfrage speichern**].

   Die Abfrage wird angewendet, und Karten, die die Kriterien erfüllen, werden in der Spalte „Rückstand“ angezeigt.
