---
title: Festlegen einer benutzerdefinierten Bedingung als Standard für Aufgaben und Probleme
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Wenn ein(e) Benutzende(r) auf Bearbeiten klickt oder einen Aktualisierungskommentar zu einer neuen Aufgabe hinzufügt, der er/sie zugewiesen wurde (ohne manuell eine Bedingung für die Aufgabe festzulegen), zeigt Adobe Workfront die Standardbedingung für Aufgaben an, die im Setup konfiguriert ist. Dasselbe gilt für Probleme.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
TQID: https://experienceleague.adobe.com/1pmI09IkVMY3r4YIy4RjaIeUVsQvFNtlyYLxeT-fBII
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 10%

---

# Benutzerdefinierte Bedingung als Standard für Aufgaben und Probleme festlegen

Wenn ein(e) Benutzende(r) auf Bearbeiten klickt oder einen Aktualisierungskommentar zu einer neuen Aufgabe hinzufügt, der er/sie zugewiesen wurde (ohne manuell eine Bedingung für die Aufgabe festzulegen), zeigt Adobe Workfront die Standardbedingung für Aufgaben an, die im Setup konfiguriert ist. Dasselbe gilt für Probleme.

Workfront verwendet die integrierte Bedingung reibungslos laufen als Standardbedingung für Aufgaben und separat für Probleme. Als Workfront-Administrator können Sie die Standardbedingung für diese beiden Objekttypen in eine von Ihnen erstellte benutzerdefinierte Bedingung ändern.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadmin</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Legen Sie eine benutzerdefinierte Bedingung als Standardbedingung für Aufgaben oder für Probleme fest:

{{step-1-to-setup}}

1. Klicken Sie **Projektvoreinstellungen** > **Bedingungen**.

1. Klicken Sie auf **Registerkarte** Aufgaben“ oder **Probleme**.

1. Klicken Sie **Standardbedingungen festlegen**.
1. Klicken Sie im Dropdown-Menü auf die benutzerdefinierte Bedingung, die als Standardbedingung für Aufgaben (oder Probleme) verwendet werden soll.
1. Klicken Sie auf **Speichern**.

>[!NOTE]
>
>* Ein Benutzer, der einer Aufgabe oder einem Problem zugewiesen ist oder Berechtigungen zum Verwalten dafür hat, kann seine Bedingung manuell ändern. Weitere Informationen finden Sie unter [Bedingung für Aufgaben und Probleme aktualisieren](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Die drei Standardbedingungen für Aufgaben und Probleme, die im Zusammenhang mit Workfront auftreten, funktionieren problemlos, sind Besorgnis erregend und haben schwerwiegende Probleme zur Folge. Sie können diese Bedingungen nicht ausblenden oder löschen, aber Sie können ihre Namen und Farben ändern. Sie können auch neue erstellen, die stattdessen verwendet werden, wie in [Erstellen oder Bearbeiten einer benutzerdefinierten Bedingung](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) beschrieben.

Informationen zum Konfigurieren einer benutzerdefinierten Bedingung als Standardbedingung für Projekte finden Sie unter [Festlegen einer benutzerdefinierten Bedingung als Standardbedingung für Projekte](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).
