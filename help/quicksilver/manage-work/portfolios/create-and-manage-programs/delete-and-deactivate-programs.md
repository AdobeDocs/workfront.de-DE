---
product-area: programs
navigation-topic: Create and manage programs
title: Programme löschen und deaktivieren
description: Ein Programm stellt eine Sammlung von Projekten dar, die eine gemeinsame Strategie, ein gemeinsames Ziel oder ein gemeinsames Ziel haben und Projektgrenzen überschreiten. Programme sind eine Unterteilung von Portfolios und können nicht außerhalb eines Portfolios existieren. Programme nutzen in der Regel dieselben Ressourcen wie andere Programme innerhalb desselben Portfolios. Sie können ein Programm löschen oder deaktivieren, wenn es irrelevant wird.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 605d1ec5-ca2e-4ff0-87e1-fa53d8ac4a95
TQID: https://experienceleague.adobe.com/nXFATsZ0uMLsgS-q4VlSQxL1Zh29QSCSAWTHxEGBgMw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 464
ht-degree: 7%

---

# Löschen und Deaktivieren von Programmen

Ein Programm stellt eine Sammlung von Projekten dar, die eine gemeinsame Strategie, ein gemeinsames Ziel oder ein gemeinsames Ziel haben und Projektgrenzen überschreiten. Programme sind eine Unterteilung von Portfolios und können nicht außerhalb eines Portfolios existieren. Programme nutzen in der Regel dieselben Ressourcen wie andere Programme innerhalb desselben Portfolios.

Wenn ein Programm irrelevant wird, können Sie eine der folgenden Aktionen ausführen, um zu verhindern, dass Benutzer Projekte mit dem Programm verknüpfen:

* Deaktivieren: Bestehende Projekte bleiben mit dem Programm und dem jeweiligen Portfolio verknüpft. Benutzer sehen das Programm nicht mehr als Option, wenn sie versuchen, neue Projekte mit dem Programm zu verknüpfen.
* Löschen: Bestehende Projekte verlieren ihre Zuordnung zum Programm und werden direkt in das Portfolio verschoben. Benutzer sehen das Programm nicht mehr als Option, wenn sie versuchen, ihre zukünftigen Projekte mit dem Programm zu verknüpfen.

Es wird empfohlen, ein Portfolio zu deaktivieren, anstatt es zu löschen, um die historischen Informationen für Ihre Projekte beizubehalten. Manchmal kann es jedoch erforderlich sein, ein Programm zu löschen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Packstück</td>

<td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>[!UICONTROL Standard]</p><p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf Portfolios und Programme </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für das Portfolio</p> <p>Nachdem Sie ein Programm erstellt haben, verfügen Sie standardmäßig über [!UICONTROL Manage]-Berechtigungen.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen eines Programms

{{step1-to-programs}}

1. Klicken Sie auf den Namen eines Programms, um es zu öffnen.
1. Klicken Sie auf das **Mehr**-Menü rechts neben dem Programmnamen und dann auf **Programm löschen**.
1. Klicken Sie **Ja, löschen** zur Bestätigung.

   Das Programm wird gelöscht und Folgendes geschieht:

   * Bestehende Projekte verlieren ihre Verbindung mit dem Programm und werden direkt in das Portfolio übertragen.
   * Benutzer sehen das Programm nicht mehr als Option, wenn sie versuchen, ihre zukünftigen Projekte mit dem Programm zu verknüpfen.

## Deaktivieren eines Programms

{{step1-to-programs}}

1. Klicken Sie auf den Namen eines Programms, um es zu öffnen.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf das **Mehr**-Menü rechts neben dem Programmnamen und dann auf **Programm deaktivieren**.
   * Klicken Sie auf das **Mehr**-Menü rechts neben dem Programm und anschließend auf **Bearbeiten**

     ODER

     Klicken Sie im linken Bereich auf **Programmdetails** und deaktivieren Sie das Kontrollkästchen **Ist aktiv**.

   Das Programm wird sofort deaktiviert und Folgendes geschieht:

   * Bestehende Projekte bleiben mit dem Programm und seinem jeweiligen Portfolio verknüpft.
   * Benutzer sehen das Programm nicht mehr als Option, wenn sie versuchen, neue Projekte mit dem Programm zu verknüpfen.
